# Comparing `tmp/httpx-sse-0.2.0.tar.gz` & `tmp/httpx-sse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx-sse-0.2.0.tar", last modified: Mon Mar 27 12:10:10 2023, max compression
+gzip compressed data, was "httpx-sse-0.3.0.tar", last modified: Thu Apr 27 20:24:20 2023, max compression
```

## Comparing `httpx-sse-0.2.0.tar` & `httpx-sse-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-27 12:10:10.431149 httpx-sse-0.2.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      142 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/CHANGELOG.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1072 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      565 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/Makefile
--rw-r--r--   0 vsts      (1001) docker     (123)     8152 2023-03-27 12:10:10.431149 httpx-sse-0.2.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6827 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-27 12:10:10.431149 httpx-sse-0.2.0/ci/
--rw-r--r--   0 vsts      (1001) docker     (123)      893 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/ci/azure-pipelines.yml
--rw-r--r--   0 vsts      (1001) docker     (123)     1026 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      204 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      320 2023-03-27 12:10:10.431149 httpx-sse-0.2.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-27 12:10:10.427149 httpx-sse-0.2.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-27 12:10:10.431149 httpx-sse-0.2.0/src/httpx_sse/
--rw-r--r--   0 vsts      (1001) docker     (123)      282 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/src/httpx_sse/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/src/httpx_sse/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1748 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/src/httpx_sse/_decoders.py
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/src/httpx_sse/_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/src/httpx_sse/_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/src/httpx_sse/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-27 12:10:10.431149 httpx-sse-0.2.0/src/httpx_sse.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     8152 2023-03-27 12:10:10.000000 httpx-sse-0.2.0/src/httpx_sse.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      564 2023-03-27 12:10:10.000000 httpx-sse-0.2.0/src/httpx_sse.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-27 12:10:10.000000 httpx-sse-0.2.0/src/httpx_sse.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-03-27 12:10:10.000000 httpx-sse-0.2.0/src/httpx_sse.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-27 12:10:10.431149 httpx-sse-0.2.0/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2318 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/tests/test_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1280 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/tests/test_asgi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6687 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/tests/test_event_source.py
--rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-03-27 12:09:19.000000 httpx-sse-0.2.0/tests/test_models.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      142 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (123)      883 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1072 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      565 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (123)     8500 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6829 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.640906 httpx-sse-0.3.0/ci/
+-rw-r--r--   0 vsts      (1001) docker     (123)      893 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/ci/azure-pipelines.yml
+-rw-r--r--   0 vsts      (1001) docker     (123)     1025 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      204 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      320 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.640906 httpx-sse-0.3.0/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/src/httpx_sse/
+-rw-r--r--   0 vsts      (1001) docker     (123)      282 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2157 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1748 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_decoders.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/src/httpx_sse/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/src/httpx_sse.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8500 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      564 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-27 20:24:20.000000 httpx-sse-0.3.0/src/httpx_sse.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 20:24:20.644906 httpx-sse-0.3.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2383 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1280 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_asgi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6687 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_event_source.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      559 2023-04-27 20:23:43.000000 httpx-sse-0.3.0/tests/test_models.py
```

### Comparing `httpx-sse-0.2.0/LICENSE` & `httpx-sse-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/Makefile` & `httpx-sse-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/PKG-INFO` & `httpx-sse-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: httpx-sse
-Version: 0.2.0
+Version: 0.3.0
 Summary: Consume Server-Sent Event (SSE) messages with HTTPX.
 Author-email: Florimond Manca <florimond.manca@protonmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/florimondmanca/httpx-sse
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,18 +31,18 @@
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [How-To](#how-to)
 - [API Reference](#api-reference)
 
 ## Installation
 
-**NOTE**: This is alpha software. Please be sure to pin your dependencies.
+**NOTE**: This is beta software. Please be sure to pin your dependencies.
 
 ```bash
-pip install httpx-sse=="0.2.*"
+pip install httpx-sse=="0.3.*"
 ```
 
 ## Quickstart
 
 `httpx-sse` provides the [`connect_sse`](#connect_sse) and [`aconnect_sse`](#aconnect_sse) helpers for connecting to an SSE endpoint. The resulting [`EventSource`](#eventsource) object exposes the [`.iter_sse()`](#iter_sse) and [`.aiter_sse()`](#aiter_sse) methods to iterate over the server-sent events.
 
 Example usage:
@@ -138,15 +138,15 @@
 Here's how you might achieve this using [`stamina`](https://github.com/hynek/stamina)...
 
 ```python
 import time
 from typing import Iterator
 
 import httpx
-from httpx_sse import iter_sse, ServerSentEvent
+from httpx_sse import connect_sse, ServerSentEvent
 from stamina import retry
 
 def iter_sse_retrying(client, method, url):
     last_event_id = ""
     reconnection_delay = 0.0
 
     # `stamina` will apply jitter and exponential backoff on top of
@@ -174,15 +174,15 @@
     return _iter_sse()
 ```
 
 Usage:
 
 ```python
 with httpx.Client() as client:
-    for iter_sse_retrying(client, "GET", "http://localhost:8000/sse") as sse:
+    for sse in iter_sse_retrying(client, "GET", "http://localhost:8000/sse"):
         print(sse.event, sse.data)
 ```
 
 ## API Reference
 
 ### `connect_sse`
 
@@ -276,14 +276,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## 0.3.0 - 2023-04-27
+
+### Changed
+
+* Raising an `SSEError` if the response content type is not `text/event-stream` is now performed as part of `iter_sse()` / `aiter_sse()`, instead of `connect_sse()` / `aconnect_sse()`. This allows inspecting the response before iterating on server-sent events, such as checking for error responses. (Pull #12)
+
 ## 0.2.0 - 2023-03-27
 
 ### Changed
 
 * `connect_sse()` and `aconnect_sse()` now require a `method` argument: `connect_sse(client, "GET", "https://example.org")`. This provides support for SSE requests with HTTP verbs other than `GET`. (Pull #7)
 
 ## 0.1.0 - 2023-02-05
```

### Comparing `httpx-sse-0.2.0/README.md` & `httpx-sse-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [How-To](#how-to)
 - [API Reference](#api-reference)
 
 ## Installation
 
-**NOTE**: This is alpha software. Please be sure to pin your dependencies.
+**NOTE**: This is beta software. Please be sure to pin your dependencies.
 
 ```bash
-pip install httpx-sse=="0.2.*"
+pip install httpx-sse=="0.3.*"
 ```
 
 ## Quickstart
 
 `httpx-sse` provides the [`connect_sse`](#connect_sse) and [`aconnect_sse`](#aconnect_sse) helpers for connecting to an SSE endpoint. The resulting [`EventSource`](#eventsource) object exposes the [`.iter_sse()`](#iter_sse) and [`.aiter_sse()`](#aiter_sse) methods to iterate over the server-sent events.
 
 Example usage:
@@ -118,15 +118,15 @@
 Here's how you might achieve this using [`stamina`](https://github.com/hynek/stamina)...
 
 ```python
 import time
 from typing import Iterator
 
 import httpx
-from httpx_sse import iter_sse, ServerSentEvent
+from httpx_sse import connect_sse, ServerSentEvent
 from stamina import retry
 
 def iter_sse_retrying(client, method, url):
     last_event_id = ""
     reconnection_delay = 0.0
 
     # `stamina` will apply jitter and exponential backoff on top of
@@ -154,15 +154,15 @@
     return _iter_sse()
 ```
 
 Usage:
 
 ```python
 with httpx.Client() as client:
-    for iter_sse_retrying(client, "GET", "http://localhost:8000/sse") as sse:
+    for sse in iter_sse_retrying(client, "GET", "http://localhost:8000/sse"):
         print(sse.event, sse.data)
 ```
 
 ## API Reference
 
 ### `connect_sse`
```

### Comparing `httpx-sse-0.2.0/ci/azure-pipelines.yml` & `httpx-sse-0.3.0/ci/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/pyproject.toml` & `httpx-sse-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "Consume Server-Sent Event (SSE) messages with HTTPX."
 requires-python = ">=3.7"
 license = { text = "MIT" }
 authors = [
   { name = "Florimond Manca", email = "florimond.manca@protonmail.com" },
 ]
 classifiers = [
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `httpx-sse-0.2.0/src/httpx_sse/_api.py` & `httpx-sse-0.3.0/src/httpx_sse/_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 from ._decoders import SSEDecoder
 from ._exceptions import SSEError
 from ._models import ServerSentEvent
 
 
 class EventSource:
     def __init__(self, response: httpx.Response) -> None:
-        content_type, _, _ = response.headers["content-type"].partition(";")
+        self._response = response
 
+    def _check_content_type(self) -> None:
+        content_type, _, _ = self._response.headers["content-type"].partition(";")
         if content_type != "text/event-stream":
             raise SSEError(
                 "Expected response Content-Type to be 'text/event-stream', "
                 f"got {content_type!r}"
             )
 
-        self._response = response
-
     @property
     def response(self) -> httpx.Response:
         return self._response
 
     def iter_sse(self) -> Iterator[ServerSentEvent]:
+        self._check_content_type()
         decoder = SSEDecoder()
         for line in self._response.iter_lines():
             line = line.rstrip("\n")
             sse = decoder.decode(line)
             if sse is not None:
                 yield sse
 
     async def aiter_sse(self) -> AsyncIterator[ServerSentEvent]:
+        self._check_content_type()
         decoder = SSEDecoder()
         async for line in self._response.aiter_lines():
             line = line.rstrip("\n")
             sse = decoder.decode(line)
             if sse is not None:
                 yield sse
```

### Comparing `httpx-sse-0.2.0/src/httpx_sse/_decoders.py` & `httpx-sse-0.3.0/src/httpx_sse/_decoders.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/src/httpx_sse/_models.py` & `httpx-sse-0.3.0/src/httpx_sse/_models.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/src/httpx_sse.egg-info/PKG-INFO` & `httpx-sse-0.3.0/src/httpx_sse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: httpx-sse
-Version: 0.2.0
+Version: 0.3.0
 Summary: Consume Server-Sent Event (SSE) messages with HTTPX.
 Author-email: Florimond Manca <florimond.manca@protonmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/florimondmanca/httpx-sse
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,18 +31,18 @@
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [How-To](#how-to)
 - [API Reference](#api-reference)
 
 ## Installation
 
-**NOTE**: This is alpha software. Please be sure to pin your dependencies.
+**NOTE**: This is beta software. Please be sure to pin your dependencies.
 
 ```bash
-pip install httpx-sse=="0.2.*"
+pip install httpx-sse=="0.3.*"
 ```
 
 ## Quickstart
 
 `httpx-sse` provides the [`connect_sse`](#connect_sse) and [`aconnect_sse`](#aconnect_sse) helpers for connecting to an SSE endpoint. The resulting [`EventSource`](#eventsource) object exposes the [`.iter_sse()`](#iter_sse) and [`.aiter_sse()`](#aiter_sse) methods to iterate over the server-sent events.
 
 Example usage:
@@ -138,15 +138,15 @@
 Here's how you might achieve this using [`stamina`](https://github.com/hynek/stamina)...
 
 ```python
 import time
 from typing import Iterator
 
 import httpx
-from httpx_sse import iter_sse, ServerSentEvent
+from httpx_sse import connect_sse, ServerSentEvent
 from stamina import retry
 
 def iter_sse_retrying(client, method, url):
     last_event_id = ""
     reconnection_delay = 0.0
 
     # `stamina` will apply jitter and exponential backoff on top of
@@ -174,15 +174,15 @@
     return _iter_sse()
 ```
 
 Usage:
 
 ```python
 with httpx.Client() as client:
-    for iter_sse_retrying(client, "GET", "http://localhost:8000/sse") as sse:
+    for sse in iter_sse_retrying(client, "GET", "http://localhost:8000/sse"):
         print(sse.event, sse.data)
 ```
 
 ## API Reference
 
 ### `connect_sse`
 
@@ -276,14 +276,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## 0.3.0 - 2023-04-27
+
+### Changed
+
+* Raising an `SSEError` if the response content type is not `text/event-stream` is now performed as part of `iter_sse()` / `aiter_sse()`, instead of `connect_sse()` / `aconnect_sse()`. This allows inspecting the response before iterating on server-sent events, such as checking for error responses. (Pull #12)
+
 ## 0.2.0 - 2023-03-27
 
 ### Changed
 
 * `connect_sse()` and `aconnect_sse()` now require a `method` argument: `connect_sse(client, "GET", "https://example.org")`. This provides support for SSE requests with HTTP verbs other than `GET`. (Pull #7)
 
 ## 0.1.0 - 2023-02-05
```

### Comparing `httpx-sse-0.2.0/src/httpx_sse.egg-info/SOURCES.txt` & `httpx-sse-0.3.0/src/httpx_sse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/tests/test_api.py` & `httpx-sse-0.3.0/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 def test_connect_sse_non_event_stream_received() -> None:
     def handler(request: httpx.Request) -> httpx.Response:
         assert request.url.path == "/"
         return httpx.Response(200, text="Hello, world!")
 
     with httpx.Client(transport=httpx.MockTransport(handler)) as client:
         with pytest.raises(SSEError, match="text/event-stream"):
-            with connect_sse(client, "GET", "http://testserver") as _:
-                pass  # pragma: no cover
+            with connect_sse(client, "GET", "http://testserver") as event_source:
+                for _ in event_source.iter_sse():
+                    pass  # pragma: no cover
 
 
 @pytest.mark.asyncio
 async def test_aconnect_sse() -> None:
     def handler(request: httpx.Request) -> httpx.Response:
         if request.url.path == "/":
             return httpx.Response(200, text="Hello, world!")
```

### Comparing `httpx-sse-0.2.0/tests/test_asgi.py` & `httpx-sse-0.3.0/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/tests/test_event_source.py` & `httpx-sse-0.3.0/tests/test_event_source.py`

 * *Files identical despite different names*

### Comparing `httpx-sse-0.2.0/tests/test_models.py` & `httpx-sse-0.3.0/tests/test_models.py`

 * *Files identical despite different names*

