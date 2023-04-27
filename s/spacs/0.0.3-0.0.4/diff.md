# Comparing `tmp/spacs-0.0.3.tar.gz` & `tmp/spacs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacs-0.0.3.tar", max compression
+gzip compressed data, was "spacs-0.0.4.tar", max compression
```

## Comparing `spacs-0.0.3.tar` & `spacs-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.3/LICENSE
--rw-r--r--   0        0        0      418 2023-04-27 00:22:00.267753 spacs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1503 2023-04-26 20:00:05.390203 spacs-0.0.3/README.md
--rw-r--r--   0        0        0       65 2023-04-26 19:27:37.324253 spacs-0.0.3/spacs/__init__.py
--rw-r--r--   0        0        0     7737 2023-04-27 00:19:49.860168 spacs-0.0.3/spacs/client.py
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 spacs-0.0.3/setup.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 spacs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.4/LICENSE
+-rw-r--r--   0        0        0      418 2023-04-27 14:19:10.951829 spacs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1503 2023-04-26 20:00:05.390203 spacs-0.0.4/README.md
+-rw-r--r--   0        0        0      149 2023-04-27 14:17:02.802475 spacs-0.0.4/spacs/__init__.py
+-rw-r--r--   0        0        0     8876 2023-04-27 14:18:56.817227 spacs-0.0.4/spacs/client.py
+-rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 spacs-0.0.4/setup.py
+-rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 spacs-0.0.4/PKG-INFO
```

### Comparing `spacs-0.0.3/LICENSE` & `spacs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spacs-0.0.3/README.md` & `spacs-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spacs-0.0.3/spacs/client.py` & `spacs-0.0.4/spacs/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import datetime
 import logging
 from collections.abc import Callable
 from enum import StrEnum
-from typing import Any, Coroutine, ClassVar, Self
+from typing import Any, ClassVar, Self, Awaitable, Type
 
 import aiohttp
 from aiohttp import ClientConnectorError, ClientResponse
 from pydantic import BaseModel
 
+RequestContent = BaseModel | dict[str, Any] | None
+JsonResponseContent = dict[str, Any] | list[dict[str, Any]]
+ModelResponse = BaseModel | list[BaseModel]
+SpacsClientResponse = str | JsonResponseContent | ModelResponse
+
 _logger = logging.getLogger(__name__)
 
 
 class ContentType(StrEnum):
     JSON = "application/json"
     FORM = "application/x-www-form-urlencoded"
     HTML = "text/html"
@@ -66,101 +71,113 @@
         await self._session.close()
         self._session = None
 
     async def get(
         self,
         path: str,
         *,
-        params: BaseModel | dict[str, Any] | None = None,
-        body: BaseModel | dict[str, Any] | None = None,
+        params: RequestContent = None,
+        body: RequestContent = None,
         headers: dict[str, str] | None = None,
         content_type: ContentType = ContentType.JSON,
-    ) -> dict:
+        response_model: Type[BaseModel] | None = None,
+    ) -> SpacsClientResponse:
         return await self._request(
-            self.session.get, path, params, body, headers, content_type
+            self.session.get, path, params, body, headers, content_type, response_model
         )
 
     async def post(
         self,
         path: str,
-        params: BaseModel | dict[str, Any] | None = None,
-        body: BaseModel | dict[str, Any] | None = None,
+        *,
+        params: RequestContent = None,
+        body: RequestContent = None,
         headers: dict[str, str] | None = None,
         content_type: ContentType = ContentType.JSON,
-    ) -> dict | list:
+        response_model: Type[BaseModel] | None = None,
+    ) -> SpacsClientResponse:
         return await self._request(
-            self.session.post, path, params, body, headers, content_type
+            self.session.post, path, params, body, headers, content_type, response_model
         )
 
     async def put(
         self,
         path: str,
-        params: BaseModel | dict[str, Any] | None = None,
-        body: BaseModel | dict[str, Any] | None = None,
+        *,
+        params: RequestContent = None,
+        body: RequestContent = None,
         headers: dict[str, str] | None = None,
         content_type: ContentType = ContentType.JSON,
-    ) -> dict | list:
+        response_model: Type[BaseModel] | None = None,
+    ) -> SpacsClientResponse:
         return await self._request(
-            self.session.put, path, params, body, headers, content_type
+            self.session.put, path, params, body, headers, content_type, response_model
         )
 
     async def delete(
         self,
         path: str,
-        params: BaseModel | dict[str, Any] | None = None,
-        body: BaseModel | dict[str, Any] | None = None,
+        *,
+        params: RequestContent = None,
+        body: RequestContent = None,
         headers: dict[str, str] | None = None,
         content_type: ContentType = ContentType.JSON,
-    ) -> dict | list:
+        response_model: Type[BaseModel] | None = None,
+    ) -> SpacsClientResponse:
         return await self._request(
-            self.session.delete, path, params, body, headers, content_type
+            self.session.delete,
+            path,
+            params,
+            body,
+            headers,
+            content_type,
+            response_model,
         )
 
     async def _request(
         self,
-        session_method: Callable[..., Coroutine[Any, None, ClientResponse]],
+        action: Callable[..., Awaitable[ClientResponse]],
         path: str,
-        params: BaseModel | dict[str, Any] | None = None,
-        body: BaseModel | dict[str, Any] | None = None,
+        params: RequestContent = None,
+        body: RequestContent = None,
         headers: dict[str, str] | None = None,
         content_type: ContentType = ContentType.JSON,
-    ) -> dict | list:
+        response_model: Type[BaseModel] | None = None,
+    ) -> SpacsClientResponse:
         """Generic function for issuing requests"""
-        if params is None:
-            params = {}
         if headers is None:
             headers = {}
         headers["Content-Type"] = content_type.value
 
         params_transformed = self._transform_content(params)
         body_transformed = self._transform_content(body)
         path = self._build_path(path)
 
         start_time = datetime.datetime.now(tz=datetime.timezone.utc)
         base_log_info = {
-            "method": session_method.__name__,
+            "method": action.__name__,
             "base_url": self.base_url,
             "path": path,
         }
 
         try:
-            async with session_method(
+            async with action(
                 path, params=params_transformed, json=body_transformed, headers=headers
             ) as response:
                 end_time = datetime.datetime.now(tz=datetime.timezone.utc)
                 self._logger.debug(
                     {
                         "msg": "Request completed",
                         **base_log_info,
                         "status": response.status,
                         "duration": str(end_time - start_time),
                     }
                 )
                 if response.ok:
-                    return await self._parse_response(response)
+                    return await self._handle_ok_response(response, response_model)
                 else:
                     raise SpacsRequestError(
                         status_code=response.status,
                         reason=response.reason,
                     )
         except ClientConnectorError as error:
             self._logger.error("Failed to connect to server.")
@@ -187,17 +204,15 @@
     async def close_all(cls) -> None:
         for session in cls._sessions:
             if not session.is_open:
                 continue
             await session.close()
 
     @classmethod
-    def _transform_content(
-        cls, content: BaseModel | dict[str, Any] | None
-    ) -> dict[str, str] | None:
+    def _transform_content(cls, content: RequestContent) -> dict[str, str] | None:
         """Ensures input objects are in acceptable formats for requests"""
 
         if content is None:
             return
 
         if isinstance(content, BaseModel):
             content = content.dict()
@@ -209,22 +224,39 @@
             elif isinstance(value, datetime.timedelta):
                 # `timedelta` items represented as seconds (float)
                 content[key] = value.total_seconds()
             elif isinstance(value, bool):
                 content[key] = str(value)
         return content
 
+    @classmethod
+    async def _handle_ok_response(
+        cls, response: ClientResponse, model: Type[BaseModel] | None
+    ) -> str | JsonResponseContent | ModelResponse:
+        content = await cls._parse_response(response)
+        if model is not None and not isinstance(response, str):
+            content = cls._response_content_to_model(content, model)
+        return content
+
     @staticmethod
-    async def _parse_response(response: ClientResponse):
+    async def _parse_response(response: ClientResponse) -> str | JsonResponseContent:
         match response.content_type:
             case ContentType.HTML:
                 return await response.text()
             case _:
                 return await response.json()
 
+    @staticmethod
+    def _response_content_to_model(
+        content: JsonResponseContent, model: Type[BaseModel]
+    ) -> ModelResponse:
+        if isinstance(content, list):
+            return [model(**item) for item in content]
+        return model(**content)
+
 
 class SpacsRequestError(Exception):
     def __init__(self, status_code: int, reason: str):
         self.status_code = status_code
         self.reason = reason
 
     def __repr__(self) -> str:
```

### Comparing `spacs-0.0.3/setup.py` & `spacs-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'spacs',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Simple Pydantic AIOHTTP Client Sessions',
     'long_description': '# SPACS: Simple Pydantic AIOHTTP Client Sessions\n\nA package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.\n\n## Features\n\n* Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.\n* Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.\n* Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.\n* Utilizes modern Python type hinting.\n\n## Usage\n\n```python\nimport spacs\nfrom pydantic import BaseModel\n\n...\n\nexample_client = spacs.SpacsClient(base_url="http://example.com")\n\n# Basic request with error handling\ntry:\n    apple_response = await example_client.get("fruit/apple", params={"cultivar": "honeycrisp"})\nexcept spacs.SpacsRequestError as error:\n    print({"code": error.status_code, "reason": error.reason})\n\n# Sending Pydantic objects via HTTP POST\nclass MyModel(BaseModel):\n    name: str\n    age: int\n\nexample_object = MyModel(name="James", age=25)\nperson_response = await example_client.post("person", body=example_object)\n\n# Manually closing a session\nawait example_client.close()\n# Alternatively, to close all open sessions:\nawait spacs.SpacsClient.close_all()\n```\n\n## Building\n\n```\npoetry build\n```\n',
     'author': 'rlebel12',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rlebel12/spacs',
```

### Comparing `spacs-0.0.3/PKG-INFO` & `spacs-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple Pydantic AIOHTTP Client Sessions
 Home-page: https://github.com/rlebel12/spacs
 Author: rlebel12
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

