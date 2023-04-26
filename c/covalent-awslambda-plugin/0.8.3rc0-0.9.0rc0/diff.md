# Comparing `tmp/covalent-awslambda-plugin-0.8.3rc0.tar.gz` & `tmp/covalent-awslambda-plugin-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-awslambda-plugin-0.8.3rc0.tar", last modified: Thu Sep 22 19:48:27 2022, max compression
+gzip compressed data, was "covalent-awslambda-plugin-0.9.0rc0.tar", last modified: Fri Sep 30 14:52:37 2022, max compression
```

## Comparing `covalent-awslambda-plugin-0.8.3rc0.tar` & `covalent-awslambda-plugin-0.9.0rc0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 19:48:27.355956 covalent-awslambda-plugin-0.8.3rc0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9898 2022-09-22 19:48:27.355956 covalent-awslambda-plugin-0.8.3rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7067 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 19:48:27.355956 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22876 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin/awslambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 19:48:27.355956 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9898 2022-09-22 19:48:27.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-22 19:48:27.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 19:48:27.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-22 19:48:27.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-22 19:48:27.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-22 19:48:27.000000 covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-22 19:48:27.355956 covalent-awslambda-plugin-0.8.3rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 19:48:27.355956 covalent-awslambda-plugin-0.8.3rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34421 2022-09-22 19:48:20.000000 covalent-awslambda-plugin-0.8.3rc0/tests/lambda_executor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 14:52:37.975559 covalent-awslambda-plugin-0.9.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9898 2022-09-30 14:52:37.975559 covalent-awslambda-plugin-0.9.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7067 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 14:52:37.975559 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22876 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin/awslambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 14:52:37.975559 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9898 2022-09-30 14:52:37.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-30 14:52:37.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 14:52:37.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-30 14:52:37.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-30 14:52:37.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-30 14:52:37.000000 covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-30 14:52:37.975559 covalent-awslambda-plugin-0.9.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 14:52:37.975559 covalent-awslambda-plugin-0.9.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34421 2022-09-30 14:52:20.000000 covalent-awslambda-plugin-0.9.0rc0/tests/lambda_executor_test.py
```

### Comparing `covalent-awslambda-plugin-0.8.3rc0/LICENSE` & `covalent-awslambda-plugin-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-awslambda-plugin-0.8.3rc0/PKG-INFO` & `covalent-awslambda-plugin-0.9.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-awslambda-plugin
-Version: 0.8.3rc0
+Version: 0.9.0rc0
 Summary: Covalent AWS Lambda Executor Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-awslambda-plugin
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-awslambda-plugin/archive/v0.8.3.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-awslambda-plugin/archive/v0.9.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="./assets/aws_lambda_readme_banner.jpg" width=150%>
         
         [![covalent](https://img.shields.io/badge/covalent-0.177.0-purple)](https://github.com/AgnostiqHQ/covalent)
```

### Comparing `covalent-awslambda-plugin-0.8.3rc0/README.md` & `covalent-awslambda-plugin-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin/__init__.py` & `covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin/awslambda.py` & `covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin/awslambda.py`

 * *Files identical despite different names*

### Comparing `covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin/scripts.py` & `covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin/scripts.py`

 * *Files identical despite different names*

### Comparing `covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/PKG-INFO` & `covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-awslambda-plugin
-Version: 0.8.3rc0
+Version: 0.9.0rc0
 Summary: Covalent AWS Lambda Executor Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-awslambda-plugin
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-awslambda-plugin/archive/v0.8.3.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-awslambda-plugin/archive/v0.9.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="./assets/aws_lambda_readme_banner.jpg" width=150%>
         
         [![covalent](https://img.shields.io/badge/covalent-0.177.0-purple)](https://github.com/AgnostiqHQ/covalent)
```

### Comparing `covalent-awslambda-plugin-0.8.3rc0/covalent_awslambda_plugin.egg-info/SOURCES.txt` & `covalent-awslambda-plugin-0.9.0rc0/covalent_awslambda_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-awslambda-plugin-0.8.3rc0/pyproject.toml` & `covalent-awslambda-plugin-0.9.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-awslambda-plugin-0.8.3rc0/setup.py` & `covalent-awslambda-plugin-0.9.0rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 # Covalent is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE. See the License for more details.
 #
 # Relief from the License may be granted by purchasing a commercial license.
 
+import os
 import re
 import site
 import sys
 
 from setuptools import find_packages, setup
 
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
@@ -77,8 +78,9 @@
     ],
     "entry_points": {
         "covalent.executor.executor_plugins": plugins_list,
     },
 }
 
 if __name__ == "__main__":
+    os.environ["BASE_COVALENT_AWS_PLUGINS_ONLY"] = "True"
     setup(**setup_info)
```

### Comparing `covalent-awslambda-plugin-0.8.3rc0/tests/lambda_executor_test.py` & `covalent-awslambda-plugin-0.9.0rc0/tests/lambda_executor_test.py`

 * *Files identical despite different names*

