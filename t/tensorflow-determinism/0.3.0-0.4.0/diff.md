# Comparing `tmp/tensorflow-determinism-0.3.0.tar.gz` & `tmp/tensorflow-determinism-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorflow-determinism-0.3.0.tar", last modified: Thu Oct 24 23:48:23 2019, max compression
+gzip compressed data, was "dist/tensorflow-determinism-0.4.0.tar", last modified: Wed Apr 26 23:18:29 2023, max compression
```

## Comparing `tensorflow-determinism-0.3.0.tar` & `tensorflow-determinism-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/tensorflow_determinism.egg-info/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    16169 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/tensorflow_determinism.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       14 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/tensorflow_determinism.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/tensorflow_determinism.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      347 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/tensorflow_determinism.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    16169 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2450 2019-10-07 22:38:37.000000 tensorflow-determinism-0.3.0/setup.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    13451 2019-10-24 23:42:10.000000 tensorflow-determinism-0.3.0/README.md
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/tfdeterminism/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      717 2019-10-24 23:36:41.000000 tensorflow-determinism-0.3.0/tfdeterminism/version.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     5169 2019-10-24 23:36:41.000000 tensorflow-determinism-0.3.0/tfdeterminism/patch.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      875 2019-10-07 22:38:37.000000 tensorflow-determinism-0.3.0/tfdeterminism/__init__.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/test/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      904 2019-10-07 22:38:37.000000 tensorflow-determinism-0.3.0/test/test_patch_apply.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      979 2019-10-07 22:38:37.000000 tensorflow-determinism-0.3.0/test/test_misc.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    17519 2019-10-24 23:36:41.000000 tensorflow-determinism-0.3.0/test/test_patch_bias_add.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       38 2019-10-24 23:48:23.000000 tensorflow-determinism-0.3.0/setup.cfg
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/tensorflow_determinism.egg-info/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      665 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/tensorflow_determinism.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       14 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/tensorflow_determinism.egg-info/top_level.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/tensorflow_determinism.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      230 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/tensorflow_determinism.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      665 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1937 2023-04-26 23:14:53.000000 tensorflow-determinism-0.4.0/setup.py
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/tfdeterminism/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1175 2023-04-26 23:14:29.000000 tensorflow-determinism-0.4.0/tfdeterminism/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       38 2023-04-26 23:18:29.000000 tensorflow-determinism-0.4.0/setup.cfg
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       18 2023-04-26 23:17:40.000000 tensorflow-determinism-0.4.0/MANIFEST.in
```

### Comparing `tensorflow-determinism-0.3.0/test/test_patch_apply.py` & `tensorflow-determinism-0.4.0/tfdeterminism/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 The TensorFlow-Determinism Authors. All Rights Reserved
+# Copyright 2023 NVIDIA. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,21 @@
 # limitations under the License.
 # ========================================================================
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-import sys
+distribution_name = "tensorflow-determinism"
 
-import tensorflow as tf
+version = "0.4.0"
 
-sys.path.append('..')
-from tfdeterminism import patch
-patch()
+long_description = """
+The `tensorflow-determinism` PyPI distribution has been deprecated and the
+`tfdeterminism` package in this distribution contains no code.
+
+Please install the latest version of the
+[framework-reproducibility](https://pypi.org/project/framework-reproducibility/)
+PyPI distribution.
+"""
+
+print(long_description)
```

