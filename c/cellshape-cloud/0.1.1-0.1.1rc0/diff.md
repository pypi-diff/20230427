# Comparing `tmp/cellshape-cloud-0.1.1.tar.gz` & `tmp/cellshape-cloud-0.1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellshape-cloud-0.1.1.tar", last modified: Wed Apr 26 14:46:10 2023, max compression
+gzip compressed data, was "cellshape-cloud-0.1.1rc0.tar", last modified: Wed Apr 26 14:16:51 2023, max compression
```

## Comparing `cellshape-cloud-0.1.1.tar` & `cellshape-cloud-0.1.1rc0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/cellshape_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/cloud_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/extract_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/helper_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/lightning_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/lightning_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/pointcloud_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/simclr_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/train_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/training_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/cellshape_cloud/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/vendor/chamfer_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/vendor/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/vendor/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/cellshape_cloud/vendor/graph_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/cellshape_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-26 14:46:10.000000 cellshape-cloud-0.1.1/cellshape_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-26 14:46:10.000000 cellshape-cloud-0.1.1/cellshape_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:46:10.000000 cellshape-cloud-0.1.1/cellshape_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:46:10.000000 cellshape-cloud-0.1.1/cellshape_cloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-26 14:46:10.000000 cellshape-cloud-0.1.1/cellshape_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 14:46:10.000000 cellshape-cloud-0.1.1/cellshape_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-26 14:46:10.839009 cellshape-cloud-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/tests/test_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:46:10.835009 cellshape-cloud-0.1.1/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/tests/test_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 14:45:46.000000 cellshape-cloud-0.1.1/tests/test_unit/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.875791 cellshape-cloud-0.1.1rc0/cellshape_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/cloud_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/extract_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/helper_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/pointcloud_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/simclr_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/train_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/training_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/chamfer_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/graph_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 14:16:51.000000 cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/test_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:51.879791 cellshape-cloud-0.1.1rc0/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 14:16:34.000000 cellshape-cloud-0.1.1rc0/tests/test_unit/test_placeholder.py
```

### Comparing `cellshape-cloud-0.1.1/LICENSE` & `cellshape-cloud-0.1.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/PKG-INFO` & `cellshape-cloud-0.1.1rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape-cloud
-Version: 0.1.1
+Version: 0.1.1rc0
 Summary: 3D cell shape analysis using geometric deep learning on point clouds
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape-cloud
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape-cloud/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-cloud-0.1.1/README.md` & `cellshape-cloud-0.1.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/cloud_autoencoder.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/cloud_autoencoder.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/extract.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/extract.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/extract_features.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/extract_features.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/lightning_autoencoder.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_autoencoder.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/lightning_classifier.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/lightning_classifier.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/main.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/main.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/plotting.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/plotting.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/pointcloud_dataset.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/pointcloud_dataset.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/reports.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/reports.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/train_autoencoder.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/train_autoencoder.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/training_functions.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/training_functions.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/transformations.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/transformations.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/vendor/chamfer_distance.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/vendor/decoders.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/decoders.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/vendor/encoders.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/encoders.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud/vendor/graph_functions.py` & `cellshape-cloud-0.1.1rc0/cellshape_cloud/vendor/graph_functions.py`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud.egg-info/PKG-INFO` & `cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape-cloud
-Version: 0.1.1
+Version: 0.1.1rc0
 Summary: 3D cell shape analysis using geometric deep learning on point clouds
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape-cloud
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape-cloud/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-cloud-0.1.1/cellshape_cloud.egg-info/SOURCES.txt` & `cellshape-cloud-0.1.1rc0/cellshape_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellshape-cloud-0.1.1/setup.cfg` & `cellshape-cloud-0.1.1rc0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.1-rc0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<rc>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{rc}
 	{major}.{minor}.{patch}
```

### Comparing `cellshape-cloud-0.1.1/setup.py` & `cellshape-cloud-0.1.1rc0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "scikit-learn",
     "tensorboard",
     "h5py",
 ]
 
 setup(
     name="cellshape-cloud",
-    version="0.1.1",
+    version="0.1.1-rc0",
     description="3D cell shape analysis using geometric deep"
     " learning on point clouds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     extras_require={
         "dev": [
```

