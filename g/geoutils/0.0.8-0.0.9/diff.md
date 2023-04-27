# Comparing `tmp/geoutils-0.0.8.tar.gz` & `tmp/geoutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoutils-0.0.8.tar", last modified: Thu Aug 25 08:53:24 2022, max compression
+gzip compressed data, was "geoutils-0.0.9.tar", last modified: Mon Sep 26 08:51:43 2022, max compression
```

## Comparing `geoutils-0.0.8.tar` & `geoutils-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 08:53:24.732800 geoutils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-08-25 08:53:17.000000 geoutils-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3208 2022-08-25 08:53:24.732800 geoutils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-08-25 08:53:17.000000 geoutils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 08:53:24.728799 geoutils-0.0.8/geoutils/
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 08:53:24.732800 geoutils-0.0.8/geoutils/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)   490752 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/datasets/LE71400412000304SGS00_B4_crop.TIF
--rw-r--r--   0 runner    (1001) docker     (121)   127240 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/datasets/LE71400412000304SGS00_B4_crop2.TIF
--rw-r--r--   0 runner    (1001) docker     (121)  1573698 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/datasets/LE71400412000304SGS00_RGB.TIF
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   413696 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/datasets/glacier_outlines.gpkg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 08:53:24.732800 geoutils-0.0.8/geoutils/georaster/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/georaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    84824 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/georaster/raster.py
--rw-r--r--   0 runner    (1001) docker     (121)    21429 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/geovector.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7167 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/geoviewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6530 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6560 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/projtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    13869 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/satimg.py
--rw-r--r--   0 runner    (1001) docker     (121)    18617 2022-08-25 08:53:17.000000 geoutils-0.0.8/geoutils/spatial_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-25 08:53:24.000000 geoutils-0.0.8/geoutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 08:53:24.728799 geoutils-0.0.8/geoutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3208 2022-08-25 08:53:24.000000 geoutils-0.0.8/geoutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-08-25 08:53:24.000000 geoutils-0.0.8/geoutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 08:53:24.000000 geoutils-0.0.8/geoutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 08:53:24.000000 geoutils-0.0.8/geoutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-08-25 08:53:24.000000 geoutils-0.0.8/geoutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-25 08:53:24.000000 geoutils-0.0.8/geoutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-25 08:53:17.000000 geoutils-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-25 08:53:24.732800 geoutils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-08-25 08:53:17.000000 geoutils-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 08:51:43.084403 geoutils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-26 08:51:29.000000 geoutils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-09-26 08:51:43.084403 geoutils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2933 2022-09-26 08:51:29.000000 geoutils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 08:51:43.084403 geoutils-0.0.9/geoutils/
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3428 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 08:51:43.084403 geoutils-0.0.9/geoutils/georaster/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/georaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   103214 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/georaster/raster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21433 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/geovector.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7170 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/geoviewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7942 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/projtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13746 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/satimg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22556 2022-09-26 08:51:29.000000 geoutils-0.0.9/geoutils/spatial_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-26 08:51:42.000000 geoutils-0.0.9/geoutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 08:51:43.084403 geoutils-0.0.9/geoutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-09-26 08:51:42.000000 geoutils-0.0.9/geoutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-09-26 08:51:43.000000 geoutils-0.0.9/geoutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 08:51:42.000000 geoutils-0.0.9/geoutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 08:51:42.000000 geoutils-0.0.9/geoutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-26 08:51:42.000000 geoutils-0.0.9/geoutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-26 08:51:42.000000 geoutils-0.0.9/geoutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-26 08:51:29.000000 geoutils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-26 08:51:43.084403 geoutils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-09-26 08:51:29.000000 geoutils-0.0.9/setup.py
```

### Comparing `geoutils-0.0.8/LICENSE` & `geoutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geoutils-0.0.8/PKG-INFO` & `geoutils-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: geoutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for working with geospatial data
 Home-page: https://www.github.com/GlacioHack/geoutils/
 Author: The GlacioHack Team
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rioxarray
 License-File: LICENSE
 
-# GeoUtils
+# geoutils
 Set of tools to handle raster and vector data sets in Python.
 
 ![](https://readthedocs.org/projects/geoutils/badge/?version=latest)
-[![build](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml/badge.svg)](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml)
+[![build](https://github.com/GlacioHack/geoutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![PyPI version](https://badge.fury.io/py/geoutils.svg)](https://badge.fury.io/py/geoutils)
+[![Coverage Status](https://coveralls.io/repos/github/GlacioHack/geoutils/badge.svg?branch=main)](https://coveralls.io/github/GlacioHack/geoutils?branch=main)
 
 This package offers Python classes and functions as well as command line tools to work with both geospatial raster and vector datasets. It is built upon rasterio and GeoPandas. In a single command it can import any geo-referenced dataset that is understood by these libraries, complete with all geo-referencing information, various helper functions and interface between vector/raster data.
 
 
 ## Installation
 
 #### With conda (recommended)
@@ -38,32 +40,32 @@
 From PyPI:
 ```bash
 pip install geoutils
 ```
 
 Or from the repository tarball: make sure GDAL and PROJ are properly installed, then:
 ```bash
-pip install https://github.com/GlacioHack/GeoUtils/tarball/main
+pip install https://github.com/GlacioHack/geoutils/tarball/main
 ```
 
 ## Documentation
 See the full documentation at https://geoutils.readthedocs.io.
 
 
 ## Structure
 
-GeoUtils are composed of three libraries:
+GeoUtils is composed of three libraries:
 - `georaster.py` to handle raster data set. In particular, a Raster class to load a raster file along with metadata.
 - `geovector.py` to handle vector data set. In particular, a Vector class to load a raster file along with metadata.
 - `projtools.py` with various tools around projections.
 
 
 ## How to contribute
 
-You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/GeoUtils/issues) section. All contributions are welcome.
+You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/geoutils/issues) section. All contributions are welcome.
 
 1. Fork the repository to your personal GitHub account, clone to your computer.
 2. (Optional but preferred:) Make a feature branch.
 3. Push to your feature branch.
 4. When ready, submit a Pull Request from your feature branch to `GlacioHack/geoutils:master`.
 5. The PR will be reviewed by at least one other person. Usually your PR will be merged via 'squash and merge'.
```

### Comparing `geoutils-0.0.8/README.md` & `geoutils-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# GeoUtils
+# geoutils
 Set of tools to handle raster and vector data sets in Python.
 
 ![](https://readthedocs.org/projects/geoutils/badge/?version=latest)
-[![build](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml/badge.svg)](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml)
+[![build](https://github.com/GlacioHack/geoutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![PyPI version](https://badge.fury.io/py/geoutils.svg)](https://badge.fury.io/py/geoutils)
+[![Coverage Status](https://coveralls.io/repos/github/GlacioHack/geoutils/badge.svg?branch=main)](https://coveralls.io/github/GlacioHack/geoutils?branch=main)
 
 This package offers Python classes and functions as well as command line tools to work with both geospatial raster and vector datasets. It is built upon rasterio and GeoPandas. In a single command it can import any geo-referenced dataset that is understood by these libraries, complete with all geo-referencing information, various helper functions and interface between vector/raster data.
 
 
 ## Installation
 
 #### With conda (recommended)
@@ -24,32 +25,32 @@
 From PyPI:
 ```bash
 pip install geoutils
 ```
 
 Or from the repository tarball: make sure GDAL and PROJ are properly installed, then:
 ```bash
-pip install https://github.com/GlacioHack/GeoUtils/tarball/main
+pip install https://github.com/GlacioHack/geoutils/tarball/main
 ```
 
 ## Documentation
 See the full documentation at https://geoutils.readthedocs.io.
 
 
 ## Structure
 
-GeoUtils are composed of three libraries:
+GeoUtils is composed of three libraries:
 - `georaster.py` to handle raster data set. In particular, a Raster class to load a raster file along with metadata.
 - `geovector.py` to handle vector data set. In particular, a Vector class to load a raster file along with metadata.
 - `projtools.py` with various tools around projections.
 
 
 ## How to contribute
 
-You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/GeoUtils/issues) section. All contributions are welcome.
+You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/geoutils/issues) section. All contributions are welcome.
 
 1. Fork the repository to your personal GitHub account, clone to your computer.
 2. (Optional but preferred:) Make a feature branch.
 3. Push to your feature branch.
 4. When ready, submit a Pull Request from your feature branch to `GlacioHack/geoutils:master`.
 5. The PR will be reviewed by at least one other person. Usually your PR will be merged via 'squash and merge'.
```

### Comparing `geoutils-0.0.8/geoutils/__init__.py` & `geoutils-0.0.9/geoutils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 GeoUtils is a python package of raster and vector tools.
 """
 
 from geoutils import spatial_tools  # noqa
-from geoutils import datasets, georaster, geovector, projtools, satimg  # noqa
+from geoutils import examples, georaster, geovector, projtools, satimg  # noqa
 from geoutils.georaster import Raster  # noqa
 from geoutils.geovector import Vector  # noqa
 from geoutils.satimg import SatelliteImage  # noqa
 
 try:
     from geoutils.version import version as __version__  # noqa
 except ImportError:  # pragma: no cover
```

### Comparing `geoutils-0.0.8/geoutils/georaster/raster.py` & `geoutils-0.0.9/geoutils/georaster/raster.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 geoutils.georaster provides a toolset for working with raster data.
 """
 from __future__ import annotations
 
-import copy
 import os
 import warnings
 from collections import abc
+from collections.abc import Iterable
+from contextlib import ExitStack
 from numbers import Number
 from typing import IO, Any, Callable, TypeVar, overload
 
 import geopandas as gpd
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
@@ -20,19 +21,17 @@
 import rasterio.transform
 import rasterio.warp
 import rasterio.windows
 from affine import Affine
 from matplotlib import cm, colors
 from rasterio.crs import CRS
 from rasterio.features import shapes
-from rasterio.io import MemoryFile
 from rasterio.plot import show as rshow
 from rasterio.warp import Resampling
 from scipy.ndimage import map_coordinates
-from shapely.geometry.polygon import Polygon
 
 import geoutils.geovector as gv
 from geoutils._typing import AnyNumber, ArrayLike, DTypeLike
 from geoutils.geovector import Vector
 
 # If python38 or above, Literal is builtin. Otherwise, use typing_extensions
 try:
@@ -45,81 +44,185 @@
 except ImportError:
     _has_rioxarray = False
 else:
     _has_rioxarray = True
 
 RasterType = TypeVar("RasterType", bound="Raster")
 
+# List of numpy functions that are handled: nan statistics function, normal statistics function and sorting/counting
+_HANDLED_FUNCTIONS = (
+    [
+        "nansum",
+        "nanmax",
+        "nanmin",
+        "nanargmax",
+        "nanargmin",
+        "nanmean",
+        "nanmedian",
+        "nanpercentile",
+        "nanvar",
+        "nanstd",
+        "nanprod",
+        "nancumsum",
+        "nancumprod",
+        "nanquantile",
+    ]
+    + [
+        "sum",
+        "amax",
+        "amin",
+        "argmax",
+        "argmin",
+        "mean",
+        "median",
+        "percentile",
+        "var",
+        "std",
+        "prod",
+        "cumsum",
+        "cumprod",
+        "quantile",
+    ]
+    + ["sort", "count_nonzero", "unique"]
+)
+
 
 # Function to set the default nodata values for any given dtype
 # Similar to GDAL for int types, but without absurdly long nodata values for floats.
 # For unsigned types, the maximum value is chosen (with a max of 99999).
 # For signed types, the minimum value is chosen (with a min of -99999).
-def _default_ndv(dtype: str | np.dtype | type) -> int:
+def _default_nodata(dtype: str | np.dtype | type) -> int:
     """
     Set the default nodata value for any given dtype, when this is not provided.
     """
-    default_ndv_lookup = {
+    default_nodata_lookup = {
         "uint8": 255,
         "int8": -128,
         "uint16": 65535,
         "int16": -32768,
         "uint32": 99999,
         "int32": -99999,
+        "float16": -99999,
         "float32": -99999,
         "float64": -99999,
         "float128": -99999,
+        "longdouble": -99999,  # This is float64 on Windows, float128 on other systems, for compatibility
     }
     # Check argument dtype is as expected
     if not isinstance(dtype, (str, np.dtype, type)):
         raise ValueError(f"dtype {dtype} not understood")
 
     # Convert numpy types to string
     if isinstance(dtype, type):
         dtype = np.dtype(dtype).name
 
     # Convert np.dtype to string
     if isinstance(dtype, np.dtype):
         dtype = dtype.name
 
-    if dtype in default_ndv_lookup.keys():
-        return default_ndv_lookup[dtype]
+    if dtype in default_nodata_lookup.keys():
+        return default_nodata_lookup[dtype]
     else:
         raise NotImplementedError(f"No default nodata value set for dtype {dtype}")
 
 
+# Set default attributes to be kept from rasterio's DatasetReader
+_default_rio_attrs = [
+    "bounds",
+    "count",
+    "crs",
+    "driver",
+    "dtypes",
+    "height",
+    "indexes",
+    "name",
+    "nodata",
+    "res",
+    "shape",
+    "transform",
+    "width",
+]
+
+
+def _load_rio(
+    dataset: rio.io.DatasetReader,
+    bands: int | list[int] | None = None,
+    masked: bool = False,
+    transform: Affine | None = None,
+    shape: tuple[int, int] | None = None,
+    **kwargs: Any,
+) -> np.ma.masked_array:
+    r"""
+    Load specific bands of the dataset, using rasterio.read().
+
+    Ensure that self.data.ndim = 3 for ease of use (needed e.g. in show)
+
+    :param dataset: The dataset to read (opened with "rio.open(filename)")
+    :param bands: The band(s) to load. Note that rasterio begins counting at 1, not 0.
+    :param masked: Should the mask be read (if any exists), and/or should the nodata be used to mask values
+    :param transform: Create a window from the given transform (to read only parts of the raster)
+    :param shape: The expected shape of the read ndarray. Must be given together with the 'transform' argument.
+
+    :raises ValueError: If only one of 'transform' and 'shape' are given.
+
+    :returns: A numpy array if masked == False or a masked_array
+
+    \*\*kwargs: any additional arguments to rasterio.io.DatasetReader.read.
+    Useful ones are:
+    .. hlist::
+    * out_shape : to load a subsampled version
+    * window : to load a cropped version
+    * resampling : to set the resampling algorithm
+    """
+    if transform is not None and shape is not None:
+        if transform == dataset.transform:
+            row_off, col_off = 0, 0
+        else:
+            row_off, col_off = (round(val) for val in dataset.index(transform[2], abs(transform[4])))
+
+        window = rio.windows.Window(col_off, row_off, *shape[::-1])
+    elif sum(param is None for param in [shape, transform]) == 1:
+        raise ValueError("If 'shape' or 'transform' is provided, BOTH must be given.")
+    else:
+        window = None
+
+    if bands is None:
+        data = dataset.read(masked=masked, window=window, **kwargs)
+    else:
+        data = dataset.read(bands, masked=masked, window=window, **kwargs)
+    if len(data.shape) == 2:
+        data = data[np.newaxis, :, :]
+    return np.ma.masked_array(data)
+
+
 class Raster:
     """
     Create a Raster object from a rasterio-supported raster dataset.
 
     If not otherwise specified below, attribute types and contents correspond
     to the attributes defined by rasterio.
 
     Attributes:
-        filename : str
+        filename_or_dataset : str
             The path/filename of the loaded, file, only set if a disk-based file is read in.
         data : np.array
             Loaded image. Dimensions correspond to (bands, height, width).
         nbands : int
             Number of bands loaded into .data
         bands : tuple
             The indexes of the opened dataset which correspond to the bands loaded into data.
         is_loaded : bool
             True if the image data have been loaded into this Raster.
-        ds : rio.io.DatasetReader
-            Link to underlying DatasetReader object.
 
         bounds
 
         count
 
         crs
 
-        dataset_mask
-
         driver
 
         dtypes
 
         height
 
         indexes
@@ -133,48 +236,23 @@
         shape
 
         transform
 
         width
     """
 
-    # This only gets set if a disk-based file is read in.
-    # If the Raster is created with from_array, from_mem etc, this stays as None.
-    filename = None
-    _is_modified: bool | None = None
-    _disk_hash: int | None = None
-
-    # Rasterio-inherited names and types are defined here to get proper type hints.
-    # Maybe these don't have to be hard-coded in the future?
-    _data: np.ndarray | np.ma.masked_array
-    transform: Affine
-    crs: CRS
-    nodata: int | float | None
-    res: tuple[float, float]
-    bounds: rio.coords.BoundingBox
-    height: int
-    width: int
-    shape: tuple[int, int]
-    indexes: list[int]
-    count: int
-    dataset_mask: np.ndarray | None
-    driver: str
-    dtypes: list[str]
-    name: str
-
     def __init__(
         self,
-        filename_or_dataset: str | RasterType | rio.io.DatasetReader | rio.io.MemoryFile,
+        filename_or_dataset: str | RasterType | rio.io.DatasetReader | rio.io.MemoryFile | dict[str, Any],
         bands: None | int | list[int] = None,
         load_data: bool = True,
         downsample: AnyNumber = 1,
         masked: bool = True,
-        nodata: abc.Sequence[int | float] | int | float | None = None,
+        nodata: int | float | list[int] | list[float] | None = None,
         attrs: list[str] | None = None,
-        as_memfile: bool = False,
     ) -> None:
         """
         Load a rasterio-supported dataset, given a filename.
 
         :param filename_or_dataset: The filename of the dataset.
 
         :param bands: The band(s) to load into the object. Default is to load all bands.
@@ -184,118 +262,222 @@
         :param downsample: Reduce the size of the image loaded by this factor. Default is 1
 
         :param masked: the data is loaded as a masked array, with no data values masked. Default is True.
 
         :param nodata: nodata to be used (overwrites the metadata). Default is None, i.e. reads from metadata.
 
         :param attrs: Additional attributes from rasterio's DataReader class to add to the Raster object.
-            Default list is ['bounds', 'count', 'crs', 'dataset_mask', 'driver', 'dtypes', 'height', 'indexes',
+            Default list is set by geoutils.georaster.raster._default_rio_attrs, i.e.
+            ['bounds', 'count', 'crs', 'driver', 'dtypes', 'height', 'indexes',
             'name', 'nodata', 'res', 'shape', 'transform', 'width'] - if no attrs are specified, these will be added.
 
-        :param as_memfile: open the dataset via a rio.MemoryFile.
-
         :return: A Raster object
         """
+        self.driver: str | None = None
+        self.name: str | None = None
+        self.filename: str | None = None
+        self.tags: dict[str, Any] = {}
+
+        self._data: np.ma.masked_array | None = None
+        self._nodata: int | float | list[int] | list[float] | None = nodata
+        self._bands = bands
+        self._masked = masked
+        self._disk_hash: int | None = None
+        self._is_modified = True
+        self._disk_shape: tuple[int, int, int] | None = None
+        self._disk_indexes: tuple[int] | None = None
+        self._disk_dtypes: tuple[str] | None = None
+
+        # This is for Raster.from_array to work.
+        if isinstance(filename_or_dataset, dict):
+            # Important to pass the nodata before the data setter, which uses it in turn
+            self._nodata = filename_or_dataset["nodata"]
+            self.data = filename_or_dataset["data"]
+            self.transform: rio.transform.Affine = filename_or_dataset["transform"]
+            self.crs: rio.crs.CRS = filename_or_dataset["crs"]
+            for key in filename_or_dataset:
+                if key in ["data", "transform", "crs", "nodata"]:
+                    continue
+                setattr(self, key, filename_or_dataset[key])
+            return
+
         # If Raster is passed, simply point back to Raster
         if isinstance(filename_or_dataset, Raster):
             for key in filename_or_dataset.__dict__:
                 setattr(self, key, filename_or_dataset.__dict__[key])
             return
         # Image is a file on disk.
-        elif isinstance(filename_or_dataset, str):
-            # Save the absolute on-disk filename
-            self.filename = os.path.abspath(filename_or_dataset)
-            if as_memfile:
-                # open the file in memory
-                memfile = MemoryFile(open(filename_or_dataset, "rb"))
-                # Read the file as a rasterio dataset
-                self.ds = memfile.open()
-            else:
-                self.ds = rio.open(filename_or_dataset, "r")
+        elif isinstance(filename_or_dataset, (str, rio.io.DatasetReader, rio.io.MemoryFile)):
 
-        # If rio.Dataset is passed
-        elif isinstance(filename_or_dataset, rio.io.DatasetReader):
-            self.filename = filename_or_dataset.files[0]
-            self.ds = filename_or_dataset
-
-        # Or, image is already a Memory File.
-        elif isinstance(filename_or_dataset, rio.io.MemoryFile):
-            self.ds = filename_or_dataset.open()
+            # ExitStack is used instead of "with rio.open(filename_or_dataset) as ds:".
+            # This is because we might not actually want to open it like that, so this is equivalent
+            # to the pseudocode:
+            # "with rio.open(filename_or_dataset) as ds if isinstance(filename_or_dataset, str) else ds:"
+            # This is slightly black magic, but it works!
+            with ExitStack():
+                if isinstance(filename_or_dataset, str):
+                    ds: rio.io.DatasetReader = rio.open(filename_or_dataset)
+                    self.filename = filename_or_dataset
+                elif isinstance(filename_or_dataset, rio.io.DatasetReader):
+                    ds = filename_or_dataset
+                    self.filename = filename_or_dataset.files[0]
+                else:  # This is if it's a MemoryFile
+                    ds = filename_or_dataset.open()
+                    self.filename = None
+
+                self.transform = ds.transform
+                self.crs = ds.crs
+                self._nodata = ds.nodata
+                self.name = ds.name
+                self.driver = ds.driver
+                self.tags.update(ds.tags())
+
+                self._disk_shape = (ds.count, ds.height, ds.width)
+                self._disk_indexes = ds.indexes
+                self._disk_dtypes = ds.dtypes
+
+                if attrs is not None:
+                    for attr in attrs:
+                        self.__setattr__(attr, ds.__getattr__(attr))
+
+            # Check number of bands to be loaded
+            if bands is None:
+                nbands = self.nbands
+            elif isinstance(bands, int):
+                nbands = 1
+            elif isinstance(bands, abc.Iterable):
+                nbands = len(bands)
+
+            # Downsampled image size
+            if not isinstance(downsample, (int, float)):
+                raise ValueError("downsample must be of type int or float")
+            if downsample == 1:
+                out_shape = (nbands, self.height, self.width)
+            else:
+                down_width = int(np.ceil(self.width / downsample))
+                down_height = int(np.ceil(self.height / downsample))
+                out_shape = (nbands, down_height, down_width)
+                res = tuple(np.asarray(self.res) * downsample)
+                self.transform = rio.transform.from_origin(self.bounds.left, self.bounds.top, res[0], res[1])
+
+            if load_data:
+                # Mypy doesn't like the out_shape for some reason. I can't figure out why! (erikmannerfelt, 14/01/2022)
+                self._data = _load_rio(ds, bands=bands, masked=masked, out_shape=out_shape)  # type: ignore
+                if isinstance(filename_or_dataset, str):
+                    self._is_modified = False
+                    self._disk_hash = hash((self.data.tobytes(), self.transform, self.crs, self.nodata))
+
+            # Set nodata
+            if nodata is not None:
+                self.set_nodata(nodata)
 
         # Provide a catch in case trying to load from data array
         elif isinstance(filename_or_dataset, np.ndarray):
             raise ValueError("np.array provided as filename. Did you mean to call Raster.from_array(...) instead? ")
 
         # Don't recognise the input, so stop here.
         else:
             raise ValueError("filename argument not recognised.")
 
-        self._read_attrs(attrs)
+    @property
+    def nbands(self) -> int:
+        if not self.is_loaded and self._disk_shape is not None:
+            return self._disk_shape[0]
+        return int(self.data.shape[0])
 
-        # Save _masked attribute to be used by self.load()
-        self._masked = masked
+    @property
+    def count(self) -> int:
+        if self._disk_shape is not None:
+            return self._disk_shape[0]
+        return self.nbands
+
+    @property
+    def height(self) -> int:
+        """Return the height of the Raster in pixels."""
+        if not self.is_loaded:
+            return self._disk_shape[1]  # type: ignore
+        return int(self.data.shape[1])
+
+    @property
+    def width(self) -> int:
+        """Return the width of the Raster in pixels."""
+        if not self.is_loaded:
+            return self._disk_shape[2]  # type: ignore
+        return int(self.data.shape[2])
+
+    @property
+    def shape(self) -> tuple[int, int]:
+        """Return a (height, width) tuple of the data shape in pixels."""
+        if not self.is_loaded:
+            return self._disk_shape[1], self._disk_shape[2]  # type: ignore
+        return int(self.data.shape[1]), int(self.data.shape[2])
+
+    @property
+    def res(self) -> tuple[float | int, float | int]:
+        """Return the X/Y resolution in georeferenced units of the Raster."""
+        return self.transform[0], abs(self.transform[4])
+
+    @property
+    def bounds(self) -> rio.coords.BoundingBox:
+        """Return the bounding coordinates of the Raster."""
+        return rio.coords.BoundingBox(*rio.transform.array_bounds(self.height, self.width, self.transform))
+
+    @property
+    def is_loaded(self) -> bool:
+        """Return False if the data attribute is None, and True if data exists."""
+        return self._data is not None
+
+    @property
+    def dtypes(self) -> tuple[str, ...]:
+        """Return the string representations of the data types for each band."""
+        if not self.is_loaded and self._disk_dtypes is not None:
+            return self._disk_dtypes
+        return (str(self.data.dtype),) * self.nbands
+
+    @property
+    def indexes(self) -> tuple[int, ...]:
+        if self._disk_indexes is not None:
+            return self._disk_indexes
+        return tuple(range(1, self.nbands + 1))
+
+    @property
+    def bands(self) -> tuple[int, ...]:
+        if self._bands is not None:
+            if isinstance(self._bands, int):
+                return (self._bands,)
+            return tuple(self._bands)
+        return self.indexes
+
+    def load(self, **kwargs: Any) -> None:
+        """
+        Load the data from disk.
+
+        :param kwargs: Optional keyword arguments sent to '_load_rio()'
 
-        # Check number of bands to be loaded
-        if bands is None:
-            nbands = self.count
-        elif isinstance(bands, int):
-            nbands = 1
-        elif isinstance(bands, abc.Iterable):
-            nbands = len(bands)
-
-        # Downsampled image size
-        if not isinstance(downsample, (int, float)):
-            raise ValueError("downsample must be of type int or float")
-        if downsample == 1:
-            out_shape = (nbands, self.height, self.width)
-        else:
-            down_width = int(np.ceil(self.width / downsample))
-            down_height = int(np.ceil(self.height / downsample))
-            out_shape = (nbands, down_height, down_width)
-
-        if load_data:
-            self.load(bands=bands, out_shape=out_shape)
-            self.nbands = self._data.shape[0]
-            self.is_loaded = True
-            if isinstance(filename_or_dataset, str):
-                self._is_modified = False
-                self._disk_hash = hash((self._data.tobytes(), self.transform, self.crs, self.nodata))
-        else:
-            self._data = None
-            self.nbands = None
-            self.is_loaded = False
-
-        # update attributes when downsample is not 1
-        if downsample != 1:
-
-            # Original attributes
-            meta = self.ds.meta
-
-            # width and height must be same as data
-            meta.update({"width": down_width, "height": down_height})
-
-            # Resolution is set, transform must be updated accordingly
-            res = tuple(np.asarray(self.res) * downsample)
-            transform = rio.transform.from_origin(self.bounds.left, self.bounds.top, res[0], res[1])
-            meta.update({"transform": transform})
-
-            # Update metadata
-            self._update(self.data, metadata=meta)
-
-        # Set nodata
-        if nodata is not None:
-            self.set_ndv(nodata)
+        :raises ValueError: If the data are already loaded.
+        :raises AttributeError: If no 'filename' attribute exists.
+        """
+        if self.is_loaded:
+            raise ValueError("Data are already loaded")
+
+        if self.filename is None:
+            raise AttributeError("'filename' is not set")
+
+        with rio.open(self.filename) as dataset:
+            self.data = _load_rio(
+                dataset, bands=self._bands, masked=self._masked, transform=self.transform, shape=self.shape, **kwargs
+            )
 
     @classmethod
     def from_array(
         cls: type[RasterType],
         data: np.ndarray | np.ma.masked_array,
         transform: tuple[float, ...] | Affine,
-        crs: CRS | int,
-        nodata: int | float | None = None,
+        crs: CRS | int | None,
+        nodata: int | float | list[int] | list[float] | None = None,
     ) -> RasterType:
         """Create a Raster from a numpy array and some geo-referencing information.
 
         :param data: data array
 
         :param transform: the 2-D affine transform for the image mapping.
             Either a tuple(x_res, 0.0, top_left_x, 0.0, y_res, top_left_y) or
@@ -325,81 +507,52 @@
             else:
                 raise ValueError("transform argument needs to be Affine or tuple.")
 
         # Enable shortcut to create CRS from an EPSG ID.
         if isinstance(crs, int):
             crs = CRS.from_epsg(crs)
 
-        # If a 2-D ('single-band') array is passed in, give it a band dimension.
-        if len(data.shape) < 3:
-            data = np.expand_dims(data, 0)
-
-        # Preserves input mask
-        if isinstance(data, np.ma.masked_array):
-            if nodata is None:
-                if np.sum(data.mask) > 0:
-                    raise ValueError("For masked arrays, a nodata value must be set")
-            else:
-                data.data[data.mask] = nodata
-
-        # Open handle to new memory file
-        mfh = MemoryFile()
-
-        # Create the memory file
-        with rio.open(
-            mfh,
-            "w",
-            height=data.shape[1],
-            width=data.shape[2],
-            count=data.shape[0],
-            dtype=data.dtype,
-            crs=crs,
-            transform=transform,
-            nodata=nodata,
-            driver="GTiff",
-        ) as ds:
-
-            ds.write(data)
-
-        # Initialise a Raster object created with MemoryFile.
-        # (i.e., __init__ will now be run.)
-        return cls(mfh)
+        return cls({"data": data, "transform": transform, "crs": crs, "nodata": nodata})
 
     def __repr__(self) -> str:
         """Convert object to formal string representation."""
-        L = [getattr(self, item) for item in self._saved_attrs]
-        s: str = "{}.{}({})".format(type(self).__module__, type(self).__qualname__, ", ".join(map(str, L)))
+        return self.__str__()
+        # L = [getattr(self, item) for item in self._saved_attrs]
+        # s: str = "{}.{}({})".format(type(self).__module__, type(self).__qualname__, ", ".join(map(str, L)))
 
-        return s
+        # return s
 
     def __str__(self) -> str:
         """Provide string of information about Raster."""
         return self.info()
 
     def __eq__(self, other: object) -> bool:
-        """Check if a Raster's data and georeferencing is equal to another."""
-        from geoutils.misc import array_equal
+        """Check if a Raster masked array's data (including masked values), mask, fill_value and dtype are equal,
+        as well as the Raster's nodata, and georeferencing."""
 
         if not isinstance(other, type(self)):  # TODO: Possibly add equals to SatelliteImage?
             return NotImplemented
         return all(
             [
-                array_equal(self.data, other.data, equal_nan=True),
+                np.array_equal(self.data.data, other.data.data, equal_nan=True),
+                np.array_equal(self.data.mask, other.data.mask),
+                self.data.fill_value == other.data.fill_value,
+                self.data.dtype == other.data.dtype,
                 self.transform == other.transform,
                 self.crs == other.crs,
                 self.nodata == other.nodata,
             ]
         )
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     def _overloading_check(
         self: RasterType, other: RasterType | np.ndarray | Number
-    ) -> tuple[np.ndarray, np.ndarray | Number, float | int | None]:
+    ) -> tuple[np.ma.masked_array, np.ma.masked_array | Number, float | int | list[int] | list[float] | None]:
         """
         Before any operation overloading, check input data type and return both self and other data as either \
 a np.ndarray or number, converted to the minimum compatible dtype between both datasets.
         Also returns the best compatible nodata value.
 
         The nodata value is set in the following order:
         - to nodata of self, if output dtype is same as self's dtype
@@ -413,20 +566,20 @@
 np.ndarray or number and correct dtype, the compatible nodata value.
         """
         # Check that other is of correct type
         # If not, a NotImplementedError should be raised, in case other's class has a method implemented.
         # See https://docs.python.org/3/reference/datamodel.html#emulating-numeric-types
         if not isinstance(other, (Raster, np.ndarray, Number)):
             raise NotImplementedError(
-                f"Operation between an object of type {type(other)} and a Raster impossible. \
-Must be a Raster, np.ndarray or single number."
+                f"Operation between an object of type {type(other)} and a Raster impossible. Must be a Raster, "
+                f"np.ndarray or single number."
             )
 
         # Get self's dtype and nodata
-        ndv1 = self.nodata
+        nodata1 = self.nodata
         dtype1 = self.data.dtype
 
         # Case 1 - other is a Raster
         if isinstance(other, Raster):
             # Check that both data are loaded
             if not (self.is_loaded & other.is_loaded):
                 raise ValueError("Raster's data must be loaded with self.load().")
@@ -434,72 +587,69 @@
             # Check that both rasters have the same shape and georeferences
             if (self.data.shape == other.data.shape) & (self.transform == other.transform) & (self.crs == other.crs):
                 pass
             else:
                 raise ValueError("Both rasters must have the same shape, transform and CRS.")
 
             other_data = other.data
-            ndv2 = other.nodata
+            nodata2 = other.nodata
             dtype2 = other_data.dtype
 
         # Case 2 - other is a numpy array
         elif isinstance(other, np.ndarray):
             # Check that both array have the same shape
-            if self.data.shape == other.shape:
+
+            if len(other.shape) == 2:
+                other_data = other[np.newaxis, :, :]
+            else:
+                other_data = other
+
+            if self.data.shape == other_data.shape:
                 pass
             else:
                 raise ValueError("Both rasters must have the same shape.")
 
-            other_data = other
-            ndv2 = None
+            nodata2 = None
             dtype2 = other_data.dtype
 
         # Case 3 - other is a single number
         else:
             other_data = other
-            ndv2 = None
+            nodata2 = None
             dtype2 = rio.dtypes.get_minimum_dtype(other_data)
 
         # Figure out output dtype
         out_dtype = np.find_common_type([dtype1, dtype2], [])
 
         # Figure output nodata
-        out_ndv = None
-        if (ndv2 is not None) and (out_dtype == dtype2):
-            out_ndv = ndv2
-        if (ndv1 is not None) and (out_dtype == dtype1):
-            out_ndv = ndv1
-
-        # Convert output data to correct dtype and masked_array
-        if isinstance(other_data, np.ndarray):
-            other_data = np.ma.asarray(other_data).astype(out_dtype, copy=False)
+        out_nodata = None
+        if (nodata2 is not None) and (out_dtype == dtype2):
+            out_nodata = nodata2
+        if (nodata1 is not None) and (out_dtype == dtype1):
+            out_nodata = nodata1
 
-        self_data = self.data.astype(out_dtype)
+        self_data = self.data
 
-        return self_data, other_data, out_ndv
+        return self_data, other_data, out_nodata
 
     def __add__(self: RasterType, other: RasterType | np.ndarray | Number) -> RasterType:
         """
         Sum up the data of two rasters or a raster and a numpy array, or a raster and single number.
         If other is a Raster, it must have the same data.shape, transform and crs as self.
         If other is a np.ndarray, it must have the same shape.
         Otherwise, other must be a single number.
         """
         # Check inputs and return compatible data, output dtype and nodata value
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
 
         # Run calculation
         out_data = self_data + other_data
 
-        # Check that if no ndv was set, a default value is used
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-
         # Save to output Raster
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
 
         return out_rst
 
     def __radd__(self: RasterType, other: np.ndarray | Number) -> RasterType:
         """
         Addition overloading when other is first item in the operation (e.g. 1 + rst).
         """
@@ -509,42 +659,36 @@
         """Return self with self.data set to -self.data"""
         return self.from_array(-self.data, self.transform, self.crs, nodata=self.nodata)
 
     def __sub__(self, other: Raster | np.ndarray | Number) -> Raster:
         """
         Subtract two rasters. Both rasters must have the same data.shape, transform and crs.
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = self_data - other_data
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-        return self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        return self.from_array(out_data, self.transform, self.crs, nodata=nodata)
 
     def __rsub__(self: RasterType, other: np.ndarray | Number) -> RasterType:
         """
         Subtraction overloading when other is first item in the operation (e.g. 1 - rst).
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = other_data - self_data
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-        return self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        return self.from_array(out_data, self.transform, self.crs, nodata=nodata)
 
     def __mul__(self: RasterType, other: RasterType | np.ndarray | Number) -> RasterType:
         """
         Multiply the data of two rasters or a raster and a numpy array, or a raster and single number.
         If other is a Raster, it must have the same data.shape, transform and crs as self.
         If other is a np.ndarray, it must have the same shape.
         Otherwise, other must be a single number.
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = self_data * other_data
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
         return out_rst
 
     def __rmul__(self: RasterType, other: np.ndarray | Number) -> RasterType:
         """
         Multiplication overloading when other is first item in the operation (e.g. 2 * rst).
         """
         return self.__mul__(other)
@@ -552,88 +696,77 @@
     def __truediv__(self: RasterType, other: RasterType | np.ndarray | Number) -> RasterType:
         """
         True division of the data of two rasters or a raster and a numpy array, or a raster and single number.
         If other is a Raster, it must have the same data.shape, transform and crs as self.
         If other is a np.ndarray, it must have the same shape.
         Otherwise, other must be a single number.
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = self_data / other_data
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
         return out_rst
 
     def __rtruediv__(self: RasterType, other: np.ndarray | Number) -> RasterType:
         """
         True division overloading when other is first item in the operation (e.g. 1/rst).
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = other_data / self_data
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
         return out_rst
 
     def __floordiv__(self: RasterType, other: RasterType | np.ndarray | Number) -> RasterType:
         """
         Floor division of the data of two rasters or a raster and a numpy array, or a raster and single number.
         If other is a Raster, it must have the same data.shape, transform and crs as self.
         If other is a np.ndarray, it must have the same shape.
         Otherwise, other must be a single number.
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = self_data // other_data
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
         return out_rst
 
     def __rfloordiv__(self: RasterType, other: np.ndarray | Number) -> RasterType:
         """
         Floor division overloading when other is first item in the operation (e.g. 1/rst).
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = other_data // self_data
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
         return out_rst
 
     def __mod__(self: RasterType, other: RasterType | np.ndarray | Number) -> RasterType:
         """
         Modulo of the data of two rasters or a raster and a numpy array, or a raster and single number.
         If other is a Raster, it must have the same data.shape, transform and crs as self.
         If other is a np.ndarray, it must have the same shape.
         Otherwise, other must be a single number.
         """
-        self_data, other_data, ndv = self._overloading_check(other)
+        self_data, other_data, nodata = self._overloading_check(other)
         out_data = self_data % other_data
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=ndv)
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
         return out_rst
 
     def __pow__(self: RasterType, power: int | float) -> RasterType:
         """
         Calculate the power of self.data and returns a Raster.
         """
         # Check that input is a number
         if not isinstance(power, Number):
             raise ValueError("Power needs to be a number.")
 
         # Calculate the product of arrays and save to new Raster
         out_data = self.data**power
-        ndv = self.nodata
-        if (np.sum(out_data.mask) > 0) & (ndv is None):
-            ndv = _default_ndv(out_data.dtype)
-
-        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=self.nodata)
+        nodata = self.nodata
+        out_rst = self.from_array(out_data, self.transform, self.crs, nodata=nodata)
         return out_rst
 
     @overload
-    def astype(self, dtype: DTypeLike, inplace: Literal[False]) -> Raster:
+    def astype(self, dtype: DTypeLike, inplace: Literal[False] = False) -> Raster:
         ...
 
     @overload
     def astype(self, dtype: DTypeLike, inplace: Literal[True]) -> None:
         ...
 
     def astype(self, dtype: DTypeLike, inplace: bool = False) -> Raster | None:
@@ -654,140 +787,271 @@
             warnings.warn(
                 "dtype conversion will result in a loss of information. "
                 f"{rio.dtypes.get_minimum_dtype(self.data)} is the minimum type to represent the data."
             )
 
         out_data = self.data.astype(dtype)
         if inplace:
-            meta = self.ds.meta
-            meta.update({"dtype": dtype})
-            self._update(imgdata=out_data, metadata=meta)
+            self._data = out_data
             return None
         else:
             return self.from_array(out_data, self.transform, self.crs, nodata=self.nodata)
 
-    def _get_rio_attrs(self) -> list[str]:
-        """Get the attributes that have the same name in rio.DatasetReader and Raster."""
-        rio_attrs: list[str] = []
-        for attr in Raster.__annotations__.keys():
-            if "__" in attr or attr not in dir(self.ds):
-                continue
-            rio_attrs.append(attr)
-        return rio_attrs
-
-    def _read_attrs(self, attrs: list[str] | str | None = None) -> None:
-        # Copy most used attributes/methods
-        rio_attrs = self._get_rio_attrs()
-        for attr in self.__annotations__.keys():
-            if "__" in attr or attr not in dir(self.ds):
-                continue
-            rio_attrs.append(attr)
-        if attrs is None:
-            self._saved_attrs = rio_attrs
-            attrs = rio_attrs
-        else:
-            if isinstance(attrs, str):
-                attrs = [attrs]
-            for attr in rio_attrs:
-                if attr not in attrs:
-                    attrs.append(attr)
-            self._saved_attrs = attrs
-
-        for attr in attrs:
-            setattr(self, attr, getattr(self.ds, attr))
-
     @property
     def is_modified(self) -> bool:
         """Check whether file has been modified since it was created/opened.
 
         :returns: True if Raster has been modified.
 
         """
         if not self._is_modified:
-            new_hash = hash((self._data.tobytes(), self.transform, self.crs, self.nodata))
+            new_hash = hash(
+                (self._data.tobytes() if self._data is not None else 0, self.transform, self.crs, self.nodata)
+            )
             self._is_modified = not (self._disk_hash == new_hash)
 
         return self._is_modified
 
     @property
-    def data(self) -> np.ndarray | np.ma.masked_array:
+    def nodata(self) -> int | float | list[int] | list[float] | None:
+        """
+        Get nodata value.
+
+        :returns: Nodata value
+        """
+        return self._nodata
+
+    @nodata.setter
+    def nodata(self, new_nodata: int | float | list[int] | list[float] | None) -> None:
+        """
+        Set .nodata and update .data by calling set_nodata() with default parameters.
+
+        By default, the old nodata values are updated into the new nodata in the data array .data.data, and the
+        mask .data.mask is updated to mask all new nodata values (i.e., the mask from old nodata stays and is extended
+        to potential new values of new nodata found in the array).
+
+        To set nodata for more complex cases (e.g., redefining a wrong nodata that has a valid value in the array),
+        call the function set_nodata() directly to set the arguments update_array and update_mask adequately.
+
+        :param new_nodata: New nodata to assign to this instance of Raster
+        """
+
+        self.set_nodata(nodata=new_nodata)
+
+    def set_nodata(
+        self, nodata: int | float | list[int] | list[float] | None, update_array: bool = True, update_mask: bool = True
+    ) -> None:
+        """
+        Set a new nodata value for each band. This updates the old nodata into a new nodata value in the metadata,
+        replaces the nodata values in the data of the masked array, and updates the mask of the masked array.
+
+        Careful! If the new nodata value already exists in the array, the related grid cells will be masked by default.
+
+        If the nodata value was not defined in the raster, run this function with a new nodata value corresponding to
+        the value of nodata that exists in the data array and is not yet accounted for. All those values will be masked.
+
+        If a nodata value was correctly defined in the raster, and you wish to change it to a new value, run
+        this function with that new value. All values having either the old or new nodata value will be masked.
+
+        If the nodata value was wrongly defined in the raster, and you wish to change it to a new value without
+        affecting data that might have the value of the old nodata, run this function with the update_array
+        argument as False. Only the values of the new nodata will be masked.
+
+        If you wish to set nodata value without updating the mask, run this function with the update_mask argument as
+        False.
+
+        If None is passed as nodata, only the metadata is updated and the mask of oldnodata unset.
+
+        :param nodata: Nodata values
+        :param update_array: Update the old nodata values into new nodata values in the data array
+        :param update_mask: Update the old mask by unmasking old nodata and masking new nodata (if array is updated,
+            old nodata are changed to new nodata and thus stay masked)
+        """
+        if nodata is not None and not isinstance(nodata, (list, int, float, np.integer, np.floating)):
+            raise ValueError("Type of nodata not understood, must be list or float or int")
+
+        elif (isinstance(nodata, (int, float, np.integer, np.floating))) and self.count > 1:
+            nodata = [nodata] * self.count
+
+        elif isinstance(nodata, list) and self.count == 1:
+            nodata = list(nodata)[0]
+
+        elif nodata is None:
+            nodata = None
+
+        # Check that nodata has same length as number of bands in self
+        if isinstance(nodata, list):
+            if len(nodata) != self.count:
+                raise ValueError(f"Length of nodata ({len(nodata)}) incompatible with number of bands ({self.count})")
+            # Check that nodata value is compatible with dtype
+            for k in range(len(nodata)):
+                if not rio.dtypes.can_cast_dtype(nodata[k], self.dtypes[k]):
+                    raise ValueError(f"nodata value {nodata[k]} incompatible with self.dtype {self.dtypes[k]}")
+        elif isinstance(nodata, (int, float, np.integer, np.floating)):
+            if not rio.dtypes.can_cast_dtype(nodata, self.dtypes[0]):
+                raise ValueError(f"nodata value {nodata} incompatible with self.dtype {self.dtypes[0]}")
+
+        # If we update mask or array, get the masked array
+        if update_array or update_mask:
+
+            # Extract the data variable, so the self.data property doesn't have to be called a bunch of times
+            imgdata = self.data
+
+            # Loop through the bands
+            for i, new_nodata in enumerate(nodata if isinstance(nodata, Iterable) else [nodata]):
+
+                # Get the index of old nodatas
+                index_old_nodatas = imgdata.data[i, :, :] == self.nodata
+
+                # Get the index of new nodatas, if it is defined
+                index_new_nodatas = imgdata.data[i, :, :] == new_nodata
+
+                if np.count_nonzero(index_new_nodatas) > 0:
+                    if update_array and update_mask:
+                        warnings.warn(
+                            message="New nodata value found in the data array. Those will be masked, and the old "
+                            "nodata cells will now take the same value. Use set_nodata() with update_array=False "
+                            "and/or update_mask=False to change this behaviour.",
+                            category=UserWarning,
+                        )
+                    elif update_array:
+                        warnings.warn(
+                            "New nodata value found in the data array. The old nodata cells will now take the same "
+                            "value. Use set_nodata() with update_array=False to change this behaviour.",
+                            category=UserWarning,
+                        )
+                    elif update_mask:
+                        warnings.warn(
+                            "New nodata value found in the data array. Those will be masked. Use set_nodata() "
+                            "with update_mask=False to change this behaviour.",
+                            category=UserWarning,
+                        )
+
+                if update_array:
+                    # Only update array with new nodata if it is defined
+                    if nodata is not None:
+                        # Replace the nodata value in the Raster
+                        imgdata.data[i, index_old_nodatas] = new_nodata
+
+                if update_mask:
+                    # If a mask already exists, unmask the old nodata values before masking the new ones
+                    # Can be skipped if array is updated (nodata is transferred from old to new, this part of the mask
+                    # stays the same)
+                    if np.ma.is_masked(imgdata) and (not update_array or nodata is None):
+                        # No way to unmask a value from the masked array, so we modify the mask directly
+                        imgdata.mask[i, index_old_nodatas] = False
+
+                    # Masking like this works from the masked array directly, whether a mask exists or not
+                    imgdata[i, index_new_nodatas] = np.ma.masked
+
+            # Update the data
+            self._data = imgdata
+
+        # Update the nodata value
+        self._nodata = nodata
+
+    @property
+    def data(self) -> np.ma.masked_array:
         """
         Get data.
 
         :returns: data array.
 
         """
+        if not self.is_loaded and self._data is None:
+            raise ValueError("Data are not loaded")
         return self._data
 
     @data.setter
     def data(self, new_data: np.ndarray | np.ma.masked_array) -> None:
         """
-        Set the contents of .data.
+        Set the contents of .data and possibly update .nodata.
+
+        The data setter behaviour is the following:
 
-        new_data must have the same shape as existing data! (bands dimension included)
+        1. Writes the data in a masked array, whether the input is a classic array or a masked_array,
+        2. Reshapes the data in a 3D array if it is 2D that can be broadcasted, raises an error otherwise,
+        3. Raises an error if the dtype is different from that of the Raster, and points towards .copy() or .astype(),
+        4. Sets a new nodata value to the Raster if none is set and if the provided array contains non-finite values
+            that are unmasked (including if there is no mask at all, e.g. NaNs in a classic array),
+        5. Masks non-finite values that are unmasked, whether the input is a classic array or a masked_array. Note that
+            these values are not overwritten and can still be accessed in .data.data.
 
         :param new_data: New data to assign to this instance of Raster
 
         """
         # Check that new_data is a Numpy array
         if not isinstance(new_data, np.ndarray):
             raise ValueError("New data must be a numpy array.")
 
+        if len(new_data.shape) == 2:
+            new_data = new_data[np.newaxis, :, :]
+
         # Check that new_data has correct shape
-        if self.is_loaded:
-            orig_shape = self._data.shape
+        if self._data is not None:
+            dtype = str(self._data.dtype)
+            orig_shape = self._data.shape[1:]
+        elif self.filename is not None:
+            dtype = self.dtypes[0]
+            orig_shape = self.shape
         else:
-            orig_shape = (self.count, self.height, self.width)
-
-        if new_data.shape != orig_shape:
-            raise ValueError(f"New data must be of the same shape as existing data: {orig_shape}.")
+            dtype = str(new_data.dtype)
+            orig_shape = new_data.shape[1:]
 
         # Check that new_data has the right type
-        if new_data.dtype != self._data.dtype:
+        if str(new_data.dtype) != dtype:
             raise ValueError(
-                "New data must be of the same type as existing\
- data: {}".format(
-                    self.data.dtype
-                )
+                "New data must be of the same type as existing data: {}. Use copy() to set a new array with "
+                "different dtype, or astype() to change type.".format(dtype)
             )
 
-        self._data = new_data
+        if new_data.shape[1:] != orig_shape:
+            raise ValueError(
+                f"New data must be of the same shape as existing data: {orig_shape}. Given: {new_data.shape[1:]}."
+            )
 
-    def _update(
-        self,
-        imgdata: np.ndarray | None = None,
-        metadata: dict[str, Any] | None = None,
-        vrt_to_driver: str = "GTiff",
-    ) -> None:
-        """
-        Update the object with a new image or metadata.
+        # If the new data is not masked and has non-finite values, we define a default nodata value
+        if (not np.ma.is_masked(new_data) and self.nodata is None and np.count_nonzero(~np.isfinite(new_data)) > 0) or (
+            np.ma.is_masked(new_data)
+            and self.nodata is None
+            and np.count_nonzero(~np.isfinite(new_data.data[~new_data.mask])) > 0
+        ):
+            warnings.warn(
+                "Setting default nodata {:.0f} to mask non-finite values found in the array, as "
+                "no nodata value was defined.".format(_default_nodata(dtype)),
+                UserWarning,
+            )
+            self._nodata = _default_nodata(dtype)
 
-        :param imgdata: image data to update with.
-        :param metadata: metadata to update with.
-        :param vrt_to_driver: name of driver to coerce a VRT to. This is required
-        because rasterio does not support writing to to a VRTSourcedRasterBand.
-        """
-        memfile = MemoryFile()
-        if imgdata is None:
-            imgdata = self.data
-        if metadata is None:
-            metadata = self.ds.meta
+        # Now comes the important part, the data setting!
+        # Several cases to consider:
 
-        if metadata["driver"] == "VRT":
-            metadata["driver"] = vrt_to_driver
+        # 1/ If the new data is not masked (either classic array or masked array with no mask, hence the use of
+        # as array) and contains non-finite values such as NaNs, define a mask
+        if not np.ma.is_masked(new_data) and np.count_nonzero(~np.isfinite(new_data)) > 0:
+            self._data = np.ma.masked_array(
+                data=np.asarray(new_data), mask=~np.isfinite(new_data.data), fill_value=self.nodata
+            )
 
-        with memfile.open(**metadata) as ds:
-            ds.write(imgdata)
+        # 2/ If the new data is masked but some non-finite values aren't masked, add them to the mask
+        elif np.ma.is_masked(new_data) and np.count_nonzero(~np.isfinite(new_data.data[~new_data.mask])) > 0:
+            self._data = np.ma.masked_array(
+                data=new_data.data,
+                mask=np.logical_or(~np.isfinite(new_data.data), new_data.mask),
+                fill_value=self.nodata,
+            )
 
-        self.ds = memfile.open()
-        self._read_attrs()
-        if self.is_loaded:
-            self.load()
+        # 3/ If the new data is a Masked Array, we pass data.data and data.mask independently (passing directly the
+        # masked array to data= has a strange behaviour that redefines fill_value)
+        elif np.ma.isMaskedArray(new_data):
+            self._data = np.ma.masked_array(data=new_data.data, mask=new_data.mask, fill_value=self.nodata)
 
-        self._is_modified = True
+        # 4/ If the new data is classic ndarray
+        else:
+            self._data = np.ma.masked_array(data=new_data, fill_value=self.nodata)
 
     def set_mask(self, mask: np.ndarray) -> None:
         """
         Mask all pixels of self.data where `mask` is set to True or > 0.
 
         Masking is performed in place.
         `mask` must have the same shape as loaded data, unless the first dimension is 1, then it is ignored.
@@ -796,15 +1060,15 @@
         """
         # Check that mask is a Numpy array
         if not isinstance(mask, np.ndarray):
             raise ValueError("mask must be a numpy array.")
 
         # Check that new_data has correct shape
         if self.is_loaded:
-            orig_shape = self._data.shape
+            orig_shape = self.data.shape
         else:
             raise AttributeError("self.data must be loaded first, with e.g. self.load()")
 
         if mask.shape != orig_shape:
             # In case first dimension is empty and other dimensions match -> reshape mask
             if (orig_shape[0] == 1) & (orig_shape[1:] == mask.shape):
                 mask = mask.reshape(orig_shape)
@@ -828,23 +1092,23 @@
             f"Driver:               {self.driver} \n",
             f"Opened from file:     {self.filename} \n",
             f"Filename:             {self.name} \n",
             f"Raster modified since disk load?  {self._is_modified} \n",
             f"Size:                 {self.width}, {self.height}\n",
             f"Number of bands:      {self.count:d}\n",
             f"Data types:           {self.dtypes}\n",
-            f"Coordinate System:    EPSG:{self.crs.to_epsg()}\n",
+            f"Coordinate System:    {[self.crs.to_string() if self.crs is not None else None]}\n",
             f"NoData Value:         {self.nodata}\n",
             "Pixel Size:           {}, {}\n".format(*self.res),
             "Upper Left Corner:    {}, {}\n".format(*self.bounds[:2]),
             "Lower Right Corner:   {}, {}\n".format(*self.bounds[2:]),
         ]
 
         if stats:
-            if self.data is not None:
+            if self.is_loaded:
                 if self.nbands == 1:
                     as_str.append(f"[MAXIMUM]:          {np.nanmax(self.data):.2f}\n")
                     as_str.append(f"[MINIMUM]:          {np.nanmin(self.data):.2f}\n")
                     as_str.append(f"[MEDIAN]:           {np.ma.median(self.data):.2f}\n")
                     as_str.append(f"[MEAN]:             {np.nanmean(self.data):.2f}\n")
                     as_str.append(f"[STD DEV]:          {np.nanstd(self.data):.2f}\n")
                 else:
@@ -866,62 +1130,191 @@
         :param new_array: New array to use for the copied Raster
 
         :return:
         """
         if new_array is not None:
             data = new_array
         else:
-            data = self.data
+            data = self.data.copy()
 
         cp = self.from_array(data=data, transform=self.transform, crs=self.crs, nodata=self.nodata)
 
         return cp
 
-    @property
-    def __array_interface__(self) -> dict[str, Any]:
-        if self._data is None:
-            self.load()
+    @overload
+    def get_nanarray(self, return_mask: Literal[False] = False) -> np.ndarray:
+        ...
+
+    @overload
+    def get_nanarray(self, return_mask: Literal[True]) -> tuple[np.ndarray, np.ndarray]:
+        ...
 
-        return self._data.__array_interface__  # type: ignore
+    def get_nanarray(self, return_mask: bool = False) -> np.ndarray | tuple[np.ndarray, np.ndarray]:
+        """
+        Method to return the squeezed masked array filled with NaNs and associated squeezed mask, both as a copy.
+
+        :param return_mask: Whether to return the mask of valid data
+
+        :returns Array with masked data as NaNs, (Optional) Mask of valid data
+        """
 
-    def load(self, bands: int | list[int] | None = None, **kwargs: Any) -> None:
-        r"""
-        Load specific bands of the dataset, using rasterio.read().
-        Ensure that self.data.ndim = 3 for ease of use (needed e.g. in show)
-
-        :param bands: The band(s) to load. Note that rasterio begins counting at 1, not 0.
-
-
-        \*\*kwargs: any additional arguments to rasterio.io.DatasetReader.read.
-        Useful ones are:
-        .. hlist::
-        * out_shape : to load a subsampled version
-        * window : to load a cropped version
-        * resampling : to set the resampling algorithm
-        """
-        if bands is None:
-            self._data = self.ds.read(masked=self._masked, **kwargs)
-            bands = self.ds.indexes
-        else:
-            self._data = self.ds.read(bands, masked=self._masked, **kwargs)
-            if type(bands) is int:
-                bands = bands
-
-        # If ndim is 2, expand to 3
-        if self._data.ndim == 2:
-            self._data = np.expand_dims(self._data, 0)
-
-        self.nbands = self._data.shape[0]
-        self.is_loaded = True
-        self.bands = bands
+        # Get the array with masked value fill with NaNs
+        nanarray = self.data.filled(fill_value=np.nan).squeeze()
+
+        # The function np.ma.filled() only returns a copy if the array is masked, copy the array if it's not the case
+        if not np.ma.is_masked(self.data):
+            nanarray = np.copy(nanarray)
+
+        # Return the NaN array, and possibly the mask as well
+        if return_mask:
+            return nanarray, np.copy(np.ma.getmaskarray(self.data).squeeze())
+        else:
+            return nanarray
+
+    def __array__(self) -> np.ndarray:
+        """Method to cast np.array() or np.asarray() function directly on Raster classes."""
+
+        return self._data
+
+    def __array_ufunc__(
+        self,
+        ufunc: Callable[[np.ndarray | tuple[np.ndarray, np.ndarray]], np.ndarray | tuple[np.ndarray, np.ndarray]],
+        method: str,
+        *inputs: Raster | tuple[Raster, Raster] | tuple[np.ndarray, Raster] | tuple[Raster, np.ndarray],
+        **kwargs: Any,
+    ) -> Raster | tuple[Raster, Raster]:
+        """
+        Method to cast NumPy universal functions directly on Raster classes, by passing to the masked array.
+        This function basically applies the ufunc (with its method and kwargs) to .data, and rebuilds the Raster from
+        self.__class__. The cases separate the number of input nin and output nout, to properly feed .data and return
+        Raster objects.
+        See more details in NumPy doc, e.g., https://numpy.org/doc/stable/user/basics.dispatch.html#basics-dispatch.
+        """
+
+        # In addition to running ufuncs, this function takes over arithmetic operations (__add__, __multiply__, etc...)
+        # when the first input provided is a NumPy array and second input a Raster.
+
+        # The Raster ufuncs behave exactly as arithmetic operations (+, *, .) of NumPy masked array (call np.ma instead
+        # of np when available). There is an inconsistency when calling np.ma: operations return a full boolean mask
+        # even when there is no invalid value (true_divide and floor_divide).
+        # We find one exception, however, for modulo: np.ma.remainder is not called but np.remainder instead one the
+        # masked array is the second input (an inconsistency in NumPy!), so we mirror this exception below:
+        if "remainder" in ufunc.__name__:
+            final_ufunc = getattr(ufunc, method)
+        else:
+            try:
+                final_ufunc = getattr(getattr(np.ma, ufunc.__name__), method)
+            except AttributeError:
+                final_ufunc = getattr(ufunc, method)
+
+        # If the universal function takes only one input
+        if ufunc.nin == 1:
+            # If the universal function has only one output
+            if ufunc.nout == 1:
+                return self.from_array(
+                    data=final_ufunc(inputs[0].data, **kwargs),  # type: ignore
+                    transform=self.transform,
+                    crs=self.crs,
+                    nodata=self.nodata,
+                )  # type: ignore
+
+            # If the universal function has two outputs (Note: no ufunc exists that has three outputs or more)
+            else:
+                output = final_ufunc(inputs[0].data, **kwargs)  # type: ignore
+                return self.from_array(
+                    data=output[0], transform=self.transform, crs=self.crs, nodata=self.nodata
+                ), self.from_array(data=output[1], transform=self.transform, crs=self.crs, nodata=self.nodata)
+
+        # If the universal function takes two inputs (Note: no ufunc exists that has three inputs or more)
+        else:
+            if ufunc.nout == 1:
+                return self.from_array(
+                    data=final_ufunc(inputs[0].data, inputs[1].data, **kwargs),  # type: ignore
+                    transform=self.transform,
+                    crs=self.crs,
+                    nodata=self.nodata,
+                )
+
+            # If the universal function has two outputs (Note: no ufunc exists that has three outputs or more)
+            else:
+                output = final_ufunc(inputs[0].data, inputs[1].data, **kwargs)  # type: ignore
+                return self.from_array(
+                    data=output[0], transform=self.transform, crs=self.crs, nodata=self.nodata
+                ), self.from_array(data=output[1], transform=self.transform, crs=self.crs, nodata=self.nodata)
+
+    def __array_function__(
+        self, func: Callable[[np.ndarray, Any], Any], types: tuple[type], args: Any, kwargs: Any
+    ) -> Any:
+        """
+        Method to cast NumPy array function directly on a Raster object by applying it to the masked array.
+        A limited number of function is supported, listed in raster._HANDLED_FUNCTIONS.
+        """
+
+        # If function is not implemented
+        if func.__name__ not in _HANDLED_FUNCTIONS:
+            return NotImplemented
+
+        # For subclassing
+        if not all(issubclass(t, self.__class__) for t in types):
+            return NotImplemented
+
+        # We now choose the behaviour of array functions
+        # For median, np.median ignores masks of masked array, so we force np.ma.median
+        if func.__name__ in ["median", "nanmedian"]:
+            func = np.ma.median
+            first_arg = args[0].data
+
+        # For percentiles and quantiles, there exist no masked array version, so we compute on the valid data directly
+        elif func.__name__ in ["percentile", "nanpercentile"]:
+            first_arg = args[0].data.compressed()
+
+        elif func.__name__ in ["quantile", "nanquantile"]:
+            first_arg = args[0].data.compressed()
+
+        # Otherwise, we run the numpy function normally (most take masks into account)
+        else:
+            first_arg = args[0].data
+
+        return func(first_arg, *args[1:], **kwargs)  # type: ignore
+
+    # Note the star is needed because of the default argument 'mode' preceding non default arg 'inplace'
+    # Then the final overload must be duplicated
+    @overload
+    def crop(
+        self: RasterType,
+        cropGeom: RasterType | Vector | list[float] | tuple[float, ...],
+        mode: Literal["match_pixel"] | Literal["match_extent"] = "match_pixel",
+        *,
+        inplace: Literal[True],
+    ) -> None:
+        ...
+
+    @overload
+    def crop(
+        self: RasterType,
+        cropGeom: RasterType | Vector | list[float] | tuple[float, ...],
+        mode: Literal["match_pixel"] | Literal["match_extent"] = "match_pixel",
+        *,
+        inplace: Literal[False],
+    ) -> RasterType:
+        ...
+
+    @overload
+    def crop(
+        self: RasterType,
+        cropGeom: RasterType | Vector | list[float] | tuple[float, ...],
+        mode: Literal["match_pixel"] | Literal["match_extent"] = "match_pixel",
+        inplace: bool = True,
+    ) -> RasterType | None:
+        ...
 
     def crop(
         self: RasterType,
-        cropGeom: Raster | Vector | list[float] | tuple[float, ...],
-        mode: str = "match_pixel",
+        cropGeom: RasterType | Vector | list[float] | tuple[float, ...],
+        mode: Literal["match_pixel"] | Literal["match_extent"] = "match_pixel",
         inplace: bool = True,
     ) -> RasterType | None:
         """
         Crop the Raster to a given extent.
 
         :param cropGeom: Geometry to crop raster to, as either a Raster object, a Vector object, or a list of
             coordinates. If cropGeom is a Raster, crop() will crop to the boundary of the raster as returned by
@@ -941,81 +1334,71 @@
         if isinstance(cropGeom, (Raster, Vector)):
             xmin, ymin, xmax, ymax = cropGeom.bounds
         elif isinstance(cropGeom, (list, tuple)):
             xmin, ymin, xmax, ymax = cropGeom
         else:
             raise ValueError("cropGeom must be a Raster, Vector, or list of coordinates.")
 
-        meta = copy.copy(self.ds.meta)
-
         if mode == "match_pixel":
-            crop_bbox = Polygon([(xmin, ymin), (xmax, ymin), (xmax, ymax), (xmin, ymax)])
-
-            crop_img, tfm = rio.mask.mask(self.ds, [crop_bbox], crop=True, all_touched=True)
-            meta.update(
-                {
-                    "height": crop_img.shape[1],
-                    "width": crop_img.shape[2],
-                    "transform": tfm,
-                }
-            )
-
-        else:
-            window = rio.windows.from_bounds(xmin, ymin, xmax, ymax, transform=self.transform)
-            new_height = int(window.height)
-            new_width = int(window.width)
-            new_tfm = rio.transform.from_bounds(xmin, ymin, xmax, ymax, width=new_width, height=new_height)
+            ref_win = rio.windows.from_bounds(xmin, ymin, xmax, ymax, transform=self.transform)
+            self_win = rio.windows.from_bounds(*self.bounds, transform=self.transform)
+            final_window = ref_win.intersection(self_win).round_lengths().round_offsets()
+            new_xmin, new_ymin, new_xmax, new_ymax = rio.windows.bounds(final_window, transform=self.transform)
+            tfm = rio.transform.from_origin(new_xmin, new_ymax, *self.res)
 
             if self.is_loaded:
-                new_img = np.zeros((self.nbands, new_height, new_width), dtype=self.data.dtype)
+                (rowmin, rowmax), (colmin, colmax) = final_window.toranges()
+                crop_img = self.data[:, rowmin:rowmax, colmin:colmax]
             else:
-                new_img = np.zeros((self.count, new_height, new_width), dtype=self.data.dtype)
+                with rio.open(self.filename) as raster:
+                    crop_img = raster.read(
+                        self._bands,
+                        masked=self._masked,
+                        window=final_window,
+                    )
 
-            crop_img, tfm = rio.warp.reproject(
-                self.data,
-                new_img,
-                src_transform=self.transform,
-                dst_transform=new_tfm,
-                src_crs=self.crs,
-                dst_crs=self.crs,
-            )
-            meta.update({"height": new_height, "width": new_width, "transform": tfm})
+        else:
+            bbox = rio.coords.BoundingBox(left=xmin, bottom=ymin, right=xmax, top=ymax)
+            out_rst = self.reproject(dst_bounds=bbox)  # should we instead raise an issue and point to reproject?
+            crop_img = out_rst.data
+            tfm = out_rst.transform
 
         if inplace:
-            self._update(crop_img, meta)
+            self._data = crop_img
+            self.transform = tfm
+            self.tags["AREA_OR_POINT"] = "Area"  # TODO: Explain why this should have an area interpretation now
             return None
         else:
-            return self.from_array(crop_img, meta["transform"], meta["crs"], meta["nodata"])
+            newraster = self.from_array(crop_img, tfm, self.crs, self.nodata)
+            newraster.tags["AREA_OR_POINT"] = "Area"
+            return newraster
 
     def reproject(
         self: RasterType,
         dst_ref: RasterType | rio.io.Dataset | str | None = None,
         dst_crs: CRS | str | None = None,
         dst_size: tuple[int, int] | None = None,
         dst_bounds: dict[str, float] | rio.coords.BoundingBox | None = None,
         dst_res: float | abc.Iterable[float] | None = None,
-        dst_nodata: int | float | None = None,
-        src_nodata: int | float | None = None,
+        dst_nodata: int | float | list[int] | list[float] | None = None,
+        src_nodata: int | float | list[int] | list[float] | None = None,
         dtype: np.dtype | None = None,
         resampling: Resampling | str = Resampling.bilinear,
         silent: bool = False,
         n_threads: int = 0,
         memory_limit: int = 64,
     ) -> RasterType:
         """
         Reproject raster to a specified grid.
 
         The output grid can either be given by a reference Raster (using `dst_ref`),
         or by manually providing the output CRS (`dst_crs`), dimensions (`dst_size`),
         resolution (with `dst_size`) and/or bounds (`dst_bounds`).
         Any resampling algorithm implemented in rasterio can be used.
 
-        Currently: requires image data to have been loaded into memory.
-        NOT SUITABLE for large datasets yet! This requires work...
-
         To reproject a Raster with different source bounds, first run Raster.crop.
 
         :param dst_ref: a reference raster. If set will use the attributes of this
             raster for the output grid. Can be provided as Raster/rasterio data set or as path to the file.
         :param crs: Specify the Coordinate Reference System to reproject to. If dst_ref not set, defaults to self.crs.
         :param dst_size: Raster size to write to (x, y). Do not use with dst_res.
         :param dst_bounds: a BoundingBox object or a dictionary containing\
@@ -1078,15 +1461,29 @@
             src_nodata = self.nodata
 
         # Set destination nodata if provided. This is needed in areas not covered by the input data.
         # If None, will use GeoUtils' default, as rasterio's default is unknown, hence cannot be handled properly.
         if dst_nodata is None:
             dst_nodata = self.nodata
             if dst_nodata is None:
-                dst_nodata = _default_ndv(dtype)
+                dst_nodata = _default_nodata(dtype)
+                # if dst_nodata is already being used, raise a warning.
+                # TODO: for uint8, if all values are used, apply rio.warp to mask to identify invalid values
+                if not self.is_loaded:
+                    warnings.warn(
+                        f"For reprojection, dst_nodata must be set. Setting default nodata to {dst_nodata}. You may "
+                        f"set a different nodata with `dst_nodata`."
+                    )
+
+                elif dst_nodata in self.data:
+                    warnings.warn(
+                        f"For reprojection, dst_nodata must be set. Default chosen value {dst_nodata} exists in "
+                        f"self.data. This may have unexpected consequences. Consider setting a different nodata with "
+                        f"self.set_nodata()."
+                    )
 
         from geoutils.misc import resampling_method_from_str
 
         # Basic reprojection options, needed in all cases.
         reproj_kwargs = {
             "src_transform": self.transform,
             "src_crs": self.crs,
@@ -1168,55 +1565,66 @@
         # Check that reprojection is actually needed
         # Caution, dst_size is (width, height) while shape is (height, width)
         if all(
             [
                 (dst_transform == self.transform) or (dst_transform is None),
                 (dst_crs == self.crs) or (dst_crs is None),
                 (dst_size == self.shape[::-1]) or (dst_size is None),
-                (dst_res == self.res) or (dst_res == self.res[0] == self.res[1]) or (dst_res is None),
+                np.all(dst_res == self.res) or (dst_res == self.res[0] == self.res[1]) or (dst_res is None),
             ]
         ):
             if (dst_nodata == self.nodata) or (dst_nodata is None):
                 if not silent:
                     warnings.warn("Output projection, bounds and size are identical -> return self (not a copy!)")
                 return self
 
             elif dst_nodata is not None:
                 if not silent:
                     warnings.warn(
-                        "Only nodata is different, consider using the 'set_ndv()' method instead'\
+                        "Only nodata is different, consider using the 'set_nodata()' method instead'\
                     ' -> return self (not a copy!)"
                     )
                 return self
 
         # Set the performance keywords
         if n_threads == 0:
             # Default to cpu count minus one. If the cpu count is undefined, num_threads will be 1
             cpu_count = os.cpu_count() or 2
             num_threads = cpu_count - 1
         else:
             num_threads = n_threads
         reproj_kwargs.update({"num_threads": num_threads, "warp_mem_limit": memory_limit})
 
         # If data is loaded, reproject the numpy array directly
-        if self.data is not None:
-            dst_data, dst_transformed = rio.warp.reproject(self.data, **reproj_kwargs)
+        if self.is_loaded:
+
+            # All masked values must be set to a nodata value for rasterio's reproject to work properly
+            # TODO: another option is to apply rio.warp.reproject to the mask to identify invalid pixels
+            if src_nodata is None and np.sum(self.data.mask) > 0:
+                raise ValueError("No nodata set, use `src_nodata`.")
+
+            # Mask not taken into account by rasterio, need to fill with src_nodata
+            dst_data, dst_transformed = rio.warp.reproject(self.data.filled(src_nodata), **reproj_kwargs)
 
         # If not, uses the dataset instead
         else:
             dst_data = []
             for k in range(self.count):
-                band = rio.band(self.ds, k + 1)
-                dst_band, dst_transformed = rio.warp.reproject(band, **reproj_kwargs)
-                dst_data.append(dst_band.squeeze())
+                with rio.open(self.filename) as ds:
+                    band = rio.band(ds, k + 1)
+                    dst_band, dst_transformed = rio.warp.reproject(band, **reproj_kwargs)
+                    dst_data.append(dst_band.squeeze())
 
             dst_data = np.array(dst_data)
 
         # Enforce output type
-        dst_data = dst_data.astype(dtype)
+        dst_data = np.ma.masked_array(dst_data.astype(dtype), fill_value=dst_nodata)
+
+        if dst_nodata is not None:
+            dst_data.mask = dst_data == dst_nodata
 
         # Check for funny business.
         if dst_transform is not None:
             assert dst_transform == dst_transformed
 
         # Write results to a new Raster.
         dst_r = self.from_array(dst_data, dst_transformed, dst_crs, dst_nodata)
@@ -1228,82 +1636,17 @@
         Translate the Raster by a given x,y offset.
 
         :param xoff: Translation x offset.
         :param yoff: Translation y offset.
 
 
         """
-        # Check that data is loaded, as it is necessary for this method
-        assert self.is_loaded, "Data must be loaded, use self.load"
-
-        meta = self.ds.meta
         dx, b, xmin, d, dy, ymax = list(self.transform)[:6]
 
-        meta.update({"transform": rio.transform.Affine(dx, b, xmin + xoff, d, dy, ymax + yoff)})
-        self._update(metadata=meta)
-
-    def set_ndv(self, ndv: abc.Sequence[int | float] | int | float, update_array: bool = False) -> None:
-        """
-        Set new nodata values for bands (and possibly update arrays).
-
-        :param ndv: nodata values
-        :param update_array: change the existing nodata in array
-        """
-
-        if not isinstance(ndv, (abc.Sequence, int, float, np.integer, np.floating)):
-            raise ValueError("Type of ndv not understood, must be list or float or int")
-
-        elif (isinstance(ndv, (int, float, np.integer, np.floating))) and self.count > 1:
-            print("Several raster band: using nodata value for all bands")
-            ndv = [ndv] * self.count
-
-        elif isinstance(ndv, abc.Sequence) and self.count == 1:
-            print("Only one raster band: using first nodata value provided")
-            ndv = list(ndv)[0]
-
-        # Check that ndv has same length as number of bands in self
-        if isinstance(ndv, abc.Sequence):
-            if len(ndv) != self.count:
-                raise ValueError(f"Length of ndv ({len(ndv)}) incompatible with number of bands ({self.count})")
-            # Check that ndv value is compatible with dtype
-            for k in range(len(ndv)):
-                if not rio.dtypes.can_cast_dtype(ndv[k], self.dtypes[k]):
-                    raise ValueError(f"ndv value {ndv[k]} incompatible with self.dtype {self.dtypes[k]}")
-        else:
-            if not rio.dtypes.can_cast_dtype(ndv, self.dtypes[0]):
-                raise ValueError(f"ndv value {ndv} incompatible with self.dtype {self.dtypes[0]}")
-
-        meta = self.ds.meta
-        imgdata = self.data
-        pre_ndv = self.nodata
-
-        meta.update({"nodata": ndv})
-
-        if update_array and pre_ndv is not None:
-            # nodata values are specific to each band
-
-            # let's do a loop then
-            if self.count == 1:
-                if np.ma.isMaskedArray(imgdata):
-                    imgdata.data[imgdata.mask] = ndv  # type: ignore
-                else:
-                    ind = imgdata[:] == pre_ndv
-                    imgdata[ind] = ndv
-            else:
-                # At this point, ndv is definitely iterable, but mypy doesn't understand that.
-                for i in range(self.count):
-                    if np.ma.isMaskedArray(imgdata):
-                        imgdata.data[i, imgdata.mask[i, :]] = ndv[i]  # type: ignore
-                    else:
-                        ind = imgdata[i, :] == pre_ndv[i]  # type: ignore
-                        imgdata[i, ind] = ndv[i]  # type: ignore
-        else:
-            imgdata = None
-
-        self._update(metadata=meta, imgdata=imgdata)
+        self.transform = rio.transform.Affine(dx, b, xmin + xoff, d, dy, ymax + yoff)
 
     def save(
         self,
         filename: str | IO[bytes],
         driver: str = "GTiff",
         dtype: DTypeLike | None = None,
         nodata: AnyNumber | None = None,
@@ -1354,39 +1697,40 @@
         # Use nodata set by user, otherwise default to self's
         nodata = nodata if nodata is not None else self.nodata
 
         if (self.data is None) & (blank_value is None):
             raise AttributeError("No data loaded, and alternative blank_value not set.")
         elif blank_value is not None:
             if isinstance(blank_value, int) | isinstance(blank_value, float):
-                save_data = np.zeros((self.ds.count, self.ds.height, self.ds.width))
+                save_data = np.zeros(self.data.shape)
                 save_data[:, :, :] = blank_value
             else:
                 raise ValueError("blank_values must be one of int, float (or None).")
         else:
             save_data = self.data
 
             # if masked array, save with masked values replaced by nodata
-            # In this case, nodata = None is not compatible, so revert to default values
-            if isinstance(save_data, np.ma.masked_array) & (np.count_nonzero(save_data.mask) > 0):
-                if nodata is None:
-                    nodata = _default_ndv(save_data.dtype)
+            if isinstance(save_data, np.ma.masked_array):
+
+                # In this case, nodata=None is not compatible, so revert to default values, only if masked values exist
+                if (nodata is None) & (np.count_nonzero(save_data.mask) > 0):
+                    nodata = _default_nodata(save_data.dtype)
                     warnings.warn(f"No nodata set, will use default value of {nodata}")
                 save_data = save_data.filled(nodata)
 
         with rio.open(
             filename,
             "w",
             driver=driver,
-            height=self.ds.height,
-            width=self.ds.width,
-            count=self.ds.count,
+            height=self.height,
+            width=self.width,
+            count=self.count,
             dtype=save_data.dtype,
-            crs=self.ds.crs,
-            transform=self.ds.transform,
+            crs=self.crs,
+            transform=self.transform,
             nodata=nodata,
             compress=compress,
             tiled=tiled,
             **co_opts,
         ) as dst:
 
             dst.write(save_data)
@@ -1401,18 +1745,15 @@
             if len(gcps) > 0:
                 rio_gcps = []
                 for gcp in gcps:
                     rio_gcps.append(rio.control.GroundControlPoint(*gcp))
 
                 # Warning: this will overwrite the transform
                 if dst.transform != rio.transform.Affine(1, 0, 0, 0, 1, 0):
-                    warnings.warn(
-                        "A geotransform previously set is going \
-to be cleared due to the setting of GCPs."
-                    )
+                    warnings.warn("A geotransform previously set is going to be cleared due to the setting of GCPs.")
 
                 dst.gcps = (rio_gcps, gcps_crs)
 
     def to_xarray(self, name: str | None = None) -> rioxarray.DataArray:
         """Convert this Raster into an xarray DataArray using rioxarray.
 
         This method uses rioxarray to generate a DataArray with associated
@@ -1448,61 +1789,54 @@
         # rasterio's default is a bit low for very large images
         # instead, use image dimensions, with a maximum of 50000
         densify_pts = min(max(self.width, self.height), densify_pts_max)
 
         # Calculate new bounds
         left, bottom, right, top = self.bounds
         new_bounds = rio.warp.transform_bounds(self.crs, out_crs, left, bottom, right, top, densify_pts)
+        new_bounds = rio.coords.BoundingBox(*new_bounds)
 
         return new_bounds
 
-    def intersection(self, rst: str | Raster) -> tuple[float, float, float, float]:
+    def intersection(self, rst: str | Raster, match_ref: bool = True) -> tuple[float, float, float, float]:
         """
         Returns the bounding box of intersection between this image and another.
 
         If the rasters have different projections, the intersection extent is given in self's projection system.
 
         :param rst : path to the second image (or another Raster instance)
-
+        :param match_ref: if set to True, returns the smallest intersection that aligns with that of self, i.e. same \
+        resolution and offset with self's origin is a multiple of the resolution
         :returns: extent of the intersection between the 2 images \
         (xmin, ymin, xmax, ymax) in self's coordinate system.
 
         """
         from geoutils import projtools
 
         # If input rst is string, open as Raster
         if isinstance(rst, str):
             rst = Raster(rst, load_data=False)
 
-        # Check if both files have the same projection
-        # To be implemented
-        same_proj = True
-
-        # Find envelope of rasters' intersections
-        poly1 = projtools.bounds2poly(self.bounds)
-        # poly1.AssignSpatialReference(self.crs)
-
-        # Create a polygon of the envelope of the second image
-        poly2 = projtools.bounds2poly(rst.bounds)
-        # poly2.AssignSpatialReference(rst.srs)
-
-        # If coordinate system is different, reproject poly2 into poly1
-        if not same_proj:
-            raise NotImplementedError()
-
-        # Compute intersection envelope
-        intersect = poly1.intersection(poly2)
-        extent: tuple[float, float, float, float] = intersect.envelope.bounds
-
-        # check that intersection is not void
-        if intersect.area == 0:
-            warnings.warn("Warning: Intersection is void")
+        # Reproject the bounds of rst to self's
+        rst_bounds_sameproj = rst.get_bounds_projected(self.crs)
+
+        # Calculate intersection of bounding boxes
+        intersection = projtools.merge_bounds([self.bounds, rst_bounds_sameproj], merging_algorithm="intersection")
+
+        # check that intersection is not void, otherwise return 0 everywhere
+        if intersection == ():
+            warnings.warn("Intersection is void")
             return (0.0, 0.0, 0.0, 0.0)
 
-        return extent
+        # if required, ensure the intersection is aligned with self's georeferences
+        if match_ref:
+            intersection = projtools.align_bounds(self.transform, intersection)
+
+        # mypy raises a type issue, not sure how to address the fact that output of merge_bounds can be ()
+        return intersection  # type: ignore
 
     def show(
         self,
         band: int | None = None,
         cmap: matplotlib.colors.Colormap | str | None = None,
         vmin: float | int | None = None,
         vmax: float | int | None = None,
@@ -1661,15 +1995,15 @@
         :returns: If multiple band Raster and the band is not specified, a \
             dictionary containing the value of the pixel in each band.
         :returns: In addition, if return_window=True, return tuple of \
             (values, arrays)
 
         :examples:
 
-            >>> self.value_at_coords(-48.125,67.8901,window=3)  # doctest: +SKIP
+            >>> self.value_at_coords(-48.125, 67.8901, window=3)  # doctest: +SKIP
             Returns mean of a 3*3 window:
                 v v v \
                 v c v  | = float(mean)
                 v v v /
             (c = provided coordinate, v= value of surrounding coordinate)
 
         """
@@ -1692,15 +2026,15 @@
         # Need to implement latlon option later
         if latlon:
             from geoutils import projtools
 
             x, y = projtools.reproject_from_latlon((y, x), self.crs)
 
         # Convert coordinates to pixel space
-        row, col = self.ds.index(x, y, op=round)
+        row, col = rio.transform.rowcol(self.transform, x, y, op=round)
 
         # Decide what pixel coordinates to read:
         if window is not None:
             half_win = (window - 1) / 2
             # Subtract start coordinates back to top left of window
             col = col - half_win
             row = row - half_win
@@ -1715,58 +2049,36 @@
         # Make sure coordinates are int
         col = int(col)
         row = int(row)
 
         # Create rasterio's window for reading
         window = rio.windows.Window(col, row, width, height)
 
-        # Get values for all bands
-        if band is None:
+        if self.is_loaded:
+            data = self.data[slice(None) if band is None else band + 1, row : row + height, col : col + width]
+            value = format_value(data)
+            win: np.ndarray | dict[int, np.ndarray] = data
 
-            # Deal with single band case
+        else:
             if self.nbands == 1:
-                data = self.ds.read(
-                    window=window,
-                    fill_value=self.nodata,
-                    boundless=boundless,
-                    masked=masked,
-                )
+                with rio.open(self.filename) as raster:
+                    data = raster.read(window=window, fill_value=self.nodata, boundless=boundless, masked=masked)
                 value = format_value(data)
                 win = data
-
-            # Deal with multiband case
             else:
                 value = {}
                 win = {}
-
-                for b in self.indexes:
-                    data = self.ds.read(
-                        window=window,
-                        fill_value=self.nodata,
-                        boundless=boundless,
-                        indexes=b,
-                        masked=masked,
-                    )
-                    val = format_value(data)
-                    # Store according to GDAL band numbers
-                    value[b] = val
-                    win[b] = data
-
-        # Or just for specified band in multiband case
-        elif isinstance(band, int):
-            data = self.ds.read(
-                window=window,
-                fill_value=self.nodata,
-                boundless=boundless,
-                indexes=band,
-                masked=masked,
-            )
-            value = format_value(data)
-        else:
-            raise ValueError("Value provided for band was not int or None.")
+                with rio.open(self.filename) as raster:
+                    for b in self.indexes:
+                        data = raster.read(
+                            window=window, fill_value=self.nodata, boundless=boundless, masked=masked, indexes=b
+                        )
+                        val = format_value(data)
+                        value[b] = val
+                        win[b] = data  # type: ignore
 
         if return_window:
             return (value, win)
 
         return value
 
     def coords(self, offset: str = "corner", grid: bool = True) -> tuple[np.ndarray, np.ndarray]:
@@ -1828,15 +2140,15 @@
                 "return unreliable indexes due to rounding issues."
             )
         if area_or_point not in [None, "Area", "Point"]:
             raise ValueError(
                 'Argument "area_or_point" must be either None (falls back to GDAL metadata), "Point" or "Area".'
             )
 
-        i, j = self.ds.index(x, y, op=op, precision=precision)
+        i, j = rio.transform.rowcol(self.transform, x, y, op=op, precision=precision)
 
         # # necessary because rio.Dataset.index does not return abc.Iterable for a single point
         if not isinstance(i, abc.Iterable):
             i, j = (
                 np.asarray(
                     [
                         i,
@@ -1854,15 +2166,15 @@
         # AREA_OR_POINT GDAL attribute, i.e. does the value refer to the upper left corner (AREA) or
         # the center of pixel (POINT)
         # This has no influence on georeferencing, it's only about the interpretation of the raster values,
         # and thus only affects sub-pixel interpolation
 
         # if input is None, default to GDAL METADATA
         if area_or_point is None:
-            area_or_point = self.ds.tags()["AREA_OR_POINT"]
+            area_or_point = self.tags.get("AREA_OR_POINT", "Point")
 
         if area_or_point == "Point":
             if not isinstance(i.flat[0], np.floating):
                 raise ValueError(
                     "Operator must return np.floating values to perform AREA_OR_POINT subpixel index shifting"
                 )
 
@@ -1880,15 +2192,15 @@
         :param i: row (i) index of pixel.
         :param j: column (j) index of pixel.
         :param offset: return coordinates as "corner" or "center" of pixel
 
         :returns x, y: x,y coordinates of i,j in reference system.
         """
 
-        x, y = self.ds.xy(i, j, offset=offset)
+        x, y = rio.transform.xy(self.transform, i, j, offset=offset)
 
         return x, y
 
     def outside_image(self, xi: ArrayLike, yj: ArrayLike, index: bool = True) -> bool:
         """
         Check whether a given point falls outside of the raster.
 
@@ -2014,28 +2326,27 @@
             raise ValueError(f"'subset' got invalid type: {type(subset)}. Expected list[int], int or None")
 
         if copy:
             for band_n in indices:
                 # Generate a new Raster from a copy of the band's data
                 bands.append(
                     self.from_array(
-                        self.data[band_n, :, :],
+                        self.data[band_n, :, :].copy(),
                         transform=self.transform,
                         crs=self.crs,
                         nodata=self.nodata,
                     )
                 )
         else:
             for band_n in indices:
                 # Generate a new instance with the same underlying values.
                 raster = Raster(self)
                 # Set the data to a slice of the original array
                 raster._data = self.data[band_n, :, :].reshape((1,) + self.data.shape[1:])
                 # Set the nbands
-                raster.nbands = 1
                 bands.append(raster)
 
         return bands
 
     @overload
     def to_points(
         self, subset: float | int, as_frame: Literal[True], pixel_offset: Literal["center", "corner"]
@@ -2093,15 +2404,16 @@
         # Extract the coordinates of the pixels and filter by the chosen pixels.
         x_coords, y_coords = (np.array(a) for a in self.ij2xy(rows, cols, offset=pixel_offset))
 
         # If the Raster is loaded, pick from the data, otherwise use the disk-sample method from rasterio.
         if self.is_loaded:
             pixel_data = self.data[:, rows, cols]
         else:
-            pixel_data = np.array(list(self.ds.sample(zip(x_coords, y_coords)))).T
+            with rio.open(self.filename) as raster:
+                pixel_data = np.array(list(raster.sample(zip(x_coords, y_coords)))).T
 
         if isinstance(pixel_data, np.ma.masked_array):
             pixel_data = np.where(pixel_data.mask, np.nan, pixel_data.data)
 
         # Merge the coordinates and pixel data into a point cloud.
         points = np.vstack((x_coords.reshape(1, -1), y_coords.reshape(1, -1), pixel_data)).T
```

### Comparing `geoutils-0.0.8/geoutils/geovector.py` & `geoutils-0.0.9/geoutils/geovector.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 hence one geometry "steps" slightly on the neighbor buffer in some cases.
         The algorithm may also yield unexpected results on very simple geometries.
 
         Note: A similar functionality is provided by momepy (http://docs.momepy.org) and is probably more robust.
         It could be implemented in GeoPandas in the future: https://github.com/geopandas/geopandas/issues/2015
 
         :examples:
-        >>> outlines = gu.Vector(gu.datasets.get_path('glacier_outlines'))
+        >>> outlines = gu.Vector(gu.examples.get_path('everest_rgi_outlines'))
         >>> outlines = gu.Vector(outlines.ds.to_crs('EPSG:32645'))
         >>> buffer = outlines.buffer_without_overlap(500)
         >>> ax = buffer.ds.plot()  # doctest: +SKIP
         >>> outlines.ds.plot(ax=ax, ec='k', fc='none')  # doctest: +SKIP
         >>> plt.show()  # doctest: +SKIP
 
         :param buffer_size: Buffer size in self's coordinate system units.
```

### Comparing `geoutils-0.0.8/geoutils/geoviewer.py` & `geoutils-0.0.9/geoutils/geoviewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         nodata = img.nodata
     else:
         try:
             nodata = float(args.nodata)
         except ValueError:
             raise ValueError("ERROR: nodata must be a float, currently set to %s" % args.nodata)
 
-        img.set_ndv(nodata)
+        img.set_nodata(nodata)
 
     # Set default parameters #
 
     # vmin
     if args.vmin is not None:
         try:
             vmin: float | None = float(args.vmin)
```

### Comparing `geoutils-0.0.8/geoutils/projtools.py` & `geoutils-0.0.9/geoutils/projtools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
-GeoUtils.projtools provides a toolset for dealing with different coordinate reference systems (CRS).
+projtools provides a set of tools for dealing with different coordinate reference systems (CRS) and bounds.
 """
 from __future__ import annotations
 
 from collections import abc
+from math import ceil, floor
 
 import geopandas as gpd
 import numpy as np
 import pyproj
 import rasterio as rio
 import shapely.ops
 from rasterio.crs import CRS
@@ -29,17 +30,14 @@
     :param boundsGeom: A geometry with bounds. Can be either a list of coordinates (xmin, ymin, xmax, ymax),\
             a rasterio/Raster object, a geoPandas/Vector object
     :param in_crs: Input CRS
     :param out_crs: Output CRS
 
     :returns: Output polygon
     """
-    if in_crs is not None:
-        raise NotImplementedError
-
     # If boundsGeom is a GeoPandas or Vector object (warning, has both total_bounds and bounds attributes)
     if hasattr(boundsGeom, "total_bounds"):
         xmin, ymin, xmax, ymax = boundsGeom.total_bounds  # type: ignore
         in_crs = boundsGeom.crs  # type: ignore
     # If boundsGeom is a rasterio or Raster object
     elif hasattr(boundsGeom, "bounds"):
         xmin, ymin, xmax, ymax = boundsGeom.bounds  # type: ignore
@@ -48,18 +46,20 @@
     elif isinstance(boundsGeom, (list, tuple)):
         xmin, ymin, xmax, ymax = boundsGeom
     else:
         raise ValueError(
             "boundsGeom must a list/tuple of coordinates or an object with attributes bounds or total_bounds."
         )
 
-    bbox = Polygon([(xmin, ymin), (xmax, ymin), (xmax, ymax), (xmin, ymax)])
+    corners = ((xmin, ymin), (xmax, ymin), (xmax, ymax), (xmin, ymax))
+
+    if (in_crs is not None) & (out_crs is not None):
+        corners = np.transpose(reproject_points(np.transpose(corners), in_crs, out_crs))
 
-    if out_crs is not None:
-        raise NotImplementedError()
+    bbox = Polygon(corners)
 
     return bbox
 
 
 def merge_bounds(
     bounds_list: abc.Iterable[list[float] | Raster | rio.io.DatasetReader | Vector | gpd.GeoDataFrame],
     merging_algorithm: str = "union",
@@ -67,15 +67,15 @@
     """
     Merge a list of bounds into single bounds, using either the union or intersection.
 
     :param bounds_list: A list of geometries with bounds, i.e. a list of coordinates (xmin, ymin, xmax, ymax), \
 a rasterio/Raster object, a geoPandas/Vector object.
     :param merging_algorithm: the algorithm to use for merging, either "union" or "intersection"
 
-    :returns: Output bounds (xmin, ymin, xmax, ymax)
+    :returns: Output bounds (xmin, ymin, xmax, ymax) or empty tuple
     """
     # Check that bounds_list is a list of bounds objects
     assert isinstance(bounds_list, (list, tuple)), "bounds_list must be a list/tuple"
     for bounds in bounds_list:
         assert hasattr(bounds, "bounds") or hasattr(bounds, "total_bounds") or isinstance(bounds, (list, tuple)), (
             "bounds_list must be a list of lists/tuples of coordinates or an object with attributes bounds "
             "or total_bounds"
@@ -93,14 +93,44 @@
         else:
             raise ValueError("merging_algorithm must be 'union' or 'intersection'")
 
     new_bounds: tuple[float] = output_poly.bounds
     return new_bounds
 
 
+def align_bounds(
+    ref_transform: rio.transform.Affine,
+    src_bounds: rio.coords.BoundingBox | tuple[float, float, float, float],
+) -> tuple[float, float, float, float]:
+    """
+    Aligns the bounds in src_bounds so that it matches the georeferences in ref_transform
+    i.e. the distance between the upper-left pixels of ref and src is a multiple of resolution and
+    the width/height of the bounds are a multiple of resolution.
+    The bounds are padded so that the output bounds always contain the input bounds.
+
+    :param ref_transform: The transform of the dataset to be used as reference
+    :param src_bounds: The initial bounds that needs to be aligned to ref_transform. \
+    Must be a rasterio BoundingBox or list or tuple with coordinates (left, bottom, right, top).
+
+    :returns: the aligned bounding box (left, bottom, right, top)
+    """
+    left, bottom, right, top = src_bounds
+    xres = ref_transform.a
+    yres = ref_transform.e
+    ref_left = ref_transform.xoff
+    ref_top = ref_transform.yoff
+
+    left = ref_left + floor((left - ref_left) / xres) * xres
+    right = left + ceil((right - left) / xres) * xres
+    top = ref_top + floor((top - ref_top) / yres) * yres
+    bottom = top + ceil((bottom - top) / yres) * yres
+
+    return (left, bottom, right, top)
+
+
 def reproject_points(pts: list[list[float]] | np.ndarray, in_crs: CRS, out_crs: CRS) -> tuple[list[float], list[float]]:
     """
     Reproject a set of point from input_crs to output_crs.
 
     :param pts: Input points to be reprojected. Must be of shape (2, N), i.e (x coords, y coords)
     :param in_crs: Input CRS
     :param out_crs: Output CRS
```

### Comparing `geoutils-0.0.8/geoutils/satimg.py` & `geoutils-0.0.9/geoutils/satimg.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,14 @@
 
     def __init__(
         self,
         filename_or_dataset: str | RasterType | rio.io.DatasetReader | rio.io.MemoryFile,
         attrs: list[str] | None = None,
         load_data: bool = True,
         bands: int | list[int] | None = None,
-        as_memfile: bool = False,
         read_from_fn: bool = True,
         datetime: dt.datetime | None = None,
         tile_name: str | None = None,
         satellite: str | None = None,
         sensor: str | None = None,
         product: str | None = None,
         version: str | None = None,
@@ -260,15 +259,14 @@
 
         :param filename_or_dataset: The filename of the dataset.
         :param attrs: Additional attributes from rasterio's DataReader class to add to the Raster object.
            Default list is ['bounds', 'count', 'crs', 'dataset_mask', 'driver', 'dtypes', 'height', 'indexes',
            'name', 'nodata', 'res', 'shape', 'transform', 'width'] - if no attrs are specified, these will be added.
         :param load_data: Load the raster data into the object. Default is True.
         :param bands: The band(s) to load into the object. Default is to load all bands.
-        :param as_memfile: open the dataset via a rio.MemoryFile.
         :param read_from_fn: Try to read metadata from the filename
         :param datetime: Provide datetime attribute
         :param tile_name: Provide tile name
         :param satellite: Provide satellite name
         :param sensor: Provide sensor name
         :param product: Provide data product name
         :param version: Provide data version
@@ -282,15 +280,15 @@
         # If SatelliteImage is passed, simply point back to SatelliteImage
         if isinstance(filename_or_dataset, SatelliteImage):
             for key in filename_or_dataset.__dict__:
                 setattr(self, key, filename_or_dataset.__dict__[key])
             return
         # Else rely on parent Raster class options (including raised errors)
         else:
-            super().__init__(filename_or_dataset, attrs=attrs, load_data=load_data, bands=bands, as_memfile=as_memfile)
+            super().__init__(filename_or_dataset, attrs=attrs, load_data=load_data, bands=bands)
 
         # priority to user input
         self.datetime = datetime
         self.tile_name = tile_name
         self.satellite = satellite
         self.sensor = sensor
         self.product = product
```

### Comparing `geoutils-0.0.8/geoutils/spatial_tools.py` & `geoutils-0.0.9/geoutils/spatial_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 Optional dependencies:
     skimage.transform (@subdivide_array)
 
 """
 from __future__ import annotations
 
 import warnings
-from typing import Callable
+from typing import Any, Callable
 
 import numpy as np
 import rasterio as rio
 import rasterio.warp
 from tqdm import tqdm
 
 import geoutils as gu
 from geoutils.georaster import Raster, RasterType
-from geoutils.georaster.raster import _default_ndv
+from geoutils.georaster.raster import _default_nodata
 from geoutils.misc import resampling_method_from_str
 
 
 def get_mask(array: np.ndarray | np.ma.masked_array) -> np.ndarray:
     """
     Return the mask of invalid values, whether array is a ndarray with NaNs or a np.ma.masked_array.
 
@@ -84,14 +84,107 @@
     else:
         valid_mask = array
     cols_nonzero = np.where(np.count_nonzero(valid_mask, axis=0) > 0)[0]
     rows_nonzero = np.where(np.count_nonzero(valid_mask, axis=1) > 0)[0]
     return rows_nonzero[0], rows_nonzero[-1], cols_nonzero[0], cols_nonzero[-1]
 
 
+def load_multiple_rasters(
+    raster_paths: list[str], crop: bool = True, ref_grid: int | None = None, **kwargs: Any
+) -> list[RasterType]:
+    """
+    Function to load multiple rasters at once in a memory efficient way.
+    First load metadata only.
+    Optionally, crop all rasters to their intersection (default).
+    Optionally, reproject all rasters to the grid of one raster set as reference (after optional crop).
+    Otherwise, simply load the full rasters.
+
+    :param raster_paths: List of paths to the rasters to be loaded
+    :param crop: if set to True, will only load rasters in the area they intersect
+    :param ref_grid: If set to an integer value, the raster with that index will be considered as the reference
+    and all other rasters will be reprojected on the same grid (after optional crop)
+    :param kwargs: optional arguments to be passed to Raster.reproject, e.g. the resampling method
+
+    :returns: a list of loaded Raster instances
+    """
+    # If ref_grid is provided, need to reproject
+    if isinstance(ref_grid, int):
+        reproject = True
+    # if no ref_grid provided, still need a reference CRS, use first by default
+    elif ref_grid is None:
+        ref_grid = 0
+        reproject = False
+    else:
+        raise ValueError("`ref_grid` must be None or an integer")
+
+    # Need to define a reference CRS for calculating intersection
+    ref_crs = gu.Raster(raster_paths[ref_grid], load_data=False).crs
+
+    # First load all rasters metadata
+    output_rst = []
+    bounds = []
+    for path in raster_paths:
+        # Initialize raster
+        rst = gu.Raster(path, load_data=False)
+        output_rst.append(rst)
+
+        # Get bound in reference CRS
+        bound = rst.get_bounds_projected(ref_crs)
+        bounds.append(bound)
+
+    # Second get the intersection of all raster bounds
+    intersection = gu.projtools.merge_bounds(bounds, "intersection")
+
+    # Optionally, crop the rasters
+    if crop:
+        # Check that intersection is not void
+        if intersection == ():
+            warnings.warn("Intersection is void, returning unloaded rasters.")
+            return output_rst
+
+        for rst in output_rst:
+            # Calculate bounds in rst's CRS
+            # rasterio's default for densify_pts is too low for very large images, set a default of 5000
+            new_bounds = rio.warp.transform_bounds(
+                ref_crs, rst.crs, intersection[0], intersection[1], intersection[2], intersection[3], densify_pts=5000
+            )
+            # Ensure bounds align with the original ones, to avoid resampling at this stage
+            new_bounds = gu.projtools.align_bounds(rst.transform, new_bounds)
+            rst.crop(new_bounds, mode="match_pixel")
+
+    # Optionally, reproject all rasters to the reference grid
+    if reproject:
+
+        ref_rst = output_rst[ref_grid]
+
+        # Set output bounds - intersection if crop is True, otherwise use that of ref_grid
+        if crop:
+            # make sure new bounds align with reference's bounds (to avoid resampling ref)
+            new_bounds = intersection
+            new_bounds = gu.projtools.align_bounds(ref_rst.transform, intersection)
+        else:
+            new_bounds = ref_rst.bounds
+
+        # Reproject all rasters
+        for index, rst in enumerate(output_rst):
+            out_rst = rst.reproject(
+                dst_crs=ref_rst.crs, dst_bounds=new_bounds, dst_res=ref_rst.res, silent=True, **kwargs
+            )
+            if not out_rst.is_loaded:
+                out_rst.load()
+            output_rst[index] = out_rst
+
+    # if no crop or reproject option, simply load the rasters
+    if (not crop) & (not reproject):
+        for rst in output_rst:
+            rst.load()
+
+    return output_rst
+
+
 def merge_bounding_boxes(bounds: list[rio.coords.BoundingBox], resolution: float) -> rio.coords.BoundingBox:
     max_bounds = dict(zip(["left", "right", "top", "bottom"], [np.nan] * 4))
     for bound in bounds:
         for key in "right", "top":
             max_bounds[key] = np.nanmax([max_bounds[key], bound.__getattribute__(key)])
         for key in "bottom", "left":
             max_bounds[key] = np.nanmin([max_bounds[key], bound.__getattribute__(key)])
@@ -160,43 +253,45 @@
     for raster in tqdm(rasters, disable=not progress):
 
         # Check that data is loaded, otherwise temporarily load it
         if not raster.is_loaded:
             raster.load()
             raster.is_loaded = False
 
+        nodata = reference_raster.nodata or gu.georaster.raster._default_nodata(reference_raster.data.dtype)
         # Reproject to reference grid
         reprojected_raster = raster.reproject(
             dst_bounds=dst_bounds,
             dst_res=reference_raster.res,
             dst_crs=reference_raster.crs,
             dtype=reference_raster.data.dtype,
             dst_nodata=reference_raster.nodata,
             silent=True,
         )
+        reprojected_raster.set_nodata(nodata)
 
         # Optionally calculate difference
         if diff:
             diff_to_ref = (reference_raster.data - reprojected_raster.data).squeeze()
             diff_to_ref, _ = get_array_and_mask(diff_to_ref)
             data.append(diff_to_ref)
         else:
-            img_data, _ = get_array_and_mask(reprojected_raster.data.squeeze())
-            data.append(img_data)
+            # img_data, _ = get_array_and_mask(reprojected_raster.data.squeeze())
+            data.append(reprojected_raster.data.squeeze())
 
         # Remove unloaded rasters
         if not raster.is_loaded:
             raster._data = None
 
     # Convert to masked array
     data = np.ma.asarray(data)
     if reference_raster.nodata is not None:
         nodata = reference_raster.nodata
     else:
-        nodata = _default_ndv(data.dtype)
+        nodata = _default_nodata(data.dtype)
     data[np.isnan(data)] = nodata
 
     # Save as gu.Raster - needed as some child classes may not accept multiple bands
     r = gu.Raster.from_array(
         data=data,
         transform=rio.transform.from_bounds(*dst_bounds, width=data[0].shape[1], height=data[0].shape[0]),
         crs=reference_raster.crs,
@@ -275,15 +370,15 @@
             merged_data.append(np.apply_along_axis(algo, axis=0, arr=raster_stack.data))
 
     # Convert to masked array, and set all Nans to nodata
     merged_data = np.ma.asarray(merged_data)
     if reference_raster.nodata is not None:
         nodata = reference_raster.nodata
     else:
-        nodata = _default_ndv(merged_data.dtype)
+        nodata = _default_nodata(merged_data.dtype)
     merged_data[np.isnan(merged_data)] = nodata
 
     # Save as gu.Raster
     merged_raster = reference_raster.from_array(
         data=np.reshape(merged_data, (len(merged_data),) + merged_data[0].shape),
         transform=rio.transform.from_bounds(
             *raster_stack.bounds, width=merged_data[0].shape[1], height=merged_data[0].shape[0]
```

### Comparing `geoutils-0.0.8/geoutils.egg-info/PKG-INFO` & `geoutils-0.0.9/geoutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: geoutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for working with geospatial data
 Home-page: https://www.github.com/GlacioHack/geoutils/
 Author: The GlacioHack Team
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rioxarray
 License-File: LICENSE
 
-# GeoUtils
+# geoutils
 Set of tools to handle raster and vector data sets in Python.
 
 ![](https://readthedocs.org/projects/geoutils/badge/?version=latest)
-[![build](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml/badge.svg)](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml)
+[![build](https://github.com/GlacioHack/geoutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/GlacioHack/GeoUtils/actions/workflows/python-app.yml)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/geoutils.svg)](https://anaconda.org/conda-forge/geoutils)
 [![PyPI version](https://badge.fury.io/py/geoutils.svg)](https://badge.fury.io/py/geoutils)
+[![Coverage Status](https://coveralls.io/repos/github/GlacioHack/geoutils/badge.svg?branch=main)](https://coveralls.io/github/GlacioHack/geoutils?branch=main)
 
 This package offers Python classes and functions as well as command line tools to work with both geospatial raster and vector datasets. It is built upon rasterio and GeoPandas. In a single command it can import any geo-referenced dataset that is understood by these libraries, complete with all geo-referencing information, various helper functions and interface between vector/raster data.
 
 
 ## Installation
 
 #### With conda (recommended)
@@ -38,32 +40,32 @@
 From PyPI:
 ```bash
 pip install geoutils
 ```
 
 Or from the repository tarball: make sure GDAL and PROJ are properly installed, then:
 ```bash
-pip install https://github.com/GlacioHack/GeoUtils/tarball/main
+pip install https://github.com/GlacioHack/geoutils/tarball/main
 ```
 
 ## Documentation
 See the full documentation at https://geoutils.readthedocs.io.
 
 
 ## Structure
 
-GeoUtils are composed of three libraries:
+GeoUtils is composed of three libraries:
 - `georaster.py` to handle raster data set. In particular, a Raster class to load a raster file along with metadata.
 - `geovector.py` to handle vector data set. In particular, a Vector class to load a raster file along with metadata.
 - `projtools.py` with various tools around projections.
 
 
 ## How to contribute
 
-You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/GeoUtils/issues) section. All contributions are welcome.
+You can find ways to improve the libraries in the [issues](https://github.com/GlacioHack/geoutils/issues) section. All contributions are welcome.
 
 1. Fork the repository to your personal GitHub account, clone to your computer.
 2. (Optional but preferred:) Make a feature branch.
 3. Push to your feature branch.
 4. When ready, submit a Pull Request from your feature branch to `GlacioHack/geoutils:master`.
 5. The PR will be reviewed by at least one other person. Usually your PR will be merged via 'squash and merge'.
```

### Comparing `geoutils-0.0.8/setup.py` & `geoutils-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from glob import glob
 from os import path
 from typing import Optional
 
 from setuptools import setup
 
-FULLVERSION = "0.0.8"
+FULLVERSION = "0.0.9"
 VERSION = FULLVERSION
 
 write_version = True
 
 
 def write_version_py(filename: Optional[str] = None) -> None:
     cnt = """\
@@ -24,37 +24,29 @@
     finally:
         a.close()
 
 
 if write_version:
     write_version_py()
 
-# get all data in the datasets module
-
-data_files = []
-
-for item in glob("geoutils/datasets/*"):
-    bname = path.basename(item)
-    if not bname.startswith("__"):
-        data_files.append(path.join("datasets", bname))
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="geoutils",
     version=FULLVERSION,
     description="Tools for working with geospatial data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.github.com/GlacioHack/geoutils/",
     author="The GlacioHack Team",
     license="BSD-3",
-    packages=["geoutils", "geoutils.datasets", "geoutils.georaster"],
-    package_data={"geoutils": data_files},
+    packages=["geoutils", "geoutils.georaster"],
+    python_requires=">=3.8",
     install_requires=[
         "rasterio",
         "geopandas >= 0.10.0",
         "pyproj",
         "scipy",
         "typing-extensions; python_version < '3.8'",
         "matplotlib",
```

