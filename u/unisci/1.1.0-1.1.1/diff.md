# Comparing `tmp/unisci-1.1.0.tar.gz` & `tmp/unisci-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.1.0.tar", last modified: Wed Apr 26 23:38:24 2023, max compression
+gzip compressed data, was "unisci-1.1.1.tar", last modified: Wed Apr 26 23:42:48 2023, max compression
```

## Comparing `unisci-1.1.0.tar` & `unisci-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:38:24.429962 unisci-1.1.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.1.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-26 23:10:44.000000 unisci-1.1.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1378 2023-04-26 23:38:24.429669 unisci-1.1.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1118 2023-04-26 23:32:35.000000 unisci-1.1.0/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-26 23:38:24.430046 unisci-1.1.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      482 2023-04-26 23:35:51.000000 unisci-1.1.0/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:38:24.426296 unisci-1.1.0/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-26 23:37:29.000000 unisci-1.1.0/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.1.0/unisci/constants.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.1.0/unisci/conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.1.0/unisci/error.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:38:24.428051 unisci-1.1.0/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.1.0/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     8112 2023-04-26 16:06:26.000000 unisci-1.1.0/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.1.0/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:38:24.429272 unisci-1.1.0/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.1.0/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.1.0/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.1.0/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    38836 2023-04-26 16:06:26.000000 unisci-1.1.0/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:38:24.427526 unisci-1.1.0/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1378 2023-04-26 23:38:24.000000 unisci-1.1.0/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      463 2023-04-26 23:38:24.000000 unisci-1.1.0/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-26 23:38:24.000000 unisci-1.1.0/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-26 23:38:24.000000 unisci-1.1.0/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:42:48.821871 unisci-1.1.1/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.1.1/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-26 23:10:44.000000 unisci-1.1.1/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1457 2023-04-26 23:42:48.821601 unisci-1.1.1/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1197 2023-04-26 23:42:15.000000 unisci-1.1.1/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-26 23:42:48.821946 unisci-1.1.1/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      482 2023-04-26 23:40:40.000000 unisci-1.1.1/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:42:48.818214 unisci-1.1.1/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-26 23:40:27.000000 unisci-1.1.1/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.1.1/unisci/constants.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.1.1/unisci/conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.1.1/unisci/error.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:42:48.820067 unisci-1.1.1/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.1.1/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     8112 2023-04-26 16:06:26.000000 unisci-1.1.1/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.1.1/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:42:48.821254 unisci-1.1.1/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.1.1/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.1.1/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.1.1/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    38836 2023-04-26 16:06:26.000000 unisci-1.1.1/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-26 23:42:48.819576 unisci-1.1.1/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1457 2023-04-26 23:42:48.000000 unisci-1.1.1/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      463 2023-04-26 23:42:48.000000 unisci-1.1.1/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-26 23:42:48.000000 unisci-1.1.1/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-26 23:42:48.000000 unisci-1.1.1/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.1.0/LICENSE` & `unisci-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/PKG-INFO` & `unisci-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.1.0
+Version: 1.1.1
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UniSci
-A module to perform unit conversions for almost any scientific topic!
+A module to perform unit conversions for almost any scientific topic! This package is available on PyPI [here](https://pypi.org/project/unisci/).
 
 ## Why Use This?
-Short for "Unit Science" UniSci is primarilty focused on being able to use any unit and easily convert it to another. It supports automatic conversions for formulas, condensation of complex units like `kg-m/s²` to `N`, and more!
+Short for "Unit Science", UniSci is primarilty focused on being able to use any unit and easily convert it to another. It supports automatic conversions for formulas, condensation of complex units like `kg-m/s²` to `N`, and more!
 
 ## Installation 
 To install, simply run the following:
 ```
-pip install unisci
+$ pip install unisci
 ```
 
 Then, you can use it as you please!
 ```python
 >>> from unisci import Quantity
 >>> length = Quantity(1, {'m': 1})
 >>> print(length.converted(['ft']))
```

### Comparing `unisci-1.1.0/README.md` & `unisci-1.1.1/unisci.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,28 @@
+Metadata-Version: 2.1
+Name: unisci
+Version: 1.1.1
+Summary: Units Conversions, and Science Package
+Author: Vivaan Singhvi
+Author-email: singhvi.vivaan@gmail.com
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # UniSci
-A module to perform unit conversions for almost any scientific topic!
+A module to perform unit conversions for almost any scientific topic! This package is available on PyPI [here](https://pypi.org/project/unisci/).
 
 ## Why Use This?
-Short for "Unit Science" UniSci is primarilty focused on being able to use any unit and easily convert it to another. It supports automatic conversions for formulas, condensation of complex units like `kg-m/s²` to `N`, and more!
+Short for "Unit Science", UniSci is primarilty focused on being able to use any unit and easily convert it to another. It supports automatic conversions for formulas, condensation of complex units like `kg-m/s²` to `N`, and more!
 
 ## Installation 
 To install, simply run the following:
 ```
-pip install unisci
+$ pip install unisci
 ```
 
 Then, you can use it as you please!
 ```python
 >>> from unisci import Quantity
 >>> length = Quantity(1, {'m': 1})
 >>> print(length.converted(['ft']))
@@ -24,8 +35,8 @@
 ## Documentation
 Full documentation can be found on the [readthedocs](https://unisci.readthedocs.io/en/latest/index.html) site for the module.
 
 ## Contribution
 For adding conversions, formulas, or more, pull requests are greatly appreciated. Feel free to message me on my email singhvi.vivaan@gmail.com if you have any concerns!
 
 ## License
-This project is released under the MIT license.
+This project is released under the MIT license.
```

### Comparing `unisci-1.1.0/unisci/conversion_factors.py` & `unisci-1.1.1/unisci/conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/unisci/error.py` & `unisci-1.1.1/unisci/error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/unisci/formulas/chemistry.py` & `unisci-1.1.1/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/unisci/metric.py` & `unisci-1.1.1/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/unisci/periodic/periodic-table-lookup.json` & `unisci-1.1.1/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/unisci/periodic/periodic-table-numbers.json` & `unisci-1.1.1/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/unisci/periodic/periodic-table-symbols.json` & `unisci-1.1.1/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.1.0/unisci/types.py` & `unisci-1.1.1/unisci/types.py`

 * *Files identical despite different names*

