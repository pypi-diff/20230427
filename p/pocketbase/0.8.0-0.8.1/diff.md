# Comparing `tmp/pocketbase-0.8.0.tar.gz` & `tmp/pocketbase-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketbase-0.8.0.tar", max compression
+gzip compressed data, was "pocketbase-0.8.1.tar", max compression
```

## Comparing `pocketbase-0.8.0.tar` & `pocketbase-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     2253 2023-02-10 18:21:38.093505 pocketbase-0.8.0/README.md
--rw-r--r--   0        0        0      304 2023-02-10 18:21:38.093505 pocketbase-0.8.0/pocketbase/__init__.py
--rw-r--r--   0        0        0     4763 2023-02-10 18:21:38.093505 pocketbase-0.8.0/pocketbase/client.py
--rw-r--r--   0        0        0      199 2023-02-10 18:21:38.093505 pocketbase-0.8.0/pocketbase/models/__init__.py
--rw-r--r--   0        0        0      363 2023-02-10 18:21:38.093505 pocketbase-0.8.0/pocketbase/models/admin.py
--rw-r--r--   0        0        0     1296 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/models/collection.py
--rw-r--r--   0        0        0      486 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/models/external_auth.py
--rw-r--r--   0        0        0      390 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/models/file_upload.py
--rw-r--r--   0        0        0      767 2022-09-19 20:46:24.192181 pocketbase-0.8.0/pocketbase/models/log_request.py
--rw-r--r--   0        0        0      711 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/models/record.py
--rw-r--r--   0        0        0      108 2022-09-15 19:31:18.390137 pocketbase-0.8.0/pocketbase/models/utils/__init__.py
--rw-r--r--   0        0        0      880 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/models/utils/base_model.py
--rw-r--r--   0        0        0      313 2022-09-19 20:45:41.510702 pocketbase-0.8.0/pocketbase/models/utils/list_result.py
--rw-r--r--   0        0        0      293 2022-09-19 20:46:03.095439 pocketbase-0.8.0/pocketbase/models/utils/schema_field.py
--rw-r--r--   0        0        0      292 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/services/__init__.py
--rw-r--r--   0        0        0     4906 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/services/admin_service.py
--rw-r--r--   0        0        0     1118 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/services/collection_service.py
--rw-r--r--   0        0        0     2048 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/services/log_service.py
--rw-r--r--   0        0        0     5186 2023-02-10 18:21:38.094505 pocketbase-0.8.0/pocketbase/services/realtime_service.py
--rw-r--r--   0        0        0     9536 2023-02-10 18:21:38.096505 pocketbase-0.8.0/pocketbase/services/record_service.py
--rw-r--r--   0        0        0     1517 2023-02-10 18:21:38.096505 pocketbase-0.8.0/pocketbase/services/settings_service.py
--rw-r--r--   0        0        0      123 2023-02-10 18:21:38.096505 pocketbase-0.8.0/pocketbase/services/utils/__init__.py
--rw-r--r--   0        0        0     3460 2023-02-10 18:21:38.097505 pocketbase-0.8.0/pocketbase/services/utils/base_crud_service.py
--rw-r--r--   0        0        0      178 2022-09-19 20:46:53.658823 pocketbase-0.8.0/pocketbase/services/utils/base_service.py
--rw-r--r--   0        0        0     1941 2023-02-10 18:21:38.097505 pocketbase-0.8.0/pocketbase/services/utils/crud_service.py
--rw-r--r--   0        0        0     4032 2022-09-26 12:03:57.885996 pocketbase-0.8.0/pocketbase/services/utils/sse.py
--rw-r--r--   0        0        0       88 2022-09-15 19:28:00.514607 pocketbase-0.8.0/pocketbase/stores/__init__.py
--rw-r--r--   0        0        0     1278 2023-02-10 18:21:38.097505 pocketbase-0.8.0/pocketbase/stores/base_auth_store.py
--rw-r--r--   0        0        0     1785 2023-02-10 18:21:38.097505 pocketbase-0.8.0/pocketbase/stores/local_auth_store.py
--rw-r--r--   0        0        0     1011 2023-02-10 18:21:38.097505 pocketbase-0.8.0/pocketbase/utils.py
--rw-r--r--   0        0        0     1605 2023-02-10 18:21:38.097505 pocketbase-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3121 1970-01-01 00:00:00.000000 pocketbase-0.8.0/setup.py
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 pocketbase-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2253 2023-04-27 00:23:48.651889 pocketbase-0.8.1/README.md
+-rw-r--r--   0        0        0      304 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/__init__.py
+-rw-r--r--   0        0        0     4763 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/client.py
+-rw-r--r--   0        0        0      199 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/__init__.py
+-rw-r--r--   0        0        0      363 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/admin.py
+-rw-r--r--   0        0        0     1296 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/collection.py
+-rw-r--r--   0        0        0      486 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/external_auth.py
+-rw-r--r--   0        0        0      390 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/file_upload.py
+-rw-r--r--   0        0        0      767 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/log_request.py
+-rw-r--r--   0        0        0      797 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/record.py
+-rw-r--r--   0        0        0      108 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/base_model.py
+-rw-r--r--   0        0        0      313 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/list_result.py
+-rw-r--r--   0        0        0      293 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/models/utils/schema_field.py
+-rw-r--r--   0        0        0      292 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/__init__.py
+-rw-r--r--   0        0        0     4906 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/admin_service.py
+-rw-r--r--   0        0        0     1118 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/collection_service.py
+-rw-r--r--   0        0        0     2048 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/log_service.py
+-rw-r--r--   0        0        0     5186 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/realtime_service.py
+-rw-r--r--   0        0        0     9534 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/record_service.py
+-rw-r--r--   0        0        0     1517 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/settings_service.py
+-rw-r--r--   0        0        0      123 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/__init__.py
+-rw-r--r--   0        0        0     3460 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/base_crud_service.py
+-rw-r--r--   0        0        0      178 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/base_service.py
+-rw-r--r--   0        0        0     1941 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/crud_service.py
+-rw-r--r--   0        0        0     4032 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/services/utils/sse.py
+-rw-r--r--   0        0        0       88 2023-04-27 00:23:48.651889 pocketbase-0.8.1/pocketbase/stores/__init__.py
+-rw-r--r--   0        0        0     1278 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pocketbase/stores/base_auth_store.py
+-rw-r--r--   0        0        0     1785 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pocketbase/stores/local_auth_store.py
+-rw-r--r--   0        0        0     1011 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pocketbase/utils.py
+-rw-r--r--   0        0        0     1605 2023-04-27 00:23:48.655889 pocketbase-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 pocketbase-0.8.1/PKG-INFO
```

### Comparing `pocketbase-0.8.0/README.md` & `pocketbase-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/client.py` & `pocketbase-0.8.1/pocketbase/client.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/models/collection.py` & `pocketbase-0.8.1/pocketbase/models/collection.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/models/log_request.py` & `pocketbase-0.8.1/pocketbase/models/log_request.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/models/record.py` & `pocketbase-0.8.1/pocketbase/models/record.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from pocketbase.models.utils.base_model import BaseModel
 from pocketbase.utils import camel_to_snake
+from dataclasses import dataclass, field
 
-
+@dataclass
 class Record(BaseModel):
     collection_id: str
-    collection_name: str
-    expand: dict
+    collection_name: str = ""
+    expand: dict = field(default_factory=dict)
 
     def load(self, data: dict) -> None:
         super().load(data)
         self.expand = {}
         for key, value in data.items():
             key = camel_to_snake(key).replace("@", "")
             setattr(self, key, value)
```

### Comparing `pocketbase-0.8.0/pocketbase/models/utils/base_model.py` & `pocketbase-0.8.1/pocketbase/models/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/admin_service.py` & `pocketbase-0.8.1/pocketbase/services/admin_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/collection_service.py` & `pocketbase-0.8.1/pocketbase/services/collection_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/log_service.py` & `pocketbase-0.8.1/pocketbase/services/log_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/realtime_service.py` & `pocketbase-0.8.1/pocketbase/services/realtime_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/record_service.py` & `pocketbase-0.8.1/pocketbase/services/record_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                 "code": code,
                 "codeVerifier": code_verifier,
                 "redirectUrl": redirct_url,
                 "createData": create_data,
             }
         )
         response_data = self.client.send(
-            self.base_collection_path() + "/auth-with-password",
+            self.base_collection_path() + "/auth-with-oauth2",
             {
                 "method": "POST",
                 "params": query_params,
                 "body": body_params,
             },
         )
         return self.auth_response(response_data)
```

### Comparing `pocketbase-0.8.0/pocketbase/services/settings_service.py` & `pocketbase-0.8.1/pocketbase/services/settings_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/utils/base_crud_service.py` & `pocketbase-0.8.1/pocketbase/services/utils/base_crud_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/utils/crud_service.py` & `pocketbase-0.8.1/pocketbase/services/utils/crud_service.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/services/utils/sse.py` & `pocketbase-0.8.1/pocketbase/services/utils/sse.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/stores/base_auth_store.py` & `pocketbase-0.8.1/pocketbase/stores/base_auth_store.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/stores/local_auth_store.py` & `pocketbase-0.8.1/pocketbase/stores/local_auth_store.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pocketbase/utils.py` & `pocketbase-0.8.1/pocketbase/utils.py`

 * *Files identical despite different names*

### Comparing `pocketbase-0.8.0/pyproject.toml` & `pocketbase-0.8.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [project.urls]
 "Homepage" = "https://github.com/vaphes/pocketbase"
 "Source" = "https://github.com/vaphes/pocketbase"
 "Bug Tracker" = "https://github.com/vaphes/pocketbase/issues"
 
 [tool.poetry]
 name = "pocketbase"
-version = "0.8.0"
+version = "0.8.1"
 description = "PocketBase SDK for python."
 authors = ["Vithor Jaeger <vaphes@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/vaphes/pocketbase"
 repository = "https://github.com/vaphes/pocketbase"
 keywords = ["pocketbase", "sdk"]
```

### Comparing `pocketbase-0.8.0/PKG-INFO` & `pocketbase-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketbase
-Version: 0.8.0
+Version: 0.8.1
 Summary: PocketBase SDK for python.
 Home-page: https://github.com/vaphes/pocketbase
 Keywords: pocketbase,sdk
 Author: Vithor Jaeger
 Author-email: vaphes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pocketbase Version: 0.8.0 Summary: PocketBase SDK
+Metadata-Version: 2.1 Name: pocketbase Version: 0.8.1 Summary: PocketBase SDK
 for python. Home-page: https://github.com/vaphes/pocketbase Keywords:
 pocketbase,sdk Author: Vithor Jaeger Author-email: vaphes@gmail.com Requires-
 Python: >=3.7,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0) Project-URL: Bug
```

