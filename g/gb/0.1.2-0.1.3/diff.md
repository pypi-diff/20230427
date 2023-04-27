# Comparing `tmp/gb-0.1.2.tar.gz` & `tmp/gb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gb-0.1.2.tar", max compression
+gzip compressed data, was "gb-0.1.3.tar", max compression
```

## Comparing `gb-0.1.2.tar` & `gb-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,12 @@
--rw-r--r--   0        0        0     1075 2022-07-15 23:24:03.752873 gb-0.1.2/LICENSE
--rw-r--r--   0        0        0     2008 2023-04-25 11:55:09.016556 gb-0.1.2/README.md
--rw-r--r--   0        0        0        0 2022-07-15 23:24:03.756873 gb-0.1.2/gb/__init__.py
--rw-r--r--   0        0        0       78 2022-07-15 23:24:03.756873 gb-0.1.2/gb/__main__.py
--rw-r--r--   0        0        0     2143 2023-04-25 12:02:59.154436 gb-0.1.2/gb/command.py
--rw-r--r--   0        0        0      643 2022-07-15 23:24:03.756873 gb-0.1.2/gb/document.py
--rw-r--r--   0        0        0     1290 2022-07-15 23:24:03.756873 gb-0.1.2/gb/entry.py
--rw-r--r--   0        0        0      413 2022-07-15 23:24:03.757873 gb-0.1.2/gb/magic.py
--rw-r--r--   0        0        0     2127 2022-07-15 23:24:03.757873 gb-0.1.2/gb/mode.py
--rw-r--r--   0        0        0      669 2022-07-15 23:24:03.757873 gb-0.1.2/gb/protocol.py
--rw-r--r--   0        0        0      818 2022-07-15 23:24:03.757873 gb-0.1.2/gb/safe.py
--rw-r--r--   0        0        0     3489 2022-07-15 23:24:03.757873 gb-0.1.2/gb/server.py
--rw-r--r--   0        0        0     1080 2023-04-25 12:17:06.881206 gb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 gb-0.1.2/setup.py
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 gb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-07-15 23:24:03.752873 gb-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1315 2023-04-27 11:50:28.549812 gb-0.1.3/README.md
+-rw-r--r--   0        0        0     1595 2023-04-27 11:51:22.089705 gb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-15 23:24:03.756873 gb-0.1.3/src/gb/__init__.py
+-rw-r--r--   0        0        0      639 2023-04-26 10:11:13.451535 gb-0.1.3/src/gb/document.py
+-rw-r--r--   0        0        0     1278 2023-04-26 10:11:13.465535 gb-0.1.3/src/gb/entry.py
+-rw-r--r--   0        0        0      410 2023-04-26 10:11:13.451535 gb-0.1.3/src/gb/magic.py
+-rw-r--r--   0        0        0     2121 2023-04-26 10:11:13.472535 gb-0.1.3/src/gb/mode.py
+-rw-r--r--   0        0        0      669 2022-07-15 23:24:03.757873 gb-0.1.3/src/gb/protocol.py
+-rw-r--r--   0        0        0      806 2023-04-26 10:11:13.457535 gb-0.1.3/src/gb/safe.py
+-rw-r--r--   0        0        0     3471 2023-04-26 10:11:13.480535 gb-0.1.3/src/gb/server.py
+-rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 gb-0.1.3/PKG-INFO
```

### Comparing `gb-0.1.2/LICENSE` & `gb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gb-0.1.2/gb/document.py` & `gb-0.1.3/src/gb/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import gb.protocol
 import gb.entry
 
 
 class Document:
     """A document is an index of entries for a certain directory. It dictates
-      how those entries are joined together and if any extra information is
-      added."""
+    how those entries are joined together and if any extra information is
+    added."""
 
     entries: List[gb.entry.Entry]
 
     def __init__(self) -> None:
         self.entries = []
 
     def add_entry(self, entry: gb.entry.Entry) -> None:
```

### Comparing `gb-0.1.2/gb/entry.py` & `gb-0.1.3/src/gb/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 class Entry:
     """Gopher indexes contain entries of various types. This list is both
-       sourced from RFC 1436:
+    sourced from RFC 1436:
 
-       https://tools.ietf.org/html/rfc1436
+    https://tools.ietf.org/html/rfc1436
 
-       and the Wikipedia page for non-standard types:
+    and the Wikipedia page for non-standard types:
 
-       https://en.wikipedia.org/wiki/Gopher_(protocol)#Item_types"""
+    https://en.wikipedia.org/wiki/Gopher_(protocol)#Item_types"""
 
     host: str
     port: int
 
     def __init__(self, host: str, port: int, text: str, selector: str) -> None:
         self.host = host
         self.port = port
```

### Comparing `gb-0.1.2/gb/mode.py` & `gb-0.1.3/src/gb/mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
     def lookup(self, path: str) -> str:
         raise NotImplementedError()
 
 
 class ImplicitMode(Mode):
     """ImplicitMode looks up files recursively within a given path auto-
-       generating any required indexes."""
+    generating any required indexes."""
 
     def lookup(self, path: str) -> str:
         """Look up a path within our base path and return the contents in
-           pre-rendered Gopher format!"""
+        pre-rendered Gopher format!"""
 
         path = gb.safe.relativize(self.base_path, path)
 
         if os.path.islink(path):
             raise ValueError()
 
         if os.path.isdir(path):
```

### Comparing `gb-0.1.2/gb/protocol.py` & `gb-0.1.3/src/gb/protocol.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.2/gb/safe.py` & `gb-0.1.3/src/gb/safe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 
 def relativize(base: str, path: str) -> str:
     """Join base and path making sure that the resulting path lies
-       within the base. We do this by making path relative if it's an
-       absolute path then verifying if it's still within the base after
-       joining.
+    within the base. We do this by making path relative if it's an
+    absolute path then verifying if it's still within the base after
+    joining.
 
-       We fail hard if the calculated path is not within base."""
+    We fail hard if the calculated path is not within base."""
 
     base = os.path.abspath(base)
 
     # The nif the path starts with a separator we remove that
     if path.startswith(os.path.sep):
         path = path[len(os.path.sep) :]
```

### Comparing `gb-0.1.2/gb/server.py` & `gb-0.1.3/src/gb/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 
 log = logging.getLogger(__name__)
 
 
 class GopherServer(tornado.tcpserver.TCPServer):
     """Generic tornado TCPServer which speaks the Gopher protocol. The Gopher
-       protocol is defined in RFC 1436:
+    protocol is defined in RFC 1436:
 
-       https://tools.ietf.org/html/rfc1436."""
+    https://tools.ietf.org/html/rfc1436."""
 
     # XXX TODO has to come from somewhere!
     encoding: str
     mode: gb.mode.Mode
 
     async def handle_stream(
         self, stream: tornado.iostream.IOStream, address: Tuple[Any, ...]
     ) -> None:
         """A new incoming connection. We wait silently until the client sends
-           a selector through after which we clean and parse that selector."""
+        a selector through after which we clean and parse that selector."""
 
         log.debug("Accepted connection from %s", address)
 
         while True:
             try:
                 # clean this up, split on \n but clean both
                 selector_raw = await stream.read_until(
@@ -67,28 +67,28 @@
                 break
             except tornado.iostream.StreamClosedError:
                 log.debug("Lost connection from %s", address)
                 break
 
     async def close_stream(self, stream: tornado.iostream.IOStream) -> None:
         """Gopher connections are closed by writing a . on a single line then
-           closing the underlying transport."""
+        closing the underlying transport."""
         await stream.write(gb.protocol.eof.encode(self.encoding))
         await stream.write(gb.protocol.crlf.encode(self.encoding))
         stream.close()
 
     async def lookup(self, stream: tornado.iostream.IOStream, data: str) -> str:
         """Lookup a selector on our mode."""
         return self.mode.lookup(data)
 
 
 class ImplicitGopherServer(GopherServer):
     """The implicit gopher server serves files from a given path recursively
-       while auto generating indexes for directories. If magic is enabled then
-       the mode will auto-guess filetypes."""
+    while auto generating indexes for directories. If magic is enabled then
+    the mode will auto-guess filetypes."""
 
     def __init__(
         self, path: str, host: str, port: int, magic: bool, encoding: str
     ) -> None:
         super().__init__()
 
         log.info("Starting ImplicitGopherServer with path %s", path)
```

