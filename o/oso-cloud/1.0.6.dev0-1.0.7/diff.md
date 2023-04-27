# Comparing `tmp/oso_cloud-1.0.6.dev0-py3-none-any.whl.zip` & `tmp/oso_cloud-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 7027 bytes, number of entries: 8
--rw-r--r--  2.0 unx       62 b- defN 23-Apr-17 14:00 oso_cloud/__init__.py
--rw-r--r--  2.0 unx     9848 b- defN 23-Apr-17 14:00 oso_cloud/api.py
--rw-r--r--  2.0 unx     1619 b- defN 23-Apr-17 14:00 oso_cloud/helpers.py
--rw-r--r--  2.0 unx     6179 b- defN 23-Apr-17 14:00 oso_cloud/oso.py
--rw-r--r--  2.0 unx     3473 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      625 b- defN 23-Apr-17 14:00 oso_cloud-1.0.6.dev0.dist-info/RECORD
-8 files, 21908 bytes uncompressed, 5939 bytes compressed:  72.9%
+Zip file size: 7233 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       34 b- defN 23-Apr-27 16:03 oso_cloud/__init__.py
+-rw-r--r--  2.0 unx    10113 b- defN 23-Apr-27 16:03 oso_cloud/api.py
+-rw-r--r--  2.0 unx     1619 b- defN 23-Apr-27 16:03 oso_cloud/helpers.py
+-rw-r--r--  2.0 unx     6222 b- defN 23-Apr-27 16:03 oso_cloud/oso.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-27 16:03 oso_cloud/version.py
+-rw-r--r--  2.0 unx     3468 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      681 b- defN 23-Apr-27 16:03 oso_cloud-1.0.7.dist-info/RECORD
+9 files, 22261 bytes uncompressed, 6069 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: oso_cloud/helpers.py
 Comment: 
 
 Filename: oso_cloud/oso.py
 Comment: 
 
-Filename: oso_cloud-1.0.6.dev0.dist-info/METADATA
+Filename: oso_cloud/version.py
 Comment: 
 
-Filename: oso_cloud-1.0.6.dev0.dist-info/WHEEL
+Filename: oso_cloud-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: oso_cloud-1.0.6.dev0.dist-info/top_level.txt
+Filename: oso_cloud-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: oso_cloud-1.0.6.dev0.dist-info/RECORD
+Filename: oso_cloud-1.0.7.dist-info/top_level.txt
+Comment: 
+
+Filename: oso_cloud-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oso_cloud/__init__.py

```diff
@@ -1,3 +1 @@
 from .oso import Oso, Fact, Value
-
-__version__ = "1.0.6.dev0"
```

## oso_cloud/api.py

```diff
@@ -1,21 +1,23 @@
 # This file is generated from the openapi spec
 import json
 from dataclasses import dataclass, asdict
 from typing import List, Optional
 import requests
 import backoff
+import platform
+from .version import __version__
 
 HTTP_ERROR_MAX_RETRIES = 10
 HTTP_ERROR_MAX_TIME = 30
 
 NETWORK_ERROR_MAX_RETRIES = 10
 NETWORK_ERROR_MAX_TIME = 30
 
-TIMEOUT_INTERVALS = (1, 30)
+TIMEOUT_INTERVALS = (1, 5)
 
 
 @dataclass
 class ApiResult:
     message: str
 
 
@@ -135,17 +137,22 @@
             return False
         return 400 <= exc.response.status_code < 500
     else:
         return False
 
 
 class API:
-    def __init__(self, url="https://cloud.osohq.com", api_key=None):
+    def __init__(self, url="https://cloud.osohq.com", api_key=None, user_agent=None):
         self.url = url
         self.api_base = "api"
+        self.user_agent = (
+            f"Oso Cloud (python {platform.python_version()}; rv:{__version__})"
+        )
+        if user_agent:
+            self.user_agent = f"{self.user_agent} {user_agent}"
         if api_key:
             self.token = api_key
         else:
             raise ValueError("Must set an api_key")
         self.session = requests.Session()
         self.session.headers.update(self._default_headers())
 
@@ -158,15 +165,15 @@
             return result.json()
         except json.decoder.JSONDecodeError:
             return result.text
 
     def _default_headers(self):
         return {
             "Authorization": f"Bearer {self.token}",
-            "User-Agent": "Oso Cloud (python)",
+            "User-Agent": self.user_agent,
             "X-OsoApiVersion": "0",
         }
 
     @backoff.on_exception(
         backoff.expo,
         (requests.exceptions.ConnectionError, requests.exceptions.Timeout),
         max_time=NETWORK_ERROR_MAX_TIME,
```

## oso_cloud/oso.py

```diff
@@ -15,16 +15,18 @@
 class Oso:
     """Oso Cloud client
 
     For more detailed documentation, see
     https://www.osohq.com/docs/reference/client-apis/python
     """
 
-    def __init__(self, url: str = "https://cloud.osohq.com", api_key=None):
-        self.api = api.API(url, api_key)
+    def __init__(
+        self, url: str = "https://cloud.osohq.com", api_key=None, user_agent=None
+    ):
+        self.api = api.API(url, api_key, user_agent)
 
     def authorize(
         self,
         actor: Value,
         action: str,
         resource: Value,
         context_facts: List[Fact] = [],
```

## Comparing `oso_cloud-1.0.6.dev0.dist-info/METADATA` & `oso_cloud-1.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oso-cloud
-Version: 1.0.6.dev0
+Version: 1.0.7
 Summary: Oso Cloud Python client
 Home-page: https://www.osohq.com
 Author: Oso Security
 Author-email: support@osohq.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.osohq.com/docs
 Keywords: authorization,rbac,oso,oso cloud,authorization as a service,microservice authorization
```

