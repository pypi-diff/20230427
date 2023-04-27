# Comparing `tmp/attini-cdk-lib-1.4.0.tar.gz` & `tmp/attini-cdk-lib-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attini-cdk-lib-1.4.0.tar", last modified: Fri Apr 21 08:48:36 2023, max compression
+gzip compressed data, was "attini-cdk-lib-1.4.1.tar", last modified: Thu Apr 27 08:57:46 2023, max compression
```

## Comparing `attini-cdk-lib-1.4.0.tar` & `attini-cdk-lib-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/attini_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   148861 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/attini_cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   251659 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/_jsii/cdk@1.4.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:57:46.869453 attini-cdk-lib-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-27 08:57:46.869453 attini-cdk-lib-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 08:57:46.869453 attini-cdk-lib-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:57:46.869453 attini-cdk-lib-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:57:46.869453 attini-cdk-lib-1.4.1/src/attini_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   148861 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/src/attini_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:57:46.869453 attini-cdk-lib-1.4.1/src/attini_cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/src/attini_cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   251660 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/src/attini_cdk/_jsii/cdk@1.4.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:57:36.000000 attini-cdk-lib-1.4.1/src/attini_cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:57:46.869453 attini-cdk-lib-1.4.1/src/attini_cdk_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-27 08:57:46.000000 attini-cdk-lib-1.4.1/src/attini_cdk_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-27 08:57:46.000000 attini-cdk-lib-1.4.1/src/attini_cdk_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:57:46.000000 attini-cdk-lib-1.4.1/src/attini_cdk_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 08:57:46.000000 attini-cdk-lib-1.4.1/src/attini_cdk_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 08:57:46.000000 attini-cdk-lib-1.4.1/src/attini_cdk_lib.egg-info/top_level.txt
```

### Comparing `attini-cdk-lib-1.4.0/LICENSE` & `attini-cdk-lib-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `attini-cdk-lib-1.4.0/PKG-INFO` & `attini-cdk-lib-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attini-cdk-lib
-Version: 1.4.0
+Version: 1.4.1
 Summary: Attini CDK Constructs
 Home-page: https://attini.io
 Author: oscarostrand<contact@attini.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/attini-cloud-solutions/attini-cdk-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `attini-cdk-lib-1.4.0/README.md` & `attini-cdk-lib-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `attini-cdk-lib-1.4.0/setup.py` & `attini-cdk-lib-1.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "attini-cdk-lib",
-    "version": "1.4.0",
+    "version": "1.4.1",
     "description": "Attini CDK Constructs",
     "license": "Apache-2.0",
     "url": "https://attini.io",
     "long_description_content_type": "text/markdown",
     "author": "oscarostrand<contact@attini.io>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "attini_cdk",
         "attini_cdk._jsii"
     ],
     "package_data": {
         "attini_cdk._jsii": [
-            "cdk@1.4.0.jsii.tgz"
+            "cdk@1.4.1.jsii.tgz"
         ],
         "attini_cdk": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.1.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `attini-cdk-lib-1.4.0/src/attini_cdk/__init__.py` & `attini-cdk-lib-1.4.1/src/attini_cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/PKG-INFO` & `attini-cdk-lib-1.4.1/src/attini_cdk_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attini-cdk-lib
-Version: 1.4.0
+Version: 1.4.1
 Summary: Attini CDK Constructs
 Home-page: https://attini.io
 Author: oscarostrand<contact@attini.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/attini-cloud-solutions/attini-cdk-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

