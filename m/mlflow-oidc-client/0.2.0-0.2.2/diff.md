# Comparing `tmp/mlflow_oidc_client-0.2.0.tar.gz` & `tmp/mlflow_oidc_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_oidc_client-0.2.0.tar", max compression
+gzip compressed data, was "mlflow_oidc_client-0.2.2.tar", max compression
```

## Comparing `mlflow_oidc_client-0.2.0.tar` & `mlflow_oidc_client-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-04-27 12:58:12.762895 mlflow_oidc_client-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     3635 2023-04-27 12:58:12.763895 mlflow_oidc_client-0.2.0/README.md
--rw-r--r--   0        0        0       76 2023-04-27 12:58:12.763895 mlflow_oidc_client-0.2.0/mlflow_oidc_client/__init__.py
--rw-r--r--   0        0        0     3187 2023-04-27 12:58:12.763895 mlflow_oidc_client-0.2.0/mlflow_oidc_client/config.py
--rw-r--r--   0        0        0     4594 2023-04-27 12:58:12.763895 mlflow_oidc_client-0.2.0/mlflow_oidc_client/oidc_session.py
--rw-r--r--   0        0        0     1352 2023-04-27 12:58:12.763895 mlflow_oidc_client-0.2.0/mlflow_oidc_client/request_header_provider.py
--rw-r--r--   0        0        0     1265 2023-04-27 12:58:12.764895 mlflow_oidc_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4538 1970-01-01 00:00:00.000000 mlflow_oidc_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-27 14:30:33.307630 mlflow_oidc_client-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     3638 2023-04-27 14:30:33.307630 mlflow_oidc_client-0.2.2/README.md
+-rw-r--r--   0        0        0       76 2023-04-27 14:30:33.307630 mlflow_oidc_client-0.2.2/mlflow_oidc_client/__init__.py
+-rw-r--r--   0        0        0     3187 2023-04-27 14:30:33.307630 mlflow_oidc_client-0.2.2/mlflow_oidc_client/config.py
+-rw-r--r--   0        0        0     4758 2023-04-27 14:30:33.307630 mlflow_oidc_client-0.2.2/mlflow_oidc_client/oidc_session.py
+-rw-r--r--   0        0        0     1352 2023-04-27 14:30:33.307630 mlflow_oidc_client-0.2.2/mlflow_oidc_client/request_header_provider.py
+-rw-r--r--   0        0        0     1344 2023-04-27 14:30:33.308631 mlflow_oidc_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 mlflow_oidc_client-0.2.2/PKG-INFO
```

### Comparing `mlflow_oidc_client-0.2.0/LICENSE.md` & `mlflow_oidc_client-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client-0.2.0/README.md` & `mlflow_oidc_client-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 |-|-|-|-|
 |MLFLOW_TRACKING_URI|N/A|N/A|MLflow Tracking Server URI|
 |MLFLOW_TRACKING_OIDC_ISSUER|issuer|`None` (required)|OIDC authorization issuer URI|
 |MLFLOW_TRACKING_OIDC_CLIENT_ID|client-id|`None` (required)|OIDC client ID|
 |MLFLOW_TRACKING_OIDC_CLIENT_SECRET|client-secret|`None`|OIDC client secret|
 |MLFLOW_TRACKING_OIDC_REDIRECT_URI|redirect-uri|`"http://127.0.0.1:39303/oauth2/callback"`|OIDC redirect URI|
 |MLFLOW_TRACKING_OIDC_SCOPE|scope|`"openid profile email"`|OIDC token scope|
-|MLFLOW_TRACKING_OIDC_AUDIENCE|scope|Same as the client ID|OIDC token audience|
+|MLFLOW_TRACKING_OIDC_AUDIENCE|audience|Same as the client ID|OIDC token audience|
 |MLFLOW_TRACKING_OIDC_INTERACTIVE|interactive|Interactive by default if the application is public (no client secret)|Require a user login in a browser|
 |MLFLOW_TRACKING_OIDC_USE_ID_TOKEN|use-id-token|Use the ID token by default if the application is public (no client secret)|Use the ID token instead of the access token as `Bearer` token in the `Authorization` HTTP header|
 
 
 Examples
 --------
```

### Comparing `mlflow_oidc_client-0.2.0/mlflow_oidc_client/config.py` & `mlflow_oidc_client-0.2.2/mlflow_oidc_client/config.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client-0.2.0/mlflow_oidc_client/oidc_session.py` & `mlflow_oidc_client-0.2.2/mlflow_oidc_client/oidc_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import json
 from dataclasses import asdict, replace
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Self, Type
+from typing import Type
 
 import jwt
 from oidc_client import AuthorizationError, TokenResponse, fetch_provider_config, login
 from oidc_client.config import DEFAULT_OIDC_SCOPE, DEFAULT_REDIRECT_URI
 
+# FIXME: type-check when we drop support for Python 3.10
+try:
+    from typing import Self
+except ImportError:  # pragma: no cover
+    from typing_extensions import Self
+
 DEFAULT_CACHE_PATH = Path.home() / ".mlflow" / "oidc_client" / "cache"
 
 JWT_CLAIM_EXPIRY = "exp"
 JWT_OPTION_VERIFY_SIGNATURE = "verify_signature"
 
 
 class OIDCSessionError(RuntimeError):
```

### Comparing `mlflow_oidc_client-0.2.0/mlflow_oidc_client/request_header_provider.py` & `mlflow_oidc_client-0.2.2/mlflow_oidc_client/request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client-0.2.0/pyproject.toml` & `mlflow_oidc_client-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-oidc-client"
-version = "0.2.0"
+version = "0.2.2"
 description = "MLflow plugin adding OIDC/OAuth 2.1 client authorization"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Plugins",
@@ -37,10 +37,14 @@
 [tool.mypy]
 strict = true
 
 [[tool.mypy.overrides]]
 module = "mlflow.tracking.request_header.abstract_request_header_provider"
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+module = "cryptography"
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mlflow_oidc_client-0.2.0/PKG-INFO` & `mlflow_oidc_client-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-client
-Version: 0.2.0
+Version: 0.2.2
 Summary: MLflow plugin adding OIDC/OAuth 2.1 client authorization
 Home-page: https://gitlab.com/lzinsou/mlflow-oidc-client
 Keywords: mlflow,plugin,mlops,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -76,15 +76,15 @@
 |-|-|-|-|
 |MLFLOW_TRACKING_URI|N/A|N/A|MLflow Tracking Server URI|
 |MLFLOW_TRACKING_OIDC_ISSUER|issuer|`None` (required)|OIDC authorization issuer URI|
 |MLFLOW_TRACKING_OIDC_CLIENT_ID|client-id|`None` (required)|OIDC client ID|
 |MLFLOW_TRACKING_OIDC_CLIENT_SECRET|client-secret|`None`|OIDC client secret|
 |MLFLOW_TRACKING_OIDC_REDIRECT_URI|redirect-uri|`"http://127.0.0.1:39303/oauth2/callback"`|OIDC redirect URI|
 |MLFLOW_TRACKING_OIDC_SCOPE|scope|`"openid profile email"`|OIDC token scope|
-|MLFLOW_TRACKING_OIDC_AUDIENCE|scope|Same as the client ID|OIDC token audience|
+|MLFLOW_TRACKING_OIDC_AUDIENCE|audience|Same as the client ID|OIDC token audience|
 |MLFLOW_TRACKING_OIDC_INTERACTIVE|interactive|Interactive by default if the application is public (no client secret)|Require a user login in a browser|
 |MLFLOW_TRACKING_OIDC_USE_ID_TOKEN|use-id-token|Use the ID token by default if the application is public (no client secret)|Use the ID token instead of the access token as `Bearer` token in the `Authorization` HTTP header|
 
 
 Examples
 --------
```

