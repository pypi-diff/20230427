# Comparing `tmp/spacs-0.0.2.tar.gz` & `tmp/spacs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacs-0.0.2.tar", max compression
+gzip compressed data, was "spacs-0.0.3.tar", max compression
```

## Comparing `spacs-0.0.2.tar` & `spacs-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      418 2023-04-26 20:44:01.436132 spacs-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1503 2023-04-26 20:00:05.390203 spacs-0.0.2/README.md
--rw-r--r--   0        0        0       65 2023-04-26 19:27:37.324253 spacs-0.0.2/spacs/__init__.py
--rw-r--r--   0        0        0     7668 2023-04-26 20:41:25.607635 spacs-0.0.2/spacs/client.py
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 spacs-0.0.2/setup.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 spacs-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.3/LICENSE
+-rw-r--r--   0        0        0      418 2023-04-27 00:22:00.267753 spacs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1503 2023-04-26 20:00:05.390203 spacs-0.0.3/README.md
+-rw-r--r--   0        0        0       65 2023-04-26 19:27:37.324253 spacs-0.0.3/spacs/__init__.py
+-rw-r--r--   0        0        0     7737 2023-04-27 00:19:49.860168 spacs-0.0.3/spacs/client.py
+-rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 spacs-0.0.3/setup.py
+-rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 spacs-0.0.3/PKG-INFO
```

### Comparing `spacs-0.0.2/README.md` & `spacs-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spacs-0.0.2/spacs/client.py` & `spacs-0.0.3/spacs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,16 @@
         path: str,
         params: BaseModel | dict[str, Any] | None = None,
         body: BaseModel | dict[str, Any] | None = None,
         headers: dict[str, str] | None = None,
         content_type: ContentType = ContentType.JSON,
     ) -> dict | list:
         """Generic function for issuing requests"""
+        if params is None:
+            params = {}
         if headers is None:
             headers = {}
         headers["Content-Type"] = content_type.value
 
         params_transformed = self._transform_content(params)
         body_transformed = self._transform_content(body)
         path = self._build_path(path)
@@ -138,15 +140,15 @@
             "method": session_method.__name__,
             "base_url": self.base_url,
             "path": path,
         }
 
         try:
             async with session_method(
-                path, params=params_transformed, data=body_transformed, headers=headers
+                path, params=params_transformed, json=body_transformed, headers=headers
             ) as response:
                 end_time = datetime.datetime.now(tz=datetime.timezone.utc)
                 self._logger.debug(
                     {
                         "msg": "Request completed",
                         **base_log_info,
                         "status": response.status,
@@ -185,15 +187,17 @@
     async def close_all(cls) -> None:
         for session in cls._sessions:
             if not session.is_open:
                 continue
             await session.close()
 
     @classmethod
-    def _transform_content(cls, content: BaseModel | dict[str, Any] | None) -> dict[str, str] | None:
+    def _transform_content(
+        cls, content: BaseModel | dict[str, Any] | None
+    ) -> dict[str, str] | None:
         """Ensures input objects are in acceptable formats for requests"""
 
         if content is None:
             return
 
         if isinstance(content, BaseModel):
             content = content.dict()
```

### Comparing `spacs-0.0.2/setup.py` & `spacs-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'spacs',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Simple Pydantic AIOHTTP Client Sessions',
     'long_description': '# SPACS: Simple Pydantic AIOHTTP Client Sessions\n\nA package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.\n\n## Features\n\n* Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.\n* Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.\n* Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.\n* Utilizes modern Python type hinting.\n\n## Usage\n\n```python\nimport spacs\nfrom pydantic import BaseModel\n\n...\n\nexample_client = spacs.SpacsClient(base_url="http://example.com")\n\n# Basic request with error handling\ntry:\n    apple_response = await example_client.get("fruit/apple", params={"cultivar": "honeycrisp"})\nexcept spacs.SpacsRequestError as error:\n    print({"code": error.status_code, "reason": error.reason})\n\n# Sending Pydantic objects via HTTP POST\nclass MyModel(BaseModel):\n    name: str\n    age: int\n\nexample_object = MyModel(name="James", age=25)\nperson_response = await example_client.post("person", body=example_object)\n\n# Manually closing a session\nawait example_client.close()\n# Alternatively, to close all open sessions:\nawait spacs.SpacsClient.close_all()\n```\n\n## Building\n\n```\npoetry build\n```\n',
     'author': 'rlebel12',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rlebel12/spacs',
```

### Comparing `spacs-0.0.2/PKG-INFO` & `spacs-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple Pydantic AIOHTTP Client Sessions
 Home-page: https://github.com/rlebel12/spacs
 Author: rlebel12
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

