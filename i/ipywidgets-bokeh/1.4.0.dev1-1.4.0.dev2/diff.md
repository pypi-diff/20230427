# Comparing `tmp/ipywidgets_bokeh-1.4.0.dev1.tar.gz` & `tmp/ipywidgets_bokeh-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets_bokeh-1.4.0.dev1.tar", last modified: Tue Apr 18 08:16:01 2023, max compression
+gzip compressed data, was "ipywidgets_bokeh-1.4.0.dev2.tar", last modified: Thu Apr 27 16:58:09 2023, max compression
```

## Comparing `ipywidgets_bokeh-1.4.0.dev1.tar` & `ipywidgets_bokeh-1.4.0.dev2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-18 08:16:01.610937 ipywidgets_bokeh-1.4.0.dev1/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1494 2020-01-09 14:03:17.000000 ipywidgets_bokeh-1.4.0.dev1/LICENSE.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      184 2021-10-05 19:15:23.000000 ipywidgets_bokeh-1.4.0.dev1/MANIFEST.in
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-18 08:16:01.610937 ipywidgets_bokeh-1.4.0.dev1/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      511 2020-07-10 18:26:09.000000 ipywidgets_bokeh-1.4.0.dev1/README.md
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-18 08:16:01.602933 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       58 2023-04-18 07:31:20.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        3 2019-12-19 13:15:23.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/bokeh.ext.json
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-18 08:16:01.602933 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)   432832 2023-04-18 08:16:00.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3529 2023-04-18 08:16:00.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)  3042118 2023-04-18 08:16:00.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/ipywidgets_bokeh.js
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-18 08:16:01.610937 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       55 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/index.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      591 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/index.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      103 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/loader.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1668 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/loader.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1290 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/manager.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     7950 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/manager.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       48 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/webpack.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      292 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/webpack.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1192 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/widget.d.ts
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3971 2023-04-18 08:14:40.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/widget.js
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4713 2023-04-18 07:31:20.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/kernel.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1222 2023-04-18 07:31:20.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/package.json
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1243 2023-03-29 21:38:08.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/widget.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-18 08:16:01.602933 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-18 08:16:01.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      900 2023-04-18 08:16:01.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-04-18 08:16:01.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       53 2023-04-18 08:16:01.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-04-18 08:16:01.000000 ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/top_level.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      106 2023-04-18 08:16:01.610937 ipywidgets_bokeh-1.4.0.dev1/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1882 2023-04-18 07:31:20.000000 ipywidgets_bokeh-1.4.0.dev1/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1494 2020-01-09 14:03:17.000000 ipywidgets_bokeh-1.4.0.dev2/LICENSE.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      184 2021-10-05 19:15:23.000000 ipywidgets_bokeh-1.4.0.dev2/MANIFEST.in
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      511 2020-07-10 18:26:09.000000 ipywidgets_bokeh-1.4.0.dev2/README.md
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.757953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       58 2023-04-27 14:59:03.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        3 2019-12-19 13:15:23.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/bokeh.ext.json
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.757953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)   432832 2023-04-27 16:58:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3529 2023-04-27 16:58:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)  3042125 2023-04-27 16:58:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/ipywidgets_bokeh.js
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       55 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/index.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      591 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/index.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      103 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/loader.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1668 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/loader.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1290 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     7924 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       48 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/webpack.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      292 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/webpack.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1192 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.d.ts
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3971 2023-04-27 16:56:53.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.js
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     4480 2023-04-27 14:59:06.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/kernel.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1222 2023-04-27 14:59:16.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/package.json
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1243 2023-03-29 21:38:08.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/widget.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-04-27 16:58:09.757953 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1391 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      900 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       51 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-04-27 16:58:09.000000 ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/top_level.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      106 2023-04-27 16:58:09.765953 ipywidgets_bokeh-1.4.0.dev2/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1880 2023-04-27 16:56:09.000000 ipywidgets_bokeh-1.4.0.dev2/setup.py
```

### Comparing `ipywidgets_bokeh-1.4.0.dev1/LICENSE.txt` & `ipywidgets_bokeh-1.4.0.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/PKG-INFO` & `ipywidgets_bokeh-1.4.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets_bokeh
-Version: 1.4.0.dev1
+Version: 1.4.0.dev2
 Summary: Allows embedding of Jupyter widgets in Bokeh layouts.
 Home-page: https://github.com/bokeh/ipywidgets_bokeh
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/64.ipywidgets_bokeh.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/87.ipywidgets_bokeh.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/ipywidgets_bokeh.js` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/ipywidgets_bokeh.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -88192,15 +88192,15 @@
                     id: "" + Up++
                 };
                 this.kernel = this.kernel_manager.connectTo({
                     model: r,
                     handleComms: !0
                 }), this.kernel.registerCommTarget(this.comm_target_name, ((e, t) => {
                     const n = this._model_objs.get(t.content.comm_id);
-                    if (null != n) {
+                    if (null != n && !n.comm_live) {
                         const t = new xt.services.Comm(e);
                         this._attach_comm(t, n)
                     }
                     this._model_objs.delete(t.content.comm_id)
                 }))
             }
             _attach_comm(e, t) {
@@ -88236,15 +88236,15 @@
                     const n = e + t,
                         r = this._comms.get(n);
                     if (null != r) return r; {
                         const r = this.kernel.createComm(e, t);
                         return this._comms.set(n, r), r
                     }
                 })();
-                return (n || r) && o.open(n, r, i), new xt.services.Comm(o)
+                return o.open(n, r, i), new xt.services.Comm(o)
             }
             _get_comm_info() {
                 return Promise.resolve((0, Po.to_object)(this._known_models))
             }
             async new_model(e, t) {
                 if (void 0 === t) {
                     const n = this._known_models,
```

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/index.js` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/index.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/loader.js` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/loader.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/manager.d.ts` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.d.ts`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/manager.js` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/manager.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -118,15 +118,15 @@
         };
         this.kernel = this.kernel_manager.connectTo({
             model: kernel_model,
             handleComms: true
         });
         this.kernel.registerCommTarget(this.comm_target_name, (comm, msg) => {
             const model = this._model_objs.get(msg.content.comm_id);
-            if (model != null) {
+            if (model != null && !model.comm_live) {
                 const comm_wrapper = new shims.services.Comm(comm);
                 this._attach_comm(comm_wrapper, model);
             }
             this._model_objs.delete(msg.content.comm_id);
         });
     }
     _attach_comm(comm, model) {
@@ -180,17 +180,15 @@
                 return comm;
             else {
                 const comm = this.kernel.createComm(target_name, model_id);
                 this._comms.set(key, comm);
                 return comm;
             }
         })();
-        if (data || metadata) {
-            comm.open(data, metadata, buffers);
-        }
+        comm.open(data, metadata, buffers);
         return new shims.services.Comm(comm);
     }
     _get_comm_info() {
         return Promise.resolve(to_object(this._known_models));
     }
     async new_model(options, serialized_state) {
         // XXX: this is a hack that allows to connect to a live comm and use initial
```

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/widget.d.ts` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.d.ts`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/dist/lib/widget.js` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/dist/lib/widget.js`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/kernel.py` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/kernel.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 #-----------------------------------------------------------------------------
 from __future__ import annotations
 
 import json
 import logging
 
 from distutils.version import LooseVersion
-from functools import partial
-from typing import Union
 
 import ipykernel
 import ipykernel.kernelbase
 import jupyter_client.session as session
 
 from bokeh.document.events import MessageSentEvent
 from ipykernel.comm import CommManager
@@ -41,36 +39,23 @@
     def flush(self, arg):
         pass
 
 class SessionWebsocket(session.Session):
 
     parent: BokehKernel
 
-    def send(self, stream, msg_type, content=None, parent=None, ident=None, buffers=None, track=False, header=None, metadata=None):
-        if not isinstance(stream, WebsocketStream):
-            self.parent.log.warn(f"skipping {msg_type} ${content}")
-            return
-
-        msg = self.msg(msg_type, content=content, parent=parent, header=header, metadata=metadata)
-        msg['channel'] = stream.channel
-
-        doc = self.document
-
-        # Ensure document message handler is only added once
-        try:
-            doc.remove_on_message("ipywidgets_bokeh", self.receive)
-        except Exception:
-            pass
-        finally:
-            doc.on_message("ipywidgets_bokeh", self.receive)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.document.on_message("ipywidgets_bokeh", self.receive)
 
+    def _encode_msg(self, msg: dict[str, Any], buffers: list[bytes]) -> bytes | str:
         packed = self.pack(msg)
 
-        data: Union[bytes, str]
-        if buffers is not None and len(buffers) != 0:
+        data: bytes | str
+        if buffers:
             buffers = [packed] + buffers
             nbufs = len(buffers)
 
             start = 4*(1 + nbufs)
             offsets = [start]
 
             for buffer in buffers[:-1]:
@@ -78,31 +63,36 @@
                 offsets.append(start)
 
             u32 = lambda n: n.to_bytes(4, "big")
             items = [u32(nbufs)] + [ u32(offset) for offset in offsets ] + buffers
             data = b"".join(items)
         else:
             data = packed.decode("utf-8")
-        event = MessageSentEvent(doc, "ipywidgets_bokeh", data)
+
+        return data
+
+    def send(self, stream, msg_type, content=None, parent=None, ident=None, buffers: list[bytes] | None = None, track=False, header=None, metadata=None):
+        msg = self.msg(msg_type, content=content, parent=parent, header=header, metadata=metadata)
+        msg["channel"] = getattr(stream, "channel", "shell")
+        data = self._encode_msg(msg, buffers or [])
+        event = MessageSentEvent(self.document, "ipywidgets_bokeh", data)
         self._trigger_change(event)
 
     def receive(self, data: str) -> None:
         msg = json.loads(data)
-        msg_serialized = self.serialize(msg)
         if msg['channel'] == 'shell':
-            stream = StreamWrapper(msg['channel'])
+            msg_serialized = self.serialize(msg)
             msg_list = [BytesWrap(k) for k in msg_serialized]
-            if kernel_version > '6':
-                cb = partial(self.parent.dispatch_shell, msg_list)
-                if self.document.session_context: # Bokeh Server
-                    self.document.add_next_tick_callback(cb)
-                else: # Other Tornado based server
-                    self.parent.io_loop.add_callback(cb)
-            else:
-                self.parent.dispatch_shell(stream, msg_list)
+            async def dispatch_shell():
+                parent = self.parent
+                await parent.dispatch_shell(msg_list)
+            if self.document.session_context: # Bokeh Server
+                self.document.add_next_tick_callback(dispatch_shell)
+            else: # Other Tornado based server
+                self.parent.io_loop.add_callback(dispatch_shell)
 
     @property
     def document(self):
         from bokeh.io import curdoc
         return curdoc()
 
     def _trigger_change(self, event):
@@ -113,29 +103,29 @@
 
     def flush(self, *args):
         pass
 
 
 class BokehKernel(ipykernel.kernelbase.Kernel):
     implementation = 'ipython'
-    implementation_version = '1.4.0.dev1'
+    implementation_version = '1.4.0.dev2'
     banner = 'banner'
 
     shell_stream = Any(ShellStream(), allow_none=True)
 
     def __init__(self):
         super(BokehKernel, self).__init__()
 
         self.session = SessionWebsocket(parent=self, key=SESSION_KEY)
         self.stream = self.iopub_socket = WebsocketStream(self.session)
         self.io_loop = IOLoop.current()
 
         self.iopub_socket.channel = 'iopub'
         self.session.stream = self.iopub_socket
-        self.comm_manager = CommManager()
+        self.comm_manager = CommManager(parent=self, kernel=self)
         self.shell = None
         self.log = logging.getLogger("ipywidgets_bokeh")
 
         comm_msg_types = ['comm_open', 'comm_msg', 'comm_close']
         for msg_type in comm_msg_types:
             self.shell_handlers[msg_type] = getattr(self.comm_manager, msg_type)
```

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/package.json` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.4.0-dev.2'"}*

```diff
@@ -37,9 +37,9 @@
         "build": "tsc && webpack --mode=production",
         "clean": "rimraf dist",
         "dev": "tsc; webpack --mode=development",
         "lint": "eslint -c eslint.json src/**/*.ts",
         "prepack": "npm run clean && npm run build",
         "test": "echo 'TODO'"
     },
-    "version": "1.4.0-dev.1"
+    "version": "1.4.0-dev.2"
 }
```

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh/widget.py` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh/widget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/PKG-INFO` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets-bokeh
-Version: 1.4.0.dev1
+Version: 1.4.0.dev2
 Summary: Allows embedding of Jupyter widgets in Bokeh layouts.
 Home-page: https://github.com/bokeh/ipywidgets_bokeh
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ipywidgets_bokeh-1.4.0.dev1/ipywidgets_bokeh.egg-info/SOURCES.txt` & `ipywidgets_bokeh-1.4.0.dev2/ipywidgets_bokeh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipywidgets_bokeh-1.4.0.dev1/setup.py` & `ipywidgets_bokeh-1.4.0.dev2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,21 +22,21 @@
             self.spawn([npm, "install"])
             self.spawn([npm, "run", "prepack"])
         finally:
             os.chdir("..")
 
 install_requires = [
     "bokeh ==3.*", # TODO 3.2.dev1
-    "ipywidgets ==8.0.4",
+    "ipywidgets ==8.*",
     "ipykernel ==6.*,!=6.18.0", # until ipywidgets 8.0.6
 ]
 
 setup_args = dict(
     name="ipywidgets_bokeh",
-    version="1.4.0.dev1",
+    version="1.4.0.dev2",
     install_requires=install_requires,
     python_requires=">=3.9",
     description="Allows embedding of Jupyter widgets in Bokeh layouts.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bokeh Team",
     author_email="info@bokeh.org",
```

