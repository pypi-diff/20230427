# Comparing `tmp/pysnc-1.1.1.tar.gz` & `tmp/pysnc-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.1.tar", max compression
+gzip compressed data, was "pysnc-1.1.2.tar", max compression
```

## Comparing `pysnc-1.1.1.tar` & `pysnc-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2023-04-26 00:41:10.768887 pysnc-1.1.1/LICENSE
--rw-r--r--   0        0        0     1590 2023-04-26 00:41:10.768887 pysnc-1.1.1/README.md
--rw-r--r--   0        0        0      984 2023-04-26 00:41:10.772887 pysnc-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      129 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/__version__.py
--rw-r--r--   0        0        0     8875 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/attachment.py
--rw-r--r--   0        0        0     3778 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/auth.py
--rw-r--r--   0        0        0    15782 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/client.py
--rw-r--r--   0        0        0     1002 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/exceptions.py
--rw-r--r--   0        0        0     3809 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/query.py
--rw-r--r--   0        0        0    37242 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/record.py
--rw-r--r--   0        0        0      846 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/utils.py
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 pysnc-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-04-26 23:06:05.738981 pysnc-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1590 2023-04-26 23:06:05.738981 pysnc-1.1.2/README.md
+-rw-r--r--   0        0        0      984 2023-04-26 23:06:05.742981 pysnc-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/__version__.py
+-rw-r--r--   0        0        0     8875 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/attachment.py
+-rw-r--r--   0        0        0     3778 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/auth.py
+-rw-r--r--   0        0        0    15569 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/exceptions.py
+-rw-r--r--   0        0        0     3809 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/query.py
+-rw-r--r--   0        0        0    37242 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/record.py
+-rw-r--r--   0        0        0      846 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/utils.py
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 pysnc-1.1.2/PKG-INFO
```

### Comparing `pysnc-1.1.1/LICENSE` & `pysnc-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/README.md` & `pysnc-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/pyproject.toml` & `pysnc-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.1"
+version = "1.1.2"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
```

### Comparing `pysnc-1.1.1/pysnc/attachment.py` & `pysnc-1.1.2/pysnc/attachment.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/pysnc/auth.py` & `pysnc-1.1.2/pysnc/auth.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/pysnc/client.py` & `pysnc-1.1.2/pysnc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,23 +315,18 @@
         if prepared.body:
             now_request['body'] = base64.b64encode(prepared.body).decode()
         self.__hooks[request_id] = hook
         self.__stored_requests[request_id] = prepared
         self.__requests.append(now_request)
 
     def _transform_response(self, req: requests.PreparedRequest, serviced_request) -> requests.Response:
-        #if 'body' in serviced_request:
-        #    serviced_request['body'] = base64.b64decode(serviced_request['body'])
-
         # modeled after requests.adapters.HttpAdapter.build_response
         response = requests.Response()
         response.status_code = serviced_request['status_code']
         headers = {k: v for (k, v) in [(e['name'], e['value']) for e in serviced_request.get("headers", [])]}
-        print(serviced_request)
-        print(headers)
         response.headers = CaseInsensitiveDict(headers)
         response.encoding = get_encoding_from_headers(response.headers)
 
         body = base64.b64decode(serviced_request.get('body', ''))
         response.raw = BytesIO(body)
 
         if isinstance(req.url, bytes):
@@ -345,16 +340,14 @@
         response.cookies.extract_cookies(res, req)
 
         response.req = req
         # response.connection = None
 
         return response
 
-        #return serviced_request
-
     def execute(self):
         bid = self._next_id()
         body = {
             'batch_request_id': bid,
             'rest_requests': self.__requests
         }
         r = self.session.post(self._batch_target(), json=body)
```

### Comparing `pysnc-1.1.1/pysnc/exceptions.py` & `pysnc-1.1.2/pysnc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/pysnc/query.py` & `pysnc-1.1.2/pysnc/query.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/pysnc/record.py` & `pysnc-1.1.2/pysnc/record.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/pysnc/utils.py` & `pysnc-1.1.2/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.1/PKG-INFO` & `pysnc-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
```

