# Comparing `tmp/ocm2-0.1.0.tar.gz` & `tmp/ocm2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocm2-0.1.0.tar", last modified: Wed Apr  5 20:30:13 2023, max compression
+gzip compressed data, was "ocm2-0.2.0.tar", last modified: Thu Apr 27 21:30:47 2023, max compression
```

## Comparing `ocm2-0.1.0.tar` & `ocm2-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:30:13.606587 ocm2-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-05 20:29:58.000000 ocm2-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-05 20:29:58.000000 ocm2-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-05 20:30:13.606587 ocm2-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-05 20:29:58.000000 ocm2-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:30:13.606587 ocm2-0.1.0/ocm2/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-05 20:29:58.000000 ocm2-0.1.0/ocm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-05 20:29:58.000000 ocm2-0.1.0/ocm2/ocm2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:30:13.606587 ocm2-0.1.0/ocm2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-05 20:30:13.000000 ocm2-0.1.0/ocm2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-05 20:30:13.000000 ocm2-0.1.0/ocm2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 20:30:13.000000 ocm2-0.1.0/ocm2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 20:30:13.000000 ocm2-0.1.0/ocm2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 20:30:13.000000 ocm2-0.1.0/ocm2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-05 20:30:13.000000 ocm2-0.1.0/ocm2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-05 20:29:58.000000 ocm2-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-05 20:30:13.606587 ocm2-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-05 20:29:58.000000 ocm2-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:30:47.322476 ocm2-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 21:30:35.000000 ocm2-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 21:30:35.000000 ocm2-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-27 21:30:47.322476 ocm2-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-27 21:30:35.000000 ocm2-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:30:47.318476 ocm2-0.2.0/ocm2/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-27 21:30:35.000000 ocm2-0.2.0/ocm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-04-27 21:30:35.000000 ocm2-0.2.0/ocm2/ocm2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:30:47.318476 ocm2-0.2.0/ocm2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-27 21:30:47.000000 ocm2-0.2.0/ocm2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 21:30:47.000000 ocm2-0.2.0/ocm2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 21:30:47.000000 ocm2-0.2.0/ocm2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:30:47.000000 ocm2-0.2.0/ocm2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 21:30:47.000000 ocm2-0.2.0/ocm2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 21:30:47.000000 ocm2-0.2.0/ocm2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 21:30:35.000000 ocm2-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 21:30:47.322476 ocm2-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-27 21:30:35.000000 ocm2-0.2.0/setup.py
```

### Comparing `ocm2-0.1.0/LICENSE` & `ocm2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocm2-0.1.0/PKG-INFO` & `ocm2-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocm2
-Version: 0.1.0
+Version: 0.2.0
 Summary: This python package extracts subdatasets from OCM-2 HDF file, georeference them and exports them to GeoTIFF. The package also creates a cloud mask layer.
 Home-page: https://github.com/akhi9661/ocm2
 Author: Akhilesh Kumar
 Author-email: akhiraj9661@gmail.com
 License: MIT license
 Keywords: ocm2
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,23 +21,31 @@
 License-File: LICENSE
 
 # ocm2
 
 
 [![image](https://img.shields.io/pypi/v/ocm2.svg)](https://pypi.python.org/pypi/ocm2)
 [![image](https://img.shields.io/conda/vn/conda-forge/ocm2.svg)](https://anaconda.org/conda-forge/ocm2)
+[![Python Versions](https://img.shields.io/pypi/pyversions/ocm2.svg)](https://pypi.org/project/ocm2/)
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![image](https://github.com/akhi9661/ocm2/workflows/docs/badge.svg)](https://github.com/akhi9661/ocm2)
+[![image](https://github.com/akhi9661/ocm2/workflows/Linux%20build/badge.svg)](https://github.com/akhi9661/ocm2/actions)
 
 
-**This python package extracts subdatasets from OCM-2 HDF file, georeference them and exports them to GeoTIFF. The package also creates a cloud mask layer.**
+**This python package extracts sub-datasets from OCM-2 HDF file, geo-reference them and exports them to GeoTIFF. The package also creates a cloud mask layer.**
 
 
+
+-   GitHub repo: <https://github.com/akhi9661/ocm2>
+-   PyPI: <https://pypi.org/project/ocm2/>
 -   Free software: MIT license
--   Documentation: https://akhi9661.github.io/ocm2
+-   Documentation: <https://akhi9661.github.io/ocm2>
     
 
 ## Features
 
--   TODO
+-   Extract sub-datasets from OCM-2 HDF file
+-   Geo-reference the extracted GeoTIFF files or extract and geo-reference them if not extracted.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `ocm2-0.1.0/README.md` & `ocm2-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # ocm2
 
 
 [![image](https://img.shields.io/pypi/v/ocm2.svg)](https://pypi.python.org/pypi/ocm2)
 [![image](https://img.shields.io/conda/vn/conda-forge/ocm2.svg)](https://anaconda.org/conda-forge/ocm2)
+[![Python Versions](https://img.shields.io/pypi/pyversions/ocm2.svg)](https://pypi.org/project/ocm2/)
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![image](https://github.com/akhi9661/ocm2/workflows/docs/badge.svg)](https://github.com/akhi9661/ocm2)
+[![image](https://github.com/akhi9661/ocm2/workflows/Linux%20build/badge.svg)](https://github.com/akhi9661/ocm2/actions)
 
 
-**This python package extracts subdatasets from OCM-2 HDF file, georeference them and exports them to GeoTIFF. The package also creates a cloud mask layer.**
+**This python package extracts sub-datasets from OCM-2 HDF file, geo-reference them and exports them to GeoTIFF. The package also creates a cloud mask layer.**
 
 
+
+-   GitHub repo: <https://github.com/akhi9661/ocm2>
+-   PyPI: <https://pypi.org/project/ocm2/>
 -   Free software: MIT license
--   Documentation: https://akhi9661.github.io/ocm2
+-   Documentation: <https://akhi9661.github.io/ocm2>
     
 
 ## Features
 
--   TODO
+-   Extract sub-datasets from OCM-2 HDF file
+-   Geo-reference the extracted GeoTIFF files or extract and geo-reference them if not extracted.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `ocm2-0.1.0/ocm2.egg-info/PKG-INFO` & `ocm2-0.2.0/ocm2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocm2
-Version: 0.1.0
+Version: 0.2.0
 Summary: This python package extracts subdatasets from OCM-2 HDF file, georeference them and exports them to GeoTIFF. The package also creates a cloud mask layer.
 Home-page: https://github.com/akhi9661/ocm2
 Author: Akhilesh Kumar
 Author-email: akhiraj9661@gmail.com
 License: MIT license
 Keywords: ocm2
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,23 +21,31 @@
 License-File: LICENSE
 
 # ocm2
 
 
 [![image](https://img.shields.io/pypi/v/ocm2.svg)](https://pypi.python.org/pypi/ocm2)
 [![image](https://img.shields.io/conda/vn/conda-forge/ocm2.svg)](https://anaconda.org/conda-forge/ocm2)
+[![Python Versions](https://img.shields.io/pypi/pyversions/ocm2.svg)](https://pypi.org/project/ocm2/)
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![image](https://github.com/akhi9661/ocm2/workflows/docs/badge.svg)](https://github.com/akhi9661/ocm2)
+[![image](https://github.com/akhi9661/ocm2/workflows/Linux%20build/badge.svg)](https://github.com/akhi9661/ocm2/actions)
 
 
-**This python package extracts subdatasets from OCM-2 HDF file, georeference them and exports them to GeoTIFF. The package also creates a cloud mask layer.**
+**This python package extracts sub-datasets from OCM-2 HDF file, geo-reference them and exports them to GeoTIFF. The package also creates a cloud mask layer.**
 
 
+
+-   GitHub repo: <https://github.com/akhi9661/ocm2>
+-   PyPI: <https://pypi.org/project/ocm2/>
 -   Free software: MIT license
--   Documentation: https://akhi9661.github.io/ocm2
+-   Documentation: <https://akhi9661.github.io/ocm2>
     
 
 ## Features
 
--   TODO
+-   Extract sub-datasets from OCM-2 HDF file
+-   Geo-reference the extracted GeoTIFF files or extract and geo-reference them if not extracted.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `ocm2-0.1.0/setup.py` & `ocm2-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='ocm2',
     name='ocm2',
     packages=find_packages(include=['ocm2', 'ocm2.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/akhi9661/ocm2',
-    version='0.1.0',
+    version='0.2.0',
     zip_safe=False,
 )
```

