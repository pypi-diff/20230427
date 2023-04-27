# Comparing `tmp/scaleway_functions_python-0.1.1.tar.gz` & `tmp/scaleway_functions_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway_functions_python-0.1.1.tar", max compression
+gzip compressed data, was "scaleway_functions_python-0.2.0.tar", max compression
```

## Comparing `scaleway_functions_python-0.1.1.tar` & `scaleway_functions_python-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      510 2023-04-14 13:11:30.987608 scaleway_functions_python-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-04-14 13:11:30.987608 scaleway_functions_python-0.1.1/LICENSE
--rw-r--r--   0        0        0     4976 2023-04-14 13:11:30.987608 scaleway_functions_python-0.1.1/README.md
--rw-r--r--   0        0        0     2298 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/__init__.py
--rw-r--r--   0        0        0       23 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/framework/__init__.py
--rw-r--r--   0        0        0       29 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/framework/v1/__init__.py
--rw-r--r--   0        0        0     1370 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/framework/v1/hints.py
--rw-r--r--   0        0        0       52 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/__init__.py
--rw-r--r--   0        0        0      341 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/context.py
--rw-r--r--   0        0        0     1421 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/event.py
--rw-r--r--   0        0        0     1263 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/infra.py
--rw-r--r--   0        0        0     6104 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/serving.py
--rw-r--r--   0        0        0     6302 1970-01-01 00:00:00.000000 scaleway_functions_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      602 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4976 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/README.md
+-rw-r--r--   0        0        0     2298 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      189 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/framework/__init__.py
+-rw-r--r--   0        0        0       29 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/framework/v1/__init__.py
+-rw-r--r--   0        0        0     1370 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/framework/v1/hints.py
+-rw-r--r--   0        0        0      116 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/local/__init__.py
+-rw-r--r--   0        0        0      341 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/local/context.py
+-rw-r--r--   0        0        0     1421 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/local/event.py
+-rw-r--r--   0        0        0     1263 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/local/infra.py
+-rw-r--r--   0        0        0     7536 2023-04-27 08:01:54.075834 scaleway_functions_python-0.2.0/scaleway_functions_python/local/serving.py
+-rw-r--r--   0        0        0     6302 1970-01-01 00:00:00.000000 scaleway_functions_python-0.2.0/PKG-INFO
```

### Comparing `scaleway_functions_python-0.1.1/LICENSE` & `scaleway_functions_python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.1/README.md` & `scaleway_functions_python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.1/pyproject.toml` & `scaleway_functions_python-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway-functions-python"
-version = "0.1.1"
+version = "0.2.0"
 description = "Utilities for testing your Python handlers for Scaleway Serverless Functions."
 authors = ["Scaleway Serverless Team <opensource@scaleway.com>"]
 
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/scaleway/serverless-functions-python"
```

### Comparing `scaleway_functions_python-0.1.1/scaleway_functions_python/framework/v1/hints.py` & `scaleway_functions_python-0.2.0/scaleway_functions_python/framework/v1/hints.py`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.1/scaleway_functions_python/local/event.py` & `scaleway_functions_python-0.2.0/scaleway_functions_python/local/event.py`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.1/scaleway_functions_python/local/infra.py` & `scaleway_functions_python-0.2.0/scaleway_functions_python/local/infra.py`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.1/scaleway_functions_python/local/serving.py` & `scaleway_functions_python-0.2.0/scaleway_functions_python/local/serving.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from base64 import b64decode
 from json import JSONDecodeError
-from typing import TYPE_CHECKING, Any, ClassVar, cast
+from typing import TYPE_CHECKING, Any, ClassVar, List, Optional, cast
 
 from flask import Flask, json, jsonify, make_response, request
 from flask.views import View
 
 from ..local import infra
 from ..local.context import format_context
 from ..local.event import format_http_event
@@ -14,15 +14,15 @@
     from flask.wrappers import Request as FlaskRequest
     from flask.wrappers import Response as FlaskResponse
 
     from ..framework.v1 import hints
 
 # TODO?: Switch to https://docs.python.org/3/library/http.html#http-methods
 # for Python 3.11+
-HTTP_METHODS = [
+ALL_HTTP_METHODS = [
     "GET",
     "HEAD",
     "POST",
     "PUT",
     "DELETE",
     "CONNECT",
     "OPTIONS",
@@ -140,25 +140,65 @@
         resp.headers.add("Access-Control-Allow-Headers", "Content-Type")
 
         resp.headers.update(record.get("headers") or {})
 
         return resp
 
 
-def _create_flask_app(handler: "hints.Handler") -> Flask:
-    app = Flask(f"serverless_local_{handler.__name__}")
+class LocalFunctionServer:
+    """LocalFunctionServer serves Scaleway FaaS handlers on a local http server."""
 
-    # Create the view from the handler
-    view = HandlerWrapper(handler).as_view(handler.__name__, handler)
+    def __init__(self) -> None:
+        self.app = Flask("serverless_local")
 
-    # By default, methods contains ["GET", "HEAD", "OPTIONS"]
-    app.add_url_rule("/<path:path>", methods=HTTP_METHODS, view_func=view)
-    app.add_url_rule("/", methods=HTTP_METHODS, defaults={"path": ""}, view_func=view)
+    def add_handler(
+        self,
+        handler: "hints.Handler",
+        relative_url: Optional[str] = None,
+        http_methods: Optional[List[str]] = None,
+    ) -> "LocalFunctionServer":
+        """Add a handler to be served by the server.
+
+        :param handler: serverless python handler
+        :param relative_url: path to the handler, defaults to / + handler's name
+        :param http_methods: HTTP methods for the handler, defaults to all methods
+        """
+        relative_url = relative_url if relative_url else "/" + handler.__name__
+        if not relative_url.startswith("/"):
+            relative_url = "/" + relative_url
+
+        http_methods = http_methods if http_methods else ALL_HTTP_METHODS
+        http_methods = [method.upper() for method in http_methods]
+
+        view = HandlerWrapper(handler).as_view(handler.__name__, handler)
+
+        # By default, methods contains ["GET", "HEAD", "OPTIONS"]
+        self.app.add_url_rule(
+            f"{relative_url}/<path:path>", methods=http_methods, view_func=view
+        )
+        self.app.add_url_rule(
+            relative_url,
+            methods=http_methods,
+            defaults={"path": ""},
+            view_func=view,
+        )
+
+        return self
+
+    def serve(
+        self, *args: Any, port: int = 8080, debug: bool = True, **kwargs: Any
+    ) -> None:
+        """Serve the added FaaS handlers.
 
-    return app
+        :param port: port that the server should listen on, defaults to 8080
+        :param debug: run Flask in debug mode, enables hot-reloading and stack trace.
+        """
+        kwargs["port"] = port
+        kwargs["debug"] = debug
+        self.app.run(*args, **kwargs)
 
 
 def serve_handler(
     handler: "hints.Handler",
     *args: Any,
     port: int = 8080,
     debug: bool = True,
@@ -171,11 +211,10 @@
     :param debug: run Flask in debug mode, enables hot-reloading and stack trace.
 
     Example:
         >>> def handle(event, _context):
         ...     return {"body": event["httpMethod"]}
         >>> serve_handler_locally(handle, port=8080)
     """
-    app: Flask = _create_flask_app(handler)
-    kwargs["port"] = port
-    kwargs["debug"] = debug
-    app.run(*args, **kwargs)
+    server = LocalFunctionServer()
+    server.add_handler(handler=handler, relative_url="/")
+    server.serve(*args, port=port, debug=debug, **kwargs)
```

### Comparing `scaleway_functions_python-0.1.1/PKG-INFO` & `scaleway_functions_python-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-functions-python
-Version: 0.1.1
+Version: 0.2.0
 Summary: Utilities for testing your Python handlers for Scaleway Serverless Functions.
 Home-page: https://github.com/scaleway/serverless-functions-python
 License: MIT
 Keywords: serverless,scaleway,functions,cloud,faas
 Author: Scaleway Serverless Team
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8.1,<3.12
```

