# Comparing `tmp/cellxgene_census-0.13.0.tar.gz` & `tmp/cellxgene_census-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-0.13.0.tar", last modified: Tue Apr  4 18:20:22 2023, max compression
+gzip compressed data, was "cellxgene_census-1.0.0rc1.tar", last modified: Thu Apr 27 16:40:27 2023, max compression
```

## Comparing `cellxgene_census-0.13.0.tar` & `cellxgene_census-1.0.0rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:20:22.521535 cellxgene_census-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-04 18:20:22.521535 cellxgene_census-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:20:22.517535 cellxgene_census-0.13.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 18:20:22.521535 cellxgene_census-0.13.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:20:22.517535 cellxgene_census-0.13.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:20:22.517535 cellxgene_census-0.13.0/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:20:22.521535 cellxgene_census-0.13.0/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-04 18:20:22.000000 cellxgene_census-0.13.0/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-04 18:20:22.000000 cellxgene_census-0.13.0/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:20:22.000000 cellxgene_census-0.13.0/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 18:20:22.000000 cellxgene_census-0.13.0/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-04 18:20:22.000000 cellxgene_census-0.13.0/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:20:22.521535 cellxgene_census-0.13.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-04 18:20:06.000000 cellxgene_census-0.13.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.310041 cellxgene_census-1.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 16:40:27.000000 cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:40:27.314041 cellxgene_census-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-27 16:40:08.000000 cellxgene_census-1.0.0rc1/tests/test_util.py
```

### Comparing `cellxgene_census-0.13.0/LICENSE` & `cellxgene_census-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/PKG-INFO` & `cellxgene_census-1.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 0.13.0
+Version: 1.0.0rc1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
-The `cell_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
+The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
 
 **Status**: Pre-release, under rapid development. Expect API changes.
 
 
 ## For More Help
 For more help, please file a issue on the repo, or contact us at <soma@chanzuckerberg.com>.
```

### Comparing `cellxgene_census-0.13.0/README.md` & `cellxgene_census-1.0.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # CZ CELLxGENE Discover Census
 
-The `cell_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
+The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
 
 **Status**: Pre-release, under rapid development. Expect API changes.
 
 
 ## For More Help
 For more help, please file a issue on the repo, or contact us at <soma@chanzuckerberg.com>.
```

### Comparing `cellxgene_census-0.13.0/pyproject.toml` & `cellxgene_census-1.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,23 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies= [
     # NOTE: the tiledbsoma version must be >= to the version used in the Census builder, to
     # ensure that the assets are readable (tiledbsoma supports backward compatible reading).
     # Make sure this version does not fall behind the builder's tiledbsoma version.
-    "tiledbsoma==1.2.1",
+    "tiledbsoma==1.2.2",
     "anndata",
     "numpy>=1.21,<1.24",  # numpy is constrained by numba and the old pip solver
     "requests",
     "typing_extensions",
     "s3fs",
     "scipy",
+    # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
+    "certifi",
 ]
 
 [project.urls]
 homepage = "https://github.com/chanzuckerberg/cellxgene-census"
 repository = "https://github.com/chanzuckerberg/cellxgene-census"
 
 [tool.setuptools.packages.find]
```

### Comparing `cellxgene_census-0.13.0/release_process.md` & `cellxgene_census-1.0.0rc1/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census/__init__.py` & `cellxgene_census-1.0.0rc1/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.0.0rc1/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.0.0rc1/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census/_open.py` & `cellxgene_census-1.0.0rc1/src/cellxgene_census/_open.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 Contains methods to open publicly hosted versions of Census object and access its source datasets.
 """
 
 import os.path
 import urllib.parse
 from typing import Any, Dict, Optional
 
+import certifi
 import s3fs
 import tiledbsoma as soma
 
 from ._release_directory import CensusLocator, get_census_version_description
 from ._util import _uri_join
 
 DEFAULT_TILEDB_CONFIGURATION: Dict[str, Any] = {
     # https://docs.tiledb.com/main/how-to/configuration#configuration-parameters
     "py.init_buffer_bytes": 1 * 1024**3,
     "soma.init_buffer_bytes": 1 * 1024**3,
+    # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
+    "vfs.s3.ca_file": certifi.where(),
 }
 
 
 def _open_soma(locator: CensusLocator, context: Optional[soma.options.SOMATileDBContext] = None) -> soma.Collection:
     """Private. Merge config defaults and return open census as a soma Collection/context."""
     s3_region = locator.get("s3_region")
```

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.0.0rc1/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.0.0rc1/src/cellxgene_census/_release_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         "soma": CensusLocator,  # SOMA objects locator
         "h5ads": CensusLocator,  # source H5ADs locator
     },
 )
 CensusDirectory = Dict[CensusVersionName, Union[CensusVersionName, CensusVersionDescription]]
 
 
-# URL for the default top-level directory of all public data, formatted as a CensusDirectory
-CELL_CENSUS_RELEASE_DIRECTORY_URL = "https://s3.us-west-2.amazonaws.com/cellxgene-data-public/cell-census/release.json"
+# URL for the default top-level directory of all public data
+CELL_CENSUS_RELEASE_DIRECTORY_URL = "https://census.cellxgene.cziscience.com/cell-census/release.json"
 
 
 def get_census_version_description(census_version: str) -> CensusVersionDescription:
     """Get release description for given Census version, from the Census release directory.
 
     Args:
         census_version:
```

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 0.13.0
+Version: 1.0.0rc1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
-The `cell_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
+The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/). 
 
 **Status**: Pre-release, under rapid development. Expect API changes.
 
 
 ## For More Help
 For more help, please file a issue on the repo, or contact us at <soma@chanzuckerberg.com>.
```

### Comparing `cellxgene_census-0.13.0/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.0.0rc1/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/tests/README.md` & `cellxgene_census-1.0.0rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/tests/test_acceptance.py` & `cellxgene_census-1.0.0rc1/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/tests/test_directory.py` & `cellxgene_census-1.0.0rc1/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/tests/test_get_anndata.py` & `cellxgene_census-1.0.0rc1/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/tests/test_get_helpers.py` & `cellxgene_census-1.0.0rc1/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/tests/test_open.py` & `cellxgene_census-1.0.0rc1/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-0.13.0/tests/test_util.py` & `cellxgene_census-1.0.0rc1/tests/test_util.py`

 * *Files identical despite different names*

