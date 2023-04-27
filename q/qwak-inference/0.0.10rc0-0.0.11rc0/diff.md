# Comparing `tmp/qwak_inference-0.0.10rc0.tar.gz` & `tmp/qwak_inference-0.0.11rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.0.10rc0.tar", max compression
+gzip compressed data, was "qwak_inference-0.0.11rc0.tar", max compression
```

## Comparing `qwak_inference-0.0.10rc0.tar` & `qwak_inference-0.0.11rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10480 2023-04-19 18:10:36.387069 qwak_inference-0.0.10rc0/LICENSE
--rw-r--r--   0        0        0      267 2023-04-19 18:10:36.387069 qwak_inference-0.0.10rc0/README.md
--rw-r--r--   0        0        0     1890 2023-04-19 18:11:50.006166 qwak_inference-0.0.10rc0/pyproject.toml
--rw-r--r--   0        0        0      548 2023-04-19 18:11:50.006166 qwak_inference-0.0.10rc0/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 18:10:36.387069 qwak_inference-0.0.10rc0/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    19154 2023-04-19 18:10:36.387069 qwak_inference-0.0.10rc0/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-04-19 18:10:36.387069 qwak_inference-0.0.10rc0/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0      739 2023-04-19 18:10:36.387069 qwak_inference-0.0.10rc0/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      558 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     3821 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     1076 2023-04-19 18:10:36.391069 qwak_inference-0.0.10rc0/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 qwak_inference-0.0.10rc0/setup.py
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 qwak_inference-0.0.10rc0/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/LICENSE
+-rw-r--r--   0        0        0      267 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/README.md
+-rw-r--r--   0        0        0     1897 2023-04-27 06:35:10.372577 qwak_inference-0.0.11rc0/pyproject.toml
+-rw-r--r--   0        0        0      548 2023-04-27 06:35:10.372577 qwak_inference-0.0.11rc0/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    19154 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0      739 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     4795 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     1076 2023-04-27 06:34:17.828277 qwak_inference-0.0.11rc0/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2052 1970-01-01 00:00:00.000000 qwak_inference-0.0.11rc0/setup.py
+-rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 qwak_inference-0.0.11rc0/PKG-INFO
```

### Comparing `qwak_inference-0.0.10rc0/LICENSE` & `qwak_inference-0.0.11rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/pyproject.toml` & `qwak_inference-0.0.11rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.0.10.rc0"
+version = "0.0.11.rc0"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
@@ -18,15 +18,15 @@
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
 requests = "^2.0.0"
 qwak-core = { version=">=0.0.23", optional=true}
 boto3 = { version="^1.24.89", optional=true }
 pandas = [
     {version="<1.4", python=">=3.7.1,<3.8", optional=true},
-    {version=">=1.4.3", python=">=3.8,<3.10", optional=true}
+    {version=">=1.4.3,<2.0.0", python=">=3.8,<3.10", optional=true}
 ]
 joblib = { version="^1.1.0", optional=true }
 pyarrow = { version=">=6.0.0, <11.0.0", optional=true }
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 black = "23.1.0"
```

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/__init__.py` & `qwak_inference-0.0.11rc0/qwak_inference/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     # not support them due to the pandas, numpy, joblib, etc. dependencies
     pass
 
 from qwak_inference.realtime_client import RealTimeClient
 
 __all__ = ["BatchInferenceClient", "FeedbackClient", "RealTimeClient"]
 
-__version__ = "0.0.10.rc0"
+__version__ = "0.0.11.rc0"
```

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.0.11rc0/qwak_inference/batch_client/batch_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.0.11rc0/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/batch_client/s3.py` & `qwak_inference-0.0.11rc0/qwak_inference/batch_client/s3.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/configuration/account.py` & `qwak_inference-0.0.11rc0/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/configuration/auth.py` & `qwak_inference-0.0.11rc0/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/configuration/session.py` & `qwak_inference-0.0.11rc0/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/constants.py` & `qwak_inference-0.0.11rc0/qwak_inference/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,7 +18,11 @@
     QWAK_CONFIG_FILE: str = f"{QWAK_CONFIG_FOLDER}/config"
 
     QWAK_AUTHORIZATION_FILE: str = f"{QWAK_CONFIG_FOLDER}/auth"
 
     QWAK_DEFAULT_SECTION: str = "default"
 
     QWAK_AUTHENTICATION_URL = "https://grpc.qwak.ai/api/v1/authentication/qwak-api-key"
+
+    QWAK_AUTHENTICATED_USER_ENDPOINT: str = (
+        "https://grpc.qwak.ai/api/v0/runtime/get-authenticated-user-context"
+    )
```

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/exceptions.py` & `qwak_inference-0.0.11rc0/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/feedback_client.py` & `qwak_inference-0.0.11rc0/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/realtime_client/client.py` & `qwak_inference-0.0.11rc0/qwak_inference/realtime_client/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 from enum import Enum
+from json import JSONDecodeError
 
+from qwak_inference.constants import QwakConstants
 from qwak_inference.realtime_client.rest_helpers import RestSession
 
 try:
     from qwak.exceptions import QwakHTTPException
 except ImportError:
     from qwak_inference.exceptions import QwakHTTPException
 
@@ -12,34 +14,43 @@
 
 
 class InferenceOutputFormat(Enum):
     PANDAS = 1
     DICTIONARY = 2
 
 
+DEFAULT_ENVIRONMENT_ERROR_MESSAGE = (
+    "Failed to get default environment name. This might be due to connectivity "
+    "issues or missing account configuration."
+)
+
+
 class RealTimeClient(object):
     def __init__(
         self,
         model_id: str,
-        environment: str,
+        environment: str = None,
         variation: str = None,
         model_api: str = None,
     ):
         """
 
         :param model_id: The model id to invoke against. If not provided, will attempt to extract the model ID from the
         `QWAK_MODEL_ID` environment variable
         """
 
+        self.r_session = RestSession()
+        if not environment:
+            environment = _get_default_environment_name(self.r_session)
+
         self.model_id = model_id
         self.content_type = "application/json; format=pandas-split"
         self.model_api = (
             model_api if model_api else _get_model_url(model_id, environment, variation)
         )
-        self.r_session = RestSession()
 
     def predict(
         self,
         feature_vectors,
         output_format=InferenceOutputFormat.DICTIONARY,
         metadata: dict = {},
     ):
@@ -97,10 +108,24 @@
                 )
         except QwakHTTPException as e:
             raise e
         except Exception as e:
             raise RuntimeError(f"Failed to make a prediction request. Error is: {e}")
 
 
+def _get_default_environment_name(r_session) -> str:
+    try:
+        response = r_session.post(QwakConstants.QWAK_AUTHENTICATED_USER_ENDPOINT)
+        account_details = response.json()["authenticatedUserContext"]["user"][
+            "accountDetails"
+        ]
+        default_environment_id = account_details["defaultEnvironmentId"]
+        return account_details["environmentById"][default_environment_id]["name"]
+    except JSONDecodeError:
+        raise RuntimeError(DEFAULT_ENVIRONMENT_ERROR_MESSAGE)
+    except Exception:
+        raise RuntimeError(DEFAULT_ENVIRONMENT_ERROR_MESSAGE + " Error is: {e}")
+
+
 def _get_model_url(model_id, environment, variation=None) -> str:
     model_route = f"{model_id}/{variation}" if variation else model_id
     return f"https://models.{environment}.qwak.ai/v1/{model_route}/predict"
```

### Comparing `qwak_inference-0.0.10rc0/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.0.11rc0/qwak_inference/realtime_client/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.0.10rc0/setup.py` & `qwak_inference-0.0.11rc0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 extras_require = \
 {'batch': ['qwak-core>=0.0.23',
            'boto3>=1.24.89,<2.0.0',
            'joblib>=1.1.0,<2.0.0',
            'pyarrow>=6.0.0,<11.0.0'],
  'batch:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                      'pandas<1.4'],
- 'batch:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3',
-                                                               'pandas>=1.4.3'],
+ 'batch:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
+                                                               'pandas>=1.4.3,<2.0.0'],
  'feedback': ['qwak-core>=0.0.23',
               'boto3>=1.24.89,<2.0.0',
               'joblib>=1.1.0,<2.0.0'],
  'feedback:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                         'pandas<1.4'],
- 'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3',
-                                                                  'pandas>=1.4.3']}
+ 'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
+                                                                  'pandas>=1.4.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.0.10rc0',
+    'version': '0.0.11rc0',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_inference-0.0.10rc0/PKG-INFO` & `qwak_inference-0.0.11rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.0.10rc0
+Version: 0.0.11rc0
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: batch
 Provides-Extra: feedback
 Requires-Dist: boto3 (>=1.24.89,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
-Requires-Dist: pandas (>=1.4.3) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
+Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
 Requires-Dist: qwak-core (>=0.0.23) ; extra == "batch" or extra == "feedback"
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Qwak Inference
```

