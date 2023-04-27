# Comparing `tmp/cellshape-0.0.9.tar.gz` & `tmp/cellshape-0.0.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellshape-0.0.9.tar", last modified: Wed Jun 29 13:04:47 2022, max compression
+gzip compressed data, was "cellshape-0.0.9rc0.tar", last modified: Tue Jun 28 14:44:39 2022, max compression
```

## Comparing `cellshape-0.0.9.tar` & `cellshape-0.0.9rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:04:47.218381 cellshape-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-29 13:04:29.000000 cellshape-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6911 2022-06-29 13:04:47.218381 cellshape-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-06-29 13:04:29.000000 cellshape-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:04:47.218381 cellshape-0.0.9/cellshape/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-29 13:04:29.000000 cellshape-0.0.9/cellshape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-06-29 13:04:29.000000 cellshape-0.0.9/cellshape/cellshape_train.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-29 13:04:29.000000 cellshape-0.0.9/cellshape/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    18325 2022-06-29 13:04:29.000000 cellshape-0.0.9/cellshape/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 13:04:47.218381 cellshape-0.0.9/cellshape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6911 2022-06-29 13:04:46.000000 cellshape-0.0.9/cellshape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-06-29 13:04:47.000000 cellshape-0.0.9/cellshape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 13:04:46.000000 cellshape-0.0.9/cellshape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 13:04:44.000000 cellshape-0.0.9/cellshape.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-06-29 13:04:46.000000 cellshape-0.0.9/cellshape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-29 13:04:47.000000 cellshape-0.0.9/cellshape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-06-29 13:04:29.000000 cellshape-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-06-29 13:04:47.218381 cellshape-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-06-29 13:04:29.000000 cellshape-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 14:44:39.053691 cellshape-0.0.9rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6914 2022-06-28 14:44:39.053691 cellshape-0.0.9rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 14:44:39.049691 cellshape-0.0.9rc0/cellshape/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/cellshape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/cellshape/cellshape_train.py
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/cellshape/example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9104 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/cellshape/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 14:44:39.053691 cellshape-0.0.9rc0/cellshape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6914 2022-06-28 14:44:38.000000 cellshape-0.0.9rc0/cellshape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-06-28 14:44:39.000000 cellshape-0.0.9rc0/cellshape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 14:44:38.000000 cellshape-0.0.9rc0/cellshape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 14:44:36.000000 cellshape-0.0.9rc0/cellshape.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-06-28 14:44:38.000000 cellshape-0.0.9rc0/cellshape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-28 14:44:38.000000 cellshape-0.0.9rc0/cellshape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-06-28 14:44:39.053691 cellshape-0.0.9rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-06-28 14:44:20.000000 cellshape-0.0.9rc0/setup.py
```

### Comparing `cellshape-0.0.9/PKG-INFO` & `cellshape-0.0.9rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape
-Version: 0.0.9
+Version: 0.0.9rc0
 Summary: 3D shape analysis using deep learning
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-0.0.9/README.md` & `cellshape-0.0.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `cellshape-0.0.9/cellshape/cellshape_train.py` & `cellshape-0.0.9rc0/cellshape/cellshape_train.py`

 * *Files identical despite different names*

### Comparing `cellshape-0.0.9/cellshape.egg-info/PKG-INFO` & `cellshape-0.0.9rc0/cellshape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellshape
-Version: 0.0.9
+Version: 0.0.9rc0
 Summary: 3D shape analysis using deep learning
 Author: Matt De Vries, Lucas Dent, Adam Tyson
 Author-email: mattdevries.ai@gmail.com
 Project-URL: Source Code, https://github.com/Sentinal4D/cellshape
 Project-URL: Bug Tracker, https://github.com/Sentinal4D/cellshape/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cellshape-0.0.9/setup.cfg` & `cellshape-0.0.9rc0/setup.cfg`

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

### Comparing `cellshape-0.0.9/setup.py` & `cellshape-0.0.9rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "plotly",
     "napari[all]",
 ]
 
 
 setup(
     name="cellshape",
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

