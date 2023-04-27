# Comparing `tmp/yaecs-3.0.8.tar.gz` & `tmp/yaecs-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-3.0.8.tar", last modified: Wed Apr 26 15:08:44 2023, max compression
+gzip compressed data, was "yaecs-3.0.9.tar", last modified: Thu Apr 27 10:00:06 2023, max compression
```

## Comparing `yaecs-3.0.8.tar` & `yaecs-3.0.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.472321 yaecs-3.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.456321 yaecs-3.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 15:08:18.000000 yaecs-3.0.8/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-26 15:08:18.000000 yaecs-3.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-04-26 15:08:18.000000 yaecs-3.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-26 15:08:18.000000 yaecs-3.0.8/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-26 15:08:18.000000 yaecs-3.0.8/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    71342 2023-04-26 15:08:18.000000 yaecs-3.0.8/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-26 15:08:18.000000 yaecs-3.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 15:08:18.000000 yaecs-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-26 15:08:44.472321 yaecs-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-26 15:08:18.000000 yaecs-3.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-26 15:08:18.000000 yaecs-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-26 15:08:18.000000 yaecs-3.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-04-26 15:08:18.000000 yaecs-3.0.8/resources/yaecs_constructor_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:08:44.472321 yaecs-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-26 15:08:18.000000 yaecs-3.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-26 15:08:18.000000 yaecs-3.0.8/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.456321 yaecs-3.0.8/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-26 15:08:18.000000 yaecs-3.0.8/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    34035 2023-04-26 15:08:18.000000 yaecs-3.0.8/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-26 15:08:18.000000 yaecs-3.0.8/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.472321 yaecs-3.0.8/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43721 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.472321 yaecs-3.0.8/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.849664 yaecs-3.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.829663 yaecs-3.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.837664 yaecs-3.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 09:59:47.000000 yaecs-3.0.9/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-27 09:59:47.000000 yaecs-3.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-04-27 09:59:47.000000 yaecs-3.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-27 09:59:47.000000 yaecs-3.0.9/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-27 09:59:47.000000 yaecs-3.0.9/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    71342 2023-04-27 09:59:47.000000 yaecs-3.0.9/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-27 09:59:47.000000 yaecs-3.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 09:59:47.000000 yaecs-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-27 10:00:06.849664 yaecs-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-27 09:59:47.000000 yaecs-3.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-27 09:59:47.000000 yaecs-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 09:59:47.000000 yaecs-3.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.837664 yaecs-3.0.9/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-04-27 09:59:47.000000 yaecs-3.0.9/resources/yaecs_constructor_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 10:00:06.849664 yaecs-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 09:59:47.000000 yaecs-3.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-27 09:59:47.000000 yaecs-3.0.9/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.829663 yaecs-3.0.9/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.837664 yaecs-3.0.9/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-27 09:59:47.000000 yaecs-3.0.9/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34035 2023-04-27 09:59:47.000000 yaecs-3.0.9/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-27 09:59:47.000000 yaecs-3.0.9/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.837664 yaecs-3.0.9/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.837664 yaecs-3.0.9/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.841664 yaecs-3.0.9/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.841664 yaecs-3.0.9/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.841664 yaecs-3.0.9/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-27 09:59:47.000000 yaecs-3.0.9/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.845664 yaecs-3.0.9/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.849664 yaecs-3.0.9/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43721 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-04-27 09:59:47.000000 yaecs-3.0.9/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:00:06.845664 yaecs-3.0.9/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-27 10:00:06.000000 yaecs-3.0.9/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-27 10:00:06.000000 yaecs-3.0.9/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:00:06.000000 yaecs-3.0.9/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 10:00:06.000000 yaecs-3.0.9/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 10:00:06.000000 yaecs-3.0.9/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-3.0.8/.github/workflows/pipy_deployment.yaml` & `yaecs-3.0.9/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/.gitignore` & `yaecs-3.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/.pylintrc` & `yaecs-3.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/COPYING.LESSER.md` & `yaecs-3.0.9/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/COPYING.md` & `yaecs-3.0.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/DOCUMENTATION_WIP.md` & `yaecs-3.0.9/DOCUMENTATION_WIP.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/LICENSE.md` & `yaecs-3.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/PKG-INFO` & `yaecs-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.0.8
+Version: 3.0.9
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.LESSER.md
 License-File: COPYING.md
 
 # YAECS (Yet Another Experiment Config System)
```

### Comparing `yaecs-3.0.8/README.md` & `yaecs-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/pyproject.toml` & `yaecs-3.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 [project]
 name = "yaecs"
 authors = [
     {name="Reactive Reality AG"},
 ]
 description = """A Config System designed for experimental purposes"""
-requires-python = ">=3.8"
+requires-python = ">=3.6"
 keywords = ["template", "machine", "learning"]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["readme", "version"]
 dependencies = ["pyyaml==6.0", "mock==4.0.3"]
+
 [tool.setuptools]
-py-modules = ["template"]
+py-modules = ["yaecs", "yaecs.config"]
 license-files = ['LICEN[CS]E*', 'COPYING*', 'NOTICE*', 'AUTHORS*']
 
 [tool.setuptools_scm]
 
 [project.urls]
 Source = "https://gitlab.com/reactivereality/public/yaecs"
```

### Comparing `yaecs-3.0.8/resources/yaecs_constructor_overview.png` & `yaecs-3.0.9/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/setup.py` & `yaecs-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/short-readme.md` & `yaecs-3.0.9/short-readme.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/unittests/config/conftest.py` & `yaecs-3.0.9/unittests/config/conftest.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/unittests/config/test_config.py` & `yaecs-3.0.9/unittests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/unittests/config/utils.py` & `yaecs-3.0.9/unittests/config/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/usage_example/configs/project_config.py` & `yaecs-3.0.9/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/usage_example/main.py` & `yaecs-3.0.9/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/usage_example/project_utils/utils.py` & `yaecs-3.0.9/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/__init__.py` & `yaecs-3.0.9/yaecs/__init__.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/config/config.py` & `yaecs-3.0.9/yaecs/config/config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/config/config_base.py` & `yaecs-3.0.9/yaecs/config/config_base.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/config/config_convenience.py` & `yaecs-3.0.9/yaecs/config/config_convenience.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/config/config_getters.py` & `yaecs-3.0.9/yaecs/config/config_getters.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/config/config_hooks.py` & `yaecs-3.0.9/yaecs/config/config_hooks.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/config/config_setters.py` & `yaecs-3.0.9/yaecs/config/config_setters.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/config_history.py` & `yaecs-3.0.9/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/experiment.py` & `yaecs-3.0.9/yaecs/experiment.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/pytorch_lightning_utils.py` & `yaecs-3.0.9/yaecs/pytorch_lightning_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/user_utils.py` & `yaecs-3.0.9/yaecs/user_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs/yaecs_utils.py` & `yaecs-3.0.9/yaecs/yaecs_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.0.8/yaecs.egg-info/PKG-INFO` & `yaecs-3.0.9/yaecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.0.8
+Version: 3.0.9
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.LESSER.md
 License-File: COPYING.md
 
 # YAECS (Yet Another Experiment Config System)
```

### Comparing `yaecs-3.0.8/yaecs.egg-info/SOURCES.txt` & `yaecs-3.0.9/yaecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

