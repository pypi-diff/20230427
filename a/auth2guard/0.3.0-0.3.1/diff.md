# Comparing `tmp/auth2guard-0.3.0.tar.gz` & `tmp/auth2guard-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth2guard-0.3.0.tar", max compression
+gzip compressed data, was "auth2guard-0.3.1.tar", max compression
```

## Comparing `auth2guard-0.3.0.tar` & `auth2guard-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-03-10 20:48:38.786247 auth2guard-0.3.0/LICENSE
--rw-r--r--   0        0        0     5192 2023-04-02 11:10:00.237028 auth2guard-0.3.0/README.md
--rw-r--r--   0        0        0     2473 2023-04-02 11:10:00.237028 auth2guard-0.3.0/auth2guard/__init__.py
--rw-r--r--   0        0        0     7391 2023-04-02 11:10:00.237028 auth2guard-0.3.0/auth2guard/sentinel.py
--rw-r--r--   0        0        0      637 2023-04-02 11:10:16.892856 auth2guard-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 auth2guard-0.3.0/setup.py
--rw-r--r--   0        0        0     5698 1970-01-01 00:00:00.000000 auth2guard-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-10 20:48:38.786247 auth2guard-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5192 2023-04-02 11:11:04.452348 auth2guard-0.3.1/README.md
+-rw-r--r--   0        0        0     2473 2023-04-02 11:11:04.452348 auth2guard-0.3.1/auth2guard/__init__.py
+-rw-r--r--   0        0        0     7462 2023-04-26 22:32:30.982947 auth2guard-0.3.1/auth2guard/sentinel.py
+-rw-r--r--   0        0        0      637 2023-04-26 22:31:11.824672 auth2guard-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 auth2guard-0.3.1/setup.py
+-rw-r--r--   0        0        0     5698 1970-01-01 00:00:00.000000 auth2guard-0.3.1/PKG-INFO
```

### Comparing `auth2guard-0.3.0/LICENSE` & `auth2guard-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auth2guard-0.3.0/README.md` & `auth2guard-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `auth2guard-0.3.0/auth2guard/__init__.py` & `auth2guard-0.3.1/auth2guard/__init__.py`

 * *Files identical despite different names*

### Comparing `auth2guard-0.3.0/auth2guard/sentinel.py` & `auth2guard-0.3.1/auth2guard/sentinel.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,17 @@
                 message="authentication.not_from_origin",
             )
 
     def _supervision(self, request: Request) -> dict:
         token_type_and_content = self.__get_token(request=request)
         token_content = self.__decode_token(token_content=token_type_and_content[1])
         token_scope = token_content.get("scope", "")
-        scopes = set(token_scope.split(" "))
+        scopes = set(
+            token_scope.split(" ") if isinstance(token_scope, str) else token_scope
+        )
         scopes_sub_set = self.__allowed_scopes - scopes
         and_validation_satisfied = not scopes_sub_set and self.__and_validation
         or_operation_satisfied = (
             bool(len(self.__allowed_scopes) - len(scopes_sub_set))
             and not self.__and_validation
         )
         if not (and_validation_satisfied or or_operation_satisfied):
```

### Comparing `auth2guard-0.3.0/pyproject.toml` & `auth2guard-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auth2guard"
-version = "0.3.0"
+version = "0.3.1"
 description = "OAuth 2.0 scope validator"
 authors = ["Marco Sievers de Almeida Ximit Gaia <im.ximit@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "auth2guard"},
     { include = "auth2guard/**/*.py" },
```

### Comparing `auth2guard-0.3.0/setup.py` & `auth2guard-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['jwt>=1.3.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'auth2guard',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'OAuth 2.0 scope validator',
     'long_description': '```\n░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░\n░░░░░░░  ░░░░░░░░░░░░░░░░░░░   ░░░░░░░░░░░░░░░░░░░░░░░░░░     ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░   ░\n▒▒▒▒▒▒  ▒  ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒   ▒▒▒   ▒▒▒▒▒▒▒   ▒  ▒▒▒▒▒  ▒▒▒▒   ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒   ▒\n▒▒▒▒▒  ▒▒   ▒▒▒▒▒   ▒▒   ▒    ▒  ▒   ▒▒▒▒▒▒  ▒▒▒▒▒   ▒  ▒▒▒▒▒▒▒▒▒▒▒   ▒▒   ▒▒▒▒   ▒▒▒▒▒  ▒    ▒▒▒▒▒▒   ▒\n▓▓▓▓   ▓▓▓   ▓▓▓▓   ▓▓   ▓▓▓   ▓▓▓     ▓▓▓▓▓▓▓▓▓   ▓▓▓   ▓▓▓▓▓▓▓▓▓▓   ▓▓   ▓▓   ▓▓   ▓▓▓   ▓▓▓▓▓   ▓   ▓\n▓▓▓       ▓   ▓▓▓   ▓▓   ▓▓▓   ▓▓▓   ▓▓  ▓▓▓▓▓   ▓▓▓▓▓   ▓▓▓      ▓   ▓▓   ▓   ▓▓▓   ▓▓▓   ▓▓▓▓  ▓▓▓   ▓\n▓▓   ▓▓▓▓▓▓▓   ▓▓   ▓▓   ▓▓▓   ▓ ▓  ▓▓▓   ▓▓   ▓▓▓▓▓▓▓▓   ▓▓▓▓  ▓▓▓   ▓▓   ▓   ▓▓▓   ▓▓▓   ▓▓▓▓  ▓▓▓   ▓\n█   █████████   ███      ████   ██  ███   █         ████      ███████      ███   █    █    █████   █   █\n████████████████████████████████████████████████████████████████████████████████████████████████████████\nBy: CenturyBoys\n```\n\nA simple route decorator JWT scope validator.\n\nThis project work with the follow frameworks:\n\n✅ [FastApi](https://fastapi.tiangolo.com/)\n\n✅ [aiohttp](https://docs.aiohttp.org/en/stable/)\n\n## Config\n\nConfiguration are exposed and can be set in any time including out of the use scope.\n\nObs: all configs are saved as singleton.\n\n### jwk\n\nThe jwk key to validate JWT can be bytes, str or dict. This config need to be set!\n\n### http_header_name_token\n\nIf your application use a custom header to send the authentication token you can use this param to indicate his name. By default, the value is \'Authorization\'\n\n### request_token_callback\n\nIf to extract the request token you need to perform some operation you can set a callback for it. Will receive the request as param and must return a str with token type and the token \'Basic XXX\'\n\n```python\nimport auth2guard\n\nclass Request:\n    def __init__(self, headers: dict):\n        self._headers = headers\n\n    @property\n    def headers(self) -> dict:\n        return self._headersclass\n    \nrequest = Request(headers={"x-token": f"Basic Akj817Hakn122i..."})\n\ndef request_token_callback(request: Request):\n        return request.headers.get("x-token")\n    \n    \nauth2guard.set_config(\n    jwk=\'{"p":"-7pCvLlzsNIRD7utbLZqB...\',\n    http_header_name_token="x-token",\n    request_token_callback=request_token_callback\n)\n```\n\n## Exceptions\n\nThe package raise exceptions for some cases se bellow.\n\nObs: By default, all exception are ValueError.\n\n### token_not_found\nError when token was not found. \n\nObs: The config `request_token_callback` can be the problem.\n\n### not_from_origin\nError when token was generated not by the giving JWK. \n\nObs: Validate the config jwk.\n\n### expired\nError when exp JWT param exceeded the time.\n\n### unauthorized\nError when the JWT has not all necessary scope to proceed.\n\n```python\nimport auth2guard\n\nclass MyException(Exception):\n    pass\n\nauth2guard.overwrite_exceptions(unauthorized=MyException)\n```\n\n## Validator\n\nCan be used as decorator and receive a list of scopes. The validator will operate AND validation or a OR validation with the token scope content. For the AND validation all scopes in the `allowed_scopes` param need to be present in the jwt scope and in the OR if any scope is present that\'s enough. You can receive the token content if you want by setting `token_content` to `True` this will inject the param `token_content: dict` into your function as `kwargs`\n\n```python\nimport auth2guard\n\n\nclass Request:\n    def __init__(self, headers: dict):\n        self._headers = headers\n\n    @property\n    def headers(self) -> dict:\n        return self._headers\n\nauth2guard.set_config(jwk=\'{"p":"-7pCvLlzsNIRD7utbLZqB...\')\n\n@auth2guard.validate(["test1"], and_validation=True, token_content=True)\ndef route_callback(request, token_content: dict):\n    pass\n\nrequest = Request(headers={"Authorization": f"Basic XXX"})\nroute_callback(request=request)\n```',
     'author': 'Marco Sievers de Almeida Ximit Gaia',
     'author_email': 'im.ximit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `auth2guard-0.3.0/PKG-INFO` & `auth2guard-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth2guard
-Version: 0.3.0
+Version: 0.3.1
 Summary: OAuth 2.0 scope validator
 License: Apache-2.0
 Author: Marco Sievers de Almeida Ximit Gaia
 Author-email: im.ximit@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

