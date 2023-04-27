# Comparing `tmp/mlflow_oidc_client_plugin-0.1.2.tar.gz` & `tmp/mlflow_oidc_client_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_oidc_client_plugin-0.1.2.tar", max compression
+gzip compressed data, was "mlflow_oidc_client_plugin-0.1.3.tar", max compression
```

## Comparing `mlflow_oidc_client_plugin-0.1.2.tar` & `mlflow_oidc_client_plugin-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-04-27 00:27:11.113093 mlflow_oidc_client_plugin-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     2915 2023-04-27 00:27:11.113093 mlflow_oidc_client_plugin-0.1.2/README.md
--rw-r--r--   0        0        0       76 2023-04-27 00:27:11.113093 mlflow_oidc_client_plugin-0.1.2/mlflow_oidc_client_plugin/__init__.py
--rw-r--r--   0        0        0     3187 2023-04-27 00:27:11.113093 mlflow_oidc_client_plugin-0.1.2/mlflow_oidc_client_plugin/config.py
--rw-r--r--   0        0        0     4594 2023-04-27 00:27:11.113093 mlflow_oidc_client_plugin-0.1.2/mlflow_oidc_client_plugin/oidc_session.py
--rw-r--r--   0        0        0     1352 2023-04-27 00:27:11.113093 mlflow_oidc_client_plugin-0.1.2/mlflow_oidc_client_plugin/request_header_provider.py
--rw-r--r--   0        0        0     1293 2023-04-27 00:27:11.114093 mlflow_oidc_client_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 mlflow_oidc_client_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-27 00:48:10.392638 mlflow_oidc_client_plugin-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2936 2023-04-27 00:48:10.392638 mlflow_oidc_client_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0       76 2023-04-27 00:48:10.392638 mlflow_oidc_client_plugin-0.1.3/mlflow_oidc_client_plugin/__init__.py
+-rw-r--r--   0        0        0     3224 2023-04-27 00:48:10.392638 mlflow_oidc_client_plugin-0.1.3/mlflow_oidc_client_plugin/config.py
+-rw-r--r--   0        0        0     4594 2023-04-27 00:48:10.392638 mlflow_oidc_client_plugin-0.1.3/mlflow_oidc_client_plugin/oidc_session.py
+-rw-r--r--   0        0        0     1352 2023-04-27 00:48:10.392638 mlflow_oidc_client_plugin-0.1.3/mlflow_oidc_client_plugin/request_header_provider.py
+-rw-r--r--   0        0        0     1293 2023-04-27 00:48:10.394638 mlflow_oidc_client_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 mlflow_oidc_client_plugin-0.1.3/PKG-INFO
```

### Comparing `mlflow_oidc_client_plugin-0.1.2/LICENSE.md` & `mlflow_oidc_client_plugin-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client_plugin-0.1.2/README.md` & `mlflow_oidc_client_plugin-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 
 
 
 Installation
 ------------
 
 ```console
-pip install mlflow-oidc-plugin
+pip install mlflow-oidc-client-plugin
 ```
 
 
 Getting Started
 ---------------
 
 First, add the following to the project's `pyproject.toml` configuration file:
 ```toml
-[[tool.mlflow-oidc-plugin.tracking-servers]]
+[[tool.mlflow-oidc-client-plugin.tracking-servers]]
 uri = "http://mlflow.example.com/"            # URI of your MLflow Tracking Server
 issuer = "https://auth.example.com/"          # URI of your OIDC provider
 client-id = "<application ID>"                # Client ID of your project
 ```
 
 You can now run MLflow client commands without any change. The plugin will match the `MLFLOW_TRACKING_URI` environment variable to the appropriate server configuration found in `pyproject.toml`.
 ```console
@@ -45,15 +45,15 @@
 
 
 Configuration
 -------------
 
 Options may be set with environment variables or in the `pyproject.toml` configuration file, with environment variables taking precedence.
 
-Each tracking server has its own `[[tool.mlflow-oidc-plugin.tracking-servers]]` block, which can be given multiple times in the same `pyproject.toml`.
+Each tracking server has its own `[[tool.mlflow-oidc-client-plugin.tracking-servers]]` block, which can be given multiple times in the same `pyproject.toml`.
 
 |Environment Variable|Config File|Default Value|Description|
 |-|-|-|-|
 |MLFLOW_TRACKING_URI|N/A|N/A|MLflow Tracking Server URI|
 |MLFLOW_TRACKING_OIDC_ISSUER|issuer|`None` (required)|OIDC authorization issuer URI|
 |MLFLOW_TRACKING_OIDC_CLIENT_ID|client-id|`None` (required)|OIDC client ID|
 |MLFLOW_TRACKING_OIDC_CLIENT_SECRET|client-secret|`None`|OIDC client secret|
```

### Comparing `mlflow_oidc_client_plugin-0.1.2/mlflow_oidc_client_plugin/config.py` & `mlflow_oidc_client_plugin-0.1.3/mlflow_oidc_client_plugin/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     path: Path = DEFAULT_CONFIG_FILE,
 ) -> TrackingServerOIDCSettings:
     """Read tracking server authorization settings for the matching URI."""
     matched_server_conf = {}
     try:
         with open(path) as config_file:
             data = tomllib.loads(config_file.read())
-            known_server_confs = data["tool"]["mlflow-oidc-plugin"]["tracking-servers"]
+            known_server_confs = data["tool"]["mlflow-oidc-client-plugin"][
+                "tracking-servers"
+            ]
             for server_conf in known_server_confs:
                 if not server_conf.get("uri"):
                     continue
                 if server_conf["uri"] == match_uri:
                     matched_server_conf = server_conf
     except (FileNotFoundError, KeyError, TypeError):
         pass
```

### Comparing `mlflow_oidc_client_plugin-0.1.2/mlflow_oidc_client_plugin/oidc_session.py` & `mlflow_oidc_client_plugin-0.1.3/mlflow_oidc_client_plugin/oidc_session.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client_plugin-0.1.2/mlflow_oidc_client_plugin/request_header_provider.py` & `mlflow_oidc_client_plugin-0.1.3/mlflow_oidc_client_plugin/request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client_plugin-0.1.2/pyproject.toml` & `mlflow_oidc_client_plugin-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-oidc-client-plugin"
-version = "0.1.2"
+version = "0.1.3"
 description = "MLflow plugin adding OIDC/OAuth 2.1 client authorization"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Plugins",
```

### Comparing `mlflow_oidc_client_plugin-0.1.2/PKG-INFO` & `mlflow_oidc_client_plugin-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-client-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: MLflow plugin adding OIDC/OAuth 2.1 client authorization
 Home-page: https://gitlab.com/lzinsou/mlflow-oidc-client-plugin
 Keywords: mlflow,plugin,mlops,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -40,24 +40,24 @@
 
 
 
 Installation
 ------------
 
 ```console
-pip install mlflow-oidc-plugin
+pip install mlflow-oidc-client-plugin
 ```
 
 
 Getting Started
 ---------------
 
 First, add the following to the project's `pyproject.toml` configuration file:
 ```toml
-[[tool.mlflow-oidc-plugin.tracking-servers]]
+[[tool.mlflow-oidc-client-plugin.tracking-servers]]
 uri = "http://mlflow.example.com/"            # URI of your MLflow Tracking Server
 issuer = "https://auth.example.com/"          # URI of your OIDC provider
 client-id = "<application ID>"                # Client ID of your project
 ```
 
 You can now run MLflow client commands without any change. The plugin will match the `MLFLOW_TRACKING_URI` environment variable to the appropriate server configuration found in `pyproject.toml`.
 ```console
@@ -67,15 +67,15 @@
 
 
 Configuration
 -------------
 
 Options may be set with environment variables or in the `pyproject.toml` configuration file, with environment variables taking precedence.
 
-Each tracking server has its own `[[tool.mlflow-oidc-plugin.tracking-servers]]` block, which can be given multiple times in the same `pyproject.toml`.
+Each tracking server has its own `[[tool.mlflow-oidc-client-plugin.tracking-servers]]` block, which can be given multiple times in the same `pyproject.toml`.
 
 |Environment Variable|Config File|Default Value|Description|
 |-|-|-|-|
 |MLFLOW_TRACKING_URI|N/A|N/A|MLflow Tracking Server URI|
 |MLFLOW_TRACKING_OIDC_ISSUER|issuer|`None` (required)|OIDC authorization issuer URI|
 |MLFLOW_TRACKING_OIDC_CLIENT_ID|client-id|`None` (required)|OIDC client ID|
 |MLFLOW_TRACKING_OIDC_CLIENT_SECRET|client-secret|`None`|OIDC client secret|
```

