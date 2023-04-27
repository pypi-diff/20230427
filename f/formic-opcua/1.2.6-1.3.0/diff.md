# Comparing `tmp/formic_opcua-1.2.6.tar.gz` & `tmp/formic_opcua-1.3.0.tar.gz`

## Comparing `formic_opcua-1.2.6.tar` & `formic_opcua-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/core/parse.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.0/PKG-INFO
```

### Comparing `formic_opcua-1.2.6/.pre-commit-config.yaml` & `formic_opcua-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/examples/opcua_client.py` & `formic_opcua-1.3.0/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.3.0/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.3.0/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.3.0/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.3.0/formic_opcua/client/async_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/formic_opcua/client/opcua_client.py` & `formic_opcua-1.3.0/formic_opcua/client/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/formic_opcua/core/parse.py` & `formic_opcua-1.3.0/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/formic_opcua/core/type_conversions.py` & `formic_opcua-1.3.0/formic_opcua/core/type_conversions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # Copyright Formic Technologies 2023
 import uuid
 import logging
+import hashlib
 from datetime import datetime
 
 logger = logging.getLogger(__name__)
 
 from asyncua.ua.uatypes import VariantType
 
+def positive_sha256_hash(obj):
+    sha256_hash = hashlib.sha256()
+    sha256_hash.update(str(obj).encode('utf-8'))
+    return int(sha256_hash.hexdigest()[:8], 16)  # Make sure there are not too many bytes for UInt32
+
 type_map = {
     VariantType.SByte: int,
     VariantType.Byte: int,
     VariantType.ByteString: bytes,
-    VariantType.Int16: int,
     VariantType.Int32: int,
     VariantType.Int64: int,
     VariantType.UInt16: int,
     VariantType.UInt32: int,
     VariantType.UInt64: int,
     VariantType.Boolean: bool,
     VariantType.Double: float,
@@ -23,13 +28,12 @@
     VariantType.String: str,
     VariantType.DateTime: datetime,
     VariantType.Guid: uuid.UUID,
 }
 
 
 def convert_type(value, var_type):
-
-    if var_type == VariantType.String and (type_map[var_type] == int or type_map[var_type] == float):
-        logger.info(f'\n\n\n {var_type} {value} \n\n\n')
-        value = hash(value)
+    if (type_map[var_type] == int or type_map[var_type] == float) and isinstance(value, str):
+        value = positive_sha256_hash(value)
 
     return type_map[var_type](value)
+
```

### Comparing `formic_opcua-1.2.6/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.3.0/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.3.0/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/formic_opcua/server/opcua_server.py` & `formic_opcua-1.3.0/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/hooks/add_issue_prefix.py` & `formic_opcua-1.3.0/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/tests/test_server_config.py` & `formic_opcua-1.3.0/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/.gitignore` & `formic_opcua-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.6/pyproject.toml` & `formic_opcua-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.2.6"
+version = "1.3.0"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

