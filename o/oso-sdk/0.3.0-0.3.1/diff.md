# Comparing `tmp/oso_sdk-0.3.0.tar.gz` & `tmp/oso_sdk-0.3.1.tar.gz`

## Comparing `oso_sdk-0.3.0.tar` & `oso_sdk-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,34 @@
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/SECURITY.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/.github/workflows/cla.yml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/examples/fastapi/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/examples/fastapi/main.py
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/examples/flask/README.md
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/examples/flask/app.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/constants.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/py.typed
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/integrations/__init__.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/integrations/fastapi.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/integrations/flask.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/oso_sdk/integrations/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/tests/test_oso_sdk.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/tests/integrations/fastapi/test_fastapi.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/tests/integrations/flask/test_flask.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/README.md
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 oso_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/SECURITY.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/.devcontainer/fastapi-sample-app/devcontainer.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/.github/workflows/cla.yml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/fastapi/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/fastapi/main.py
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/flask/README.md
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/flask/app.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/starter-policy/fastapi/README.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/starter-policy/fastapi/requirements.txt
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/starter-policy/fastapi/sample_application.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/examples/starter-policy/fastapi/starter_policy.polar
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/constants.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/py.typed
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/integrations/__init__.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/integrations/fastapi.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/integrations/flask.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/oso_sdk/integrations/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/tests/test_oso_sdk.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/tests/integrations/fastapi/test_fastapi.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/tests/integrations/flask/test_flask.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/README.md
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 oso_sdk-0.3.1/PKG-INFO
```

### Comparing `oso_sdk-0.3.0/CODE_OF_CONDUCT.md` & `oso_sdk-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/CONTRIBUTING.md` & `oso_sdk-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/.github/workflows/cla.yml` & `oso_sdk-0.3.1/.github/workflows/cla.yml`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/.github/workflows/publish.yml` & `oso_sdk-0.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/.github/workflows/test.yml` & `oso_sdk-0.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/examples/fastapi/README.md` & `oso_sdk-0.3.1/examples/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/examples/fastapi/main.py` & `oso_sdk-0.3.1/examples/fastapi/main.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/examples/flask/README.md` & `oso_sdk-0.3.1/examples/flask/README.md`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/examples/flask/app.py` & `oso_sdk-0.3.1/examples/flask/app.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/oso_sdk/__init__.py` & `oso_sdk-0.3.1/oso_sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from typing import Any, Optional
 
 import oso_cloud  # type: ignore
 
 from .constants import OSO_URL
 from .integrations import Integration
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 _shared = None
 
 
 class OsoSdk(oso_cloud.Oso, Integration):
     def __init__(self, api_key: str, optin: bool, exception: Optional[Exception]):
-        oso_cloud.Oso.__init__(self, OSO_URL, api_key)
+        user_agent = (
+            f"{OsoSdk.__name__}/{__version__}"
+            if self.__class__ == OsoSdk
+            else f"{OsoSdk.__name__}{self.__class__.__name__}/{__version__}"
+        )
+        oso_cloud.Oso.__init__(self, OSO_URL, api_key, user_agent)
         Integration.__init__(self, optin, exception)
 
     """A handle to Oso Cloud.
 
     You should not instantiate this class directly. Use `oso_sdk.init` or
     `oso_sdk.global_oso` instead.
     """
```

### Comparing `oso_sdk-0.3.0/oso_sdk/integrations/__init__.py` & `oso_sdk-0.3.1/oso_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/oso_sdk/integrations/fastapi.py` & `oso_sdk-0.3.1/oso_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/oso_sdk/integrations/flask.py` & `oso_sdk-0.3.1/oso_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/oso_sdk/integrations/utils.py` & `oso_sdk-0.3.1/oso_sdk/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/tests/conftest.py` & `oso_sdk-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/tests/test_oso_sdk.py` & `oso_sdk-0.3.1/tests/test_oso_sdk.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/tests/test_utils.py` & `oso_sdk-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/tests/integrations/fastapi/test_fastapi.py` & `oso_sdk-0.3.1/tests/integrations/fastapi/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/tests/integrations/flask/test_flask.py` & `oso_sdk-0.3.1/tests/integrations/flask/test_flask.py`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/.gitignore` & `oso_sdk-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/LICENSE` & `oso_sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oso_sdk-0.3.0/README.md` & `oso_sdk-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 The Oso SDK provides web framework middleware for [`oso-cloud`](https://pypi.org/project/oso-cloud/), the Oso Cloud Client for Python.
 
 **Please Note: The SDK is currently released as a developer preview. Do not use this SDK for production workloads.**
 
 
 ## Getting Started
 
+>If you are looking for the sample application, navigate to [examples/starter-policy/fastapi](examples/starter-policy/fastapi/).
+
 ### Install
 
 ```bash
 pip install --upgrade oso-sdk
 ```
 
 ### Integrations
@@ -39,8 +41,8 @@
 Please refer to [CONTRIBUTING.md](https://github.com/osohq/oso-python/blob/main/CONTRIBUTING.md).
 
 ## License
 
 Licensed under the Apache 2.0 license, see [LICENSE](https://github.com/osohq/oso-python/blob/main/LICENSE).
 
 [join-slack-link]: https://user-images.githubusercontent.com/282595/128394344-1bd9e5b2-e83d-4666-b446-2e4f431ffcea.png
-[badge-slack-link]: https://join-slack.osohq.com/
+[badge-slack-link]: https://join-slack.osohq.com/
```

### Comparing `oso_sdk-0.3.0/pyproject.toml` & `oso_sdk-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dependencies = ["oso-cloud>=1.0.0"]
+dependencies = ["oso-cloud>=1.0.7"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://www.osohq.com/"
 Documentation = "https://www.osohq.com/docs"
 
 [project.optional-dependencies]
```

### Comparing `oso_sdk-0.3.0/PKG-INFO` & `oso_sdk-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oso-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python integrations for Oso Cloud
 Project-URL: Homepage, https://www.osohq.com/
 Project-URL: Documentation, https://www.osohq.com/docs
 Author-email: Oso Security <support@osohq.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: oso-cloud>=1.0.0
+Requires-Dist: oso-cloud>=1.0.7
 Provides-Extra: example
 Requires-Dist: uvicorn[standard]>=0.21.0; extra == 'example'
 Provides-Extra: fastapi
 Requires-Dist: fastapi>=0.79.0; extra == 'fastapi'
 Requires-Dist: starlette>=0.19.1; extra == 'fastapi'
 Provides-Extra: flask
 Requires-Dist: flask>=2.0.0; extra == 'flask'
@@ -49,14 +49,16 @@
 The Oso SDK provides web framework middleware for [`oso-cloud`](https://pypi.org/project/oso-cloud/), the Oso Cloud Client for Python.
 
 **Please Note: The SDK is currently released as a developer preview. Do not use this SDK for production workloads.**
 
 
 ## Getting Started
 
+>If you are looking for the sample application, navigate to [examples/starter-policy/fastapi](examples/starter-policy/fastapi/).
+
 ### Install
 
 ```bash
 pip install --upgrade oso-sdk
 ```
 
 ### Integrations
@@ -85,8 +87,8 @@
 Please refer to [CONTRIBUTING.md](https://github.com/osohq/oso-python/blob/main/CONTRIBUTING.md).
 
 ## License
 
 Licensed under the Apache 2.0 license, see [LICENSE](https://github.com/osohq/oso-python/blob/main/LICENSE).
 
 [join-slack-link]: https://user-images.githubusercontent.com/282595/128394344-1bd9e5b2-e83d-4666-b446-2e4f431ffcea.png
-[badge-slack-link]: https://join-slack.osohq.com/
+[badge-slack-link]: https://join-slack.osohq.com/
```

