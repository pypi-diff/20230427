# Comparing `tmp/brandpy-0.0.2.tar.gz` & `tmp/brandpy-0.0.3.tar.gz`

## Comparing `brandpy-0.0.2.tar` & `brandpy-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 brandpy-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 brandpy-0.0.2/src/brandpy/__about__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 brandpy-0.0.2/src/brandpy/__init__.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 brandpy-0.0.2/src/brandpy/bw_api_caller.py
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 brandpy-0.0.2/src/brandpy/bw_api_helper.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 brandpy-0.0.2/src/brandpy/bw_auth_config.py
--rw-r--r--   0        0        0   334905 2020-02-02 00:00:00.000000 brandpy-0.0.2/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip
--rw-r--r--   0        0        0 26474074 2020-02-02 00:00:00.000000 brandpy-0.0.2/tests/BrandwatchAPI_Lookup.ipynb
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 brandpy-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 brandpy-0.0.2/tests/bw_auth_config_test.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 brandpy-0.0.2/tests/end_to_end_test.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 brandpy-0.0.2/tests/import_test.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 brandpy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 brandpy-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 brandpy-0.0.2/README.md
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 brandpy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 brandpy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/__about__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/__init__.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/bw_api_caller.py
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/bw_api_helper.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 brandpy-0.0.3/src/brandpy/bw_auth_config.py
+-rw-r--r--   0        0        0   334905 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip
+-rw-r--r--   0        0        0 26474074 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/BrandwatchAPI_Lookup.ipynb
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/bw_auth_config_test.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/end_to_end_test.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 brandpy-0.0.3/tests/import_test.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 brandpy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 brandpy-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 brandpy-0.0.3/README.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 brandpy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 brandpy-0.0.3/PKG-INFO
```

### Comparing `brandpy-0.0.2/src/brandpy/bw_api_caller.py` & `brandpy-0.0.3/src/brandpy/bw_api_caller.py`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/src/brandpy/bw_api_helper.py` & `brandpy-0.0.3/src/brandpy/bw_api_helper.py`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/src/brandpy/bw_auth_config.py` & `brandpy-0.0.3/src/brandpy/bw_auth_config.py`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip` & `brandpy-0.0.3/tests/2022_02_23_H_00_to_2022_02_23_H_01_cdondim_BWAPI_UkraineRussiaWarSO.csv.zip`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/tests/BrandwatchAPI_Lookup.ipynb` & `brandpy-0.0.3/tests/BrandwatchAPI_Lookup.ipynb`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/tests/end_to_end_test.py` & `brandpy-0.0.3/tests/end_to_end_test.py`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/.gitignore` & `brandpy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/LICENSE.txt` & `brandpy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `brandpy-0.0.2/pyproject.toml` & `brandpy-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "BrandPy"
+name = "brandpy"
 dynamic = ["version"]
 description = 'This is a simple python wrapper for lookup calls of Brandwatch API.'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
@@ -23,17 +23,17 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["requests","numpy"]
 
 [project.urls]
-Documentation = "https://github.com/unknown/brandpy#readme"
-Issues = "https://github.com/unknown/brandpy/issues"
-Source = "https://github.com/unknown/brandpy"
+Documentation = "https://github.com/deamonpog/BrandPy#readme"
+Issues = "https://github.com/deamonpog/BrandPy/issues"
+Source = "https://github.com/deamonpog/BrandPy"
 
 [tool.hatch.version]
 path = "src/brandpy/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```

### Comparing `brandpy-0.0.2/PKG-INFO` & `brandpy-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: BrandPy
-Version: 0.0.2
+Name: brandpy
+Version: 0.0.3
 Summary: This is a simple python wrapper for lookup calls of Brandwatch API.
-Project-URL: Documentation, https://github.com/unknown/brandpy#readme
-Project-URL: Issues, https://github.com/unknown/brandpy/issues
-Project-URL: Source, https://github.com/unknown/brandpy
+Project-URL: Documentation, https://github.com/deamonpog/BrandPy#readme
+Project-URL: Issues, https://github.com/deamonpog/BrandPy/issues
+Project-URL: Source, https://github.com/deamonpog/BrandPy
 Author-email: deamonpog <pog666@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

