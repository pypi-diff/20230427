# Comparing `tmp/newtgw-0.0.6.tar.gz` & `tmp/newtgw-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newtgw-0.0.6.tar", last modified: Mon Apr 24 13:22:07 2023, max compression
+gzip compressed data, was "newtgw-0.0.7.tar", last modified: Wed Apr 26 21:16:32 2023, max compression
```

## Comparing `newtgw-0.0.6.tar` & `newtgw-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:22:07.399085 newtgw-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 13:21:53.000000 newtgw-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 13:21:53.000000 newtgw-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 13:22:07.399085 newtgw-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 13:21:53.000000 newtgw-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 13:21:53.000000 newtgw-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:22:07.399085 newtgw-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-24 13:21:53.000000 newtgw-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:22:07.399085 newtgw-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:22:07.399085 newtgw-0.0.6/src/newtgw/
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-24 13:21:53.000000 newtgw-0.0.6/src/newtgw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:22:07.399085 newtgw-0.0.6/src/newtgw/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 13:21:53.000000 newtgw-0.0.6/src/newtgw/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-24 13:21:53.000000 newtgw-0.0.6/src/newtgw/_jsii/newtgw@0.0.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:21:53.000000 newtgw-0.0.6/src/newtgw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:22:07.399085 newtgw-0.0.6/src/newtgw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 13:22:07.000000 newtgw-0.0.6/src/newtgw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 13:22:07.000000 newtgw-0.0.6/src/newtgw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:22:07.000000 newtgw-0.0.6/src/newtgw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:22:07.000000 newtgw-0.0.6/src/newtgw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 13:22:07.000000 newtgw-0.0.6/src/newtgw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:16:32.036443 newtgw-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 21:16:15.000000 newtgw-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 21:16:15.000000 newtgw-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 21:16:32.036443 newtgw-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 21:16:15.000000 newtgw-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 21:16:15.000000 newtgw-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:16:32.036443 newtgw-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-26 21:16:15.000000 newtgw-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:16:32.032443 newtgw-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:16:32.036443 newtgw-0.0.7/src/newtgw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-26 21:16:15.000000 newtgw-0.0.7/src/newtgw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:16:32.036443 newtgw-0.0.7/src/newtgw/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-26 21:16:15.000000 newtgw-0.0.7/src/newtgw/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-04-26 21:16:15.000000 newtgw-0.0.7/src/newtgw/_jsii/newtgw@0.0.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:16:15.000000 newtgw-0.0.7/src/newtgw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:16:32.036443 newtgw-0.0.7/src/newtgw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 21:16:31.000000 newtgw-0.0.7/src/newtgw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 21:16:32.000000 newtgw-0.0.7/src/newtgw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:16:31.000000 newtgw-0.0.7/src/newtgw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 21:16:31.000000 newtgw-0.0.7/src/newtgw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 21:16:31.000000 newtgw-0.0.7/src/newtgw.egg-info/top_level.txt
```

### Comparing `newtgw-0.0.6/LICENSE` & `newtgw-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `newtgw-0.0.6/PKG-INFO` & `newtgw-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtgw
-Version: 0.0.6
+Version: 0.0.7
 Summary: newtgw
 Home-page: https://github.com/cmorgia/newtgw.git
 Author: Claudio Morgia<cmorgia@amazon.ch>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cmorgia/newtgw.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `newtgw-0.0.6/setup.py` & `newtgw-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "newtgw",
-    "version": "0.0.6",
+    "version": "0.0.7",
     "description": "newtgw",
     "license": "Apache-2.0",
     "url": "https://github.com/cmorgia/newtgw.git",
     "long_description_content_type": "text/markdown",
     "author": "Claudio Morgia<cmorgia@amazon.ch>",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,23 @@
     },
     "packages": [
         "newtgw",
         "newtgw._jsii"
     ],
     "package_data": {
         "newtgw._jsii": [
-            "newtgw@0.0.6.jsii.tgz"
+            "newtgw@0.0.7.jsii.tgz"
         ],
         "newtgw": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.76.0, <3.0.0",
-        "aws-cdk.aws-lambda-python-alpha==2.76.0.a0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `newtgw-0.0.6/src/newtgw.egg-info/PKG-INFO` & `newtgw-0.0.7/src/newtgw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtgw
-Version: 0.0.6
+Version: 0.0.7
 Summary: newtgw
 Home-page: https://github.com/cmorgia/newtgw.git
 Author: Claudio Morgia<cmorgia@amazon.ch>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cmorgia/newtgw.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

