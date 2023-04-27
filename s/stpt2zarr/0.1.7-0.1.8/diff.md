# Comparing `tmp/stpt2zarr-0.1.7.tar.gz` & `tmp/stpt2zarr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stpt2zarr-0.1.7.tar", last modified: Mon Oct 24 09:29:00 2022, max compression
+gzip compressed data, was "stpt2zarr-0.1.8.tar", last modified: Thu Apr 27 08:55:09 2023, max compression
```

## Comparing `stpt2zarr-0.1.7.tar` & `stpt2zarr-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 09:29:00.502388 stpt2zarr-0.1.7/
--rw-r--r--   0 root         (0) root         (0)     1111 2022-10-24 09:29:00.502388 stpt2zarr-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      547 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1388 2022-10-24 09:29:00.502388 stpt2zarr-0.1.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 09:29:00.501388 stpt2zarr-0.1.7/stpt2zarr/
--rw-rw-rw-   0 root         (0) root         (0)     7009 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/stpt2zarr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 09:29:00.501388 stpt2zarr-0.1.7/stpt2zarr/stptlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/stpt2zarr/stptlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/stpt2zarr/stptlib/mosaicdict.py
--rw-rw-rw-   0 root         (0) root         (0)     4441 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/stpt2zarr/stptlib/stptraw.py
--rw-rw-rw-   0 root         (0) root         (0)     5501 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/stpt2zarr/stptlib/stptsectionraw.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-10-24 09:28:49.000000 stpt2zarr-0.1.7/stpt2zarr/stptlib/stpttileraw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 09:29:00.501388 stpt2zarr-0.1.7/stpt2zarr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1111 2022-10-24 09:29:00.000000 stpt2zarr-0.1.7/stpt2zarr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2022-10-24 09:29:00.000000 stpt2zarr-0.1.7/stpt2zarr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-24 09:29:00.000000 stpt2zarr-0.1.7/stpt2zarr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-10-24 09:29:00.000000 stpt2zarr-0.1.7/stpt2zarr.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2022-10-24 09:29:00.000000 stpt2zarr-0.1.7/stpt2zarr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-10-24 09:29:00.000000 stpt2zarr-0.1.7/stpt2zarr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:09.971084 stpt2zarr-0.1.8/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-04-27 08:55:09.971084 stpt2zarr-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2023-04-27 08:55:09.972084 stpt2zarr-0.1.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:09.970084 stpt2zarr-0.1.8/stpt2zarr/
+-rw-rw-rw-   0 root         (0) root         (0)     6997 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/stpt2zarr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:09.971084 stpt2zarr-0.1.8/stpt2zarr/stptlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/stpt2zarr/stptlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/stpt2zarr/stptlib/mosaicdict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/stpt2zarr/stptlib/stptraw.py
+-rw-rw-rw-   0 root         (0) root         (0)     5501 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/stpt2zarr/stptlib/stptsectionraw.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-04-27 08:54:55.000000 stpt2zarr-0.1.8/stpt2zarr/stptlib/stpttileraw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:55:09.971084 stpt2zarr-0.1.8/stpt2zarr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-04-27 08:55:09.000000 stpt2zarr-0.1.8/stpt2zarr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-27 08:55:09.000000 stpt2zarr-0.1.8/stpt2zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 08:55:09.000000 stpt2zarr-0.1.8/stpt2zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-27 08:55:09.000000 stpt2zarr-0.1.8/stpt2zarr.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-27 08:55:09.000000 stpt2zarr-0.1.8/stpt2zarr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-27 08:55:09.000000 stpt2zarr-0.1.8/stpt2zarr.egg-info/top_level.txt
```

### Comparing `stpt2zarr-0.1.7/PKG-INFO` & `stpt2zarr-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpt2zarr
-Version: 0.1.7
+Version: 0.1.8
 Summary: STPT scan to Zarr conversion
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/stpt2zarr
 Author: Mo Alsad and Eduardo Gonzalez Solares
 Author-email: "msa51@cam.ac.uk
 Project-URL: Bug Tracker, https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/stpt2zarr/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stpt2zarr-0.1.7/README.md` & `stpt2zarr-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `stpt2zarr-0.1.7/setup.cfg` & `stpt2zarr-0.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.7
+current_version = 0.1.8
 commit = True
 tag = True
 
 [metadata]
 name = stpt2zarr
 version = attr: stpt2zarr.__version__
 author = Mo Alsad and Eduardo Gonzalez Solares
```

### Comparing `stpt2zarr-0.1.7/stpt2zarr/__init__.py` & `stpt2zarr-0.1.8/stpt2zarr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 from imaxt_image.io import TiffImage
 import click
 import logging
 
 from .stptlib.stptraw import StptRaw
 
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 __author__ = "Mo Alsad and Eduardo Gonzalez Solares"
 __email__ = "msa51@cam.ac.uk"
 _credits__ = ["Mo Alsad", "Eduardo Gonzalez Solares"]
 
 
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger()
 
-if "owl.daemon.pipeline" in logger.manager.loggerDict:
-    logger = logging.getLogger("owl.daemon.pipeline")
+if "owl2.pipeline" in logger.manager.loggerDict:
+    logger = logging.getLogger("owl2.pipeline")
 
 
 def _write_dataset(s, *, output, dtype):
     """Write array for each section
     """
     logger.info('Preprocessing section {}'.format(s.num))
     s_name = 'S{}'.format(str(s.num).zfill(3))
```

### Comparing `stpt2zarr-0.1.7/stpt2zarr/stptlib/mosaicdict.py` & `stpt2zarr-0.1.8/stpt2zarr/stptlib/mosaicdict.py`

 * *Files identical despite different names*

### Comparing `stpt2zarr-0.1.7/stpt2zarr/stptlib/stptraw.py` & `stpt2zarr-0.1.8/stpt2zarr/stptlib/stptraw.py`

 * *Files identical despite different names*

### Comparing `stpt2zarr-0.1.7/stpt2zarr/stptlib/stptsectionraw.py` & `stpt2zarr-0.1.8/stpt2zarr/stptlib/stptsectionraw.py`

 * *Files identical despite different names*

### Comparing `stpt2zarr-0.1.7/stpt2zarr.egg-info/PKG-INFO` & `stpt2zarr-0.1.8/stpt2zarr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpt2zarr
-Version: 0.1.7
+Version: 0.1.8
 Summary: STPT scan to Zarr conversion
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/stpt2zarr
 Author: Mo Alsad and Eduardo Gonzalez Solares
 Author-email: "msa51@cam.ac.uk
 Project-URL: Bug Tracker, https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/stpt2zarr/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

