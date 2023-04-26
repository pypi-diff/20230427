# Comparing `tmp/pyensign-0.1a1.tar.gz` & `tmp/pyensign-0.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyensign-0.1a1.tar", last modified: Fri Mar 31 22:48:47 2023, max compression
+gzip compressed data, was "pyensign-0.6b0.tar", last modified: Wed Apr 26 21:53:45 2023, max compression
```

## Comparing `pyensign-0.1a1.tar` & `pyensign-0.6b0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.357025 pyensign-0.1a1/
--rw-r--r--   0 patrick    (501) staff       (20)     1329 2023-03-31 21:19:30.000000 pyensign-0.1a1/DESCRIPTION.md
--rw-r--r--   0 patrick    (501) staff       (20)      180 2023-03-31 22:11:32.000000 pyensign-0.1a1/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)      394 2023-03-29 13:11:36.000000 pyensign-0.1a1/Makefile
--rw-r--r--   0 patrick    (501) staff       (20)     2577 2023-03-31 22:48:47.357146 pyensign-0.1a1/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     2788 2023-03-31 22:41:57.000000 pyensign-0.1a1/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.351668 pyensign-0.1a1/pyensign/
--rw-r--r--   0 patrick    (501) staff       (20)      507 2023-03-29 13:11:36.000000 pyensign-0.1a1/pyensign/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.354097 pyensign-0.1a1/pyensign/api/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-31 22:18:49.000000 pyensign-0.1a1/pyensign/api/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.355872 pyensign-0.1a1/pyensign/api/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-23 14:22:39.000000 pyensign-0.1a1/pyensign/api/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     5078 2023-03-23 16:52:53.000000 pyensign-0.1a1/pyensign/api/v1beta1/ensign_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)    17926 2023-03-23 16:52:53.000000 pyensign-0.1a1/pyensign/api/v1beta1/ensign_pb2_grpc.py
--rw-r--r--   0 patrick    (501) staff       (20)     2718 2023-03-23 16:52:53.000000 pyensign-0.1a1/pyensign/api/v1beta1/event_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-03-23 14:22:40.000000 pyensign-0.1a1/pyensign/api/v1beta1/groups_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     4296 2023-03-23 16:52:53.000000 pyensign-0.1a1/pyensign/api/v1beta1/topic_pb2.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.356272 pyensign-0.1a1/pyensign/auth/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-31 22:18:28.000000 pyensign-0.1a1/pyensign/auth/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2603 2023-03-23 23:25:41.000000 pyensign-0.1a1/pyensign/auth/client.py
--rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-03-31 14:40:41.000000 pyensign-0.1a1/pyensign/connection.py
--rw-r--r--   0 patrick    (501) staff       (20)     7856 2023-03-31 21:19:30.000000 pyensign-0.1a1/pyensign/ensign.py
--rw-r--r--   0 patrick    (501) staff       (20)     1917 2023-03-31 21:19:30.000000 pyensign-0.1a1/pyensign/events.py
--rw-r--r--   0 patrick    (501) staff       (20)     3351 2023-03-30 12:50:26.000000 pyensign-0.1a1/pyensign/exceptions.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.356488 pyensign-0.1a1/pyensign/mimetype/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-31 22:18:57.000000 pyensign-0.1a1/pyensign/mimetype/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.356835 pyensign-0.1a1/pyensign/mimetype/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-23 14:22:40.000000 pyensign-0.1a1/pyensign/mimetype/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-03-23 14:22:40.000000 pyensign-0.1a1/pyensign/mimetype/v1beta1/mimetype_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)      965 2023-03-31 22:48:34.000000 pyensign-0.1a1/pyensign/version.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-03-31 22:48:47.353747 pyensign-0.1a1/pyensign.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)     2577 2023-03-31 22:48:47.000000 pyensign-0.1a1/pyensign.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)      807 2023-03-31 22:48:47.000000 pyensign-0.1a1/pyensign.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-03-31 22:48:47.000000 pyensign-0.1a1/pyensign.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-03-31 22:48:47.000000 pyensign-0.1a1/pyensign.egg-info/not-zip-safe
--rw-r--r--   0 patrick    (501) staff       (20)       68 2023-03-31 22:48:47.000000 pyensign-0.1a1/pyensign.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        9 2023-03-31 22:48:47.000000 pyensign-0.1a1/pyensign.egg-info/top_level.txt
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-10 20:05:11.000000 pyensign-0.1a1/pyproject.toml
--rw-r--r--   0 patrick    (501) staff       (20)       67 2023-03-31 22:21:35.000000 pyensign-0.1a1/requirements.txt
--rw-r--r--   0 patrick    (501) staff       (20)       38 2023-03-31 22:48:47.357472 pyensign-0.1a1/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-03-31 22:42:46.000000 pyensign-0.1a1/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.953862 pyensign-0.6b0/
+-rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-04-19 19:47:14.000000 pyensign-0.6b0/CONTRIBUTING.md
+-rw-r--r--   0 patrick    (501) staff       (20)     1329 2023-03-31 21:19:30.000000 pyensign-0.6b0/DESCRIPTION.md
+-rw-r--r--   0 patrick    (501) staff       (20)      180 2023-04-07 12:54:37.000000 pyensign-0.6b0/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)      394 2023-03-29 13:11:36.000000 pyensign-0.6b0/Makefile
+-rw-r--r--   0 patrick    (501) staff       (20)     2577 2023-04-26 21:53:45.953994 pyensign-0.6b0/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     3307 2023-04-19 19:47:14.000000 pyensign-0.6b0/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.948073 pyensign-0.6b0/pyensign/
+-rw-r--r--   0 patrick    (501) staff       (20)      507 2023-03-29 13:11:36.000000 pyensign-0.6b0/pyensign/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.950103 pyensign-0.6b0/pyensign/api/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-04-07 12:54:37.000000 pyensign-0.6b0/pyensign/api/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.951859 pyensign-0.6b0/pyensign/api/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-23 14:22:39.000000 pyensign-0.6b0/pyensign/api/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5078 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)    17926 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2718 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/event_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-03-23 14:22:40.000000 pyensign-0.6b0/pyensign/api/v1beta1/groups_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4296 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/topic_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.952515 pyensign-0.6b0/pyensign/auth/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-04-07 12:54:37.000000 pyensign-0.6b0/pyensign/auth/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3937 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/auth/client.py
+-rw-r--r--   0 patrick    (501) staff       (20)      347 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/auth/tokens.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-03-31 14:40:41.000000 pyensign-0.6b0/pyensign/connection.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8844 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/ensign.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1917 2023-03-31 21:19:30.000000 pyensign-0.6b0/pyensign/events.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3602 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/exceptions.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.952729 pyensign-0.6b0/pyensign/mimetype/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-04-07 12:54:37.000000 pyensign-0.6b0/pyensign/mimetype/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.953204 pyensign-0.6b0/pyensign/mimetype/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-23 14:22:40.000000 pyensign-0.6b0/pyensign/mimetype/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-03-23 14:22:40.000000 pyensign-0.6b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.953459 pyensign-0.6b0/pyensign/utils/
+-rw-r--r--   0 patrick    (501) staff       (20)      983 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/utils/cache.py
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-04-26 21:49:48.000000 pyensign-0.6b0/pyensign/version.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.949869 pyensign-0.6b0/pyensign.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     2577 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)      871 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/not-zip-safe
+-rw-r--r--   0 patrick    (501) staff       (20)       81 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-10 20:05:11.000000 pyensign-0.6b0/pyproject.toml
+-rw-r--r--   0 patrick    (501) staff       (20)       80 2023-04-26 21:48:16.000000 pyensign-0.6b0/requirements.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-04-26 21:53:45.954318 pyensign-0.6b0/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-03-31 22:42:46.000000 pyensign-0.6b0/setup.py
```

### Comparing `pyensign-0.1a1/DESCRIPTION.md` & `pyensign-0.6b0/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/PKG-INFO` & `pyensign-0.6b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.1a1
+Version: 0.6b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.1a1
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.6b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
```

### Comparing `pyensign-0.1a1/README.md` & `pyensign-0.6b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,84 @@
 # pyensign
 Welcome to pyensign!
 
 This repository contains the Ensign driver, SDK, and helpers for Python. For the main ensign repo, go [here](https://github.com/rotationalio/ensign). We also have SDKs for [Javascript](https://github.com/rotationalio/ensignjs) and [Go](https://github.com/rotationalio/goensign).
 
-## Dependencies
+## Installation
 
-The project dependencies can be installed with pip.
+PyEnsign is compatible with Python >= 3.7 (Note: we can't guarantee PyEnsign's compatibility with earlier versions of Python due to PyEnsign's dependence on the [`grpcio` package](https://pypi.org/project/grpcio/)). The simplest way to install PyEnsign and its dependencies is from PyPI with pip, Python's preferred package installer.
 
 ```
-$ pip install -r requirements.txt
-```
-
-If you wish to run the tests, you must install the test dependencies instead.
-
-```
-$ pip install -r tests/requirements.txt
+pip install pyensign
 ```
 
 ## Configuration
 
 The `Ensign` client provides access to the unified API for managing topics and publishing/subscribing to topics. Creating a client requires a client ID and client secret (your API key).
 
 ```python
 from pyensign.ensign import Ensign
 
 client = Ensign(client_id=<your client ID>, client_secret=<your client secret>)
 ```
 
 If not provided the client ID and client secret will be obtained from the `ENSIGN_CLIENT_ID` and `ENSIGN_CLIENT_SECRET` environment variables.
 
-## Publishing
+## Getting to know the PyEnsign API
+
+The sample code below describes some of the core PyEnsign API, but if you're looking for a minimal end-to-example, [check this out first](https://github.com/rotationalio/ensign-examples/tree/main/python/minimal).
+
+### Publishing
 
 Use `Ensign.publish()` to publish events to a topic. All events must contain some data and a mimetype. If the topic doesn't exist in your project, it will be automatically created.
 
 ```python
 from pyensign.events import Event
 
 # Publishing a single event
 event = Event(b'{"temp": 72, "units": "fahrenheit"}', "APPLICATION_JSON")
 await client.publish("weather", event)
 
-# Publishing mulitple events
+# Publishing multiple events
 events = [
-    Event(b'{"temp": 72, "units": "fahrenheit"}', "APPLICATION_JSON")
+    Event(b'{"temp": 72, "units": "fahrenheit"}', "APPLICATION_JSON"),
     Event(b'{"temp": 76, "units": "fahrenheit"}', "APPLICATION_JSON")
 ]
 await client.publish("weather", events)
 ```
 
-## Subscribing
+### Subscribing
 
 Use `Ensign.subscribe()` to subscribe to one or more topics.
 
 ```python
 async for event in client.subscribe("weather", "forecast")
     print("Received event: {}".format(event))
 ```
 
-## Design patterns
+### Design patterns
 
 Most event-driven applications require some form of concurrency. Therefore, the `Ensign` class is designed to be used asynchronously by defining coroutines. You can use Python's builtin `asyncio` package to schedule and run coroutines from the main thread.
 
 ```python
 import asyncio
 from pyensign.ensign import Ensign
 
 async def subscriber(topic):
     ...
 
     async for event in client.subscribe(topic):
         # Do something with the event
 
 def main():
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(subscriber("weather"))
+    asyncio.run(subscribe(topic))
 ```
 
-## Building the protocol buffers
+## Contributing to PyEnsign
 
-This repo relies on [protocol buffers](https://protobuf.dev/) for code generation. If you need to rebuild the protocol buffers, clone the ensign repo to the parent directory.
+Wow, you want to contribute to PyEnsign? 😍 We would absolutely love that!
 
-```bash
-$ git clone git@github.com:rotationalio/ensign.git ../ensign
-```
+PyEnsign is an open source project that is supported by a community who will gratefully and humbly accept any contributions you might make to the project. Large or small, any contribution makes a big difference; and if you've never contributed to an open source project before, we hope you will start with PyEnsign!
 
-Then run make to build the protocol buffers from the .proto definitions.
+Please check out our Contributor's Guide in `CONTRIBUTING.md` to get a quick orientation first.
 
-```
-$ make grpc
-```
+We can't wait to hear from you!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyensign-0.1a1/pyensign/api/v1beta1/ensign_pb2.py` & `pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/api/v1beta1/ensign_pb2_grpc.py` & `pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/api/v1beta1/event_pb2.py` & `pyensign-0.6b0/pyensign/api/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/api/v1beta1/groups_pb2.py` & `pyensign-0.6b0/pyensign/api/v1beta1/groups_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/api/v1beta1/topic_pb2.py` & `pyensign-0.6b0/pyensign/api/v1beta1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/auth/client.py` & `pyensign-0.6b0/pyensign/auth/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import grpc
+import time
 import requests
 
 from pyensign.exceptions import AuthenticationError
+from pyensign.auth.tokens import expires_at, not_before
 
 ACCESS_TOKEN = "access_token"
 REFRESH_TOKEN = "refresh_token"
 
 
 class AuthClient(grpc.AuthMetadataPlugin):
     """
@@ -34,38 +36,76 @@
         self._access_token = ""
         self._refresh_token = ""
         self._last_login = None
 
     def __call__(self, _, callback):
         """
         gRPC callback to add the access token on each request.
+        TODO: Refresh credentials in the background to avoid blocking RPC calls
         """
-        # TODO: If access token is expired, refresh instead
-        exception = None
         meta = []
-        if not self._access_token:
-            try:
-                self.authenticate()
-            except AuthenticationError as e:
-                exception = e
-        if not exception:
-            meta.append(("authorization", "Bearer " + self._access_token))
+        exception = None
+        try:
+            meta.append(self.credentials())
+        except AuthenticationError as e:
+            exception = e
         callback(meta, exception)
 
+    def credentials(self):
+        """
+        Returns the list of credentials to use for token-based authentication. This
+        uses the tokens that are already available if possible, otherwise this function
+        will attempt to request tokens from the authentication server.
+        """
+
+        # If tokens are missing or parital, authenticate
+        if not self._access_token or not self._refresh_token:
+            self.authenticate()
+
+        # Refresh the access token if not valid
+        if not self._access_valid():
+            # If refresh is valid then it can be used to get a new access token
+            # Otherwise, full authentication is required
+            if self._refresh_valid():
+                self.refresh()
+            else:
+                self.authenticate()
+
+        # Return the credentials
+        return ("authorization", "Bearer " + self._access_token)
+
     def authenticate(self):
-        # TODO: Check if access token is expired
         self._do(self.url + "/v1/authenticate", self.creds)
 
     def refresh(self):
-        # TODO: Check if refresh token is expired
         if not self._refresh_token:
             raise AuthenticationError("No refresh token available")
         body = {"refresh_token": self._refresh_token}
         self._do(self.url + "/v1/refresh", body)
 
+    def _access_valid(self):
+        """
+        Returns True if the access token is not expired.
+        """
+        if not self._access_token:
+            return False
+        return time.time() < expires_at(self._access_token)
+
+    def _refresh_valid(self):
+        """
+        Returns True if the refresh token has not expired and it is after the not
+        before time.
+        """
+        if not self._refresh_token:
+            return False
+        now = time.time()
+        return now > not_before(self._refresh_token) and now < expires_at(
+            self._refresh_token
+        )
+
     def _do(self, url, body):
         response = requests.post(url, json=body)
         if response.status_code != 200:
             raise AuthenticationError(
                 "Failed to authenticate with API credentials: %s" % response.text
             )
         rep = response.json()
```

### Comparing `pyensign-0.1a1/pyensign/connection.py` & `pyensign-0.6b0/pyensign/connection.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/ensign.py` & `pyensign-0.6b0/pyensign/ensign.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import os
 from ulid import ULID
 
 from pyensign.connection import Client
+from pyensign.utils.cache import Cache
 from pyensign.connection import Connection
 from pyensign.api.v1beta1 import topic_pb2
 from pyensign.auth.client import AuthClient
-from pyensign.exceptions import EnsignResponseType, EnsignTopicCreateError
+from pyensign.exceptions import (
+    CacheMissError,
+    EnsignResponseType,
+    EnsignTopicCreateError,
+    EnsignTopicNotFoundError,
+)
 
 
 class Ensign:
     """
     Ensign connects to an Ensign server and provides access to the Ensign API.
     """
 
     def __init__(
         self,
         client_id="",
         client_secret="",
         endpoint="ensign.rotational.app:443",
         insecure=False,
         auth_url="https://auth.rotational.app",
+        disable_topic_cache=False,
     ):
         """
         Create a new Ensign client with API credentials.
 
         Parameters
         ----------
         client_id : str
@@ -34,14 +41,16 @@
             is loaded from the ENSIGN_CLIENT_SECRET environment variable.
         endpoint : str (optional)
             The endpoint of the Ensign server.
         insecure : bool (optional)
             Set to True to use an insecure connection.
         auth_url : str (optional)
             The URL of the Ensign authentication server.
+        disable_topic_cache: bool (optional)
+            Set to True to disable topic ID caching.
         """
 
         if not client_id or client_id == "":
             client_id = os.environ.get("ENSIGN_CLIENT_ID")
         if not client_secret or client_secret == "":
             client_secret = os.environ.get("ENSIGN_CLIENT_SECRET")
         if client_id is None:
@@ -58,14 +67,19 @@
             raise TypeError("client_secret must be a string")
 
         creds = {"client_id": client_id, "client_secret": client_secret}
         auth = AuthClient(auth_url, creds)
         connection = Connection(addrport=endpoint, insecure=insecure, auth=auth)
         self.client = Client(connection)
 
+        if disable_topic_cache:
+            self.topics = None
+        else:
+            self.topics = Cache()
+
     async def publish(self, topic_name, *events):
         """
         Publish events to an Ensign topic.
 
         Parameters
         ----------
         topic_name : str
@@ -77,19 +91,19 @@
 
         if topic_name == "":
             raise ValueError("topic_name is required")
 
         if len(events) == 0:
             raise ValueError("no events provided")
 
-        # Get the topic ID from the topic name
-        topic_id = await self.topic_id(topic_name)
-
-        # Ensure the topic exists
-        if topic_id == "":
+        # Ensure the topic ID exists by getting or creating it
+        topic_id = ""
+        try:
+            topic_id = await self.topic_id(topic_name)
+        except EnsignTopicNotFoundError:
             topic = await self.create_topic(topic_name)
             topic_id = str(ULID.from_bytes(topic.id))
 
         # TODO: Support user-defined generators
         def next():
             for event in events:
                 yield event.proto(topic_id)
@@ -212,29 +226,42 @@
         ----------
         name: str
             The name of the topic.
 
         Returns
         -------
         str
-            The ID of the topic or None.
+            The ID of the topic.
+
+        Raises
+        ------
+        EnsignTopicNotFoundError
         """
 
-        # TODO: cache topic IDs to avoid repeated API calls
+        # Attempt to get the topic ID from the cache
+        if self.topics is not None:
+            try:
+                return self.topics.get(name)
+            except CacheMissError:
+                pass
 
+        # Get the topic ID from Ensign
         page = None
         token = ""
         while page is None or token != "":
             # TODO: We could use topic_names but it currently requires hashing the
             # topic name with murmur3.
             page, token = await self.client.list_topics(next_page_token=token)
             for topic in page:
                 if topic.name == name:
-                    return str(ULID(topic.id))
-        return ""
+                    id = str(ULID(topic.id))
+                    if self.topics is not None:
+                        self.topics.add(name, id)
+                    return id
+        raise EnsignTopicNotFoundError(f"topic not found by name: {name}")
 
     async def topic_exists(self, name):
         """
         Check if a topic exists by name.
 
         Parameters
         ----------
@@ -243,14 +270,19 @@
 
         Returns
         -------
         bool
             True if the topic exists, False otherwise.
         """
 
+        # Attempt to check existence using the cache
+        if self.topics is not None and self.topics.exists(name):
+            return True
+
+        # Check existence using Ensign
         _, exists = await self.client.topic_exists(topic_name=name)
         return exists
 
     async def status(self):
         """
         Check the status of the Ensign server.
```

### Comparing `pyensign-0.1a1/pyensign/events.py` & `pyensign-0.6b0/pyensign/events.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/exceptions.py` & `pyensign-0.6b0/pyensign/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,22 @@
     """
     Raised when PyEnsign fails to authenticate with the Auth server
     """
 
     pass
 
 
+class CacheMissError(PyEnsignError):
+    """
+    Raised when PyEnsign fails to find a cached value
+    """
+
+    pass
+
+
 class EnsignError(PyEnsignError):
     """
     Raised when PyEnsign receives an error from the Ensign server
     """
 
     pass
 
@@ -145,7 +153,15 @@
 
 class EnsignTopicCreateError(EnsignError):
     """
     Raised when Ensign failed to create a topic
     """
 
     pass
+
+
+class EnsignTopicNotFoundError(EnsignError):
+    """
+    Raised when a topic could not be retrieved from Ensign
+    """
+
+    pass
```

### Comparing `pyensign-0.1a1/pyensign/mimetype/v1beta1/mimetype_pb2.py` & `pyensign-0.6b0/pyensign/mimetype/v1beta1/mimetype_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.1a1/pyensign/version.py` & `pyensign-0.6b0/pyensign/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
-    "minor": 1,
+    "minor": 6,
     "micro": 0,
-    "releaselevel": "alpha",
-    "serial": 1,
+    "releaselevel": "beta",
+    "serial": 0,
 }
 
 ##########################################################################
 ## Helper Functions
 ##########################################################################
```

### Comparing `pyensign-0.1a1/pyensign.egg-info/PKG-INFO` & `pyensign-0.6b0/pyensign.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.1a1
+Version: 0.6b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.1a1
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.6b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
```

### Comparing `pyensign-0.1a1/pyensign.egg-info/SOURCES.txt` & `pyensign-0.6b0/pyensign.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CONTRIBUTING.md
 DESCRIPTION.md
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
@@ -23,10 +24,12 @@
 pyensign/api/v1beta1/ensign_pb2.py
 pyensign/api/v1beta1/ensign_pb2_grpc.py
 pyensign/api/v1beta1/event_pb2.py
 pyensign/api/v1beta1/groups_pb2.py
 pyensign/api/v1beta1/topic_pb2.py
 pyensign/auth/__init__.py
 pyensign/auth/client.py
+pyensign/auth/tokens.py
 pyensign/mimetype/__init__.py
 pyensign/mimetype/v1beta1/__init__.py
-pyensign/mimetype/v1beta1/mimetype_pb2.py
+pyensign/mimetype/v1beta1/mimetype_pb2.py
+pyensign/utils/cache.py
```

### Comparing `pyensign-0.1a1/setup.py` & `pyensign-0.6b0/setup.py`

 * *Files identical despite different names*

