# Comparing `tmp/yaecs-1.0.2.tar.gz` & `tmp/yaecs-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-1.0.2.tar", last modified: Wed Sep 14 15:35:37 2022, max compression
+gzip compressed data, was "yaecs-3.0.8.tar", last modified: Wed Apr 26 15:08:44 2023, max compression
```

## Comparing `yaecs-1.0.2.tar` & `yaecs-3.0.8.tar`

### file list

```diff
@@ -1,22 +1,62 @@
-drwxrwxr-x   0 valentingoldite  (1000) valentingoldite  (1000)        0 2022-09-14 15:35:37.190203 yaecs-1.0.2/
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     7641 2022-09-14 15:28:44.000000 yaecs-1.0.2/COPYING.LESSER.md
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)    34915 2022-09-14 15:28:44.000000 yaecs-1.0.2/COPYING.md
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)    34915 2022-09-14 15:28:44.000000 yaecs-1.0.2/LICENSE.md
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)       24 2022-09-14 15:28:44.000000 yaecs-1.0.2/MANIFEST.in
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     3710 2022-09-14 15:35:37.190203 yaecs-1.0.2/PKG-INFO
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     5421 2022-09-14 15:28:44.000000 yaecs-1.0.2/README.md
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)       38 2022-09-14 15:35:37.190203 yaecs-1.0.2/setup.cfg
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     1424 2022-09-14 15:32:32.000000 yaecs-1.0.2/setup.py
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     3394 2022-09-14 15:28:44.000000 yaecs-1.0.2/short-readme.md
-drwxrwxr-x   0 valentingoldite  (1000) valentingoldite  (1000)        0 2022-09-14 15:35:37.190203 yaecs-1.0.2/yaecs/
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     1015 2022-09-14 14:50:54.000000 yaecs-1.0.2/yaecs/__init__.py
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)    83427 2022-09-14 15:22:12.000000 yaecs-1.0.2/yaecs/config.py
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)    23150 2022-09-14 14:50:54.000000 yaecs-1.0.2/yaecs/config_history.py
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)    16642 2022-09-14 15:08:37.000000 yaecs-1.0.2/yaecs/config_utils.py
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     8534 2022-09-14 14:50:54.000000 yaecs-1.0.2/yaecs/user_utils.py
-drwxrwxr-x   0 valentingoldite  (1000) valentingoldite  (1000)        0 2022-09-14 15:35:37.190203 yaecs-1.0.2/yaecs.egg-info/
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)     3710 2022-09-14 15:35:37.000000 yaecs-1.0.2/yaecs.egg-info/PKG-INFO
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)      330 2022-09-14 15:35:37.000000 yaecs-1.0.2/yaecs.egg-info/SOURCES.txt
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)        1 2022-09-14 15:35:37.000000 yaecs-1.0.2/yaecs.egg-info/dependency_links.txt
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)        7 2022-09-14 15:35:37.000000 yaecs-1.0.2/yaecs.egg-info/requires.txt
--rw-rw-r--   0 valentingoldite  (1000) valentingoldite  (1000)        6 2022-09-14 15:35:37.000000 yaecs-1.0.2/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.472321 yaecs-3.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.456321 yaecs-3.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 15:08:18.000000 yaecs-3.0.8/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-26 15:08:18.000000 yaecs-3.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-04-26 15:08:18.000000 yaecs-3.0.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-26 15:08:18.000000 yaecs-3.0.8/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-26 15:08:18.000000 yaecs-3.0.8/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    71342 2023-04-26 15:08:18.000000 yaecs-3.0.8/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-04-26 15:08:18.000000 yaecs-3.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 15:08:18.000000 yaecs-3.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-26 15:08:44.472321 yaecs-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-26 15:08:18.000000 yaecs-3.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-26 15:08:18.000000 yaecs-3.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-26 15:08:18.000000 yaecs-3.0.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-04-26 15:08:18.000000 yaecs-3.0.8/resources/yaecs_constructor_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:08:44.472321 yaecs-3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-26 15:08:18.000000 yaecs-3.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-26 15:08:18.000000 yaecs-3.0.8/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.456321 yaecs-3.0.8/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-26 15:08:18.000000 yaecs-3.0.8/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34035 2023-04-26 15:08:18.000000 yaecs-3.0.8/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-26 15:08:18.000000 yaecs-3.0.8/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.464321 yaecs-3.0.8/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-26 15:08:18.000000 yaecs-3.0.8/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.468321 yaecs-3.0.8/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.472321 yaecs-3.0.8/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43721 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33291 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-04-26 15:08:18.000000 yaecs-3.0.8/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:08:44.472321 yaecs-3.0.8/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 15:08:44.000000 yaecs-3.0.8/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-1.0.2/COPYING.LESSER.md` & `yaecs-3.0.8/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-1.0.2/COPYING.md` & `yaecs-3.0.8/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-1.0.2/LICENSE.md` & `yaecs-3.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-1.0.2/PKG-INFO` & `yaecs-3.0.8/short-readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-Metadata-Version: 2.1
-Name: yaecs
-Version: 1.0.2
-Summary: Reactive Reality Machine Learning Config System
-Home-page: https://gitlab.com/reactivereality/public/yaecs
-Author: Reactive Reality AG
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: COPYING.LESSER.md
-License-File: COPYING.md
-
 # YAECS (Yet Another Experiment Config System)
 
 [![Offial repo](https://img.shields.io/badge/official%20repo-YAECS-%23ff9626?logo=gitlab)](https://gitlab.com/reactivereality/public/yaecs)
 ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
 [![License](https://img.shields.io/badge/license-LGPLV3%2B-%23c4c2c2)](https://www.gnu.org/licenses/)
 
 ---
 
 This package is a Config System which allows easy manipulation of config files
 for safe, clear and repeatable experiments.
 
 **DISCLAIMER:** This repository is the public version of a repository that is
 the property of [Reactive Reality](https://www.reactivereality.com/). This
-repository IS NOT OFFICIAL and can not to be maintained in the future. Some
-minor changed* are applied from the
+repository IS NOT OFFICIAL and might not be maintained in the future. Some
+minor changes* are applied from the
 [official repository (GitLab)](https://gitlab.com/reactivereality/public/yaecs)
 (under lesser GNU license).
 
 *documentation and other PyPI related changes
 
 [LINK TO DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home)
```

### Comparing `yaecs-1.0.2/README.md` & `yaecs-3.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
 [![License](https://img.shields.io/badge/license-LGPLV3%2B-%23c4c2c2)](https://www.gnu.org/licenses/)
 
 ---
 
 **DISCLAIMER: This repository is the public version of a repository that is the
 property of [Reactive Reality](https://www.reactivereality.com/). This
-repository IS NOT OFFICIAL and can not to be maintained in the future. Some
-minor changed * are applied from the
+repository IS NOT OFFICIAL and might not be maintained in the future. Some
+minor changes * are applied from the
 [official repository (GitLab)](https://gitlab.com/reactivereality/public/yaecs)
 (under lesser GNU license).**
 
 This package is a Config System which allows easy manipulation of config files
 for safe, clear and repeatable experiments. In a few words, it is:
 
 - built for Machine Learning with its constraints in mind, but also usable
```

### Comparing `yaecs-1.0.2/setup.py` & `yaecs-3.0.8/unittests/config/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""
-Reactive Reality Machine Learning Config System - setup file
-Copyright (C) 2022  Reactive Reality
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Lesser General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Lesser General Public License for more details.
-
-    You should have received a copy of the GNU Lesser General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import pathlib
-
-from setuptools import setup
-
-VERSION = '1.0.2'
-
-# The directory containing this file
-HERE = pathlib.Path(__file__).parent
-
-# The text of the README file
-SHORT_README = (HERE / "short-readme.md").read_text()
-
-setup(name='yaecs', version=VERSION,
-      description='Reactive Reality Machine Learning Config System',
-      long_description=SHORT_README,
-      long_description_content_type="text/markdown",
-      url='https://gitlab.com/reactivereality/public/yaecs',
-      author='Reactive Reality AG', packages=['yaecs'],
-      package_dir={'yaecs': 'yaecs'}, install_requires=["pyyaml"])
+"""
+Reactive Reality Machine Learning Config System - unit tests
+Copyright (C) 2022  Reactive Reality
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Lesser General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Lesser General Public License for more details.
+
+    You should have received a copy of the GNU Lesser General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from yaecs.user_utils import get_template_class, make_config
+
+
+def load_config(*configs, default_config=None, preprocessing=None,
+                postprocessing=None):
+    return make_config(default_config, *configs,
+                       pre_processing_dict=preprocessing,
+                       post_processing_dict=postprocessing,
+                       additional_configs_suffix="_path",
+                       variations_suffix="var*", grids_suffix="grid",
+                       do_not_merge_command_line=True)
+
+
+def template(default_config=None):
+    return get_template_class(default_config_path=default_config,
+                              additional_configs_suffix="_path",
+                              variations_suffix="var*", grids_suffix="grid")
```

### Comparing `yaecs-1.0.2/yaecs/__init__.py` & `yaecs-3.0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Reactive Reality Machine Learning Config System
+Reactive Reality Machine Learning Config System - setup file
 Copyright (C) 2022  Reactive Reality
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU Lesser General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
@@ -12,14 +12,10 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from .config import Configuration
-from .config_history import ConfigHistory
-from .user_utils import get_template_class, make_config
+from setuptools import setup
 
-__all__ = [
-    'ConfigHistory', 'Configuration', 'get_template_class', 'make_config'
-]
+setup()
```

### Comparing `yaecs-1.0.2/yaecs/config_history.py` & `yaecs-3.0.8/yaecs/config_history.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,532 +1,545 @@
-"""
-Reactive Reality Machine Learning Config System - ConfigHistory object
-Copyright (C) 2022  Reactive Reality
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Lesser General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Lesser General Public License for more details.
-
-    You should have received a copy of the GNU Lesser General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import glob
-import importlib
-import io
-import os
-import sys
-import time
-from functools import partial
-from pathlib import Path
-
-try:
-    import pygraphviz as pgv
-except ImportError:
-    pass
-
-from .config import Configuration
-
-
-class ConfigHistory:
-    """Configuration history manager."""
-
-    def __init__(self, folder_path, config_filters=None,
-                 difference_processor=None, ignore_for_graphing=None,
-                 add_relevant_edges=False, tolerance=0, group_by=None,
-                 metrics=None, display_span=False, config_class=Configuration):
-        if not importlib.util.find_spec("pygraphviz"):
-            raise ImportError("ConfigHistory requires pygraphviz - "
-                              "currently not installed!")
-        self.difference_processor = self.make_processor(difference_processor)
-        self.ignore_for_graphing = self.make_processor(ignore_for_graphing)
-        self.group_by = group_by
-
-        print("Loading configs...")
-        if not isinstance(folder_path, dict):
-            yaml_files = glob.glob(os.path.join(folder_path, "**/*.yaml"),
-                                   recursive=True)
-            self.paths = [
-                file[:-len("_hierarchy.yaml")] + ".yaml" for file in yaml_files
-                if file.endswith("_hierarchy.yaml")
-            ]
-            self.names = [
-                self.get_experiment_name_from_file(file, folder_path)
-                for file in self.paths
-            ]
-            self.folders = [("", folder_path)] * len(self.paths)
-        else:
-            self.paths = []
-            self.names = []
-            self.folders = []
-            for i in folder_path:
-                yaml_files = glob.glob(
-                    os.path.join(folder_path[i], "**/*.yaml"), recursive=True)
-                to_add = [
-                    fil[:-len("_hierarchy.yaml")] + ".yaml"
-                    for fil in yaml_files if fil.endswith("_hierarchy.yaml")
-                ]
-                self.paths += to_add
-                self.folders += [(i, folder_path[i])] * len(to_add)
-                self.names += [
-                    self.get_experiment_name_from_file(fil, folder_path[i],
-                                                       name=i)
-                    for fil in to_add
-                ]
-
-        if config_filters is not None:
-            if not isinstance(config_filters, list):
-                config_filters = [config_filters]
-            for filt in config_filters:
-                good = [filt(i) for i in self.paths]
-                self.paths = [
-                    self.paths[i] for i in range(len(self.paths)) if good[i]
-                ]
-                self.names = [
-                    self.names[i] for i in range(len(self.names)) if good[i]
-                ]
-                self.folders = [
-                    self.folders[i] for i in range(len(self.folders))
-                    if good[i]
-                ]
-
-        self.modification_times = [os.path.getmtime(fil) for fil in self.paths]
-        self.configs = []
-        for path in self.paths:
-            try:
-                sys.stdout = io.StringIO()
-                self.configs.append(config_class.load_config(path))
-                sys.stdout = sys.__stdout__
-            except Exception as exception:
-                sys.stdout = sys.__stdout__
-                print(f"Error while loading config {path} : ", exception)
-        for i, config in enumerate(self.configs):
-            if config.get("_former_saving_time", None) is not None:
-                modification_time = config._former_saving_time
-                self.modification_times[i] = modification_time
-
-        print(f"Successfully loaded {len(self.configs)} configs from folder(s)"
-              f" {folder_path}. Analysing differences...")
-
-        self.matrix = self.compute_difference_matrix()
-        self.span = self.compute_span()
-        self.similarity_matrix = [[
-            len(
-                self.ignore_for_graphing(list(self.matrix[row][col]), row, col,
-                                         self))
-            for col in range(len(self.matrix[row]))
-        ] for row in range(len(self.matrix))]
-        self.similarity_coefficients = [
-            sum(row) for row in self.similarity_matrix
-        ]
-        self.metrics = self.compute_metrics(metrics)
-        self.config_graph = pgv.AGraph(
-            strict=True, directed=True,
-            label=self.format_span() if display_span else "")
-        self.compute_graph(add_relevant_edges=add_relevant_edges,
-                           tolerance=tolerance)
-        print("Config graph done !")
-
-    def compute_span(self):
-        span = {}
-        for i, row in enumerate(self.matrix):
-            for j, elem in enumerate(row):
-                ignored = self.ignore_for_graphing(elem, i, j, self)
-                for param in ignored:
-                    if param[0] not in span:
-                        span[param[0]] = [param[1]]
-                    elif param[1] not in span[param[0]]:
-                        span[param[0]].append(param[1])
-        return span
-
-    def compute_metrics(self, metrics):
-        if metrics is None:
-            return {}
-        if (isinstance(metrics, (list, tuple)) and all(
-                isinstance(i, (list, tuple)) and len(i) in [2, 3]
-                for i in metrics)):
-            pass
-        elif isinstance(metrics, (list, tuple)) and len(metrics) in [2, 3]:
-            metrics = [metrics]
-        else:
-            raise Exception(f"Unrecognized format for metric {metrics}.")
-        to_return = {}
-        folder_paths = [Path(i).parents[0] for i in self.paths]
-        for metric in metrics:
-            try:
-                metric_value = metric[1](folder_paths)
-            except Exception as exception:
-                print("There was an error parsing metrics : ", exception)
-                raise exception
-            if len(metric) == 2:
-                to_return[metric[0]] = (metric_value, "")
-            else:
-                to_return[metric[0]] = (metric_value, metric[2])
-        return to_return
-
-    def compute_graph(self, add_relevant_edges=False, tolerance=0):
-
-        def add_directed_edge(first, second):
-            if (self.modification_times[first] >
-                    self.modification_times[second]):
-                self.config_graph.add_edge(
-                    second, first, labeljust="l",
-                    label=self.format_list(self.matrix[second][first]))
-            else:
-                self.config_graph.add_edge(
-                    first, second, labeljust="l",
-                    label=self.format_list(self.matrix[first][second]))
-
-        potential_nodes = list(range(len(self.configs)))
-        potential_nodes.sort(key=lambda x: self.modification_times[x])
-        potential_nodes.sort(key=lambda x: self.similarity_coefficients[x])
-        nodes_added = []
-        for _ in range(len(potential_nodes)):
-            if not nodes_added:
-                index = potential_nodes.pop(0)
-                nodes_added.append(index)
-                self.config_graph.add_node(
-                    index, style="filled", label=(
-                        f"{self.names[index]}\n"
-                        f"Date : {time.ctime(self.modification_times[index])}"
-                        f"{self.format_metrics(index)}"))
-            else:
-                # Find which node to add in priority
-                nodes_by_connectivity = nodes_added.copy()
-                nodes_by_connectivity.sort(
-                    key=lambda x: -self.modification_times[x])
-                nodes_by_connectivity.sort(
-                    key=lambda x: self.similarity_coefficients[x])
-
-                relevant_similarities = [[
-                    (self.similarity_matrix[i][j] if j in potential_nodes else
-                     max(self.similarity_matrix[i]) + 1)
-                    for j in range(len(self.similarity_matrix[i]))
-                ] for i in nodes_by_connectivity]
-                best_new_node = [min(i) for i in relevant_similarities]
-                new_parent_node = nodes_by_connectivity[best_new_node.index(
-                    min(best_new_node))]
-                potential_new_nodes = [
-                    i for i in potential_nodes
-                    if (self.similarity_matrix[new_parent_node][i] == min(
-                        best_new_node))
-                ]
-                potential_new_nodes.sort(
-                    key=lambda x: self.modification_times[x])
-                potential_new_nodes.sort(
-                    key=lambda x: self.similarity_coefficients[x])
-                new_node = potential_nodes.pop(
-                    potential_nodes.index(potential_new_nodes[0]))
-                # Add the node
-                nodes_added.append(new_node)
-                date = time.ctime(self.modification_times[new_node])
-                self.config_graph.add_node(
-                    new_node, style="filled",
-                    label=(f"{self.names[new_node]}\n"
-                           f"Date : {date}"
-                           f"{self.format_metrics(new_node)}"))
-                add_directed_edge(new_parent_node, new_node)
-
-        if self.group_by is not None:
-            if isinstance(self.group_by, str):
-                self.group_by = [self.group_by]
-            groups = {}
-            for i, config in enumerate(self.configs):
-                group = ""
-                for j in self.group_by:
-                    params = config.get_parameter_names()
-                    for param in params:
-                        if param.endswith("." + j) or param == j:
-                            group += (f" ; {j}:{config[param]}"
-                                      if group else f"{j}:{config[param]}")
-                if group and group not in groups:
-                    groups[group] = [i]
-                elif group:
-                    groups[group].append(i)
-            for group, subgraph in groups.items():
-                self.config_graph.add_subgraph(subgraph,
-                                               name="cluster_" + group,
-                                               label="\n" + group + "\n")
-
-        if add_relevant_edges:
-            relevant_similarities = [[
-                len(self.matrix[i][j]) if j != i else max(
-                    len(self.matrix[i][k])
-                    for k in range(len(self.matrix[i]))) + 1
-                for j in range(len(self.similarity_matrix[i]))
-            ] for i in range(len(self.similarity_matrix))]
-            for i, similarities in enumerate(relevant_similarities):
-                minimum = min(similarities)
-                for j, sim in enumerate(similarities):
-                    if sim - minimum < tolerance + 1:
-                        if not ((i, j) in self.config_graph.edges() or
-                                (i, j) in self.config_graph.edges()):
-                            add_directed_edge(i, j)
-
-    def compute_colors(self, scheme="date", fill="top", legend=True,
-                       base_color="white", class_scheme="/set312/",
-                       number_scheme="/blues9/"):
-        to_remove = []
-
-        # Remove previous legend
-        for i in self.config_graph.nodes():
-            if "legend" in str(i):
-                to_remove.append(i)
-        for i in to_remove:
-            self.config_graph.remove_node(i)
-
-        # Determine colouring scheme
-        unavailable = []
-        if scheme == "date":
-            indexes_values = list(
-                zip(list(range(len(self.configs))), self.modification_times))
-            indexes_values.sort(key=lambda x: x[1])
-            color_scheme = number_scheme
-        elif scheme.startswith("metric:"):
-            if scheme[7:] not in self.metrics:
-                raise Exception(f"Unknown metric : {scheme[7:]}.")
-            indexes_values = list(
-                zip(list(range(len(self.configs))),
-                    self.metrics[scheme[7:]][0]))
-            for indexes_value in indexes_values:
-                if indexes_value[1] is None:
-                    unavailable.append((indexes_value[0], None))
-            indexes_values = [
-                index for index in indexes_values
-                if index[0] not in [i[0] for i in unavailable]
-            ]
-            if all(
-                    isinstance(x[1], (int,
-                                      float)) and not isinstance(x[1], bool)
-                    for x in indexes_values):
-                indexes_values.sort(key=lambda x: x[1])
-                color_scheme = number_scheme
-            else:
-                color_scheme = class_scheme
-        elif scheme.startswith("param:"):
-            values = []
-            for config in self.configs:
-                found = False
-                params = config.get_parameter_names()
-                for param in params:
-                    if param.endswith("." + scheme[6:]) or param == scheme[6:]:
-                        if not found:
-                            values.append(config[param])
-                            found = True
-                        else:
-                            raise Exception(f"Ambiguous param : {scheme[6:]}.")
-                if not found:
-                    raise Exception(f"Unknown param : {scheme[6:]}.")
-            indexes_values = list(zip(list(range(len(self.configs))), values))
-            for indexes_value in indexes_values:
-                if indexes_value[1] is None:
-                    unavailable.append((indexes_value[0], None))
-            indexes_values = [
-                index for index in indexes_values
-                if index[0] not in [i[0] for i in unavailable]
-            ]
-            if all(
-                    isinstance(x[1], (int,
-                                      float)) and not isinstance(x[1], bool)
-                    for x in indexes_values):
-                indexes_values.sort(key=lambda x: x[1])
-                color_scheme = number_scheme
-            else:
-                color_scheme = class_scheme
-        else:
-            raise Exception(f"Unrecognized coloring scheme : {scheme}.")
-        value_set = list({x[1] for x in indexes_values})
-        if color_scheme == number_scheme:
-            value_set.sort()
-            color_set = [5]
-            if fill == "top":
-                for _ in range(len(value_set) - 1):
-                    color_set = [max([0, min(color_set) - 1])] + color_set
-            elif fill == "bottom":
-                for _ in range(len(value_set) - 1):
-                    color_set += [max([0, min(color_set) - 1])]
-            elif fill == "full":
-                factor = 6. / float(len(value_set))
-                acc = 6 - factor
-                for _ in range(len(value_set) - 1):
-                    color_set = [max([0, int(acc // 1)])] + color_set
-                    acc -= factor
-            else:
-                raise Exception(f"Unrecognized fill value : {fill}. "
-                                "Please use 'top', 'bottom' or 'full'.")
-        else:
-            color_set = [x % 13 for x in range(len(value_set))]
-        one_is_colored = False
-        for i in self.config_graph.nodes():
-            if "legend" not in str(i):
-                value = None
-                for index_value in indexes_values:
-                    if index_value[0] == int(str(i)):
-                        value = index_value[1]
-                if value is not None:
-                    color = color_set[value_set.index(value)]
-                    is_none = False
-                    for index_value in unavailable:
-                        if index_value[0] == int(str(i)):
-                            is_none = True
-                            i.attr["fillcolor"] = "gray91"
-                    if not is_none:
-                        one_is_colored = True
-                        i.attr["fillcolor"] = (color_scheme + str(color)
-                                               if color else base_color)
-                else:
-                    i.attr["fillcolor"] = "gray91"
-        if legend and one_is_colored:
-            legend_nodes = []
-            for i in range(6 if color_scheme ==
-                           number_scheme else len(value_set)):
-                if color_scheme == number_scheme:
-                    values = [
-                        value_set[v] for v in range(len(value_set))
-                        if color_set[v] == i
-                    ]
-                    if not values:
-                        label = None
-                    elif len(values) == 1:
-                        if isinstance(values[0], float) and scheme != 'date':
-                            label = f"{values[0]:.3f}"
-                        else:
-                            label = str(values[0] if scheme != 'date' else time
-                                        .ctime(values[0]))
-                    else:
-                        if isinstance(values[0], float) and scheme != 'date':
-                            label = f"[{min(values):.3f} ; {max(values):.3f}]"
-                        else:
-                            label = ("[" + str(
-                                min(values) if scheme != 'date' else time
-                                .ctime(min(values))) + " ; " + str(
-                                    max(values) if scheme != 'date' else time
-                                    .ctime(max(values))) + "]")
-                else:
-                    if i not in color_set:
-                        label = None
-                    else:
-                        label = ""
-                        for j, val in enumerate(value_set):
-                            label += f"{val}\n" if color_set[j] == i else ""
-                if label is not None:
-                    legend_nodes.append("legend_" + str(i))
-                    self.config_graph.add_node(
-                        "legend_" + str(i), label=label, style="filled",
-                        fillcolor=color_scheme + str(i) if i else base_color)
-            self.config_graph.add_subgraph(legend_nodes, name="cluster_legend",
-                                           label=f"Legend for {scheme}")
-            for i in legend_nodes:
-                self.config_graph.add_edge(
-                    self.modification_times.index(max(
-                        self.modification_times)), i, style="invis")
-
-    def draw_graph(self, path="graph.png", scheme="date", fill="top",
-                   legend=True):
-        self.compute_colors(scheme=scheme, fill=fill, legend=legend)
-        self.config_graph.layout(prog="dot")
-        self.config_graph.draw(path)
-        print("Config graph saved !")
-
-    def format_metrics(self, index):
-        string = ""
-        for i, metric in self.metrics.items():
-            if metric[0][index] is None:
-                string += f"\n{i} : UNAVAILABLE"
-            elif isinstance(metric[0][index], float):
-                string += f"\n{i} : {metric[0][index]:.3f} {metric[1]}"
-            else:
-                string += f"\n{i} : {metric[0][index]} {metric[1]}"
-        return string
-
-    def format_span(self):
-        string = "\nExploration span\n\n"
-        for i, val in self.span.items():
-            string += f"{i} : {val}" + r"\l"
-        return string
-
-    def compute_difference_matrix(self):
-        matrix = []
-        similars = []
-        for i, config_i in enumerate(self.configs):
-            row = []
-            similar = [i]
-            for j, config_j in enumerate(self.configs):
-                if j != i:
-                    differences = config_i.compare(config_j, reduce=True)
-                    row.append(
-                        self.difference_processor(differences, i, j, self))
-                    if not row[-1]:
-                        similar.append(j)
-                else:
-                    row.append([])
-            if all(similar[0] not in k for k in similars):
-                similars.append(similar)
-            matrix.append(row)
-        fuse = []
-        for i in similars:
-            if len(i) > 1:
-                dates = [
-                    self.modification_times[j] if j in i else 0
-                    for j in range(len(self.modification_times))
-                ]
-                key_func = partial(lambda x, dates: dates[x], dates=dates)
-                sort = sorted(i, key=key_func, reverse=True)
-                for j in sort:
-                    if j != dates.index(max(dates)):
-                        self.names[dates.index(max(dates))] = (
-                            f"({self.names[j]})\n"
-                            + self.names[dates.index(max(dates))])
-                fuse += [j for j in i if j != dates.index(max(dates))]
-        self.names = [
-            self.names[i] for i in range(len(self.names)) if i not in fuse
-        ]
-        self.configs = [
-            self.configs[i] for i in range(len(self.configs)) if i not in fuse
-        ]
-        self.paths = [
-            self.paths[i] for i in range(len(self.paths)) if i not in fuse
-        ]
-        self.modification_times = [
-            self.modification_times[i]
-            for i in range(len(self.modification_times)) if i not in fuse
-        ]
-        matrix = [[
-            matrix[i][j] for j in range(len(matrix[i])) if j not in fuse
-        ] for i in range(len(matrix)) if i not in fuse]
-        return matrix
-
-    @staticmethod
-    def get_experiment_name_from_file(file, folder, name=None):
-        file_parent_minus_folder = os.path.relpath(
-            Path(file).parents[0], os.path.commonpath([folder,
-                                                       file])).strip("/_")
-        if name is None:
-            return file_parent_minus_folder
-        return f"{name}:{file_parent_minus_folder}"
-
-    @staticmethod
-    def format_list(list_to_format):
-        string = " "
-        for i in list_to_format:
-            string += str(i[0]) + " : " + str(i[1]) + r"\l "
-        return string
-
-    @staticmethod
-    def make_processor(argument):
-
-        def apply_list(list_to_apply, inp, *args):
-            for func in list_to_apply:
-                inp = func(inp, *args)
-            return inp
-
-        if argument is None:
-            return lambda d, i, j, h: d
-        if not isinstance(argument, list):
-            return argument
-        return lambda d, i, j, h: apply_list(argument, d, i, j, h)
+"""
+Reactive Reality Machine Learning Config System - ConfigHistory object
+Copyright (C) 2022  Reactive Reality
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Lesser General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Lesser General Public License for more details.
+
+    You should have received a copy of the GNU Lesser General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import glob
+import io
+import logging
+import os
+import sys
+import time
+from pathlib import Path
+
+try:
+    import pygraphviz as pgv
+except ImportError:
+    pgv = None
+
+from .config.config import Configuration
+
+YAECS_LOGGER = logging.getLogger(__name__)
+
+
+class ConfigHistory:
+    """Configuration history manager."""
+
+    def __init__(self, folder_path, config_filters=None,
+                 difference_processor=None, ignore_for_graphing=None,
+                 add_relevant_edges=False, tolerance=0, group_by=None,
+                 metrics=None, display_span=False, config_class=Configuration):
+        if pgv is None:
+            raise ImportError("ConfigHistory requires pygraphviz - "
+                              "currently not installed!")
+        self.difference_processor = self.make_processor(difference_processor)
+        self.ignore_for_graphing = self.make_processor(ignore_for_graphing)
+        self.group_by = group_by
+
+        YAECS_LOGGER.info("Loading configs...")
+        if not isinstance(folder_path, dict):
+            yaml_files = glob.glob(os.path.join(folder_path, "**/*.yaml"),
+                                   recursive=True)
+            self.paths = [
+                file[:-len("_hierarchy.yaml")] + ".yaml" for file in yaml_files
+                if file.endswith("_hierarchy.yaml")
+            ]
+            self.names = [
+                self.get_experiment_name_from_file(file, folder_path)
+                for file in self.paths
+            ]
+            self.folders = [("", folder_path)] * len(self.paths)
+        else:
+            self.paths = []
+            self.names = []
+            self.folders = []
+            for i in folder_path:
+                yaml_files = glob.glob(
+                    os.path.join(folder_path[i], "**/*.yaml"), recursive=True)
+                to_add = [
+                    fil[:-len("_hierarchy.yaml")] + ".yaml"
+                    for fil in yaml_files if fil.endswith("_hierarchy.yaml")
+                ]
+                self.paths += to_add
+                self.folders += [(i, folder_path[i])] * len(to_add)
+                self.names += [
+                    self.get_experiment_name_from_file(fil, folder_path[i],
+                                                       name=i)
+                    for fil in to_add
+                ]
+
+        if config_filters is not None:
+            if not isinstance(config_filters, list):
+                config_filters = [config_filters]
+            for filt in config_filters:
+                good = [filt(i) for i in self.paths]
+                self.paths = [
+                    self.paths[i] for i in range(len(self.paths)) if good[i]
+                ]
+                self.names = [
+                    self.names[i] for i in range(len(self.names)) if good[i]
+                ]
+                self.folders = [
+                    self.folders[i] for i in range(len(self.folders))
+                    if good[i]
+                ]
+
+        self.modification_times = [os.path.getmtime(fil) for fil in self.paths]
+        self.configs = []
+        for path in self.paths:
+            try:
+                sys.stdout = io.StringIO()
+                self.configs.append(config_class.load_config(path))
+                sys.stdout = sys.__stdout__
+            except Exception:
+                sys.stdout = sys.__stdout__
+                YAECS_LOGGER.error(f"Error while loading config {path}.")
+                raise
+        for i, config in enumerate(self.configs):
+            if config.get("_former_saving_time", None) is not None:
+                modification_time = config._former_saving_time
+                self.modification_times[i] = modification_time
+
+        YAECS_LOGGER.info(f"Successfully loaded {len(self.configs)} configs from folder(s) {folder_path}. "
+                          f"Analysing differences...")
+
+        self.matrix = self.compute_difference_matrix()
+        self.span = self.compute_span()
+        self.similarity_matrix = [[
+            len(
+                self.ignore_for_graphing(list(self.matrix[row][col]), row, col,
+                                         self))
+            for col in range(len(self.matrix[row]))
+        ] for row in range(len(self.matrix))]
+        self.similarity_coefficients = [
+            sum(row) for row in self.similarity_matrix
+        ]
+        self.metrics = self.compute_metrics(metrics)
+        self.config_graph = pgv.AGraph(
+            strict=True, directed=True,
+            label=self.format_span() if display_span else "")
+        self.compute_graph(add_relevant_edges=add_relevant_edges,
+                           tolerance=tolerance)
+        YAECS_LOGGER.info("Config graph done !")
+
+    def compute_span(self):
+        """ Computes span of parameter in experiments. """
+        span = {}
+        for i, row in enumerate(self.matrix):
+            for j, elem in enumerate(row):
+                ignored = self.ignore_for_graphing(elem, i, j, self)
+                for param in ignored:
+                    if param[0] not in span:
+                        span[param[0]] = [param[1]]
+                    elif param[1] not in span[param[0]]:
+                        span[param[0]].append(param[1])
+        return span
+
+    def compute_metrics(self, metrics):
+        """ Compute all defined metrics to prepare for printing """
+        if metrics is None:
+            return {}
+        if (isinstance(metrics, (list, tuple)) and all(
+                isinstance(i, (list, tuple)) and len(i) in [2, 3]
+                for i in metrics)):
+            pass
+        elif isinstance(metrics, (list, tuple)) and len(metrics) in [2, 3]:
+            metrics = [metrics]
+        else:
+            raise Exception(f"Unrecognised format for metric {metrics}.")
+        to_return = {}
+        folder_paths = [Path(i).parents[0] for i in self.paths]
+        for metric in metrics:
+            try:
+                metric_value = metric[1](folder_paths)
+            except Exception:
+                YAECS_LOGGER.error("There was an error parsing metrics.")
+                raise
+            if len(metric) == 2:
+                to_return[metric[0]] = (metric_value, "")
+            else:
+                to_return[metric[0]] = (metric_value, metric[2])
+        return to_return
+
+    def compute_graph(self, add_relevant_edges=False, tolerance=0):
+        """ Computes the graph itself before filling it in. """
+
+        def add_directed_edge(first, second):
+            if (self.modification_times[first] >
+                    self.modification_times[second]):
+                self.config_graph.add_edge(
+                    second, first, labeljust="l",
+                    label=self.format_list(self.matrix[second][first]))
+            else:
+                self.config_graph.add_edge(
+                    first, second, labeljust="l",
+                    label=self.format_list(self.matrix[first][second]))
+
+        potential_nodes = list(range(len(self.configs)))
+        potential_nodes.sort(key=lambda x: self.modification_times[x])
+        potential_nodes.sort(key=lambda x: self.similarity_coefficients[x])
+        nodes_added = []
+        for _ in range(len(potential_nodes)):
+            if not nodes_added:
+                index = potential_nodes.pop(0)
+                nodes_added.append(index)
+                self.config_graph.add_node(
+                    index, style="filled", label=(
+                        f"{self.names[index]}\n"
+                        f"Date : {time.ctime(self.modification_times[index])}"
+                        f"{self.format_metrics(index)}"))
+            else:
+                # Find which node to add in priority
+                nodes_by_connectivity = nodes_added.copy()
+                nodes_by_connectivity.sort(
+                    key=lambda x: -self.modification_times[x])
+                nodes_by_connectivity.sort(
+                    key=lambda x: self.similarity_coefficients[x])
+
+                relevant_similarities = [[
+                    (self.similarity_matrix[i][j] if j in potential_nodes else
+                     max(self.similarity_matrix[i]) + 1)
+                    for j in range(len(self.similarity_matrix[i]))
+                ] for i in nodes_by_connectivity]
+                best_new_node = [min(i) for i in relevant_similarities]
+                new_parent_node = nodes_by_connectivity[best_new_node.index(
+                    min(best_new_node))]
+                potential_new_nodes = [
+                    i for i in potential_nodes
+                    if (self.similarity_matrix[new_parent_node][i] == min(
+                        best_new_node))
+                ]
+                potential_new_nodes.sort(
+                    key=lambda x: self.modification_times[x])
+                potential_new_nodes.sort(
+                    key=lambda x: self.similarity_coefficients[x])
+                new_node = potential_nodes.pop(
+                    potential_nodes.index(potential_new_nodes[0]))
+                # Add the node
+                nodes_added.append(new_node)
+                date = time.ctime(self.modification_times[new_node])
+                self.config_graph.add_node(
+                    new_node, style="filled",
+                    label=(f"{self.names[new_node]}\n"
+                           f"Date : {date}"
+                           f"{self.format_metrics(new_node)}"))
+                add_directed_edge(new_parent_node, new_node)
+
+        if self.group_by is not None:
+            if isinstance(self.group_by, str):
+                self.group_by = [self.group_by]
+            groups = {}
+            for i, config in enumerate(self.configs):
+                group = ""
+                for j in self.group_by:
+                    params = config.get_parameter_names()
+                    for param in params:
+                        if param.endswith("." + j) or param == j:
+                            group += (f" ; {j}:{config[param]}"
+                                      if group else f"{j}:{config[param]}")
+                if group and group not in groups:
+                    groups[group] = [i]
+                elif group:
+                    groups[group].append(i)
+            for group, subgraph in groups.items():
+                self.config_graph.add_subgraph(subgraph,
+                                               name="cluster_" + group,
+                                               label="\n" + group + "\n")
+
+        if add_relevant_edges:
+            relevant_similarities = [[
+                len(self.matrix[i][j]) if j != i else max(
+                    len(self.matrix[i][k])
+                    for k in range(len(self.matrix[i]))) + 1
+                for j in range(len(self.similarity_matrix[i]))
+            ] for i in range(len(self.similarity_matrix))]
+            for i, similarities in enumerate(relevant_similarities):
+                minimum = min(similarities)
+                for j, sim in enumerate(similarities):
+                    if sim - minimum < tolerance + 1:
+                        if not ((i, j) in self.config_graph.edges() or
+                                (i, j) in self.config_graph.edges()):
+                            add_directed_edge(i, j)
+
+    # pylint: disable=too-many-locals,too-many-branches
+    def compute_colors(self, scheme="date", fill="top", legend=True,
+                       base_color="white", class_scheme="/set312/",
+                       number_scheme="/blues9/"):
+        """ Gets the colour scheme and interpolates it properly. """
+        to_remove = []
+
+        # Remove previous legend
+        for i in self.config_graph.nodes():
+            if "legend" in str(i):
+                to_remove.append(i)
+        for i in to_remove:
+            self.config_graph.remove_node(i)
+
+        # Determine colouring scheme
+        unavailable = []
+        if scheme == "date":
+            indexes_values = list(
+                zip(list(range(len(self.configs))), self.modification_times))
+            indexes_values.sort(key=lambda x: x[1])
+            color_scheme = number_scheme
+        elif scheme.startswith("metric:"):
+            if scheme[7:] not in self.metrics:
+                raise Exception(f"Unknown metric : {scheme[7:]}.")
+            indexes_values = list(
+                zip(list(range(len(self.configs))),
+                    self.metrics[scheme[7:]][0]))
+            for indexes_value in indexes_values:
+                if indexes_value[1] is None:
+                    unavailable.append((indexes_value[0], None))
+            indexes_values = [
+                index for index in indexes_values
+                if index[0] not in [i[0] for i in unavailable]
+            ]
+            if all(
+                    isinstance(x[1], (int,
+                                      float)) and not isinstance(x[1], bool)
+                    for x in indexes_values):
+                indexes_values.sort(key=lambda x: x[1])
+                color_scheme = number_scheme
+            else:
+                color_scheme = class_scheme
+        elif scheme.startswith("param:"):
+            values = []
+            for config in self.configs:
+                found = False
+                params = config.get_parameter_names()
+                for param in params:
+                    if param.endswith("." + scheme[6:]) or param == scheme[6:]:
+                        if not found:
+                            values.append(config[param])
+                            found = True
+                        else:
+                            raise Exception(f"Ambiguous param : {scheme[6:]}.")
+                if not found:
+                    raise Exception(f"Unknown param : {scheme[6:]}.")
+            indexes_values = list(zip(list(range(len(self.configs))), values))
+            for indexes_value in indexes_values:
+                if indexes_value[1] is None:
+                    unavailable.append((indexes_value[0], None))
+            indexes_values = [
+                index for index in indexes_values
+                if index[0] not in [i[0] for i in unavailable]
+            ]
+            if all(
+                    isinstance(x[1], (int,
+                                      float)) and not isinstance(x[1], bool)
+                    for x in indexes_values):
+                indexes_values.sort(key=lambda x: x[1])
+                color_scheme = number_scheme
+            else:
+                color_scheme = class_scheme
+        else:
+            raise Exception(f"Unrecognised coloring scheme : {scheme}.")
+        value_set = list({x[1] for x in indexes_values})
+        if color_scheme == number_scheme:
+            value_set.sort()
+            color_set = [5]
+            if fill == "top":
+                for _ in range(len(value_set) - 1):
+                    color_set = [max([0, min(color_set) - 1])] + color_set
+            elif fill == "bottom":
+                for _ in range(len(value_set) - 1):
+                    color_set += [max([0, min(color_set) - 1])]
+            elif fill == "full":
+                factor = 6. / float(len(value_set))
+                acc = 6 - factor
+                for _ in range(len(value_set) - 1):
+                    color_set = [max([0, int(acc // 1)])] + color_set
+                    acc -= factor
+            else:
+                raise Exception(f"Unrecognised fill value : {fill}. "
+                                "Please use 'top', 'bottom' or 'full'.")
+        else:
+            color_set = [x % 13 for x in range(len(value_set))]
+        one_is_colored = False
+        for i in self.config_graph.nodes():
+            if "legend" not in str(i):
+                value = None
+                for index_value in indexes_values:
+                    if index_value[0] == int(str(i)):
+                        value = index_value[1]
+                if value is not None:
+                    color = color_set[value_set.index(value)]
+                    is_none = False
+                    for index_value in unavailable:
+                        if index_value[0] == int(str(i)):
+                            is_none = True
+                            i.attr["fillcolor"] = "gray91"
+                    if not is_none:
+                        one_is_colored = True
+                        i.attr["fillcolor"] = (color_scheme + str(color)
+                                               if color else base_color)
+                else:
+                    i.attr["fillcolor"] = "gray91"
+        if legend and one_is_colored:
+            legend_nodes = []
+            for i in range(6 if color_scheme ==
+                           number_scheme else len(value_set)):
+                if color_scheme == number_scheme:
+                    values = [
+                        value_set[v] for v in range(len(value_set))
+                        if color_set[v] == i
+                    ]
+                    if not values:
+                        label = None
+                    elif len(values) == 1:
+                        if isinstance(values[0], float) and scheme != 'date':
+                            label = f"{values[0]:.3f}"
+                        else:
+                            label = str(values[0] if scheme != 'date' else time
+                                        .ctime(values[0]))
+                    else:
+                        if isinstance(values[0], float) and scheme != 'date':
+                            label = f"[{min(values):.3f} ; {max(values):.3f}]"
+                        else:
+                            label = ("[" + str(
+                                min(values) if scheme != 'date' else time
+                                .ctime(min(values))) + " ; " + str(
+                                    max(values) if scheme != 'date' else time
+                                    .ctime(max(values))) + "]")
+                else:
+                    if i not in color_set:
+                        label = None
+                    else:
+                        label = ""
+                        for j, val in enumerate(value_set):
+                            label += f"{val}\n" if color_set[j] == i else ""
+                if label is not None:
+                    legend_nodes.append("legend_" + str(i))
+                    self.config_graph.add_node(
+                        "legend_" + str(i), label=label, style="filled",
+                        fillcolor=color_scheme + str(i) if i else base_color)
+            self.config_graph.add_subgraph(legend_nodes, name="cluster_legend",
+                                           label=f"Legend for {scheme}")
+            for i in legend_nodes:
+                self.config_graph.add_edge(
+                    self.modification_times.index(max(
+                        self.modification_times)), i, style="invis")
+
+    def draw_graph(self, path="graph.png", scheme="date", fill="top",
+                   legend=True):
+        """ Function called to draw the computed graph. """
+        self.compute_colors(scheme=scheme, fill=fill, legend=legend)
+        self.config_graph.layout(prog="dot")
+        self.config_graph.draw(path)
+        YAECS_LOGGER.info("Config graph saved !")
+
+    def format_metrics(self, index):
+        """ Format computed metrics for printing. """
+        string = ""
+        for i, metric in self.metrics.items():
+            if metric[0][index] is None:
+                string += f"\n{i} : UNAVAILABLE"
+            elif isinstance(metric[0][index], float):
+                string += f"\n{i} : {metric[0][index]:.3f} {metric[1]}"
+            else:
+                string += f"\n{i} : {metric[0][index]} {metric[1]}"
+        return string
+
+    def format_span(self):
+        """ Format the span of a param over experiments for printing. """
+        string = "\nExploration span\n\n"
+        for i, val in self.span.items():
+            string += f"{i} : {val}" + r"\l"
+        return string
+
+    def compute_difference_matrix(self):
+        """ Compute difference matrix to prepare for printing. """
+        matrix = []
+        similars = []
+        for i, config_i in enumerate(self.configs):
+            row = []
+            similar = [i]
+            for j, config_j in enumerate(self.configs):
+                if j != i:
+                    differences = config_i.compare(config_j, reduce=True)
+                    row.append(
+                        self.difference_processor(differences, i, j, self))
+                    if not row[-1]:
+                        similar.append(j)
+                else:
+                    row.append([])
+            if all(similar[0] not in k for k in similars):
+                similars.append(similar)
+            matrix.append(row)
+        fuse = []
+        for i in similars:
+            if len(i) > 1:
+                dates = [
+                    self.modification_times[j] if j in i else 0
+                    for j in range(len(self.modification_times))
+                ]
+                sort = sorted(i, key=lambda x: dates[x], reverse=True)  # pylint: disable=cell-var-from-loop
+                for j in sort:
+                    if j != dates.index(max(dates)):
+                        self.names[dates.index(max(dates))] = (
+                            f"({self.names[j]})\n"
+                            + self.names[dates.index(max(dates))])
+                fuse += [j for j in i if j != dates.index(max(dates))]
+        self.names = [
+            self.names[i] for i in range(len(self.names)) if i not in fuse
+        ]
+        self.configs = [
+            self.configs[i] for i in range(len(self.configs)) if i not in fuse
+        ]
+        self.paths = [
+            self.paths[i] for i in range(len(self.paths)) if i not in fuse
+        ]
+        self.modification_times = [
+            self.modification_times[i]
+            for i in range(len(self.modification_times)) if i not in fuse
+        ]
+        matrix = [[
+            matrix[i][j] for j in range(len(matrix[i])) if j not in fuse
+        ] for i in range(len(matrix)) if i not in fuse]
+        return matrix
+
+    @staticmethod
+    def get_experiment_name_from_file(file, folder, name=None):
+        """ Extracts the experiment name from the name of a file saved in an experiment folder. """
+        file_parent_minus_folder = os.path.relpath(
+            Path(file).parents[0], os.path.commonpath([folder,
+                                                       file])).strip("/_")
+        if name is None:
+            return file_parent_minus_folder
+        return f"{name}:{file_parent_minus_folder}"
+
+    @staticmethod
+    def format_list(list_to_format):
+        """ Formats list for printing """
+        string = " "
+        for i in list_to_format:
+            string += str(i[0]) + " : " + str(i[1]) + r"\l "
+        return string
+
+    @staticmethod
+    def make_processor(argument):
+        """ Returns a processor created from input. """
+
+        def apply_list(list_to_apply, inp, *args):
+            for func in list_to_apply:
+                inp = func(inp, *args)
+            return inp
+
+        if argument is None:
+            return lambda d, i, j, h: d
+        if not isinstance(argument, list):
+            return argument
+        return lambda d, i, j, h: apply_list(argument, d, i, j, h)
```

