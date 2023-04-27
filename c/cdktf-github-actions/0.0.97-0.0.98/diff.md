# Comparing `tmp/cdktf-github-actions-0.0.97.tar.gz` & `tmp/cdktf-github-actions-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-github-actions-0.0.97.tar", last modified: Wed Apr 26 00:28:46 2023, max compression
+gzip compressed data, was "cdktf-github-actions-0.0.98.tar", last modified: Thu Apr 27 00:30:40 2023, max compression
```

## Comparing `cdktf-github-actions-0.0.97.tar` & `cdktf-github-actions-0.0.98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:28:46.146444 cdktf-github-actions-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-26 00:28:46.146444 cdktf-github-actions-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:28:46.146444 cdktf-github-actions-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:28:46.142444 cdktf-github-actions-0.0.97/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:28:46.146444 cdktf-github-actions-0.0.97/src/cdktf_github-actions/
--rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/src/cdktf_github-actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:28:46.146444 cdktf-github-actions-0.0.97/src/cdktf_github-actions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/src/cdktf_github-actions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189762 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.97.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:28:34.000000 cdktf-github-actions-0.0.97/src/cdktf_github-actions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:28:46.146444 cdktf-github-actions-0.0.97/src/cdktf_github_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-26 00:28:46.000000 cdktf-github-actions-0.0.97/src/cdktf_github_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 00:28:46.000000 cdktf-github-actions-0.0.97/src/cdktf_github_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:28:46.000000 cdktf-github-actions-0.0.97/src/cdktf_github_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 00:28:46.000000 cdktf-github-actions-0.0.97/src/cdktf_github_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 00:28:46.000000 cdktf-github-actions-0.0.97/src/cdktf_github_actions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:30:40.742631 cdktf-github-actions-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-27 00:30:40.742631 cdktf-github-actions-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:30:40.742631 cdktf-github-actions-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:30:40.742631 cdktf-github-actions-0.0.98/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:30:40.742631 cdktf-github-actions-0.0.98/src/cdktf_github-actions/
+-rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/src/cdktf_github-actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:30:40.742631 cdktf-github-actions-0.0.98/src/cdktf_github-actions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/src/cdktf_github-actions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189768 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.98.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:30:28.000000 cdktf-github-actions-0.0.98/src/cdktf_github-actions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:30:40.742631 cdktf-github-actions-0.0.98/src/cdktf_github_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-27 00:30:40.000000 cdktf-github-actions-0.0.98/src/cdktf_github_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-27 00:30:40.000000 cdktf-github-actions-0.0.98/src/cdktf_github_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:30:40.000000 cdktf-github-actions-0.0.98/src/cdktf_github_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 00:30:40.000000 cdktf-github-actions-0.0.98/src/cdktf_github_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 00:30:40.000000 cdktf-github-actions-0.0.98/src/cdktf_github_actions.egg-info/top_level.txt
```

### Comparing `cdktf-github-actions-0.0.97/LICENSE` & `cdktf-github-actions-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.97/PKG-INFO` & `cdktf-github-actions-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.97
+Version: 0.0.98
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-github-actions-0.0.97/README.md` & `cdktf-github-actions-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.97/setup.py` & `cdktf-github-actions-0.0.98/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-github-actions",
-    "version": "0.0.97",
+    "version": "0.0.98",
     "description": "@awlsring/cdktf-github-actions",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-github-actions.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_github-actions",
         "cdktf_github-actions._jsii"
     ],
     "package_data": {
         "cdktf_github-actions._jsii": [
-            "cdktf-github-actions@0.0.97.jsii.tgz"
+            "cdktf-github-actions@0.0.98.jsii.tgz"
         ],
         "cdktf_github-actions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-github-actions-0.0.97/src/cdktf_github-actions/__init__.py` & `cdktf-github-actions-0.0.98/src/cdktf_github-actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.97/src/cdktf_github_actions.egg-info/PKG-INFO` & `cdktf-github-actions-0.0.98/src/cdktf_github_actions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.97
+Version: 0.0.98
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

