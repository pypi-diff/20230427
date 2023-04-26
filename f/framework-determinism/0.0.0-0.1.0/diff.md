# Comparing `tmp/framework-determinism-0.0.0.tar.gz` & `tmp/framework-determinism-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/framework-determinism-0.0.0.tar", last modified: Sat Oct 24 05:14:26 2020, max compression
+gzip compressed data, was "dist/framework-determinism-0.1.0.tar", last modified: Wed Apr 26 23:04:31 2023, max compression
```

## Comparing `framework-determinism-0.0.0.tar` & `framework-determinism-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,12 @@
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1235 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2729 2020-10-24 05:12:29.000000 framework-determinism-0.0.0/setup.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    40546 2020-10-21 16:33:56.000000 framework-determinism-0.0.0/README.md
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/fwd9m_reserve/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1191 2020-10-24 01:06:43.000000 framework-determinism-0.0.0/fwd9m_reserve/warning.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      701 2020-10-24 05:10:44.000000 framework-determinism-0.0.0/fwd9m_reserve/version.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      856 2020-10-24 01:06:19.000000 framework-determinism-0.0.0/fwd9m_reserve/__init__.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/framework_determinism.egg-info/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1235 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/framework_determinism.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       14 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/framework_determinism.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/framework_determinism.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      412 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/framework_determinism.egg-info/SOURCES.txt
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/test/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2775 2020-10-21 16:33:56.000000 framework-determinism-0.0.0/test/test_utils.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1244 2020-10-21 16:33:56.000000 framework-determinism-0.0.0/test/test_patch_apply.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1086 2020-10-21 16:33:56.000000 framework-determinism-0.0.0/test/test_misc.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      921 2020-10-21 16:33:56.000000 framework-determinism-0.0.0/test/test_enable_determinism_apply.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    18836 2020-10-21 16:33:56.000000 framework-determinism-0.0.0/test/test_patch_bias_add.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       67 2020-10-24 05:14:26.000000 framework-determinism-0.0.0/setup.cfg
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-26 23:04:31.000000 framework-determinism-0.1.0/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      654 2023-04-26 23:04:31.000000 framework-determinism-0.1.0/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1937 2023-04-26 19:42:39.000000 framework-determinism-0.1.0/setup.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      345 2023-04-26 19:40:39.000000 framework-determinism-0.1.0/README.md
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-26 23:04:31.000000 framework-determinism-0.1.0/framework_determinism.egg-info/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      654 2023-04-26 23:04:30.000000 framework-determinism-0.1.0/framework_determinism.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)        6 2023-04-26 23:04:30.000000 framework-determinism-0.1.0/framework_determinism.egg-info/top_level.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2023-04-26 23:04:30.000000 framework-determinism-0.1.0/framework_determinism.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      216 2023-04-26 23:04:31.000000 framework-determinism-0.1.0/framework_determinism.egg-info/SOURCES.txt
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-26 23:04:31.000000 framework-determinism-0.1.0/fwd9m/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1165 2023-04-26 20:13:43.000000 framework-determinism-0.1.0/fwd9m/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       38 2023-04-26 23:04:31.000000 framework-determinism-0.1.0/setup.cfg
```

### Comparing `framework-determinism-0.0.0/setup.py` & `framework-determinism-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,49 @@
-# Copyright 2020 NVIDIA Corporation. All Rights Reserved
+# Copyright 2020-2023 NVIDIA Corporation. All Rights Reserved
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ========================================================================
 
-from setuptools import setup
-import os
+import importlib
+import setuptools
 
-distribution_name = 'framework-determinism'
-package_name = 'fwd9m' + '_reserve'
-# package_name = 'fwd9m'
-
-# This file needs to be executed during installation. It's not possible to
-# import the full package during installation because it will fail to import if
-# all the supported frameworks have not been installed. By temporarility
-# appending to sys.path, it's possible to just import from the version module.
-import sys
-sys.path.append(package_name)
-from version import __version__ as version
-from warning import message as warning_message
-sys.path.remove(package_name)
-
-if warning_message:
-  long_description = warning_message
-else:
-  readme = os.path.join(os.path.dirname(os.path.realpath(__file__)),
-                        "README.md")
-  with open(readme, "r") as fp:
-    long_description = fp.read()
-
-description = ("Providing determinism in the DL frameworks")
-url = "https://github.com/NVIDIA/%s" % distribution_name
-install_requires = [] # intentionally not including the framework packages
-
-classifiers = [
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'Topic :: Scientific/Engineering :: Artificial Intelligence',
-    'License :: OSI Approved :: Apache Software License',
-    'Programming Language :: Python'
-]
-
-keywords = "framework tensorflow gpu deep-learning determinism"
-
-setup(
-  name                          = distribution_name,
-  version                       = version,
+package_name = 'fwd9m'
+# package_name = 'tfdeterminism'
+
+print("PACKAGE IMPORT WARNING (expected):")
+package = importlib.import_module(package_name)
+
+description = ("Providing reproducibility in deep learning frameworks")
+url = "https://github.com/NVIDIA/%s" % package.distribution_name
+
+print("Now running setuptools.setup()")
+
+# Note that using python 3.6 (i.e. via the `python3.6` executable) results in
+# the long_description_content_type being ignored.
+# For more info, see https://github.com/di/markdown-description-example/issues/4
+
+setuptools.setup(
+  name                          = package.distribution_name,
+  version                       = package.version,
   packages                      = [package_name],
   url                           = url,
   license                       = 'Apache 2.0',
   author                        = 'NVIDIA',
   author_email                  = 'duncan@nvidia.com',
   description                   = description,
-  long_description              = long_description,
+  long_description              = package.long_description,
   long_description_content_type = 'text/markdown',
-  install_requires              = install_requires,
-  classifiers                   = classifiers,
-  keywords                      = keywords,
-  platforms                     = ['TensorFlow']
+  install_requires              = [],
+  classifiers                   = [],
+  keywords                      = [],
+  platforms                     = []
 )
```

