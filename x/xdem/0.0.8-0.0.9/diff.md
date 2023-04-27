# Comparing `tmp/xdem-0.0.8.tar.gz` & `tmp/xdem-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdem-0.0.8.tar", last modified: Mon Apr 24 23:51:30 2023, max compression
+gzip compressed data, was "xdem-0.0.9.tar", last modified: Thu Apr 27 01:01:12 2023, max compression
```

## Comparing `xdem-0.0.8.tar` & `xdem-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.849684 xdem-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-24 23:51:10.000000 xdem-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 23:51:30.849684 xdem-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-24 23:51:10.000000 xdem-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 23:51:10.000000 xdem-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:51:30.849684 xdem-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-24 23:51:10.000000 xdem-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.845684 xdem-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_coreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_ddem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_demcollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    55340 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_spatialstats.py
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-04-24 23:51:10.000000 xdem-0.0.8/tests/test_volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.849684 xdem-0.0.8/xdem/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)   101810 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/coreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/ddem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/dem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/demcollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)   152648 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/spatialstats.py
--rw-r--r--   0 runner    (1001) docker     (123)    67439 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    33365 2023-04-24 23:51:10.000000 xdem-0.0.8/xdem/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:51:30.849684 xdem-0.0.8/xdem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 23:51:30.000000 xdem-0.0.8/xdem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:12.162807 xdem-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-27 01:00:53.000000 xdem-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-27 01:01:12.162807 xdem-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-27 01:00:53.000000 xdem-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 01:00:53.000000 xdem-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 01:01:12.162807 xdem-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-27 01:00:53.000000 xdem-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:12.158807 xdem-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_coreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_ddem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_demcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55340 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_spatialstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-04-27 01:00:53.000000 xdem-0.0.9/tests/test_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:12.162807 xdem-0.0.9/xdem/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101810 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/coreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/ddem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/demcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152648 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/spatialstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67439 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 01:01:11.000000 xdem-0.0.9/xdem/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33365 2023-04-27 01:00:53.000000 xdem-0.0.9/xdem/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:12.162807 xdem-0.0.9/xdem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-27 01:01:12.000000 xdem-0.0.9/xdem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 01:01:12.000000 xdem-0.0.9/xdem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:01:12.000000 xdem-0.0.9/xdem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:01:11.000000 xdem-0.0.9/xdem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-27 01:01:12.000000 xdem-0.0.9/xdem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 01:01:12.000000 xdem-0.0.9/xdem.egg-info/top_level.txt
```

### Comparing `xdem-0.0.8/LICENSE` & `xdem-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/PKG-INFO` & `xdem-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdem
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of tools to manipulate Digital Elevation Models (DEMs) 
 Home-page: https://github.com/GlacioHack/xdem
 Author: The GlacioHack Team
 Author-email: this-is-not-an-email@a.com
 License: BSD-3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `xdem-0.0.8/README.md` & `xdem-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/setup.py` & `xdem-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import os
 
 from setuptools import setup
 
-FULLVERSION = "0.0.8"
+FULLVERSION = "0.0.9"
 VERSION = FULLVERSION
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as infile:
     LONG_DESCRIPTION = infile.read()
 
 setup(
     name="xdem",
```

### Comparing `xdem-0.0.8/tests/test_coreg.py` & `xdem-0.0.9/tests/test_coreg.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_ddem.py` & `xdem-0.0.9/tests/test_ddem.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_dem.py` & `xdem-0.0.9/tests/test_dem.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_demcollection.py` & `xdem-0.0.9/tests/test_demcollection.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_doc.py` & `xdem-0.0.9/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_examples.py` & `xdem-0.0.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_filters.py` & `xdem-0.0.9/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_fit.py` & `xdem-0.0.9/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_misc.py` & `xdem-0.0.9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_spatialstats.py` & `xdem-0.0.9/tests/test_spatialstats.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_terrain.py` & `xdem-0.0.9/tests/test_terrain.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/tests/test_volume.py` & `xdem-0.0.9/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/__init__.py` & `xdem-0.0.9/xdem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 from xdem.dem import DEM  # noqa
 from xdem.demcollection import DEMCollection  # noqa
 
 try:
     from xdem.version import version as __version__  # noqa
 except ImportError:  # pragma: no cover
     raise ImportError(
-        "geoutils is not properly installed. If you are "
+        "xDEM is not properly installed. If you are "
         "running from the source directory, please instead "
         "create a new virtual environment (using conda or "
         "virtualenv) and then install it in-place by running: "
         "pip install -e ."
     )
```

### Comparing `xdem-0.0.8/xdem/coreg.py` & `xdem-0.0.9/xdem/coreg.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/ddem.py` & `xdem-0.0.9/xdem/ddem.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/dem.py` & `xdem-0.0.9/xdem/dem.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/demcollection.py` & `xdem-0.0.9/xdem/demcollection.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/examples.py` & `xdem-0.0.9/xdem/examples.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/filters.py` & `xdem-0.0.9/xdem/filters.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/fit.py` & `xdem-0.0.9/xdem/fit.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/misc.py` & `xdem-0.0.9/xdem/misc.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/spatialstats.py` & `xdem-0.0.9/xdem/spatialstats.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/terrain.py` & `xdem-0.0.9/xdem/terrain.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem/volume.py` & `xdem-0.0.9/xdem/volume.py`

 * *Files identical despite different names*

### Comparing `xdem-0.0.8/xdem.egg-info/PKG-INFO` & `xdem-0.0.9/xdem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdem
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of tools to manipulate Digital Elevation Models (DEMs) 
 Home-page: https://github.com/GlacioHack/xdem
 Author: The GlacioHack Team
 Author-email: this-is-not-an-email@a.com
 License: BSD-3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `xdem-0.0.8/xdem.egg-info/SOURCES.txt` & `xdem-0.0.9/xdem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

