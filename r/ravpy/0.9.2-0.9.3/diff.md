# Comparing `tmp/ravpy-0.9.2.tar.gz` & `tmp/ravpy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ravpy-0.9.2.tar", last modified: Thu Sep 15 13:45:34 2022, max compression
+gzip compressed data, was "dist/ravpy-0.9.3.tar", last modified: Thu Sep 15 13:55:14 2022, max compression
```

## Comparing `ravpy-0.9.2.tar` & `ravpy-0.9.3.tar`

### file list

```diff
@@ -1,41 +1,48 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/
--rw-r--r--   0 apple      (501) staff       (20)     1070 2022-07-14 10:02:21.000000 ravpy-0.9.2/LICENSE.rst
--rw-r--r--   0 apple      (501) staff       (20)     2959 2022-09-15 13:45:34.000000 ravpy-0.9.2/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     2628 2022-09-15 12:40:49.000000 ravpy-0.9.2/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-07-14 09:52:08.000000 ravpy-0.9.2/ravpy/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1085 2022-09-09 12:15:26.000000 ravpy-0.9.2/ravpy/config.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy/distributed/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-02-08 07:57:51.000000 ravpy-0.9.2/ravpy/distributed/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1498 2022-09-15 12:45:55.000000 ravpy-0.9.2/ravpy/distributed/benchmarking.py
--rw-r--r--   0 apple      (501) staff       (20)    16328 2022-09-15 13:42:27.000000 ravpy-0.9.2/ravpy/distributed/compute.py
--rw-r--r--   0 apple      (501) staff       (20)     4393 2022-09-15 12:51:52.000000 ravpy-0.9.2/ravpy/distributed/evaluate.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy/distributed/op_functions/
--rw-r--r--   0 apple      (501) staff       (20)       67 2022-09-15 12:40:49.000000 ravpy-0.9.2/ravpy/distributed/op_functions/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    21540 2022-09-15 12:40:49.000000 ravpy-0.9.2/ravpy/distributed/op_functions/dl_ops.py
--rw-r--r--   0 apple      (501) staff       (20)    15960 2022-09-15 12:40:49.000000 ravpy-0.9.2/ravpy/distributed/op_functions/math_ops.py
--rw-r--r--   0 apple      (501) staff       (20)     3193 2022-09-15 12:40:49.000000 ravpy-0.9.2/ravpy/distributed/op_functions/ml_ops.py
--rw-r--r--   0 apple      (501) staff       (20)      502 2022-09-15 12:52:15.000000 ravpy-0.9.2/ravpy/distributed/participate.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy/federated/
--rw-r--r--   0 apple      (501) staff       (20)       29 2022-02-10 16:57:56.000000 ravpy-0.9.2/ravpy/federated/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4107 2022-07-14 10:02:21.000000 ravpy-0.9.2/ravpy/federated/compute.py
--rw-r--r--   0 apple      (501) staff       (20)     1405 2022-07-14 10:02:21.000000 ravpy-0.9.2/ravpy/federated/participate.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy/ftp/
--rw-r--r--   0 apple      (501) staff       (20)     1543 2022-09-15 12:44:03.000000 ravpy-0.9.2/ravpy/ftp/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4477 2022-09-15 12:42:56.000000 ravpy-0.9.2/ravpy/globals.py
--rw-r--r--   0 apple      (501) staff       (20)      717 2022-09-15 12:42:45.000000 ravpy-0.9.2/ravpy/initialize.py
--rw-r--r--   0 apple      (501) staff       (20)      815 2022-07-20 07:57:06.000000 ravpy-0.9.2/ravpy/logger.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy/ml/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-02-08 08:01:52.000000 ravpy-0.9.2/ravpy/ml/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2211 2021-09-21 11:23:05.000000 ravpy-0.9.2/ravpy/ml/train_model.py
--rw-r--r--   0 apple      (501) staff       (20)      433 2022-07-14 10:02:21.000000 ravpy-0.9.2/ravpy/singleton_utils.py
--rw-r--r--   0 apple      (501) staff       (20)    10506 2022-09-15 12:40:49.000000 ravpy-0.9.2/ravpy/strings.py
--rw-r--r--   0 apple      (501) staff       (20)     7686 2022-09-15 12:43:46.000000 ravpy-0.9.2/ravpy/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     2959 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      805 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)      207 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        6 2022-09-15 13:45:34.000000 ravpy-0.9.2/ravpy.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)      107 2022-09-15 13:45:34.000000 ravpy-0.9.2/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      922 2022-09-15 13:44:46.000000 ravpy-0.9.2/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/
+-rw-r--r--   0 apple      (501) staff       (20)     1070 2022-07-14 10:02:21.000000 ravpy-0.9.3/LICENSE.rst
+-rw-r--r--   0 apple      (501) staff       (20)     2959 2022-09-15 13:55:14.000000 ravpy-0.9.3/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     2628 2022-09-15 12:40:49.000000 ravpy-0.9.3/README.md
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2022-07-14 09:52:08.000000 ravpy-0.9.3/ravpy/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1085 2022-09-09 12:15:26.000000 ravpy-0.9.3/ravpy/config.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy/distributed/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2022-02-08 07:57:51.000000 ravpy-0.9.3/ravpy/distributed/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1498 2022-09-15 12:45:55.000000 ravpy-0.9.3/ravpy/distributed/benchmarking.py
+-rw-r--r--   0 apple      (501) staff       (20)    16328 2022-09-15 13:42:27.000000 ravpy-0.9.3/ravpy/distributed/compute.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy/distributed/deep_learning/
+-rw-r--r--   0 apple      (501) staff       (20)      135 2022-09-15 13:54:27.000000 ravpy-0.9.3/ravpy/distributed/deep_learning/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1889 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/deep_learning/activation_functions.py
+-rw-r--r--   0 apple      (501) staff       (20)     2281 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/deep_learning/layers.py
+-rw-r--r--   0 apple      (501) staff       (20)      706 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/deep_learning/loss_functions.py
+-rw-r--r--   0 apple      (501) staff       (20)     1918 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/deep_learning/optimizers.py
+-rw-r--r--   0 apple      (501) staff       (20)     3526 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/deep_learning/utils.py
+-rw-r--r--   0 apple      (501) staff       (20)     4393 2022-09-15 12:51:52.000000 ravpy-0.9.3/ravpy/distributed/evaluate.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy/distributed/op_functions/
+-rw-r--r--   0 apple      (501) staff       (20)       67 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/op_functions/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    21540 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/op_functions/dl_ops.py
+-rw-r--r--   0 apple      (501) staff       (20)    15960 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/op_functions/math_ops.py
+-rw-r--r--   0 apple      (501) staff       (20)     3193 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/distributed/op_functions/ml_ops.py
+-rw-r--r--   0 apple      (501) staff       (20)      502 2022-09-15 12:52:15.000000 ravpy-0.9.3/ravpy/distributed/participate.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy/federated/
+-rw-r--r--   0 apple      (501) staff       (20)       29 2022-02-10 16:57:56.000000 ravpy-0.9.3/ravpy/federated/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4107 2022-07-14 10:02:21.000000 ravpy-0.9.3/ravpy/federated/compute.py
+-rw-r--r--   0 apple      (501) staff       (20)     1405 2022-07-14 10:02:21.000000 ravpy-0.9.3/ravpy/federated/participate.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy/ftp/
+-rw-r--r--   0 apple      (501) staff       (20)     1543 2022-09-15 12:44:03.000000 ravpy-0.9.3/ravpy/ftp/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4477 2022-09-15 12:42:56.000000 ravpy-0.9.3/ravpy/globals.py
+-rw-r--r--   0 apple      (501) staff       (20)      717 2022-09-15 12:42:45.000000 ravpy-0.9.3/ravpy/initialize.py
+-rw-r--r--   0 apple      (501) staff       (20)      815 2022-07-20 07:57:06.000000 ravpy-0.9.3/ravpy/logger.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy/ml/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2022-02-08 08:01:52.000000 ravpy-0.9.3/ravpy/ml/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2211 2021-09-21 11:23:05.000000 ravpy-0.9.3/ravpy/ml/train_model.py
+-rw-r--r--   0 apple      (501) staff       (20)      433 2022-07-14 10:02:21.000000 ravpy-0.9.3/ravpy/singleton_utils.py
+-rw-r--r--   0 apple      (501) staff       (20)    10506 2022-09-15 12:40:49.000000 ravpy-0.9.3/ravpy/strings.py
+-rw-r--r--   0 apple      (501) staff       (20)     7686 2022-09-15 12:43:46.000000 ravpy-0.9.3/ravpy/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     2959 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     1084 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)      207 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        6 2022-09-15 13:55:14.000000 ravpy-0.9.3/ravpy.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)      107 2022-09-15 13:55:14.000000 ravpy-0.9.3/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      922 2022-09-15 13:55:04.000000 ravpy-0.9.3/setup.py
```

### Comparing `ravpy-0.9.2/LICENSE.rst` & `ravpy-0.9.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/PKG-INFO` & `ravpy-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ravpy
-Version: 0.9.2
+Version: 0.9.3
 Summary: UNKNOWN
 Home-page: https://github.com/ravenprotocol/ravpy
 Author: Raven Protocol
 Author-email: kailash@ravenprotocol.com
 License: MIT
 Keywords: Ravpy,python client library for providers
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ravpy Version: 0.9.2 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: ravpy Version: 0.9.3 Summary: UNKNOWN Home-page:
 https://github.com/ravenprotocol/ravpy Author: Raven Protocol Author-email:
 kailash@ravenprotocol.com License: MIT Keywords: Ravpy,python client library
 for providers Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE.rst # Ravpy - The Provider's Library Introducing Raven
 Protocol's Python SDK for Providers that allows compute nodes across the world
 to participate in the Ravenverse. ## Working In the Ravenverse, Providers are
 those who are willing to contribute their local system's idle compute power to
```

### Comparing `ravpy-0.9.2/README.md` & `ravpy-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/config.py` & `ravpy-0.9.3/ravpy/config.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/distributed/benchmarking.py` & `ravpy-0.9.3/ravpy/distributed/benchmarking.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/distributed/compute.py` & `ravpy-0.9.3/ravpy/distributed/compute.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/distributed/evaluate.py` & `ravpy-0.9.3/ravpy/distributed/evaluate.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/distributed/op_functions/dl_ops.py` & `ravpy-0.9.3/ravpy/distributed/op_functions/dl_ops.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/distributed/op_functions/math_ops.py` & `ravpy-0.9.3/ravpy/distributed/op_functions/math_ops.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/distributed/op_functions/ml_ops.py` & `ravpy-0.9.3/ravpy/distributed/op_functions/ml_ops.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/federated/compute.py` & `ravpy-0.9.3/ravpy/federated/compute.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/federated/participate.py` & `ravpy-0.9.3/ravpy/federated/participate.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/ftp/__init__.py` & `ravpy-0.9.3/ravpy/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/globals.py` & `ravpy-0.9.3/ravpy/globals.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/initialize.py` & `ravpy-0.9.3/ravpy/initialize.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/logger.py` & `ravpy-0.9.3/ravpy/logger.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/ml/train_model.py` & `ravpy-0.9.3/ravpy/ml/train_model.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/strings.py` & `ravpy-0.9.3/ravpy/strings.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy/utils.py` & `ravpy-0.9.3/ravpy/utils.py`

 * *Files identical despite different names*

### Comparing `ravpy-0.9.2/ravpy.egg-info/PKG-INFO` & `ravpy-0.9.3/ravpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ravpy
-Version: 0.9.2
+Version: 0.9.3
 Summary: UNKNOWN
 Home-page: https://github.com/ravenprotocol/ravpy
 Author: Raven Protocol
 Author-email: kailash@ravenprotocol.com
 License: MIT
 Keywords: Ravpy,python client library for providers
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ravpy Version: 0.9.2 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: ravpy Version: 0.9.3 Summary: UNKNOWN Home-page:
 https://github.com/ravenprotocol/ravpy Author: Raven Protocol Author-email:
 kailash@ravenprotocol.com License: MIT Keywords: Ravpy,python client library
 for providers Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE.rst # Ravpy - The Provider's Library Introducing Raven
 Protocol's Python SDK for Providers that allows compute nodes across the world
 to participate in the Ravenverse. ## Working In the Ravenverse, Providers are
 those who are willing to contribute their local system's idle compute power to
```

### Comparing `ravpy-0.9.2/ravpy.egg-info/SOURCES.txt` & `ravpy-0.9.3/ravpy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 ravpy.egg-info/requires.txt
 ravpy.egg-info/top_level.txt
 ravpy/distributed/__init__.py
 ravpy/distributed/benchmarking.py
 ravpy/distributed/compute.py
 ravpy/distributed/evaluate.py
 ravpy/distributed/participate.py
+ravpy/distributed/deep_learning/__init__.py
+ravpy/distributed/deep_learning/activation_functions.py
+ravpy/distributed/deep_learning/layers.py
+ravpy/distributed/deep_learning/loss_functions.py
+ravpy/distributed/deep_learning/optimizers.py
+ravpy/distributed/deep_learning/utils.py
 ravpy/distributed/op_functions/__init__.py
 ravpy/distributed/op_functions/dl_ops.py
 ravpy/distributed/op_functions/math_ops.py
 ravpy/distributed/op_functions/ml_ops.py
 ravpy/federated/__init__.py
 ravpy/federated/compute.py
 ravpy/federated/participate.py
```

### Comparing `ravpy-0.9.2/setup.py` & `ravpy-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ravpy",
-    version="0.9.2",
+    version="0.9.3",
     license='MIT',
     author="Raven Protocol",
     author_email='kailash@ravenprotocol.com',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ravenprotocol/ravpy',
```

