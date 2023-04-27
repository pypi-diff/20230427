# Comparing `tmp/cellshape-cluster-0.0.9.tar.gz` & `tmp/cellshape-cluster-0.0.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellshape-cluster-0.0.9.tar", last modified: Wed Jun 29 13:18:21 2022, max compression
+gzip compressed data, was "cellshape-cluster-0.0.9rc0.tar", last modified: Wed Jun 29 13:08:02 2022, max compression
```

## Comparing `cellshape-cluster-0.0.9.tar` & `cellshape-cluster-0.0.9rc0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:21.081838 cellshape-cluster-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5924 2022-06-29 13:18:21.081838 cellshape-cluster-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:21.077838 cellshape-cluster-0.0.9/cellshape_cluster/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/clustering_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/deep_embedded_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:21.077838 cellshape-cluster-0.0.9/cellshape_cluster/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/helpers/check_tolerance.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/helpers/distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/helpers/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/helpers/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     6111 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/cellshape_cluster/training_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:21.077838 cellshape-cluster-0.0.9/cellshape_cluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5924 2022-06-29 13:18:20.000000 cellshape-cluster-0.0.9/cellshape_cluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-06-29 13:18:21.000000 cellshape-cluster-0.0.9/cellshape_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 13:18:20.000000 cellshape-cluster-0.0.9/cellshape_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 13:18:18.000000 cellshape-cluster-0.0.9/cellshape_cluster.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-06-29 13:18:20.000000 cellshape-cluster-0.0.9/cellshape_cluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-29 13:18:20.000000 cellshape-cluster-0.0.9/cellshape_cluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-06-29 13:18:21.081838 cellshape-cluster-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:21.077838 cellshape-cluster-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:21.077838 cellshape-cluster-0.0.9/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/tests/test_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:21.077838 cellshape-cluster-0.0.9/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/tests/test_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-29 13:18:01.000000 cellshape-cluster-0.0.9/tests/test_unit/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:08:02.972776 cellshape-cluster-0.0.9rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-06-29 13:08:02.972776 cellshape-cluster-0.0.9rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:08:02.968776 cellshape-cluster-0.0.9rc0/cellshape_cluster/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/clustering_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/deep_embedded_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:08:02.968776 cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/check_tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (121)      913 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6111 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5652 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster/training_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:08:02.968776 cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-06-29 13:08:02.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-06-29 13:08:02.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 13:08:02.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 13:08:00.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-06-29 13:08:02.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-29 13:08:02.000000 cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-06-29 13:08:02.972776 cellshape-cluster-0.0.9rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:08:02.972776 cellshape-cluster-0.0.9rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:08:02.972776 cellshape-cluster-0.0.9rc0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/tests/test_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:08:02.972776 cellshape-cluster-0.0.9rc0/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-29 13:07:43.000000 cellshape-cluster-0.0.9rc0/tests/test_unit/test_placeholder.py
```

### Comparing `cellshape-cluster-0.0.9/PKG-INFO` & `cellshape-cluster-0.0.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape-cluster
-Version: 0.0.9
+Version: 0.0.9rc0
 Summary: 3D shape analysis using deep learning
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape-cluster
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape-cluster/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-cluster-0.0.9/README.md` & `cellshape-cluster-0.0.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster/clustering_layer.py` & `cellshape-cluster-0.0.9rc0/cellshape_cluster/clustering_layer.py`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster/deep_embedded_clustering.py` & `cellshape-cluster-0.0.9rc0/cellshape_cluster/deep_embedded_clustering.py`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster/helpers/distributions.py` & `cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/distributions.py`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster/helpers/kmeans.py` & `cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/kmeans.py`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster/helpers/reports.py` & `cellshape-cluster-0.0.9rc0/cellshape_cluster/helpers/reports.py`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster/main.py` & `cellshape-cluster-0.0.9rc0/cellshape_cluster/main.py`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster/training_functions.py` & `cellshape-cluster-0.0.9rc0/cellshape_cluster/training_functions.py`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster.egg-info/PKG-INFO` & `cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape-cluster
-Version: 0.0.9
+Version: 0.0.9rc0
 Summary: 3D shape analysis using deep learning
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape-cluster
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape-cluster/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-cluster-0.0.9/cellshape_cluster.egg-info/SOURCES.txt` & `cellshape-cluster-0.0.9rc0/cellshape_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellshape-cluster-0.0.9/setup.cfg` & `cellshape-cluster-0.0.9rc0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.9
+current_version = 0.0.9-rc0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<rc>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{rc}
 	{major}.{minor}.{patch}
```

### Comparing `cellshape-cluster-0.0.9/setup.py` & `cellshape-cluster-0.0.9rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "tqdm",
     "scikit-learn",
 ]
 
 
 setup(
     name="cellshape-cluster",
-    version="0.0.9",
+    version="0.0.9-rc0",
     description="3D shape analysis using deep learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     extras_require={
         "dev": [
             "black",
```

