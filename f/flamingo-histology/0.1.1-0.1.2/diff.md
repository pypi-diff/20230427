# Comparing `tmp/flamingo_histology-0.1.1.tar.gz` & `tmp/flamingo_histology-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamingo_histology-0.1.1.tar", last modified: Mon Jul  4 16:03:17 2022, max compression
+gzip compressed data, was "flamingo_histology-0.1.2.tar", last modified: Thu Apr 27 14:02:33 2023, max compression
```

## Comparing `flamingo_histology-0.1.1.tar` & `flamingo_histology-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 16:03:17.563399 flamingo_histology-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-07-04 16:03:05.000000 flamingo_histology-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-07-04 16:03:17.563399 flamingo_histology-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-07-04 16:03:05.000000 flamingo_histology-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-07-04 16:03:05.000000 flamingo_histology-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-04 16:03:17.563399 flamingo_histology-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 16:03:17.563399 flamingo_histology-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 16:03:17.563399 flamingo_histology-0.1.1/src/flamingo/
--rw-r--r--   0 runner    (1001) docker     (121)    13850 2022-07-04 16:03:05.000000 flamingo_histology-0.1.1/src/flamingo/Flamingo.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-04 16:03:05.000000 flamingo_histology-0.1.1/src/flamingo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 16:03:17.563399 flamingo_histology-0.1.1/src/flamingo_histology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-07-04 16:03:17.000000 flamingo_histology-0.1.1/src/flamingo_histology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-07-04 16:03:17.000000 flamingo_histology-0.1.1/src/flamingo_histology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-04 16:03:17.000000 flamingo_histology-0.1.1/src/flamingo_histology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-04 16:03:17.000000 flamingo_histology-0.1.1/src/flamingo_histology.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:02:33.720433 flamingo_histology-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 14:02:22.000000 flamingo_histology-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-27 14:02:33.720433 flamingo_histology-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-27 14:02:22.000000 flamingo_histology-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-27 14:02:23.000000 flamingo_histology-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:02:33.720433 flamingo_histology-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:02:33.716433 flamingo_histology-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:02:33.720433 flamingo_histology-0.1.2/src/flamingo/
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-04-27 14:02:23.000000 flamingo_histology-0.1.2/src/flamingo/Flamingo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:02:23.000000 flamingo_histology-0.1.2/src/flamingo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:02:33.720433 flamingo_histology-0.1.2/src/flamingo_histology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-27 14:02:33.000000 flamingo_histology-0.1.2/src/flamingo_histology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 14:02:33.000000 flamingo_histology-0.1.2/src/flamingo_histology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:02:33.000000 flamingo_histology-0.1.2/src/flamingo_histology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 14:02:33.000000 flamingo_histology-0.1.2/src/flamingo_histology.egg-info/top_level.txt
```

### Comparing `flamingo_histology-0.1.1/LICENSE.md` & `flamingo_histology-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flamingo_histology-0.1.1/PKG-INFO` & `flamingo_histology-0.1.2/src/flamingo_histology.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: flamingo_histology
-Version: 0.1.1
+Name: flamingo-histology
+Version: 0.1.2
 Summary: Flamingo: a package for extracting and exporting annotations from H&E images
 Author-email: J S McKenzie <jsmckenzi@users.noreply.github.com>
-Project-URL: Homepage, https://jsmckenzie.github.io/flamingo/
-Project-URL: Bug Tracker, https://jsmckenzie.github.io/flamingo/
+Project-URL: Homepage, https://jsmckenzie.github.io/flamingo/index.html/
+Project-URL: Bug Tracker, https://jsmckenzie.github.io/flamingo/index.html
+Project-URL: Documentation, https://jsmckenzie.github.io/flamingo/index.html
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# flamingo
-<img src="https://github.com/jsmckenzie/flamingo/blob/main/docs/image.jpg" alt="From Wikipedia" height="150" align="right" caption="Text left hanging">
+# flamingo 🦩
+<img src="https://github.com/jsmckenzie/flamingo/blob/main/docs/image.jpg" alt="Flamingo" height="150" align="right" caption="Text left hanging">
 
 #### Extract annotations from .ndpa files and map on to the .ndpi image for use in other applications
 
 * * *
 
 [![PyPI version](https://badge.fury.io/py/flamingo-histology.svg)](https://pypi.org/project/flamingo-histology/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flamingo_histology-0.1.1/README.md` & `flamingo_histology-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# flamingo
-<img src="https://github.com/jsmckenzie/flamingo/blob/main/docs/image.jpg" alt="From Wikipedia" height="150" align="right" caption="Text left hanging">
+# flamingo 🦩
+<img src="https://github.com/jsmckenzie/flamingo/blob/main/docs/image.jpg" alt="Flamingo" height="150" align="right" caption="Text left hanging">
 
 #### Extract annotations from .ndpa files and map on to the .ndpi image for use in other applications
 
 * * *
 
 [![PyPI version](https://badge.fury.io/py/flamingo-histology.svg)](https://pypi.org/project/flamingo-histology/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flamingo_histology-0.1.1/pyproject.toml` & `flamingo_histology-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flamingo_histology"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="J S McKenzie", email="jsmckenzi@users.noreply.github.com"},
 ]
 description = "Flamingo: a package for extracting and exporting annotations from H&E images"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
@@ -17,9 +17,10 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Image Processing"
 ]
 
 [project.urls]
-"Homepage" = "https://jsmckenzie.github.io/flamingo/"
-"Bug Tracker" = "https://jsmckenzie.github.io/flamingo/"
+"Homepage" = "https://jsmckenzie.github.io/flamingo/index.html/"
+"Bug Tracker" = "https://jsmckenzie.github.io/flamingo/index.html"
+"Documentation" = "https://jsmckenzie.github.io/flamingo/index.html"
```

### Comparing `flamingo_histology-0.1.1/src/flamingo/Flamingo.py` & `flamingo_histology-0.1.2/src/flamingo/Flamingo.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,18 +273,18 @@
         
         
     def annotationPlot(self,type='scatter'):
         '''
         Plot image and/or annotations.
         
         Parameters:
-            type (string):  'scatter': raw annotations as a scatter plot
-                            'image':   low resolution image only 
-                            'combined' overlay scatter annotations on low res image
-                            'anno'     low res image and annotation image
+            type (string):  'scatter' : raw annotations as a scatter plot
+                            'image'   : low resolution image only 
+                            'combined': overlay scatter annotations on low res image
+                            'anno'    :  low res image and annotation image
         '''
         
         if type == 'anno':
             subPlots = 2
         else:
             subPlots = 1
         
@@ -329,15 +329,15 @@
         '''
         Save annotations/low res image to file.
         
         Parameters:
             type (string): 'json':  coordinates scaled to low res image
                            'mask':  image of coordinates
                            'image': low resolution image
-                           'all':   export both
+                           'all':   export all of the above
                             
             path (string): valid directory in which to save the results. File name is fixed.
                            If left empty then .ndpi path is used.
         '''
         
         # Where to save?
         if path is None:
```

### Comparing `flamingo_histology-0.1.1/src/flamingo_histology.egg-info/PKG-INFO` & `flamingo_histology-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: flamingo-histology
-Version: 0.1.1
+Name: flamingo_histology
+Version: 0.1.2
 Summary: Flamingo: a package for extracting and exporting annotations from H&E images
 Author-email: J S McKenzie <jsmckenzi@users.noreply.github.com>
-Project-URL: Homepage, https://jsmckenzie.github.io/flamingo/
-Project-URL: Bug Tracker, https://jsmckenzie.github.io/flamingo/
+Project-URL: Homepage, https://jsmckenzie.github.io/flamingo/index.html/
+Project-URL: Bug Tracker, https://jsmckenzie.github.io/flamingo/index.html
+Project-URL: Documentation, https://jsmckenzie.github.io/flamingo/index.html
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# flamingo
-<img src="https://github.com/jsmckenzie/flamingo/blob/main/docs/image.jpg" alt="From Wikipedia" height="150" align="right" caption="Text left hanging">
+# flamingo 🦩
+<img src="https://github.com/jsmckenzie/flamingo/blob/main/docs/image.jpg" alt="Flamingo" height="150" align="right" caption="Text left hanging">
 
 #### Extract annotations from .ndpa files and map on to the .ndpi image for use in other applications
 
 * * *
 
 [![PyPI version](https://badge.fury.io/py/flamingo-histology.svg)](https://pypi.org/project/flamingo-histology/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

