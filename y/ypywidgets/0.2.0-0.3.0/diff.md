# Comparing `tmp/ypywidgets-0.2.0.tar.gz` & `tmp/ypywidgets-0.3.0.tar.gz`

## Comparing `ypywidgets-0.2.0.tar` & `ypywidgets-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ypywidgets-0.2.0/ypywidgets/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 ypywidgets-0.2.0/ypywidgets/ypywidgets.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 ypywidgets-0.2.0/ypywidgets/yutils.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ypywidgets-0.2.0/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ypywidgets-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 ypywidgets-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/reactive.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/utils.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/ypywidgets.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/PKG-INFO
```

### Comparing `ypywidgets-0.2.0/ypywidgets/ypywidgets.py` & `ypywidgets-0.3.0/ypywidgets/ypywidgets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 from typing import Dict, Optional
 from uuid import uuid4
 
 import comm
 import y_py as Y
 
-from .yutils import (
+from .utils import (
     YMessageType,
     YSyncMessageType,
     create_update_message,
     process_sync_message,
     sync,
 )
 
 
 class Widget:
+
     def __init__(
         self,
-        name: str,
-        open_comm: bool,
+        primary: bool = True,
         comm_data: Optional[Dict] = None,
         comm_metadata: Optional[Dict] = None,
     ) -> None:
-        self.name = name
-        self.ydoc = Y.YDoc()
-        if open_comm:
-            self.comm_id = uuid4().hex
-            self.comm = comm.create_comm(
-                comm_id=self.comm_id,
-                target_name=self.name,
+        self._ydoc = Y.YDoc()
+        self._attrs = self._ydoc.get_map("_attrs")
+        self._attrs.observe(self._set_attr)
+        self._comm = None
+        if primary:
+            if comm_metadata is None:
+                comm_metadata = {"ymodel_name": self.__class__.__name__}
+            self._comm_id = uuid4().hex
+            self._comm = comm.create_comm(
+                comm_id=self._comm_id,
+                target_name="ywidget",
                 data=comm_data,
                 metadata=comm_metadata,
             )
-            self.comm.on_msg(self._receive)
-            sync(self.ydoc, self.comm)
+            self._comm.on_msg(self._receive)
+            msg = sync(self._ydoc)
+            self._comm.send(**msg)
+
+    def _set_attr(self, event):
+        for k, v in event.keys.items():
+            new_value = v["newValue"]
+            if getattr(self, k) != new_value:
+                setattr(self, k, new_value)
 
     def _repr_mimebundle_(self, **kwargs):
         plaintext = repr(self)
         if len(plaintext) > 110:
             plaintext = plaintext[:110] + '…'
         data = {
             "text/plain": plaintext,
             "application/vnd.jupyter.ywidget-view+json": {
                 "version_major": 2,
                 "version_minor": 0,
-                "model_id": self.comm_id
+                "model_id": self._comm_id
             }
         }
         return data
 
     def _receive(self, msg):
         message = bytes(msg["buffers"][0])
         if message[0] == YMessageType.SYNC:
-            process_sync_message(message[1:], self.ydoc, self.comm.send)
+            reply = process_sync_message(message[1:], self._ydoc)
+            if reply:
+                self._comm.send(buffers=[reply])
             if message[1] == YSyncMessageType.SYNC_STEP2:
-                self.ydoc.observe_after_transaction(self._send)
+                self._ydoc.observe_after_transaction(self._send)
 
     def _send(self, event: Y.AfterTransactionEvent):
         update = event.get_update()
         message = create_update_message(update)
-        self.comm.send(buffers=[message])
+        self._comm.send(buffers=[message])
```

### Comparing `ypywidgets-0.2.0/ypywidgets/yutils.py` & `ypywidgets-0.3.0/ypywidgets/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,29 +89,33 @@
     def read_var_string(self):
         message = self.read_message()
         if message is None:
             return ""
         return message.decode("utf-8")
 
 
-def process_sync_message(message: bytes, ydoc: Y.YDoc, send_callback) -> None:
+def process_sync_message(message: bytes, ydoc: Y.YDoc) -> Optional[bytes]:
     message_type = message[0]
     msg = message[1:]
+
     if message_type == YSyncMessageType.SYNC_STEP1:
         state = read_message(msg)
         update = Y.encode_state_as_update(ydoc, state)
         reply = create_sync_step2_message(update)
-        send_callback(buffers=[reply])
-    elif message_type in (
+        return reply
+
+    if message_type in (
         YSyncMessageType.SYNC_STEP2,
         YSyncMessageType.SYNC_UPDATE,
     ):
         update = read_message(msg)
         # Ignore empty updates (see https://github.com/y-crdt/ypy/issues/98)
         if update != b"\x00\x00":
             Y.apply_update(ydoc, update)
 
+    return None
+
 
-def sync(ydoc: Y.YDoc, comm):
+def sync(ydoc: Y.YDoc):
     state = Y.encode_state_vector(ydoc)
     msg = create_sync_step1_message(state)
-    comm.send(buffers=[msg])
+    return {"buffers": [msg]}
```

### Comparing `ypywidgets-0.2.0/pyproject.toml` & `ypywidgets-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 keywords = [
     "widgets",
     "jupyter",
     "ypy",
     "yjs",
 ]
 dependencies = [
-    "comm >=0.1.2",
-    "y-py >=0.5.5",
+    "comm >=0.1.2,<1",
+    "y-py >=0.6.0,<1",
+    "reacttrs >=0.1.2,<1",
 ]
 
 [project.urls]
 Homepage = "https://github.com/davidbrochart/ypywidgets"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
+    "pytest-asyncio",
 ]
 
 [tool.hatch.version]
 path = "ypywidgets/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
```

### Comparing `ypywidgets-0.2.0/PKG-INFO` & `ypywidgets-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: ypywidgets
-Version: 0.2.0
+Version: 0.3.0
 Summary: Y-based Jupyter widgets for Python
 Project-URL: Homepage, https://github.com/davidbrochart/ypywidgets
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 Keywords: jupyter,widgets,yjs,ypy
 Requires-Python: >=3.7
-Requires-Dist: comm>=0.1.2
-Requires-Dist: y-py>=0.5.5
+Requires-Dist: comm<1,>=0.1.2
+Requires-Dist: reacttrs<1,>=0.1.2
+Requires-Dist: y-py<1,>=0.6.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-asyncio; extra == 'dev'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/davidbrochart/ypywidgets/workflows/CI/badge.svg)](https://github.com/davidbrochart/ypywidgets/actions)
 
 # ypywidgets
 
 Y-based Jupyter widgets for Python.
```

