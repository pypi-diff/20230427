# Comparing `tmp/pyogrio-0.5.1.tar.gz` & `tmp/pyogrio-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyogrio-0.5.1.tar", last modified: Fri Jan 27 03:29:00 2023, max compression
+gzip compressed data, was "pyogrio-0.6.0.tar", last modified: Thu Apr 27 07:39:04 2023, max compression
```

## Comparing `pyogrio-0.5.1.tar` & `pyogrio-0.6.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:29:00.133070 pyogrio-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-27 03:28:42.000000 pyogrio-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-27 03:28:42.000000 pyogrio-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-01-27 03:29:00.133070 pyogrio-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-01-27 03:28:42.000000 pyogrio-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:29:00.133070 pyogrio-0.5.1/pyogrio/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_err.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_err.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_geometry.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_geometry.pyx
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_io.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    54788 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_io.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_ogr.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/_ogr.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-27 03:29:00.133070 pyogrio-0.5.1/pyogrio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/arrow_bridge.h
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:29:00.129070 pyogrio-0.5.1/pyogrio/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:29:00.129070 pyogrio-0.5.1/pyogrio/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:29:00.133070 pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.cpg
--rw-r--r--   0 runner    (1001) docker     (123)    48869 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.prj
--rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shp
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shx
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/test_datetime.geojson
--rw-r--r--   0 runner    (1001) docker     (123)   101524 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/test_fgdb.gdb.zip
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/test_gpkg_nulls.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/test_multisurface.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/fixtures/test_ogr_types_list.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    31219 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/test_geopandas_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/test_raw_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/tests/win32.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyogrio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 03:29:00.129070 pyogrio-0.5.1/pyogrio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-01-27 03:29:00.000000 pyogrio-0.5.1/pyogrio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-27 03:29:00.000000 pyogrio-0.5.1/pyogrio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 03:29:00.000000 pyogrio-0.5.1/pyogrio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-27 03:29:00.000000 pyogrio-0.5.1/pyogrio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-27 03:29:00.000000 pyogrio-0.5.1/pyogrio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-01-27 03:28:42.000000 pyogrio-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-27 03:29:00.133070 pyogrio-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-01-27 03:28:42.000000 pyogrio-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:39:04.167846 pyogrio-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-27 07:38:46.000000 pyogrio-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 07:38:46.000000 pyogrio-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-27 07:39:04.167846 pyogrio-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-27 07:38:46.000000 pyogrio-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:39:04.167846 pyogrio-0.6.0/pyogrio/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_err.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_err.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_geometry.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_geometry.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_io.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    58558 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_io.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_ogr.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/_ogr.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 07:39:04.167846 pyogrio-0.6.0/pyogrio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/arrow_bridge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:39:04.163845 pyogrio-0.6.0/pyogrio/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:39:04.163845 pyogrio-0.6.0/pyogrio/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:39:04.167846 pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)    48869 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.prj
+-rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shp
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shx
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/test_datetime.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)   101524 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/test_fgdb.gdb.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/test_gpkg_nulls.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/test_multisurface.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/test_nested.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/fixtures/test_ogr_types_list.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39322 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/test_geopandas_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29138 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/test_raw_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/tests/win32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyogrio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:39:04.159845 pyogrio-0.6.0/pyogrio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-27 07:39:04.000000 pyogrio-0.6.0/pyogrio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-27 07:39:04.000000 pyogrio-0.6.0/pyogrio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:39:04.000000 pyogrio-0.6.0/pyogrio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 07:39:04.000000 pyogrio-0.6.0/pyogrio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 07:39:04.000000 pyogrio-0.6.0/pyogrio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-27 07:38:46.000000 pyogrio-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-27 07:39:04.167846 pyogrio-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-04-27 07:38:46.000000 pyogrio-0.6.0/setup.py
```

### Comparing `pyogrio-0.5.1/LICENSE` & `pyogrio-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/PKG-INFO` & `pyogrio-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyogrio
-Version: 0.5.1
+Version: 0.6.0
 Summary: Vectorized spatial vector file format I/O using GDAL/OGR
-Home-page: https://github.com/pyogrio/pyogrio
+Home-page: https://github.com/geopandas/pyogrio
 Author: Brendan C. Ward
 Author-email: bcward@astutespruce.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `pyogrio-0.5.1/README.md` & `pyogrio-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/__init__.py` & `pyogrio-0.6.0/pyogrio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/_env.py` & `pyogrio-0.6.0/pyogrio/_env.py`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/_err.pyx` & `pyogrio-0.6.0/pyogrio/_err.pyx`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # ported from fiona::_err.pyx
 from enum import IntEnum
+import warnings
 
 from pyogrio._ogr cimport (
     CE_None, CE_Debug, CE_Warning, CE_Failure, CE_Fatal, CPLErrorReset,
-    CPLGetLastErrorType, CPLGetLastErrorNo, CPLGetLastErrorMsg, OGRErr)
+    CPLGetLastErrorType, CPLGetLastErrorNo, CPLGetLastErrorMsg, OGRErr,
+    CPLErr, CPLErrorHandler, CPLDefaultErrorHandler, CPLPushErrorHandler)
 
 
 # CPL Error types as an enum.
 class GDALError(IntEnum):
     none = CE_None
     debug = CE_Debug
     warning = CE_Warning
@@ -203,7 +205,42 @@
 
     Adapted from Fiona (_err.pyx).
     """
     if err != 0:
         raise CPLE_BaseError(3, err, f"OGR Error code {err}")
 
     return err
+
+
+cdef void error_handler(CPLErr err_class, int err_no, const char* err_msg) nogil:
+    """Custom CPL error handler to match the Python behaviour.
+
+    Generally we want to suppress error printing to stderr (behaviour of the
+    default GDAL error handler) because we already raise a Python exception
+    that includes the error message.
+    """
+    if err_class == CE_Fatal:
+        # If the error class is CE_Fatal, we want to have a message issued
+        # because the CPL support code does an abort() before any exception
+        # can be generated
+        CPLDefaultErrorHandler(err_class, err_no, err_msg)
+        return
+
+    elif err_class == CE_Failure:
+        # For Failures, do nothing as those are explicitly caught
+        # with error return codes and translated into Python exceptions
+        return
+
+    elif err_class == CE_Warning:
+        with gil:
+            msg_b = err_msg
+            msg = msg_b.decode('utf-8')
+            warnings.warn(msg, RuntimeWarning)
+        return
+
+    # Fall back to the default handler for non-failure messages since
+    # they won't be translated into exceptions.
+    CPLDefaultErrorHandler(err_class, err_no, err_msg)
+
+
+def _register_error_handler():
+    CPLPushErrorHandler(<CPLErrorHandler>error_handler)
```

### Comparing `pyogrio-0.5.1/pyogrio/_geometry.pyx` & `pyogrio-0.6.0/pyogrio/_geometry.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -30,45 +30,45 @@
     wkbPointZM: 'Measured 3D Point',
     wkbLineStringZM: 'Measured 3D LineString',
     wkbPolygonZM: 'Measured 3D Polygon',
     wkbMultiPointZM: 'Measured 3D MultiPoint',
     wkbMultiLineStringZM: 'Measured 3D MultiLineString',
     wkbMultiPolygonZM: 'Measured 3D MultiPolygon',
     wkbGeometryCollectionZM: 'Measured 3D GeometryCollection',
-    wkbPoint25D: '2.5D Point',
-    wkbLineString25D: '2.5D LineString',
-    wkbPolygon25D: '2.5D Polygon',
-    wkbMultiPoint25D: '2.5D MultiPoint',
-    wkbMultiLineString25D: '2.5D MultiLineString',
-    wkbMultiPolygon25D: '2.5D MultiPolygon',
-    wkbGeometryCollection25D: '2.5D GeometryCollection',
+    wkbPoint25D: 'Point Z',
+    wkbLineString25D: 'LineString Z',
+    wkbPolygon25D: 'Polygon Z',
+    wkbMultiPoint25D: 'MultiPoint Z',
+    wkbMultiLineString25D: 'MultiLineString Z',
+    wkbMultiPolygon25D: 'MultiPolygon Z',
+    wkbGeometryCollection25D: 'GeometryCollection Z',
 }
 
 GEOMETRY_TYPE_CODES = {v:k for k, v in GEOMETRY_TYPES.items()}
 
-# add additional aliases from Simple Features WKT types with Z
+# add additional aliases from 2.5D format
 GEOMETRY_TYPE_CODES.update({
-    'Point Z': wkbPoint25D,
-    'LineString Z': wkbLineString25D,
-    'Polygon Z': wkbPolygon25D,
-    'MultiPoint Z': wkbMultiPoint25D,
-    'MultiLineString Z': wkbMultiLineString25D,
-    'MultiPolygon Z': wkbMultiPolygon25D,
-    'GeometryCollection Z': wkbGeometryCollection25D
+    '2.5D Point': wkbPoint25D,
+    '2.5D LineString': wkbLineString25D,
+    '2.5D Polygon': wkbPolygon25D,
+    '2.5D MultiPoint': wkbMultiPoint25D,
+    '2.5D MultiLineString': wkbMultiLineString25D,
+    '2.5D MultiPolygon': wkbMultiPolygon25D,
+    '2.5D GeometryCollection': wkbGeometryCollection25D
 })
 
 # 2.5D also represented using negative numbers not enumerated above
 GEOMETRY_TYPES.update({
-    -2147483647: '2.5D Point',
-    -2147483646: '2.5D LineString',
-    -2147483645: '2.5D Polygon',
-    -2147483644: '2.5D MultiPoint',
-    -2147483643: '2.5D MultiLineString',
-    -2147483642: '2.5D MultiPolygon',
-    -2147483641: '2.5D GeometryCollection',
+    -2147483647: 'Point Z',
+    -2147483646: 'LineString Z',
+    -2147483645: 'Polygon Z',
+    -2147483644: 'MultiPoint Z',
+    -2147483643: 'MultiLineString Z',
+    -2147483642: 'MultiPolygon Z',
+    -2147483641: 'GeometryCollection Z',
 })
 
 
 cdef str get_geometry_type(void *ogr_layer):
     """Get geometry type for layer.
 
     Parameters
```

### Comparing `pyogrio-0.5.1/pyogrio/_io.pyx` & `pyogrio-0.6.0/pyogrio/_io.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 """IO support for OGR vector data sources
 """
 
 
+import contextlib
 import datetime
 import locale
 import logging
 import math
 import os
 import warnings
 
@@ -105,48 +106,67 @@
 #     cdef int err = GDALDatasetRollbackTransaction(ogr_dataset)
 #     if err == OGRERR_FAILURE:
 #         raise DataSourceError("Failed to rollback transaction")
 
 #     return 0
 
 
-# ported from fiona::_shim22.pyx::gdal_open_vector
-cdef void* ogr_open(const char* path_c, int mode, options) except NULL:
+cdef char** dict_to_options(object values):
+    """Convert a python dictionary into name / value pairs (stored in a char**)
+
+    Parameters
+    ----------
+    values: dict
+        all keys and values must be strings
+
+    Returns
+    -------
+    char**
+    """
+    cdef char **options = NULL
+
+    if values is None:
+        return NULL
+
+    for k, v in values.items():
+        k = k.encode('UTF-8')
+        v = v.encode('UTF-8')
+        options = CSLAddNameValue(options, <const char *>k, <const char *>v)
+
+    return options
+
+
+cdef void* ogr_open(const char* path_c, int mode, char** options) except NULL:
     cdef void* ogr_dataset = NULL
-    cdef char **ogr_drivers = NULL
-    cdef void* ogr_driver = NULL
-    cdef char **open_opts = NULL
 
     # Force linear approximations in all cases
     OGRSetNonLinearGeometriesEnabledFlag(0)
 
     flags = GDAL_OF_VECTOR | GDAL_OF_VERBOSE_ERROR
     if mode == 1:
         flags |= GDAL_OF_UPDATE
     else:
         flags |= GDAL_OF_READONLY
 
-    open_opts = CSLAddNameValue(open_opts, "VALIDATE_OPEN_OPTIONS", "NO")
 
     try:
+        # WARNING: GDAL logs warnings about invalid open options to stderr
+        # instead of raising an error
         ogr_dataset = exc_wrap_pointer(
-            GDALOpenEx(path_c, flags, <const char *const *>ogr_drivers, <const char *const *>open_opts, NULL)
+            GDALOpenEx(path_c, flags, NULL, <const char *const *>options, NULL)
         )
+
         return ogr_dataset
 
     except NullPointerError:
         raise DataSourceError("Failed to open dataset (mode={}): {}".format(mode, path_c.decode("utf-8"))) from None
 
     except CPLE_BaseError as exc:
         raise DataSourceError(str(exc))
 
-    finally:
-        CSLDestroy(ogr_drivers)
-        CSLDestroy(open_opts)
-
 
 cdef OGRLayerH get_ogr_layer(GDALDatasetH ogr_dataset, layer) except NULL:
     """Open OGR layer by index or name.
 
     Parameters
     ----------
     ogr_dataset : pointer to open OGR dataset
@@ -260,43 +280,105 @@
         wkt = get_string(ogr_wkt)
 
     finally:
         CPLFree(ogr_wkt)
         return wkt
 
 
-cdef detect_encoding(OGRDataSourceH ogr_dataset, OGRLayerH ogr_layer):
-    """Attempt to detect the encoding of the layer.
-    If it supports UTF-8, use that.
-    If it is a shapefile, it must otherwise be ISO-8859-1.
+cdef get_driver(OGRDataSourceH ogr_dataset):
+    """Get the driver for a dataset.
 
     Parameters
     ----------
     ogr_dataset : pointer to open OGR dataset
-    ogr_layer : pointer to open OGR layer
-
     Returns
     -------
     str or None
     """
     cdef void *ogr_driver
 
-    if OGR_L_TestCapability(ogr_layer, OLCStringsAsUTF8):
-        return 'UTF-8'
-
     try:
         ogr_driver = exc_wrap_pointer(GDALGetDatasetDriver(ogr_dataset))
 
     except NullPointerError:
-        raise DataLayerError(f"Could not detect encoding of layer") from None
+        raise DataLayerError(f"Could not detect driver of dataset") from None
 
     except CPLE_BaseError as exc:
         raise DataLayerError(str(exc))
 
     driver = OGR_Dr_GetName(ogr_driver).decode("UTF-8")
+    return driver
+
+
+cdef set_metadata(GDALMajorObjectH obj, object metadata):
+    """Set metadata on a dataset or layer
+
+    Parameters
+    ----------
+    obj : pointer to dataset or layer
+    metadata : dict, optional (default None)
+        keys and values must be strings
+    """
+
+    cdef char **metadata_items = NULL
+    cdef int err = 0
+
+    metadata_items = dict_to_options(metadata)
+    if metadata_items != NULL:
+        # only default namepace is currently supported
+        err = GDALSetMetadata(obj, metadata_items, NULL)
+
+        CSLDestroy(metadata_items)
+        metadata_items = NULL
+
+    if err:
+        raise RuntimeError("Could not set metadata") from None
+
+cdef get_metadata(GDALMajorObjectH obj):
+    """Get metadata for a dataset or layer
+
+    Parameters
+    ----------
+    obj : pointer to dataset or layer
+
+    Returns
+    -------
+    dict or None
+        metadata as key, value pairs
+    """
+    # only default namespace is currently supported
+    cdef char **metadata = GDALGetMetadata(obj, NULL)
+
+    if metadata != NULL:
+        return dict(
+            metadata[i].decode('UTF-8').split('=', 1)
+            for i in range(CSLCount(metadata))
+        )
+
+    return None
+
+
+cdef detect_encoding(OGRDataSourceH ogr_dataset, OGRLayerH ogr_layer):
+    """Attempt to detect the encoding of the layer.
+    If it supports UTF-8, use that.
+    If it is a shapefile, it must otherwise be ISO-8859-1.
+
+    Parameters
+    ----------
+    ogr_dataset : pointer to open OGR dataset
+    ogr_layer : pointer to open OGR layer
+
+    Returns
+    -------
+    str or None
+    """
+    if OGR_L_TestCapability(ogr_layer, OLCStringsAsUTF8):
+        return 'UTF-8'
+
+    driver = get_driver(ogr_dataset)
     if driver == 'ESRI Shapefile':
         return 'ISO-8859-1'
 
     return None
 
 
 cdef get_fields(OGRLayerH ogr_layer, str encoding, use_arrow=False):
@@ -840,31 +922,32 @@
         bounds_data = bounds_data[:, :i]
 
     return fid_data, bounds_data
 
 
 def ogr_read(
     str path,
+    object dataset_kwargs,
     object layer=None,
     object encoding=None,
     int read_geometry=True,
     int force_2d=False,
     object columns=None,
     int skip_features=0,
     int max_features=0,
     object where=None,
     tuple bbox=None,
     object fids=None,
     str sql=None,
     str sql_dialect=None,
-    int return_fids=False,
-    **kwargs):
+    int return_fids=False):
 
     cdef int err = 0
     cdef const char *path_c = NULL
+    cdef char **dataset_options = NULL
     cdef const char *where_c = NULL
     cdef const char *field_c = NULL
     cdef char **fields_c = NULL
     cdef OGRDataSourceH ogr_dataset = NULL
     cdef OGRLayerH ogr_layer = NULL
     cdef int feature_count = 0
     cdef double xmin, ymin, xmax, ymax
@@ -879,16 +962,18 @@
                 "'skip_features' or 'max_features'"
             )
         fids = np.asarray(fids, dtype=np.intc)
 
     if sql is not None and layer is not None:
         raise ValueError("'sql' paramater cannot be combined with 'layer'")
 
-    ogr_dataset = ogr_open(path_c, 0, kwargs)
     try:
+        dataset_options = dict_to_options(dataset_kwargs)
+        ogr_dataset = ogr_open(path_c, 0, dataset_options)
+
         if sql is None:
             # layer defaults to index 0
             if layer is None:
                 layer = 0
             ogr_layer = get_ogr_layer(ogr_dataset, layer)
         else:
             ogr_layer = execute_sql(ogr_dataset, sql, sql_dialect)
@@ -969,52 +1054,58 @@
                 return_fids=return_fids
             )
 
         meta = {
             'crs': crs,
             'encoding': encoding,
             'fields': fields[:,2], # return only names
-            'geometry_type': geometry_type
+            'geometry_type': geometry_type,
         }
 
     finally:
+        if dataset_options != NULL:
+            CSLDestroy(dataset_options)
+            dataset_options = NULL
+
         if ogr_dataset != NULL:
             if sql is not None:
                 GDALDatasetReleaseResultSet(ogr_dataset, ogr_layer)
 
             GDALClose(ogr_dataset)
             ogr_dataset = NULL
 
     return (
         meta,
         fid_data,
         geometries,
         field_data
     )
 
-
-def ogr_read_arrow(
+@contextlib.contextmanager
+def ogr_open_arrow(
     str path,
+    dataset_kwargs,
     object layer=None,
     object encoding=None,
     int read_geometry=True,
     int force_2d=False,
     object columns=None,
     int skip_features=0,
     int max_features=0,
     object where=None,
     tuple bbox=None,
     object fids=None,
     str sql=None,
     str sql_dialect=None,
     int return_fids=False,
-    **kwargs):
+    int batch_size=0):
 
     cdef int err = 0
     cdef const char *path_c = NULL
+    cdef char **dataset_options = NULL
     cdef const char *where_c = NULL
     cdef OGRDataSourceH ogr_dataset = NULL
     cdef OGRLayerH ogr_layer = NULL
     cdef char **fields_c = NULL
     cdef const char *field_c = NULL
     cdef char **options = NULL
     cdef ArrowArrayStream stream
@@ -1033,16 +1124,19 @@
         raise ValueError(
             "specifying 'skip_features' or 'max_features' is not supported for Arrow"
         )
 
     if sql is not None and layer is not None:
         raise ValueError("'sql' paramater cannot be combined with 'layer'")
 
-    ogr_dataset = ogr_open(path_c, 0, kwargs)
+    reader = None
     try:
+        dataset_options = dict_to_options(dataset_kwargs)
+        ogr_dataset = ogr_open(path_c, 0, dataset_options)
+
         if sql is None:
             # layer defaults to index 0
             if layer is None:
                 layer = 0
             ogr_layer = get_ogr_layer(ogr_dataset, layer)
         else:
             ogr_layer = execute_sql(ogr_dataset, sql, sql_dialect)
@@ -1086,64 +1180,78 @@
                 fields_c = CSLAddString(fields_c, field_c)
 
             OGR_L_SetIgnoredFields(ogr_layer, <const char**>fields_c)
 
         if not return_fids:
             options = CSLSetNameValue(options, "INCLUDE_FID", "NO")
 
+        if batch_size > 0:
+            options = CSLSetNameValue(
+                options,
+                "MAX_FEATURES_IN_BATCH",
+                str(batch_size).encode('UTF-8')
+            )
+
         # make sure layer is read from beginning
         OGR_L_ResetReading(ogr_layer)
 
         IF CTE_GDAL_VERSION < (3, 6, 0):
             raise RuntimeError("Need GDAL>=3.6 for Arrow support")
 
         if not OGR_L_GetArrowStream(ogr_layer, &stream, options):
             raise RuntimeError("Failed to open ArrowArrayStream from Layer")
 
         stream_ptr = <uintptr_t> &stream
 
         # stream has to be consumed before the Dataset is closed
         import pyarrow as pa
-        table = pa.RecordBatchStreamReader._import_from_c(stream_ptr).read_all()
+        reader = pa.RecordBatchStreamReader._import_from_c(stream_ptr)
 
         meta = {
             'crs': crs,
             'encoding': encoding,
             'fields': fields[:,2], # return only names
             'geometry_type': geometry_type,
             'geometry_name': geometry_name,
         }
 
+        yield meta, reader
+
     finally:
+        if reader is not None:
+            # Mark reader as closed to prevent reading batches
+            reader.close()
+
         CSLDestroy(options)
         if fields_c != NULL:
             CSLDestroy(fields_c)
             fields_c = NULL
+
+        if dataset_options != NULL:
+            CSLDestroy(dataset_options)
+            dataset_options = NULL
+
         if ogr_dataset != NULL:
             if sql is not None:
                 GDALDatasetReleaseResultSet(ogr_dataset, ogr_layer)
 
             GDALClose(ogr_dataset)
             ogr_dataset = NULL
 
-    return meta, table
-
-
 def ogr_read_bounds(
     str path,
     object layer=None,
     object encoding=None,
     int read_geometry=True,
     int force_2d=False,
     object columns=None,
     int skip_features=0,
     int max_features=0,
     object where=None,
-    tuple bbox=None,
-    **kwargs):
+    tuple bbox=None):
 
     cdef int err = 0
     cdef const char *path_c = NULL
     cdef const char *where_c = NULL
     cdef OGRDataSourceH ogr_dataset = NULL
     cdef OGRLayerH ogr_layer = NULL
     cdef int feature_count = 0
@@ -1152,15 +1260,15 @@
     path_b = path.encode('utf-8')
     path_c = path_b
 
     # layer defaults to index 0
     if layer is None:
         layer = 0
 
-    ogr_dataset = ogr_open(path_c, 0, kwargs)
+    ogr_dataset = ogr_open(path_c, 0, NULL)
     ogr_layer = get_ogr_layer(ogr_dataset, layer)
 
     # Apply the attribute filter
     if where is not None and where != "":
         apply_where_filter(ogr_layer, where)
 
     # Apply the spatial filter
@@ -1169,70 +1277,86 @@
 
     # Limit feature range to available range
     skip_features, num_features = validate_feature_range(ogr_layer, skip_features, max_features)
 
     return get_bounds(ogr_layer, skip_features, num_features)
 
 
-def ogr_read_info(str path, object layer=None, object encoding=None, **kwargs):
+def ogr_read_info(
+    str path,
+    dataset_kwargs,
+    object layer=None,
+    object encoding=None):
+
     cdef const char *path_c = NULL
+    cdef char **dataset_options = NULL
     cdef OGRDataSourceH ogr_dataset = NULL
     cdef OGRLayerH ogr_layer = NULL
 
     path_b = path.encode('utf-8')
     path_c = path_b
 
     # layer defaults to index 0
     if layer is None:
         layer = 0
 
-    ogr_dataset = ogr_open(path_c, 0, kwargs)
-    ogr_layer = get_ogr_layer(ogr_dataset, layer)
+    try:
+        dataset_options = dict_to_options(dataset_kwargs)
+        ogr_dataset = ogr_open(path_c, 0, dataset_options)
+        ogr_layer = get_ogr_layer(ogr_dataset, layer)
 
-    # Encoding is derived from the user, from the dataset capabilities / type,
-    # or from the system locale
-    encoding = (
-        encoding
-        or detect_encoding(ogr_dataset, ogr_layer)
-        or locale.getpreferredencoding()
-    )
+        # Encoding is derived from the user, from the dataset capabilities / type,
+        # or from the system locale
+        encoding = (
+            encoding
+            or detect_encoding(ogr_dataset, ogr_layer)
+            or locale.getpreferredencoding()
+        )
 
-    fields = get_fields(ogr_layer, encoding)
+        fields = get_fields(ogr_layer, encoding)
 
-    meta = {
-        'crs': get_crs(ogr_layer),
-        'encoding': encoding,
-        'fields': fields[:,2], # return only names
-        'dtypes': fields[:,3],
-        'geometry_type': get_geometry_type(ogr_layer),
-        'features': OGR_L_GetFeatureCount(ogr_layer, 1),
-        "capabilities": {
-            "random_read": OGR_L_TestCapability(ogr_layer, OLCRandomRead),
-            "fast_set_next_by_index": OGR_L_TestCapability(ogr_layer, OLCFastSetNextByIndex),
-            "fast_spatial_filter": OGR_L_TestCapability(ogr_layer, OLCFastSpatialFilter),
+        meta = {
+            'crs': get_crs(ogr_layer),
+            'encoding': encoding,
+            'fields': fields[:,2], # return only names
+            'dtypes': fields[:,3],
+            'geometry_type': get_geometry_type(ogr_layer),
+            'features': OGR_L_GetFeatureCount(ogr_layer, 1),
+            'driver': get_driver(ogr_dataset),
+            "capabilities": {
+                "random_read": OGR_L_TestCapability(ogr_layer, OLCRandomRead),
+                "fast_set_next_by_index": OGR_L_TestCapability(ogr_layer, OLCFastSetNextByIndex),
+                "fast_spatial_filter": OGR_L_TestCapability(ogr_layer, OLCFastSpatialFilter),
+            },
+            'layer_metadata': get_metadata(ogr_layer),
+            'dataset_metadata': get_metadata(ogr_dataset),
         }
-    }
 
-    if ogr_dataset != NULL:
-        GDALClose(ogr_dataset)
-    ogr_dataset = NULL
+    finally:
+        if dataset_options != NULL:
+            CSLDestroy(dataset_options)
+            dataset_options = NULL
+
+        if ogr_dataset != NULL:
+            GDALClose(ogr_dataset)
+            ogr_dataset = NULL
 
     return meta
 
 
 def ogr_list_layers(str path):
     cdef const char *path_c = NULL
     cdef const char *ogr_name = NULL
     cdef OGRDataSourceH ogr_dataset = NULL
     cdef OGRLayerH ogr_layer = NULL
 
     path_b = path.encode('utf-8')
     path_c = path_b
 
-    ogr_dataset = ogr_open(path_c, 0, None)
+    ogr_dataset = ogr_open(path_c, 0, NULL)
 
     layer_count = GDALDatasetGetLayerCount(ogr_dataset)
 
     data = np.empty(shape=(layer_count, 2), dtype=object)
     data_view = data[:]
     for i in range(layer_count):
         ogr_layer = GDALDatasetGetLayer(ogr_dataset, i)
@@ -1342,18 +1466,18 @@
             raise NotImplementedError(f"field type is not supported {dtype.name} (field index: {i})")
 
     return field_types
 
 
 # TODO: set geometry and field data as memory views?
 def ogr_write(
-    str path, str layer, str driver, geometry, field_data, fields,
+    str path, str layer, str driver, geometry, fields, field_data, field_mask,
     str crs, str geometry_type, str encoding, object dataset_kwargs,
     object layer_kwargs, bint promote_to_multi=False, bint nan_as_null=True,
-    bint append=False
+    bint append=False, dataset_metadata=None, layer_metadata=None
 ):
     cdef const char *path_c = NULL
     cdef const char *layer_c = NULL
     cdef const char *driver_c = NULL
     cdef const char *crs_c = NULL
     cdef const char *encoding_c = NULL
     cdef char **dataset_options = NULL
@@ -1380,14 +1504,23 @@
         raise ValueError("field_data and fields must be same length")
 
     if num_fields:
         for i in range(1, len(field_data)):
             if len(field_data[i]) != num_records:
                 raise ValueError("field_data arrays must be same length as geometry array")
 
+    if field_mask is not None:
+        if len(field_data) != len(field_mask):
+            raise ValueError("field_data and field_mask must be same length")
+        for i in range(0, len(field_mask)):
+            if field_mask[i] is not None and len(field_mask[i]) != num_records:
+                raise ValueError("field_mask arrays must be same length as geometry array")
+    else:
+        field_mask = [None] * len(field_data)
+
     path_b = path.encode('UTF-8')
     path_c = path_b
 
     driver_b = driver.encode('UTF-8')
     driver_c = driver_b
 
     if not layer:
@@ -1400,15 +1533,15 @@
     if driver in ('ESRI Shapefile', 'GeoJSON', 'GeoJSONSeq', 'FlatGeobuf') and os.path.exists(path):
         if not append:
             os.unlink(path)
 
     layer_exists = False
     if os.path.exists(path):
         try:
-            ogr_dataset = ogr_open(path_c, 1, None)
+            ogr_dataset = ogr_open(path_c, 1, NULL)
 
             for i in range(GDALDatasetGetLayerCount(ogr_dataset)):
                 name = OGR_L_GetName(GDALDatasetGetLayer(ogr_dataset, i))
                 if layer == name.decode('UTF-8'):
                     layer_idx = i
                     break
 
@@ -1425,19 +1558,15 @@
 
             # otherwise create from scratch
             os.unlink(path)
             ogr_dataset = NULL
 
     # either it didn't exist or could not open it in write mode
     if ogr_dataset == NULL:
-        for k, v in dataset_kwargs.items():
-            k = k.encode('UTF-8')
-            v = v.encode('UTF-8')
-            dataset_options = CSLAddNameValue(dataset_options, <const char *>k, <const char *>v)
-
+        dataset_options = dict_to_options(dataset_kwargs)
         ogr_dataset = ogr_create(path_c, driver_c, dataset_options)
 
     # if we are not appending to an existing layer, we need to create
     # the layer and all associated properties (CRS, field defs, etc)
     create_layer = not (append and layer_exists)
 
     ### Create the layer
@@ -1447,15 +1576,15 @@
             try:
                 ogr_crs = create_crs(crs)
 
             except Exception as exc:
                 OGRReleaseDataSource(ogr_dataset)
                 ogr_dataset = NULL
                 if dataset_options != NULL:
-                    CSLDestroy(<char**>dataset_options)
+                    CSLDestroy(dataset_options)
                     dataset_options = NULL
                 raise exc
 
         # Setup layer creation options
         if not encoding:
             encoding = locale.getpreferredencoding()
 
@@ -1485,14 +1614,18 @@
             ogr_layer = exc_wrap_pointer(
                     GDALDatasetCreateLayer(ogr_dataset, layer_c, ogr_crs,
                             geometry_code, layer_options))
 
         else:
             ogr_layer = exc_wrap_pointer(get_ogr_layer(ogr_dataset, layer))
 
+        # Set dataset and layer metadata
+        set_metadata(ogr_dataset, dataset_metadata)
+        set_metadata(ogr_layer, layer_metadata)
+
     except Exception as exc:
         OGRReleaseDataSource(ogr_dataset)
         ogr_dataset = NULL
         raise DataLayerError(str(exc))
 
     finally:
         if ogr_crs != NULL:
@@ -1564,15 +1697,15 @@
             if ogr_feature == NULL:
                 raise FeatureError(f"Could not create feature at index {i}") from None
 
             # create the geometry based on specific WKB type (there might be mixed types in geometries)
             # TODO: geometry must not be null or errors
             wkb = geometry[i]
             if wkb is not None:
-                wkbtype = bytearray(wkb)[1]
+                wkbtype = <int>bytearray(wkb)[1]
                 # may need to consider all 4 bytes: int.from_bytes(wkb[0][1:4], byteorder="little")
                 # use "little" if the first byte == 1
                 ogr_geometry = OGR_G_CreateGeometry(<OGRwkbGeometryType>wkbtype)
                 if ogr_geometry == NULL:
                     raise GeometryError(f"Could not create geometry at index {i} for WKB type {wkbtype}") from None
 
                 # import the WKB
@@ -1600,15 +1733,19 @@
                     raise GeometryError(f"Could not set geometry for feature at index {i}") from None
 
             # Set field values
             for field_idx in range(num_fields):
                 field_value = field_data[field_idx][i]
                 field_type = field_types[field_idx][0]
 
-                if field_type == OFTString:
+                mask = field_mask[field_idx]
+                if mask is not None and mask[i]:
+                    OGR_F_SetFieldNull(ogr_feature, field_idx)
+
+                elif field_type == OFTString:
                     # TODO: encode string using approach from _get_internal_encoding which checks layer capabilities
                     if (
                         field_value is None
                         or (isinstance(field_value, float) and isnan(field_value))
                     ):
                         OGR_F_SetFieldNull(ogr_feature, field_idx)
```

### Comparing `pyogrio-0.5.1/pyogrio/_ogr.pxd` & `pyogrio-0.6.0/pyogrio/_ogr.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,39 @@
     void    CPLFree(void *ptr)
 
     const char* CPLFindFile(const char *pszClass, const char *filename)
     const char* CPLGetConfigOption(const char* key, const char* value)
     void        CPLSetConfigOption(const char* key, const char* value)
 
 
-cdef extern from "cpl_error.h":
+cdef extern from "cpl_error.h" nogil:
     ctypedef enum CPLErr:
         CE_None
         CE_Debug
         CE_Warning
         CE_Failure
         CE_Fatal
 
     void            CPLErrorReset()
     int             CPLGetLastErrorNo()
     const char*    CPLGetLastErrorMsg()
     int             CPLGetLastErrorType()
 
+    ctypedef void (*CPLErrorHandler)(CPLErr, int, const char*)
+    void CPLDefaultErrorHandler(CPLErr, int, const char *)
+    void CPLPushErrorHandler(CPLErrorHandler handler)
+    void CPLPopErrorHandler()
+
 
 cdef extern from "cpl_string.h":
     char**      CSLAddNameValue(char **list, const char *name, const char *value)
     char**      CSLSetNameValue(char **list, const char *name, const char *value)
     void        CSLDestroy(char **list)
     char**      CSLAddString(char **list, const char *string)
+    int         CSLCount(char **list)
 
 
 cdef extern from "cpl_vsi.h" nogil:
 
     ctypedef FILE VSILFILE
 
     VSILFILE *VSIFileFromMemBuffer(const char *path, void *data,
@@ -363,12 +369,14 @@
                             const char* pszStatement,
                             OGRGeometryH hSpatialFilter,
                             const char* pszDialect)
     void            GDALDatasetReleaseResultSet(GDALDatasetH, OGRLayerH)
     OGRErr          GDALDatasetStartTransaction(GDALDatasetH ds, int bForce)
     OGRErr          GDALDatasetCommitTransaction(GDALDatasetH ds)
     OGRErr          GDALDatasetRollbackTransaction(GDALDatasetH ds)
+    char**          GDALGetMetadata(GDALMajorObjectH obj, const char *pszDomain)
     const char*     GDALGetMetadataItem(GDALMajorObjectH obj, const char *pszName, const char *pszDomain)
+    OGRErr          GDALSetMetadata(GDALMajorObjectH obj, char **metadata, const char *pszDomain)
     const char*     GDALVersionInfo(const char *pszRequest)
 
 
 cdef get_string(const char *c_str, str encoding=*)
```

### Comparing `pyogrio-0.5.1/pyogrio/_ogr.pyx` & `pyogrio-0.6.0/pyogrio/_ogr.pyx`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/arrow_bridge.h` & `pyogrio-0.6.0/pyogrio/arrow_bridge.h`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/core.py` & `pyogrio-0.6.0/pyogrio/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pyogrio._env import GDALEnv
+from pyogrio.raw import _preprocess_options_key_value
 from pyogrio.util import get_vsi_path
 
 
 with GDALEnv():
     from pyogrio._ogr import (
         get_gdal_version,
         get_gdal_version_string,
@@ -12,19 +13,21 @@
         get_gdal_config_option as _get_gdal_config_option,
         get_gdal_data_path as _get_gdal_data_path,
         init_gdal_data as _init_gdal_data,
         init_proj_data as _init_proj_data,
         remove_virtual_file,
         _register_drivers,
     )
+    from pyogrio._err import _register_error_handler
     from pyogrio._io import ogr_list_layers, ogr_read_bounds, ogr_read_info
 
     _init_gdal_data()
     _init_proj_data()
     _register_drivers()
+    _register_error_handler()
 
     __gdal_version__ = get_gdal_version()
     __gdal_version_string__ = get_gdal_version_string()
     __gdal_geos_version__ = get_gdal_geos_version()
 
 
 def list_drivers(read=False, write=False):
@@ -141,48 +144,58 @@
         )
     finally:
         if buffer is not None:
             remove_virtual_file(path)
     return result
 
 
-def read_info(path_or_buffer, /, layer=None, encoding=None):
+def read_info(path_or_buffer, /, layer=None, encoding=None, **kwargs):
     """Read information about an OGR data source.
 
     ``crs`` and ``geometry`` will be ``None`` and ``features`` will be 0 for a
     nonspatial layer.
 
     Parameters
     ----------
     path : str or pathlib.Path
     layer : [type], optional
         Name or index of layer in data source.  Reads the first layer by default.
     encoding : [type], optional (default: None)
         If present, will be used as the encoding for reading string values from
         the data source, unless encoding can be inferred directly from the data
         source.
+    **kwargs
+        Additional driver-specific dataset open options passed to OGR.  Invalid
+        options will trigger a warning.
 
     Returns
     -------
     dict
         A dictionary with the following keys::
 
             {
                 "crs": "<crs>",
                 "fields": <ndarray of field names>,
                 "dtypes": <ndarray of field dtypes>,
                 "encoding": "<encoding>",
                 "geometry": "<geometry type>",
-                "features": <feature count>
+                "features": <feature count>,
+                "driver": "<driver>",
+                "dataset_metadata" "<dict of dataset metadata or None>"
+                "layer_metadata" "<dict of layer metadata or None>"
             }
     """
     path, buffer = get_vsi_path(path_or_buffer)
 
+    dataset_kwargs = _preprocess_options_key_value(kwargs) if kwargs else {}
+
     try:
-        result = ogr_read_info(path, layer=layer, encoding=encoding)
+        result = ogr_read_info(
+            path, layer=layer, encoding=encoding, dataset_kwargs=dataset_kwargs
+        )
     finally:
         if buffer is not None:
             remove_virtual_file(path)
     return result
 
 
 def set_gdal_config_options(options):
```

### Comparing `pyogrio-0.5.1/pyogrio/errors.py` & `pyogrio-0.6.0/pyogrio/errors.py`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/geopandas.py` & `pyogrio-0.6.0/pyogrio/geopandas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from pyogrio.raw import DRIVERS_NO_MIXED_SINGLE_MULTI
+import numpy as np
+from pyogrio.raw import DRIVERS_NO_MIXED_SINGLE_MULTI, DRIVERS_NO_MIXED_DIMENSIONS
 from pyogrio.raw import detect_driver, read, read_arrow, write
+from pyogrio.errors import DataSourceError
 
 
 def _stringify_path(path):
     """
     Convert path-like to a string if possible, pass-through other objects
     """
     if isinstance(path, str):
@@ -30,14 +32,15 @@
     where=None,
     bbox=None,
     fids=None,
     sql=None,
     sql_dialect=None,
     fid_as_index=False,
     use_arrow=False,
+    **kwargs,
 ):
     """Read from an OGR data source to a GeoPandas GeoDataFrame or Pandas DataFrame.
     If the data source does not have a geometry column or ``read_geometry`` is False,
     a DataFrame will be returned.
 
     Requires ``geopandas`` >= 0.8.
 
@@ -115,14 +118,17 @@
     fid_as_index : bool, optional (default: False)
         If True, will use the FIDs of the features that were read as the
         index of the GeoDataFrame.  May start at 0 or 1 depending on the driver.
     use_arrow : bool, default False
         Whether to use Arrow as the transfer mechanism of the read data
         from GDAL to Python (requires GDAL >= 3.6 and `pyarrow` to be
         installed). When enabled, this provides a further speed-up.
+    **kwargs
+        Additional driver-specific dataset open options passed to OGR.  Invalid
+        options will trigger a warning.
 
     Returns
     -------
     GeoDataFrame or DataFrame (if no geometry is present)
 
     .. _OGRSQL: https://gdal.org/user/ogr_sql_dialect.html#ogr-sql-dialect
     .. _SQLITE: https://gdal.org/user/sql_sqlite_dialect.html#sql-sqlite-dialect
@@ -151,14 +157,15 @@
         max_features=max_features,
         where=where,
         bbox=bbox,
         fids=fids,
         sql=sql,
         sql_dialect=sql_dialect,
         return_fids=fid_as_index,
+        **kwargs,
     )
 
     if use_arrow:
         meta, table = result
         df = table.to_pandas()
         geometry_name = meta["geometry_name"] or "wkb_geometry"
         if geometry_name in df.columns:
@@ -193,14 +200,17 @@
     layer=None,
     driver=None,
     encoding=None,
     geometry_type=None,
     promote_to_multi=None,
     nan_as_null=True,
     append=False,
+    dataset_metadata=None,
+    layer_metadata=None,
+    metadata=None,
     dataset_options=None,
     layer_options=None,
     **kwargs,
 ):
     """
     Write GeoPandas GeoDataFrame to an OGR file format.
 
@@ -250,14 +260,24 @@
         default (e.g. GeoJSON will skip this property) or might treat them as
         null anyway (e.g. GeoPackage).
     append : bool, optional (default: False)
         If True, the data source specified by path already exists, and the
         driver supports appending to an existing data source, will cause the
         data to be appended to the existing records in the data source.
         NOTE: append support is limited to specific drivers and GDAL versions.
+    dataset_metadata : dict, optional (default: None)
+        Metadata to be stored at the dataset level in the output file; limited
+        to drivers that support writing metadata, such as GPKG, and silently
+        ignored otherwise. Keys and values must be strings.
+    layer_metadata : dict, optional (default: None)
+        Metadata to be stored at the layer level in the output file; limited to
+        drivers that support writing metadata, such as GPKG, and silently
+        ignored otherwise. Keys and values must be strings.
+    metadata : dict, optional (default: None)
+        alias of layer_metadata
     dataset_options : dict, optional
         Dataset creation option (format specific) passed to OGR. Specify as
         a key-value dictionary.
     layer_options : dict, optional
         Layer creation option (format specific) passed to OGR. Specify as
         a key-value dictionary.
     **kwargs
@@ -300,22 +320,50 @@
         )
 
     geometry_column = geometry_columns[0]
     geometry = df[geometry_column]
     fields = [c for c in df.columns if not c == geometry_column]
 
     # TODO: may need to fill in pd.NA, etc
-    field_data = [df[f].values for f in fields]
+    field_data = []
+    field_mask = []
+    for name in fields:
+        col = df[name].values
+        if isinstance(col, pd.api.extensions.ExtensionArray):
+            from pandas.arrays import IntegerArray, FloatingArray, BooleanArray
+
+            if isinstance(col, (IntegerArray, FloatingArray, BooleanArray)):
+                field_data.append(col._data)
+                field_mask.append(col._mask)
+            else:
+                field_data.append(np.asarray(col))
+                field_mask.append(np.asarray(col.isna()))
+        else:
+            field_data.append(col)
+            field_mask.append(None)
 
     # Determine geometry_type and/or promote_to_multi
     if geometry_type is None or promote_to_multi is None:
         tmp_geometry_type = "Unknown"
+        has_z = False
 
         # If there is data, infer layer geometry type + promote_to_multi
         if not df.empty:
+            # None/Empty geometries sometimes report as Z incorrectly, so ignore them
+            has_z_arr = geometry[
+                (geometry != np.array(None)) & (~geometry.is_empty)
+            ].has_z
+            has_z = has_z_arr.any()
+            all_z = has_z_arr.all()
+
+            if driver in DRIVERS_NO_MIXED_DIMENSIONS and has_z and not all_z:
+                raise DataSourceError(
+                    f"Mixed 2D and 3D coordinates are not supported by {driver}"
+                )
+
             geometry_types = pd.Series(geometry.type.unique()).dropna().values
             if len(geometry_types) == 1:
                 tmp_geometry_type = geometry_types[0]
                 if promote_to_multi and tmp_geometry_type in (
                     "Point",
                     "LineString",
                     "Polygon",
@@ -343,14 +391,16 @@
                     ):
                         promote_to_multi = True
                     if promote_to_multi:
                         tmp_geometry_type = multi_type
 
         if geometry_type is None:
             geometry_type = tmp_geometry_type
+            if has_z and geometry_type != "Unknown":
+                geometry_type = f"{geometry_type} Z"
 
     crs = None
     if geometry.crs:
         # TODO: this may need to be WKT1, due to issues
         # if possible use EPSG codes instead
         epsg = geometry.crs.to_epsg()
         if epsg:
@@ -360,18 +410,22 @@
 
     write(
         path,
         layer=layer,
         driver=driver,
         geometry=to_wkb(geometry.values),
         field_data=field_data,
+        field_mask=field_mask,
         fields=fields,
         crs=crs,
         geometry_type=geometry_type,
         encoding=encoding,
         promote_to_multi=promote_to_multi,
         nan_as_null=nan_as_null,
         append=append,
+        dataset_metadata=dataset_metadata,
+        layer_metadata=layer_metadata,
+        metadata=metadata,
         dataset_options=dataset_options,
         layer_options=layer_options,
         **kwargs,
     )
```

### Comparing `pyogrio-0.5.1/pyogrio/raw.py` & `pyogrio-0.6.0/pyogrio/raw.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from pyogrio._env import GDALEnv
 from pyogrio.errors import DataSourceError
 from pyogrio.util import get_vsi_path
 
 with GDALEnv():
-    from pyogrio._io import ogr_read, ogr_read_arrow, ogr_write
+    from pyogrio._io import ogr_open_arrow, ogr_read, ogr_write
     from pyogrio._ogr import (
         get_gdal_version,
         get_gdal_version_string,
         ogr_driver_supports_write,
         remove_virtual_file,
         _get_driver_metadata_item,
     )
@@ -28,14 +28,18 @@
 
 
 DRIVERS_NO_MIXED_SINGLE_MULTI = {
     "FlatGeobuf",
     "GPKG",
 }
 
+DRIVERS_NO_MIXED_DIMENSIONS = {
+    "FlatGeobuf",
+}
+
 
 def read(
     path_or_buffer,
     /,
     layer=None,
     encoding=None,
     columns=None,
@@ -45,14 +49,15 @@
     max_features=None,
     where=None,
     bbox=None,
     fids=None,
     sql=None,
     sql_dialect=None,
     return_fids=False,
+    **kwargs,
 ):
     """Read OGR data source into numpy arrays.
 
     IMPORTANT: non-linear geometry types (e.g., MultiSurface) are converted
     to their linear approximations.
 
     Parameters
@@ -99,14 +104,17 @@
         with other keywords to select a subset (`skip_features`, `max_features`,
         `where` or `bbox`). Note that the starting index is driver and file
         specific (e.g. typically 0 for Shapefile and 1 for GeoPackage, but can
         still depend on the specific file). The performance of reading a large
         number of features usings FIDs is also driver specific.
     return_fids : bool, optional (default: False)
         If True, will return the FIDs of the feature that were read.
+    **kwargs
+        Additional driver-specific dataset open options passed to OGR.  Invalid
+        options will trigger a warning.
 
     Returns
     -------
     (dict, fids, geometry, data fields)
         Returns a tuple of meta information about the data source in a dict,
         an ndarray of FIDs corresponding to the features that were read or None
         (if return_fids is False),
@@ -114,19 +122,21 @@
         geometry or read_geometry is False), a tuple of ndarrays for each field
         in the data layer.
 
         Meta is: {
             "crs": "<crs>",
             "fields": <ndarray of field names>,
             "encoding": "<encoding>",
-            "geometry": "<geometry type>"
+            "geometry_type": "<geometry type>"
         }
     """
     path, buffer = get_vsi_path(path_or_buffer)
 
+    dataset_kwargs = _preprocess_options_key_value(kwargs) if kwargs else {}
+
     try:
         result = ogr_read(
             path,
             layer=layer,
             encoding=encoding,
             columns=columns,
             read_geometry=read_geometry,
@@ -135,14 +145,15 @@
             max_features=max_features or 0,
             where=where,
             bbox=bbox,
             fids=fids,
             sql=sql,
             sql_dialect=sql_dialect,
             return_fids=return_fids,
+            dataset_kwargs=dataset_kwargs,
         )
     finally:
         if buffer is not None:
             remove_virtual_file(path)
 
     return result
 
@@ -159,50 +170,146 @@
     max_features=None,
     where=None,
     bbox=None,
     fids=None,
     sql=None,
     sql_dialect=None,
     return_fids=False,
+    **kwargs,
 ):
     """
     Read OGR data source into a pyarrow Table.
 
-    See docstring of `read` for details.
+    See docstring of `read` for parameters.
+
+    Returns
+    -------
+    (dict, pyarrow.Table)
+
+        Returns a tuple of meta information about the data source in a dict,
+        and a pyarrow Table with data.
+
+        Meta is: {
+            "crs": "<crs>",
+            "fields": <ndarray of field names>,
+            "encoding": "<encoding>",
+            "geometry_type": "<geometry_type>",
+            "geometry_name": "<name of geometry column in arrow table>",
+        }
+    """
+    with open_arrow(
+        path_or_buffer,
+        layer=layer,
+        encoding=encoding,
+        columns=columns,
+        read_geometry=read_geometry,
+        force_2d=force_2d,
+        skip_features=skip_features,
+        max_features=max_features,
+        where=where,
+        bbox=bbox,
+        fids=fids,
+        sql=sql,
+        sql_dialect=sql_dialect,
+        return_fids=return_fids,
+        **kwargs,
+    ) as source:
+        meta, reader = source
+        table = reader.read_all()
+
+    return meta, table
+
+
+def open_arrow(
+    path_or_buffer,
+    /,
+    layer=None,
+    encoding=None,
+    columns=None,
+    read_geometry=True,
+    force_2d=False,
+    skip_features=0,
+    max_features=None,
+    where=None,
+    bbox=None,
+    fids=None,
+    sql=None,
+    sql_dialect=None,
+    return_fids=False,
+    batch_size=65_536,
+    **kwargs,
+):
+    """
+    Open OGR data source as a stream of pyarrow record batches.
+
+    See docstring of `read` for parameters.
+
+    The RecordBatchStreamReader is reading from a stream provided by OGR and must not be
+    accessed after the OGR dataset has been closed, i.e. after the context manager has
+    been closed.
+
+    Examples
+    --------
+
+    >>> from pyogrio.raw import open_arrow
+    >>> import pyarrow as pa
+    >>> import shapely
+    >>>
+    >>> with open_arrow(path) as source:
+    >>>     meta, reader = source
+    >>>     for table in reader:
+    >>>         geometries = shapely.from_wkb(table[meta["geometry_name"]])
+
+    Returns
+    -------
+    (dict, pyarrow.RecordBatchStreamReader)
+
+        Returns a tuple of meta information about the data source in a dict,
+        and a pyarrow RecordBatchStreamReader with data.
+
+        Meta is: {
+            "crs": "<crs>",
+            "fields": <ndarray of field names>,
+            "encoding": "<encoding>",
+            "geometry_type": "<geometry_type>",
+            "geometry_name": "<name of geometry column in arrow table>",
+        }
     """
     try:
         import pyarrow  # noqa
     except ImportError:
         raise RuntimeError("the 'pyarrow' package is required to read using arrow")
 
     path, buffer = get_vsi_path(path_or_buffer)
 
+    dataset_kwargs = _preprocess_options_key_value(kwargs) if kwargs else {}
+
     try:
-        result = ogr_read_arrow(
+        return ogr_open_arrow(
             path,
             layer=layer,
             encoding=encoding,
             columns=columns,
             read_geometry=read_geometry,
             force_2d=force_2d,
             skip_features=skip_features,
             max_features=max_features or 0,
             where=where,
             bbox=bbox,
             fids=fids,
             sql=sql,
             sql_dialect=sql_dialect,
             return_fids=return_fids,
+            dataset_kwargs=dataset_kwargs,
+            batch_size=batch_size,
         )
     finally:
         if buffer is not None:
             remove_virtual_file(path)
 
-    return result
-
 
 def detect_driver(path):
     # try to infer driver from path
     parts = os.path.splitext(path)
     if len(parts) != 2:
         raise ValueError(
             f"Could not infer driver from path: {path}; please specify driver "
@@ -259,23 +366,27 @@
 
 
 def write(
     path,
     geometry,
     field_data,
     fields,
+    field_mask=None,
     layer=None,
     driver=None,
     # derived from meta if roundtrip
     geometry_type=None,
     crs=None,
     encoding=None,
     promote_to_multi=None,
     nan_as_null=True,
     append=False,
+    dataset_metadata=None,
+    layer_metadata=None,
+    metadata=None,
     dataset_options=None,
     layer_options=None,
     **kwargs,
 ):
     if geometry_type is None:
         raise ValueError("geometry_type must be provided")
 
@@ -291,14 +402,29 @@
 
     # prevent segfault from: https://github.com/OSGeo/gdal/issues/5739
     if append and driver == "FlatGeobuf" and get_gdal_version() <= (3, 5, 0):
         raise RuntimeError(
             "append to FlatGeobuf is not supported for GDAL <= 3.5.0 due to segfault"
         )
 
+    if metadata is not None:
+        if layer_metadata is not None:
+            raise ValueError("Cannot pass both metadata and layer_metadata")
+        layer_metadata = metadata
+
+    # validate metadata types
+    for metadata in [dataset_metadata, layer_metadata]:
+        if metadata is not None:
+            for k, v in metadata.items():
+                if not isinstance(k, str):
+                    raise ValueError(f"metadata key {k} must be a string")
+
+                if not isinstance(v, str):
+                    raise ValueError(f"metadata value {v} must be a string")
+
     if promote_to_multi is None:
         promote_to_multi = (
             geometry_type.startswith("Multi")
             and driver in DRIVERS_NO_MIXED_SINGLE_MULTI
         )
 
     if crs is None:
@@ -330,16 +456,19 @@
     ogr_write(
         str(path),
         layer=layer,
         driver=driver,
         geometry=geometry,
         geometry_type=geometry_type,
         field_data=field_data,
+        field_mask=field_mask,
         fields=fields,
         crs=crs,
         encoding=encoding,
         promote_to_multi=promote_to_multi,
         nan_as_null=nan_as_null,
         append=append,
+        dataset_metadata=dataset_metadata,
+        layer_metadata=layer_metadata,
         dataset_kwargs=dataset_kwargs,
         layer_kwargs=layer_kwargs,
     )
```

### Comparing `pyogrio-0.5.1/pyogrio/tests/conftest.py` & `pyogrio-0.6.0/pyogrio/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         meta["spatial_index"] = False
         # allow mixed Polygons/MultiPolygons type
         meta["geometry_type"] = "Unknown"
 
     elif ext == ".gpkg":
         # For .gpkg, spatial_index=False to avoid the rows being reordered
         meta["spatial_index"] = False
+        meta["geometry_type"] = "MultiPolygon"
 
     write(dst_path, geometry, field_data, **meta)
     return dst_path
 
 
 @pytest.fixture(scope="session")
 def data_dir():
```

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/README.md` & `pyogrio-0.6.0/pyogrio/tests/fixtures/README.md`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.dbf` & `pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.dbf`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shp` & `pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shp`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shx` & `pyogrio-0.6.0/pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shx`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/test_fgdb.gdb.zip` & `pyogrio-0.6.0/pyogrio/tests/fixtures/test_fgdb.gdb.zip`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/test_gpkg_nulls.gpkg` & `pyogrio-0.6.0/pyogrio/tests/fixtures/test_gpkg_nulls.gpkg`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/test_multisurface.gpkg` & `pyogrio-0.6.0/pyogrio/tests/fixtures/test_multisurface.gpkg`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/fixtures/test_ogr_types_list.geojson` & `pyogrio-0.6.0/pyogrio/tests/fixtures/test_ogr_types_list.geojson`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/test_arrow.py` & `pyogrio-0.6.0/pyogrio/tests/test_arrow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import math
+
 import pytest
 
 from pyogrio import __gdal_version__, read_dataframe
-from pyogrio.raw import read_arrow
+from pyogrio.raw import open_arrow, read_arrow
 
 try:
     import pandas as pd
     from pandas.testing import assert_frame_equal
     from geopandas.testing import assert_geodataframe_equal
 except ImportError:
     pass
@@ -70,7 +72,31 @@
     assert result["list_int64"][0].tolist() == [0, 1]
 
 
 def test_read_arrow_raw(naturalearth_lowres):
     meta, table = read_arrow(naturalearth_lowres)
     assert isinstance(meta, dict)
     assert isinstance(table, pyarrow.Table)
+
+
+def test_open_arrow(naturalearth_lowres):
+    with open_arrow(naturalearth_lowres) as (meta, reader):
+        assert isinstance(meta, dict)
+        assert isinstance(reader, pyarrow.RecordBatchReader)
+        assert isinstance(reader.read_all(), pyarrow.Table)
+
+
+def test_open_arrow_batch_size(naturalearth_lowres):
+    meta, table = read_arrow(naturalearth_lowres)
+    batch_size = math.ceil(len(table) / 2)
+
+    with open_arrow(naturalearth_lowres, batch_size=batch_size) as (meta, reader):
+        assert isinstance(meta, dict)
+        assert isinstance(reader, pyarrow.RecordBatchReader)
+        count = 0
+        tables = []
+        for table in reader:
+            tables.append(table)
+            count += 1
+
+        assert count == 2, "Should be two batches given the batch_size parameter"
+        assert len(tables[0]) == batch_size, "First table should match the batch size"
```

### Comparing `pyogrio-0.5.1/pyogrio/tests/test_core.py` & `pyogrio-0.6.0/pyogrio/tests/test_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     list_layers,
     read_bounds,
     read_info,
     set_gdal_config_options,
     get_gdal_config_option,
     get_gdal_data_path,
 )
+from pyogrio.errors import DataSourceError
 
 from pyogrio._env import GDALEnv
 
 with GDALEnv():
     # NOTE: this must be AFTER above imports, which init the GDAL and PROJ data
     # search paths
     from pyogrio._ogr import ogr_driver_supports_write, has_gdal_data, has_proj_data
@@ -95,29 +96,29 @@
         list_layers(naturalearth_lowres), [["naturalearth_lowres", "Polygon"]]
     )
 
     assert array_equal(
         list_layers(naturalearth_lowres_vsi[1]), [["naturalearth_lowres", "Polygon"]]
     )
 
-    # Measured 3D is downgraded to 2.5D during read
+    # Measured 3D is downgraded to plain 3D during read
     # Make sure this warning is raised
     with pytest.warns(
         UserWarning, match=r"Measured \(M\) geometry types are not supported"
     ):
         fgdb_layers = list_layers(test_fgdb_vsi)
         # GDAL >= 3.4.0 includes 'another_relationship' layer
         assert len(fgdb_layers) >= 7
 
         # Make sure that nonspatial layer has None for geometry
         assert array_equal(fgdb_layers[0], ["basetable_2", None])
 
-        # Confirm that measured 3D is downgraded to 2.5D during read
-        assert array_equal(fgdb_layers[3], ["test_lines", "2.5D MultiLineString"])
-        assert array_equal(fgdb_layers[6], ["test_areas", "2.5D MultiPolygon"])
+        # Confirm that measured 3D is downgraded to plain 3D during read
+        assert array_equal(fgdb_layers[3], ["test_lines", "MultiLineString Z"])
+        assert array_equal(fgdb_layers[6], ["test_areas", "MultiPolygon Z"])
 
 
 def test_read_bounds(naturalearth_lowres):
     fids, bounds = read_bounds(naturalearth_lowres)
     assert fids.shape == (177,)
     assert bounds.shape == (4, 177)
 
@@ -223,14 +224,52 @@
 
     assert meta["crs"] == "EPSG:4326"
     assert meta["geometry_type"] == "Polygon"
     assert meta["encoding"] == "UTF-8"
     assert meta["fields"].shape == (5,)
     assert meta["dtypes"].tolist() == ["int64", "object", "object", "object", "float64"]
     assert meta["features"] == 177
+    assert meta["driver"] == "ESRI Shapefile"
+
+
+@pytest.mark.parametrize(
+    "dataset_kwargs,fields",
+    [
+        ({}, ["top_level", "intermediate_level"]),
+        (
+            {"FLATTEN_NESTED_ATTRIBUTES": "YES"},
+            [
+                "top_level",
+                "intermediate_level_bottom_level",
+            ],
+        ),
+        (
+            {"flatten_nested_attributes": "yes"},
+            [
+                "top_level",
+                "intermediate_level_bottom_level",
+            ],
+        ),
+        (
+            {"flatten_nested_attributes": True},
+            [
+                "top_level",
+                "intermediate_level_bottom_level",
+            ],
+        ),
+    ],
+)
+def test_read_info_dataset_kwargs(data_dir, dataset_kwargs, fields):
+    meta = read_info(data_dir / "test_nested.geojson", **dataset_kwargs)
+    assert meta["fields"].tolist() == fields
+
+
+def test_read_info_invalid_dataset_kwargs(naturalearth_lowres):
+    with pytest.warns(RuntimeWarning, match="does not support open option INVALID"):
+        read_info(naturalearth_lowres, INVALID="YES")
 
 
 @pytest.mark.parametrize(
     "name,value,expected",
     [
         ("CPL_DEBUG", "ON", True),
         ("CPL_DEBUG", True, True),
@@ -246,7 +285,25 @@
 
 def test_reset_config_options():
     set_gdal_config_options({"foo": "bar"})
     assert get_gdal_config_option("foo") == "bar"
 
     set_gdal_config_options({"foo": None})
     assert get_gdal_config_option("foo") is None
+
+
+def test_error_handling(capfd):
+    # an operation that triggers a GDAL Failure
+    # -> error translated into Python exception + not printed to stderr
+    with pytest.raises(DataSourceError, match="No such file or directory"):
+        read_info("non-existent.shp")
+
+    assert capfd.readouterr().err == ""
+
+
+def test_error_handling_warning(capfd, naturalearth_lowres):
+    # an operation that triggers a GDAL Warning
+    # -> translated into a Python warning + not printed to stderr
+    with pytest.warns(RuntimeWarning, match="does not support open option INVALID"):
+        read_info(naturalearth_lowres, INVALID="YES")
+
+    assert capfd.readouterr().err == ""
```

### Comparing `pyogrio-0.5.1/pyogrio/tests/test_geopandas_io.py` & `pyogrio-0.6.0/pyogrio/tests/test_geopandas_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,45 @@
+import contextlib
 from datetime import datetime
 import os
+from packaging.version import Version
 
 import numpy as np
 import pytest
 
 from pyogrio import list_layers, read_info, __gdal_version__, __gdal_geos_version__
 from pyogrio.errors import DataLayerError, DataSourceError, FeatureError, GeometryError
 from pyogrio.geopandas import read_dataframe, write_dataframe
-from pyogrio.raw import DRIVERS, DRIVERS_NO_MIXED_SINGLE_MULTI
+from pyogrio.raw import (
+    DRIVERS,
+    DRIVERS_NO_MIXED_DIMENSIONS,
+    DRIVERS_NO_MIXED_SINGLE_MULTI,
+)
 from pyogrio.tests.conftest import ALL_EXTS
 
 try:
     import pandas as pd
     from pandas.testing import assert_frame_equal, assert_index_equal
 
     import geopandas as gp
+    from geopandas.array import from_wkt
     from geopandas.testing import assert_geodataframe_equal
 
     from shapely.geometry import Point
 except ImportError:
     pass
 
+has_pyarrow = False
+try:
+    import pyarrow  # noqa
+
+    has_pyarrow = True
+except ImportError:
+    pass
+
 
 pytest.importorskip("geopandas")
 
 
 # Note: this will also be false for GDAL < 3.4 when GEOS may be present but we
 # cannot verify it
 has_geos = __gdal_geos_version__ is not None
@@ -113,15 +128,19 @@
     with pytest.raises(DataLayerError, match="Layer 'wrong' could not be opened"):
         read_dataframe(naturalearth_lowres_all_ext, layer="wrong")
 
 
 @pytest.mark.filterwarnings("ignore: Measured")
 def test_read_datetime(test_fgdb_vsi):
     df = read_dataframe(test_fgdb_vsi, layer="test_lines", max_features=1)
-    assert df.SURVEY_DAT.dtype.name == "datetime64[ns]"
+    if Version(pd.__version__) >= Version("2.0.0"):
+        # starting with pandas 2.0, it preserves the passed datetime resolution
+        assert df.SURVEY_DAT.dtype.name == "datetime64[ms]"
+    else:
+        assert df.SURVEY_DAT.dtype.name == "datetime64[ns]"
 
 
 def test_read_null_values(test_fgdb_vsi):
     df = read_dataframe(test_fgdb_vsi, read_geometry=False)
 
     # make sure that Null values are preserved
     assert df.SEGMENT_NAME.isnull().max()
@@ -627,20 +646,29 @@
     geometry_type,
     expected_geometry_types,
     expected_geometry_type,
 ):
     input_gdf = read_dataframe(naturalearth_lowres)
 
     output_path = tmp_path / f"test_promote_layer_geom_type{ext}"
-    write_dataframe(
-        input_gdf,
-        output_path,
-        promote_to_multi=promote_to_multi,
-        geometry_type=geometry_type,
-    )
+
+    if ext == ".gpkg" and geometry_type in ("Polygon", "Point"):
+        ctx = pytest.warns(
+            RuntimeWarning, match="A geometry of type MULTIPOLYGON is inserted"
+        )
+    else:
+        ctx = contextlib.nullcontext()
+
+    with ctx:
+        write_dataframe(
+            input_gdf,
+            output_path,
+            promote_to_multi=promote_to_multi,
+            geometry_type=geometry_type,
+        )
 
     assert output_path.exists()
     output_gdf = read_dataframe(output_path)
     geometry_types = sorted(output_gdf.geometry.type.unique())
     assert geometry_types == expected_geometry_types
     assert read_info(output_path)["geometry_type"] == expected_geometry_type
 
@@ -839,23 +867,245 @@
         (
             "GeometryCollection Z (Point Z (0 0 0))",
             ["2.5D GeometryCollection", "GeometryCollection Z"],
         ),
     ],
 )
 def test_write_geometry_z_types(tmp_path, wkt, geom_types):
-    from geopandas.array import from_wkt
-
     filename = tmp_path / "test.fgb"
-
     gdf = gp.GeoDataFrame(geometry=from_wkt([wkt]), crs="EPSG:4326")
     for geom_type in geom_types:
         write_dataframe(gdf, filename, geometry_type=geom_type)
         df = read_dataframe(filename)
         assert_geodataframe_equal(df, gdf)
 
 
+@pytest.mark.parametrize("ext", ALL_EXTS)
+@pytest.mark.parametrize(
+    "test_descr, exp_geometry_type, mixed_dimensions, wkt",
+    [
+        ("1 Point Z", "Point Z", False, ["Point Z (0 0 0)"]),
+        ("1 LineString Z", "LineString Z", False, ["LineString Z (0 0 0, 1 1 0)"]),
+        (
+            "1 Polygon Z",
+            "Polygon Z",
+            False,
+            ["Polygon Z ((0 0 0, 0 1 0, 1 1 0, 0 0 0))"],
+        ),
+        ("1 MultiPoint Z", "MultiPoint Z", False, ["MultiPoint Z (0 0 0, 1 1 0)"]),
+        (
+            "1 MultiLineString Z",
+            "MultiLineString Z",
+            False,
+            ["MultiLineString Z ((0 0 0, 1 1 0), (2 2 2, 3 3 2))"],
+        ),
+        (
+            "1 MultiLinePolygon Z",
+            "MultiPolygon Z",
+            False,
+            [
+                "MultiPolygon Z (((0 0 0, 0 1 0, 1 1 0, 0 0 0)), ((1 1 1, 1 2 1, 2 2 1, 1 1 1)))"  # noqa: E501
+            ],
+        ),
+        (
+            "1 GeometryCollection Z",
+            "GeometryCollection Z",
+            False,
+            ["GeometryCollection Z (Point Z (0 0 0))"],
+        ),
+        ("Point Z + Point", "Point Z", True, ["Point Z (0 0 0)", "Point (0 0)"]),
+        ("Point Z + None", "Point Z", False, ["Point Z (0 0 0)", None]),
+        (
+            "Point Z + LineString Z",
+            "Unknown",
+            False,
+            ["LineString Z (0 0 0, 1 1 0)", "Point Z (0 0 0)"],
+        ),
+        (
+            "Point Z + LineString",
+            "Unknown",
+            True,
+            ["LineString (0 0, 1 1)", "Point Z (0 0 0)"],
+        ),
+    ],
+)
+def test_write_geometry_z_types_auto(
+    tmp_path, ext, test_descr, exp_geometry_type, mixed_dimensions, wkt
+):
+    # Shapefile has some different behaviour that other file types
+    if ext == ".shp":
+        if exp_geometry_type in ("GeometryCollection Z", "Unknown"):
+            pytest.skip(f"ext {ext} doesn't support {exp_geometry_type}")
+        elif exp_geometry_type == "MultiLineString Z":
+            exp_geometry_type = "LineString Z"
+        elif exp_geometry_type == "MultiPolygon Z":
+            exp_geometry_type = "Polygon Z"
+
+    column_data = {}
+    column_data["test_descr"] = [test_descr] * len(wkt)
+    column_data["idx"] = [str(idx) for idx in range(len(wkt))]
+    gdf = gp.GeoDataFrame(column_data, geometry=from_wkt(wkt), crs="EPSG:4326")
+    filename = tmp_path / f"test{ext}"
+
+    if ext == ".fgb":
+        # writing empty / null geometries not allowed by FlatGeobuf for
+        # GDAL >= 3.6.4 and were simply not written previously
+        gdf = gdf.loc[~(gdf.geometry.isna() | gdf.geometry.is_empty)]
+
+    if mixed_dimensions and DRIVERS[ext] in DRIVERS_NO_MIXED_DIMENSIONS:
+        with pytest.raises(
+            DataSourceError,
+            match=("Mixed 2D and 3D coordinates are not supported by"),
+        ):
+            write_dataframe(gdf, filename)
+        return
+    else:
+        write_dataframe(gdf, filename)
+
+    info = read_info(filename)
+    assert info["geometry_type"] == exp_geometry_type
+
+    result_gdf = read_dataframe(filename)
+    if ext == ".geojsonl":
+        result_gdf.crs = "EPSG:4326"
+
+    assert_geodataframe_equal(gdf, result_gdf)
+
+
 def test_read_multisurface(data_dir):
     df = read_dataframe(data_dir / "test_multisurface.gpkg")
 
     # MultiSurface should be converted to MultiPolygon
     assert df.geometry.type.tolist() == ["MultiPolygon"]
+
+
+@pytest.mark.parametrize(
+    "use_arrow",
+    [
+        False,
+        pytest.param(
+            True,
+            marks=pytest.mark.skipif(
+                not has_pyarrow or __gdal_version__ < (3, 6, 0),
+                reason="Arrow tests require pyarrow and GDAL>=3.6",
+            ),
+        ),
+    ],
+)
+def test_read_dataset_kwargs(data_dir, use_arrow):
+    filename = data_dir / "test_nested.geojson"
+
+    # by default, nested data are not flattened
+    df = read_dataframe(filename, use_arrow=use_arrow)
+
+    expected = gp.GeoDataFrame(
+        {
+            "top_level": ["A"],
+            "intermediate_level": ['{ "bottom_level": "B" }'],
+        },
+        geometry=[Point(0, 0)],
+        crs="EPSG:4326",
+    )
+
+    assert_geodataframe_equal(df, expected)
+
+    df = read_dataframe(filename, use_arrow=use_arrow, FLATTEN_NESTED_ATTRIBUTES="YES")
+
+    expected = gp.GeoDataFrame(
+        {
+            "top_level": ["A"],
+            "intermediate_level_bottom_level": ["B"],
+        },
+        geometry=[Point(0, 0)],
+        crs="EPSG:4326",
+    )
+
+    assert_geodataframe_equal(df, expected)
+
+
+@pytest.mark.parametrize(
+    "use_arrow",
+    [
+        False,
+        pytest.param(
+            True,
+            marks=pytest.mark.skipif(
+                not has_pyarrow or __gdal_version__ < (3, 6, 0),
+                reason="Arrow tests require pyarrow and GDAL>=3.6",
+            ),
+        ),
+    ],
+)
+def test_read_invalid_dataset_kwargs(naturalearth_lowres, use_arrow):
+    with pytest.warns(RuntimeWarning, match="does not support open option INVALID"):
+        read_dataframe(naturalearth_lowres, use_arrow=use_arrow, INVALID="YES")
+
+
+def test_write_nullable_dtypes(tmp_path):
+    path = tmp_path / "test_nullable_dtypes.gpkg"
+    test_data = {
+        "col1": pd.Series([1, 2, 3], dtype="int64"),
+        "col2": pd.Series([1, 2, None], dtype="Int64"),
+        "col3": pd.Series([0.1, None, 0.3], dtype="Float32"),
+        "col4": pd.Series([True, False, None], dtype="boolean"),
+        "col5": pd.Series(["a", None, "b"], dtype="string"),
+    }
+    input_gdf = gp.GeoDataFrame(test_data, geometry=[Point(0, 0)] * 3, crs="epsg:31370")
+    write_dataframe(input_gdf, path)
+    output_gdf = read_dataframe(path)
+    # We read it back as default (non-nullable) numpy dtypes, so we cast
+    # to those for the expected result
+    expected = input_gdf.copy()
+    expected["col2"] = expected["col2"].astype("float64")
+    expected["col3"] = expected["col3"].astype("float32")
+    expected["col4"] = expected["col4"].astype("float64")
+    expected["col5"] = expected["col5"].astype(object)
+    assert_geodataframe_equal(output_gdf, expected)
+
+
+@pytest.mark.parametrize(
+    "metadata_type", ["dataset_metadata", "layer_metadata", "metadata"]
+)
+def test_metadata_io(tmpdir, naturalearth_lowres, metadata_type):
+    metadata = {"level": metadata_type}
+
+    df = read_dataframe(naturalearth_lowres)
+
+    filename = os.path.join(str(tmpdir), "test.gpkg")
+    write_dataframe(df, filename, **{metadata_type: metadata})
+
+    metadata_key = "layer_metadata" if metadata_type == "metadata" else metadata_type
+
+    assert read_info(filename)[metadata_key] == metadata
+
+
+@pytest.mark.parametrize("metadata_type", ["dataset_metadata", "layer_metadata"])
+@pytest.mark.parametrize(
+    "metadata",
+    [
+        {1: 2},
+        {"key": None},
+        {"key": 1},
+    ],
+)
+def test_invalid_metadata(tmpdir, naturalearth_lowres, metadata_type, metadata):
+    with pytest.raises(ValueError, match="must be a string"):
+        filename = os.path.join(str(tmpdir), "test.gpkg")
+        write_dataframe(
+            read_dataframe(naturalearth_lowres), filename, **{metadata_type: metadata}
+        )
+
+
+@pytest.mark.parametrize("metadata_type", ["dataset_metadata", "layer_metadata"])
+def test_metadata_unsupported(tmpdir, naturalearth_lowres, metadata_type):
+    """metadata is silently ignored"""
+
+    filename = os.path.join(str(tmpdir), "test.geojson")
+    write_dataframe(
+        read_dataframe(naturalearth_lowres),
+        filename,
+        **{metadata_type: {"key": "value"}},
+    )
+
+    metadata_key = "layer_metadata" if metadata_type == "metadata" else metadata_type
+
+    assert read_info(filename)[metadata_key] is None
```

### Comparing `pyogrio-0.5.1/pyogrio/tests/test_path.py` & `pyogrio-0.6.0/pyogrio/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/tests/test_raw_io.py` & `pyogrio-0.6.0/pyogrio/tests/test_raw_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import json
 import os
 import sys
 
 import numpy as np
 from numpy import array_equal
 import pytest
@@ -266,14 +267,15 @@
     assert os.path.exists(filename)
     for ext in (".dbf", ".prj"):
         assert os.path.exists(filename.replace(".shp", ext))
 
 
 def test_write_gpkg(tmpdir, naturalearth_lowres):
     meta, _, geometry, field_data = read(naturalearth_lowres)
+    meta.update({"geometry_type": "MultiPolygon"})
 
     filename = os.path.join(str(tmpdir), "test.gpkg")
     write(filename, geometry, field_data, driver="GPKG", **meta)
 
     assert os.path.exists(filename)
 
 
@@ -452,17 +454,19 @@
             pytest.skip("Test requires pygeos or shapely>=2")
     assert equals_exact(
         from_wkb(geometry1), from_wkb(geometry2), tolerance=0.00001
     ).all()
     assert all([np.array_equal(f1, f2) for f1, f2 in zip(field_data1, field_data2)])
 
 
+@pytest.mark.filterwarnings("ignore:File /vsimem:RuntimeWarning")  # TODO
 @pytest.mark.parametrize("driver,ext", [("GeoJSON", "geojson"), ("GPKG", "gpkg")])
 def test_read_from_bytes(tmpdir, naturalearth_lowres, driver, ext):
     meta, index, geometry, field_data = read(naturalearth_lowres)
+    meta.update({"geometry_type": "Unknown"})
     filename = os.path.join(str(tmpdir), f"test.{ext}")
     write(filename, geometry, field_data, driver=driver, **meta)
 
     with open(filename, "rb") as f:
         buffer = f.read()
 
     result2 = read(buffer)
@@ -476,17 +480,19 @@
     with open(path, "rb") as f:
         buffer = f.read()
 
     result2 = read(buffer)
     assert_equal_result((meta, index, geometry, field_data), result2)
 
 
+@pytest.mark.filterwarnings("ignore:File /vsimem:RuntimeWarning")  # TODO
 @pytest.mark.parametrize("driver,ext", [("GeoJSON", "geojson"), ("GPKG", "gpkg")])
 def test_read_from_file_like(tmpdir, naturalearth_lowres, driver, ext):
     meta, index, geometry, field_data = read(naturalearth_lowres)
+    meta.update({"geometry_type": "Unknown"})
     filename = os.path.join(str(tmpdir), f"test.{ext}")
     write(filename, geometry, field_data, driver=driver, **meta)
 
     with open(filename, "rb") as f:
         result2 = read(f)
 
     assert_equal_result((meta, index, geometry, field_data), result2)
@@ -643,15 +649,20 @@
     write(fname, geometry, field_data, fields, **meta)
     with open(str(fname), "r") as f:
         content = f.read()
     assert '{ "col": null }' in content
 
     # set to False
     # by default, GDAL will skip the property for GeoJSON if the value is NaN
-    write(fname, geometry, field_data, fields, **meta, nan_as_null=False)
+    if dtype == "float32":
+        ctx = pytest.warns(RuntimeWarning, match="NaN of Infinity value found. Skipped")
+    else:
+        ctx = contextlib.nullcontext()
+    with ctx:
+        write(fname, geometry, field_data, fields, **meta, nan_as_null=False)
     with open(str(fname), "r") as f:
         content = f.read()
     assert '"properties": { }' in content
 
     # but can instruct GDAL to write NaN to json
     write(
         fname,
@@ -802,7 +813,35 @@
         os.unlink(str(filename).replace(".shp", ".cpg"))
         actual_meta, _, _, actual_field_data = read(filename, encoding=read_encoding)
         assert np.array_equal(fields, actual_meta["fields"])
         assert np.array_equal(field_data, actual_field_data)
         assert np.array_equal(
             fields, read_info(filename, encoding=read_encoding)["fields"]
         )
+
+
+def test_write_with_mask(tmp_path):
+    # Point(0, 0), null
+    geometry = np.array(
+        [bytes.fromhex("010100000000000000000000000000000000000000")] * 3,
+        dtype=object,
+    )
+    field_data = [np.array([1, 2, 3], dtype="int32")]
+    field_mask = [np.array([False, True, False])]
+    fields = ["col"]
+    meta = dict(geometry_type="Point", crs="EPSG:4326")
+
+    filename = tmp_path / "test.geojson"
+    write(filename, geometry, field_data, fields, field_mask, **meta)
+    result_geometry, result_fields = read(filename)[2:]
+    assert np.array_equal(result_geometry, geometry)
+    np.testing.assert_allclose(result_fields[0], np.array([1, np.nan, 3]))
+
+    # wrong length for mask
+    field_mask = [np.array([False, True])]
+    with pytest.raises(ValueError):
+        write(filename, geometry, field_data, fields, field_mask, **meta)
+
+    # wrong number of mask arrays
+    field_mask = [np.array([False, True, False])] * 2
+    with pytest.raises(ValueError):
+        write(filename, geometry, field_data, fields, field_mask, **meta)
```

### Comparing `pyogrio-0.5.1/pyogrio/tests/win32.py` & `pyogrio-0.6.0/pyogrio/tests/win32.py`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio/util.py` & `pyogrio-0.6.0/pyogrio/util.py`

 * *Files identical despite different names*

### Comparing `pyogrio-0.5.1/pyogrio.egg-info/PKG-INFO` & `pyogrio-0.6.0/pyogrio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyogrio
-Version: 0.5.1
+Version: 0.6.0
 Summary: Vectorized spatial vector file format I/O using GDAL/OGR
-Home-page: https://github.com/pyogrio/pyogrio
+Home-page: https://github.com/geopandas/pyogrio
 Author: Brendan C. Ward
 Author-email: bcward@astutespruce.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `pyogrio-0.5.1/pyogrio.egg-info/SOURCES.txt` & `pyogrio-0.6.0/pyogrio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,13 +35,14 @@
 pyogrio/tests/test_raw_io.py
 pyogrio/tests/win32.py
 pyogrio/tests/fixtures/README.md
 pyogrio/tests/fixtures/test_datetime.geojson
 pyogrio/tests/fixtures/test_fgdb.gdb.zip
 pyogrio/tests/fixtures/test_gpkg_nulls.gpkg
 pyogrio/tests/fixtures/test_multisurface.gpkg
+pyogrio/tests/fixtures/test_nested.geojson
 pyogrio/tests/fixtures/test_ogr_types_list.geojson
 pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.cpg
 pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.dbf
 pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.prj
 pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shp
 pyogrio/tests/fixtures/naturalearth_lowres/naturalearth_lowres.shx
```

### Comparing `pyogrio-0.5.1/pyproject.toml` & `pyogrio-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -10,49 +10,50 @@
     "tomli; python_version < '3.11'",
 ]
 
 [tool.cibuildwheel]
 skip = ["cp36-*", "cp37-*", "pp*", "*musllinux*"]
 archs = ["auto64"]
 manylinux-x86_64-image = "manylinux-vcpkg-gdal:latest"
+manylinux-aarch64-image = "manylinux-aarch64-vcpkg-gdal:latest"
 build-verbosity = 3
 
 [tool.cibuildwheel.linux.environment]
-VCPKG_INSTALL = "$VCPKG_INSTALLATION_ROOT/installed/x64-linux-dynamic"
+VCPKG_INSTALL = "$VCPKG_INSTALLATION_ROOT/installed/$VCPKG_DEFAULT_TRIPLET"
 GDAL_INCLUDE_PATH = "$VCPKG_INSTALL/include"
 GDAL_LIBRARY_PATH = "$VCPKG_INSTALL/lib"
-GDAL_VERSION = "3.6.2"
+GDAL_VERSION = "3.6.4"
 PYOGRIO_PACKAGE_DATA = 1
 GDAL_DATA = "$VCPKG_INSTALL/share/gdal"
 PROJ_LIB = "$VCPKG_INSTALL/share/proj"
 
 [tool.cibuildwheel.macos]
 repair-wheel-command = [
     "DYLD_LIBRARY_PATH=$GDAL_LIBRARY_PATH delocate-listdeps {wheel}",
     "DYLD_LIBRARY_PATH=$GDAL_LIBRARY_PATH delocate-wheel --require-archs {delocate_archs} -w {dest_dir} {wheel}",
 ]
 
 [tool.cibuildwheel.macos.environment]
 VCPKG_INSTALL = "$VCPKG_INSTALLATION_ROOT/installed/$VCPKG_DEFAULT_TRIPLET"
 GDAL_INCLUDE_PATH = "$VCPKG_INSTALL/include"
 GDAL_LIBRARY_PATH = "$VCPKG_INSTALL/lib"
-GDAL_VERSION = "3.6.2"
+GDAL_VERSION = "3.6.4"
 PYOGRIO_PACKAGE_DATA = 1
 GDAL_DATA = "$VCPKG_INSTALL/share/gdal"
 PROJ_LIB = "$VCPKG_INSTALL/share/proj"
 
 [tool.cibuildwheel.windows]
 before-build = "pip install delvewheel"
 repair-wheel-command = "delvewheel repair --add-path C:/vcpkg/installed/x64-windows-dynamic-release/bin -w {dest_dir} {wheel}"
 
 [tool.cibuildwheel.windows.environment]
 VCPKG_INSTALL = "$VCPKG_INSTALLATION_ROOT/installed/x64-windows-dynamic-release"
 GDAL_INCLUDE_PATH = "$VCPKG_INSTALL/include"
 GDAL_LIBRARY_PATH = "$VCPKG_INSTALL/lib"
-GDAL_VERSION = "3.6.2"
+GDAL_VERSION = "3.6.4"
 PYOGRIO_PACKAGE_DATA = 1
 GDAL_DATA = "$VCPKG_INSTALL/share/gdal"
 PROJ_LIB = "$VCPKG_INSTALL/share/proj"
 
 [tool.versioneer]
 VCS = "git"
 style = "pep440"
```

### Comparing `pyogrio-0.5.1/setup.py` & `pyogrio-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 cmdclass = versioneer.get_cmdclass()
 cmdclass["build_ext"] = build_ext
 
 setup(
     name="pyogrio",
     version=version,
     packages=find_packages(),
-    url="https://github.com/pyogrio/pyogrio",
+    url="https://github.com/geopandas/pyogrio",
     license="MIT",
     author="Brendan C. Ward",
     author_email="bcward@astutespruce.com",
     description="Vectorized spatial vector file format I/O using GDAL/OGR",
     long_description_content_type="text/markdown",
     long_description=open("README.md").read(),
     python_requires=">=3.8",
```

