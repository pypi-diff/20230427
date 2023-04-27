# Comparing `tmp/aiidalab_widgets_base-2.0.0b5.tar.gz` & `tmp/aiidalab_widgets_base-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiidalab_widgets_base-2.0.0b5.tar", last modified: Thu Mar 23 16:52:24 2023, max compression
+gzip compressed data, was "aiidalab_widgets_base-2.0.0b6.tar", last modified: Sun Mar 26 12:37:21 2023, max compression
```

## Comparing `aiidalab_widgets_base-2.0.0b5.tar` & `aiidalab_widgets_base-2.0.0b6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:52:24.328553 aiidalab_widgets_base-2.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-23 16:52:24.328553 aiidalab_widgets_base-2.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:52:24.324553 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    44666 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/computational_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:52:24.328553 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/elns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    29442 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:52:24.328553 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    43261 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:52:24.324553 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-23 16:52:24.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-23 16:52:24.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 16:52:24.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 16:52:24.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-23 16:52:24.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 16:52:24.000000 aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-23 16:52:24.328553 aiidalab_widgets_base-2.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:52:24.328553 aiidalab_widgets_base-2.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_computational_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_elns.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-23 16:52:15.000000 aiidalab_widgets_base-2.0.0b5/tests/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.304571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44666 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/computational_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.304571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/elns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29442 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43261 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.304571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_computational_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_elns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_wizard.py
```

### Comparing `aiidalab_widgets_base-2.0.0b5/LICENSE.txt` & `aiidalab_widgets_base-2.0.0b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/PKG-INFO` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aiidalab_widgets_base
-Version: 2.0.0b5
+Name: aiidalab-widgets-base
+Version: 2.0.0b6
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -34,26 +34,26 @@
 
 ## Documentation
 
 Hosted on [aiidalab-widgets-base.readthedocs.io](https://aiidalab-widgets-base.readthedocs.io).
 
 ## For maintainers
 
-To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch|--tag-num] [--tag [alpha|beta|rc]]`.
+To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch] [--tag-num --tag [alpha|beta|rc]]`.
 This will:
 
   1. Create a tagged release with bumped version and push it to the repository.
   2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
 
 Additional notes:
 
   - Use the `--dry` option to preview the release change.
   - The release tag (e.g. a/b/rc) is determined from the last release.
     Use the `--tag` option to switch the release tag.
-  - This packages follows semantic versioning.
+  - This packages follows [semantic versioning](https://semver.org/).
 
 ## License
 
 MIT
 
 ## Citation
```

### Comparing `aiidalab_widgets_base-2.0.0b5/README.md` & `aiidalab_widgets_base-2.0.0b6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 ## Documentation
 
 Hosted on [aiidalab-widgets-base.readthedocs.io](https://aiidalab-widgets-base.readthedocs.io).
 
 ## For maintainers
 
-To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch|--tag-num] [--tag [alpha|beta|rc]]`.
+To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch] [--tag-num --tag [alpha|beta|rc]]`.
 This will:
 
   1. Create a tagged release with bumped version and push it to the repository.
   2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
 
 Additional notes:
 
   - Use the `--dry` option to preview the release change.
   - The release tag (e.g. a/b/rc) is determined from the last release.
     Use the `--tag` option to switch the release tag.
-  - This packages follows semantic versioning.
+  - This packages follows [semantic versioning](https://semver.org/).
 
 ## License
 
 MIT
 
 ## Citation
```

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/__init__.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,8 +72,8 @@
     "SubmitButtonWidget",
     "WizardAppWidget",
     "WizardAppWidgetStep",
     "register_viewer_widget",
     "viewer",
 ]
 
-__version__ = "2.0.0b5"
+__version__ = "2.0.0b6"
```

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/bug_report.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/computational_resources.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/data/__init__.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/databases.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/databases.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,17 @@
             children=(providers_header, providers, filters),
             layout=layout,
             **kwargs,
         )
 
     def _update_structure(self, change: dict) -> None:
         """New structure chosen"""
-        self.structure = change["new"].as_ase if change["new"] else None
+        self.structure = (
+            change["new"].as_aiida_structuredata.get_ase() if change["new"] else None
+        )
 
 
 class ComputationalResourcesDatabaseWidget(ipw.VBox):
     """Extract the setup of a known computer from the AiiDA code registry."""
 
     default_calc_job_plugin = tl.Unicode(allow_none=True)
     ssh_config = tl.Dict()
```

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/dicts.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/dicts.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/elns.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/export.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/misc.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/misc.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/nodes.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/nodes.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/process.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/process.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/structures.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/structures.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/utils/__init__.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/viewers.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/viewers.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base/wizard.py` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/wizard.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/PKG-INFO` & `aiidalab_widgets_base-2.0.0b6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aiidalab-widgets-base
-Version: 2.0.0b5
+Name: aiidalab_widgets_base
+Version: 2.0.0b6
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -34,26 +34,26 @@
 
 ## Documentation
 
 Hosted on [aiidalab-widgets-base.readthedocs.io](https://aiidalab-widgets-base.readthedocs.io).
 
 ## For maintainers
 
-To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch|--tag-num] [--tag [alpha|beta|rc]]`.
+To create a new release, clone the repository, install development dependencies with `pip install -e '.[dev]'`, and then execute `bumpver update [--major|--minor|--patch] [--tag-num --tag [alpha|beta|rc]]`.
 This will:
 
   1. Create a tagged release with bumped version and push it to the repository.
   2. Trigger a GitHub actions workflow that creates a GitHub release and publishes it on PyPI.
 
 Additional notes:
 
   - Use the `--dry` option to preview the release change.
   - The release tag (e.g. a/b/rc) is determined from the last release.
     Use the `--tag` option to switch the release tag.
-  - This packages follows semantic versioning.
+  - This packages follows [semantic versioning](https://semver.org/).
 
 ## License
 
 MIT
 
 ## Citation
```

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/SOURCES.txt` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/aiidalab_widgets_base.egg-info/requires.txt` & `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/setup.cfg` & `aiidalab_widgets_base-2.0.0b6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 per-file-ignores = 
 	aiidalab_widgets_base/__init__.py: E402
 exclude = 
 	docs/,
 	docs/source/conf.py
 
 [bumpver]
-current_version = "v2.0.0b5"
+current_version = "v2.0.0b6"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_bug_report.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_computational_resources.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_databases.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_elns.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_export.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_nodes.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_process.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_structures.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_viewers.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_viewers.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b5/tests/test_wizard.py` & `aiidalab_widgets_base-2.0.0b6/tests/test_wizard.py`

 * *Files identical despite different names*

