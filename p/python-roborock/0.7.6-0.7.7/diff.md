# Comparing `tmp/python_roborock-0.7.6.tar.gz` & `tmp/python_roborock-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.7.6.tar", max compression
+gzip compressed data, was "python_roborock-0.7.7.tar", max compression
```

## Comparing `python_roborock-0.7.6.tar` & `python_roborock-0.7.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-26 17:59:05.013439 python_roborock-0.7.6/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-26 17:59:05.013439 python_roborock-0.7.6/README.md
--rw-r--r--   0        0        0     1370 2023-04-26 17:59:05.897431 python_roborock-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/__init__.py
--rw-r--r--   0        0        0    19297 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/cli.py
--rw-r--r--   0        0        0     8241 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/cloud_api.py
--rw-r--r--   0        0        0     4329 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/code_mappings.py
--rw-r--r--   0        0        0     9872 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/exceptions.py
--rw-r--r--   0        0        0     6194 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/roborock_future.py
--rw-r--r--   0        0        0     6232 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/roborock_message.py
--rw-r--r--   0        0        0    12046 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/typing.py
--rw-r--r--   0        0        0      783 2023-04-26 17:59:05.013439 python_roborock-0.7.6/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 22:55:35.577039 python_roborock-0.7.7/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-26 22:55:35.577039 python_roborock-0.7.7/README.md
+-rw-r--r--   0        0        0     1370 2023-04-26 22:55:36.497046 python_roborock-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-26 22:55:35.577039 python_roborock-0.7.7/roborock/__init__.py
+-rw-r--r--   0        0        0    19297 2023-04-26 22:55:35.577039 python_roborock-0.7.7/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-26 22:55:35.577039 python_roborock-0.7.7/roborock/cli.py
+-rw-r--r--   0        0        0     8241 2023-04-26 22:55:35.577039 python_roborock-0.7.7/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4329 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9872 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/exceptions.py
+-rw-r--r--   0        0        0     6321 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6232 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12046 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/typing.py
+-rw-r--r--   0        0        0      783 2023-04-26 22:55:35.581039 python_roborock-0.7.7/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.7/PKG-INFO
```

### Comparing `python_roborock-0.7.6/LICENSE` & `python_roborock-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/README.md` & `python_roborock-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/pyproject.toml` & `python_roborock-0.7.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.7.6"
+version = "0.7.7"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.7.6/roborock/api.py` & `python_roborock-0.7.7/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/cli.py` & `python_roborock-0.7.7/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/cloud_api.py` & `python_roborock-0.7.7/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/code_mappings.py` & `python_roborock-0.7.7/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/containers.py` & `python_roborock-0.7.7/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/exceptions.py` & `python_roborock-0.7.7/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/local_api.py` & `python_roborock-0.7.7/roborock/local_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,15 @@
             timestamp=timestamp,
             protocol=request_protocol,
             payload=payload,
         )
 
     async def send_command(self, device_id: str, method: RoborockCommand, params: Optional[list] = None):
         roborock_message = self.build_roborock_message(method, params)
-        response = (await self.send_message(device_id, roborock_message))[0]
-        if isinstance(response, BaseException):
-            raise response
-        return response
+        return (await self.send_message(device_id, roborock_message))[0]
 
     async def async_local_response(self, roborock_message: RoborockMessage):
         request_id = roborock_message.get_request_id()
         if request_id is not None:
             # response_protocol = 5 if roborock_message.prefix == secured_prefix else 4
             response_protocol = 4
             (response, err) = await self._async_response(request_id, response_protocol)
@@ -85,18 +82,23 @@
         # Send the command to the Roborock device
         listener = self.device_listener.get(device_id)
         if listener is None:
             raise RoborockException(f"No device listener for {device_id}")
         _LOGGER.debug(f"Requesting device with {roborock_messages}")
         await listener.send_message(msg)
 
-        return await asyncio.gather(
+        responses = await asyncio.gather(
             *[self.async_local_response(roborock_message) for roborock_message in roborock_messages],
             return_exceptions=True,
         )
+        exception = next((response for response in responses if isinstance(response, BaseException)), None)
+        if exception:
+            listener.disconnect()
+            raise exception
+        return responses
 
 
 class RoborockSocket(socket.socket):
     _closed = None
 
     @property
     def is_closed(self):
@@ -126,15 +128,15 @@
             message = self.remaining + message
             self.remaining = b""
         (parser_msg, remaining) = RoborockParser.decode(message, self.local_key)
         self.remaining = remaining
         self.on_message(parser_msg)
 
     def connection_lost(self, exc):
-        print("The server closed the connection")
+        _LOGGER.debug("The server closed the connection")
 
     def is_connected(self):
         return self.transport and self.transport.is_reading()
 
     async def connect(self):
         try:
             if not self.is_connected():
```

### Comparing `python_roborock-0.7.6/roborock/roborock_future.py` & `python_roborock-0.7.7/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/roborock_message.py` & `python_roborock-0.7.7/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/typing.py` & `python_roborock-0.7.7/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/roborock/util.py` & `python_roborock-0.7.7/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.6/PKG-INFO` & `python_roborock-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.7.6
+Version: 0.7.7
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.7.6 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.7.7 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

