# Comparing `tmp/cmem_plugin_base-3.1.0.tar.gz` & `tmp/cmem_plugin_base-3.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_base-3.1.0.tar", max compression
+gzip compressed data, was "cmem_plugin_base-3.1.0rc1.tar", max compression
```

## Comparing `cmem_plugin_base-3.1.0.tar` & `cmem_plugin_base-3.1.0rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11334 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/LICENSE
--rw-r--r--   0        0        0      246 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/README-public.md
--rw-r--r--   0        0        0       73 2023-04-27 13:33:45.503335 cmem_plugin_base-3.1.0/cmem_plugin_base/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/__init__.py
--rw-r--r--   0        0        0     3992 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/context.py
--rw-r--r--   0        0        0     8897 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/description.py
--rw-r--r--   0        0        0     2765 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/discovery.py
--rw-r--r--   0        0        0     1370 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/entity.py
--rw-r--r--   0        0        0       37 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/__init__.py
--rw-r--r--   0        0        0     1557 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/choice.py
--rw-r--r--   0        0        0     2243 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/dataset.py
--rw-r--r--   0        0        0     3629 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/graph.py
--rw-r--r--   0        0        0      334 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/multiline.py
--rw-r--r--   0        0        0     1739 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/password.py
--rw-r--r--   0        0        0     2625 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/plugins.py
--rw-r--r--   0        0        0     8501 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/types.py
--rw-r--r--   0        0        0     3429 2023-04-27 13:33:14.894934 cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/utils.py
--rw-r--r--   0        0        0     2085 2023-04-27 13:33:45.499335 cmem_plugin_base-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 cmem_plugin_base-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      246 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/README-public.md
+-rw-r--r--   0        0        0       76 2023-03-10 08:38:40.281874 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/__init__.py
+-rw-r--r--   0        0        0     3992 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/context.py
+-rw-r--r--   0        0        0     8897 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/description.py
+-rw-r--r--   0        0        0     2742 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/discovery.py
+-rw-r--r--   0        0        0     1370 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/entity.py
+-rw-r--r--   0        0        0       37 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/__init__.py
+-rw-r--r--   0        0        0     1557 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py
+-rw-r--r--   0        0        0     2243 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py
+-rw-r--r--   0        0        0     3629 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py
+-rw-r--r--   0        0        0      334 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/multiline.py
+-rw-r--r--   0        0        0     1739 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/password.py
+-rw-r--r--   0        0        0     2625 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/plugins.py
+-rw-r--r--   0        0        0     8501 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/types.py
+-rw-r--r--   0        0        0     3429 2023-03-10 08:38:07.487562 cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/utils.py
+-rw-r--r--   0        0        0     2088 2023-03-10 08:38:40.281874 cmem_plugin_base-3.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 cmem_plugin_base-3.1.0rc1/PKG-INFO
```

### Comparing `cmem_plugin_base-3.1.0/LICENSE` & `cmem_plugin_base-3.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/context.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/context.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/description.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/description.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/discovery.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 def get_packages():
     """Get installed python packages.
 
     Returns a list of dict with the following keys:
      - name - package name
      - version - package version
     """
-    return json.loads(
-        check_output(["pip", "list", "--format", "json"], shell=False)  # nosec
-    )
+    return json.loads(check_output(["pip", "list", "--format", "json"], shell=False))
 
 
 def discover_plugins_in_module(
     package_name: str = "cmem",
 ) -> list[PluginDescription]:
     """Finds all plugins within a base package.
```

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/entity.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/entity.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/choice.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/dataset.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/graph.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/parameter/password.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/parameter/password.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/plugins.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/plugins.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/types.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/types.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/cmem_plugin_base/dataintegration/utils.py` & `cmem_plugin_base-3.1.0rc1/cmem_plugin_base/dataintegration/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-3.1.0/pyproject.toml` & `cmem_plugin_base-3.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-base"
-version = "3.1.0"
+version = "3.1.0rc1"
 license = "Apache-2.0"
 description = "Base classes for developing eccenca Coporate Memory plugins."
 authors = ["eccenca <cmempy-developer@eccenca.com>"]
 maintainers = [
     "Sebastian Tramp <sebastian.tramp@eccenca.com>",
     "Robert Isele <robert.isele@eccenca.com>"
 ]
@@ -16,15 +16,15 @@
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugins", "DataIntegration"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-cmem-cmempy = "==23.1"
+cmem-cmempy = ">=22.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
 pytest-memray = "^1.3.0"
 black = "^23.1.0"
 bandit = "^1.7.2"
```

### Comparing `cmem_plugin_base-3.1.0/PKG-INFO` & `cmem_plugin_base-3.1.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-base
-Version: 3.1.0
+Version: 3.1.0rc1
 Summary: Base classes for developing eccenca Coporate Memory plugins.
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugins,DataIntegration
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
@@ -13,15 +13,15 @@
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-cmempy (==23.1)
+Requires-Dist: cmem-cmempy (>=22.1)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-base
 
 Python base classes for developing eccenca Coporate Memory plugins.
 
 In order to kick-start developing eccenca Corporate Memory Plugins, please check out this project template: https://github.com/eccenca/cmem-plugin-template
```

