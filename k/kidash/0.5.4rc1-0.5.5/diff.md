# Comparing `tmp/kidash-0.5.4rc1.tar.gz` & `tmp/kidash-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kidash-0.5.4rc1.tar", max compression
+gzip compressed data, was "kidash-0.5.5.tar", max compression
```

## Comparing `kidash-0.5.4rc1.tar` & `kidash-0.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      300 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/LICENSE
--rw-r--r--   0        0        0     1132 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/NEWS
--rw-r--r--   0        0        0     2525 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/README.md
--rw-r--r--   0        0        0      894 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/__init__.py
--rw-r--r--   0        0        0       91 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/_version.py
--rwxr-xr-x   0        0        0     4355 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/bin/kidash.py
--rwxr-xr-x   0        0        0    59367 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/kidash.py
--rw-r--r--   0        0        0     1307 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/pyproject.toml
--rw-r--r--   0        0        0    54328 2023-04-20 14:54:08.677521 kidash-0.5.4rc1/tests/data/overview-with-index-patterns.json
--rwxr-xr-x   0        0        0     1166 2023-04-20 14:54:08.677521 kidash-0.5.4rc1/tests/run_tests.py
--rw-r--r--   0        0        0     2131 2023-04-20 14:54:08.677521 kidash-0.5.4rc1/tests/test_export.py
--rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 kidash-0.5.4rc1/PKG-INFO
+-rw-r--r--   0        0        0      300 2023-04-27 08:58:08.106531 kidash-0.5.5/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-27 08:58:08.106531 kidash-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1288 2023-04-27 08:58:08.106531 kidash-0.5.5/NEWS
+-rw-r--r--   0        0        0     2525 2023-04-27 08:58:08.106531 kidash-0.5.5/README.md
+-rw-r--r--   0        0        0      894 2023-04-27 08:58:08.106531 kidash-0.5.5/kidash/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-27 08:58:08.106531 kidash-0.5.5/kidash/_version.py
+-rwxr-xr-x   0        0        0     4355 2023-04-27 08:58:08.106531 kidash-0.5.5/kidash/bin/kidash.py
+-rwxr-xr-x   0        0        0    59367 2023-04-27 08:58:08.106531 kidash-0.5.5/kidash/kidash.py
+-rw-r--r--   0        0        0     1302 2023-04-27 08:58:08.106531 kidash-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    54328 2023-04-27 08:58:08.106531 kidash-0.5.5/tests/data/overview-with-index-patterns.json
+-rwxr-xr-x   0        0        0     1166 2023-04-27 08:58:08.106531 kidash-0.5.5/tests/run_tests.py
+-rw-r--r--   0        0        0     2131 2023-04-27 08:58:08.106531 kidash-0.5.5/tests/test_export.py
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 kidash-0.5.5/PKG-INFO
```

### Comparing `kidash-0.5.4rc1/LICENSE` & `kidash-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/NEWS` & `kidash-0.5.5/NEWS`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+  ## kidash 0.5.5 - (2023-04-27)
+  
+  * Update Poetry's package dependencies
+
+  ## kidash 0.5.4 - (2023-04-21)
+  
+  * Update Poetry's package dependencies
+
   ## kidash 0.5.3 - (2023-02-01)
   
   * Update Poetry's package dependencies
 
   ## kidash 0.5.2 - (2022-10-31)
   
   * Update Poetry's package dependencies
```

### Comparing `kidash-0.5.4rc1/README.md` & `kidash-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/kidash/__init__.py` & `kidash-0.5.5/kidash/__init__.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/kidash/bin/kidash.py` & `kidash-0.5.5/kidash/bin/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/kidash/kidash.py` & `kidash-0.5.5/kidash/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/pyproject.toml` & `kidash-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kidash"
-version = "0.5.4-rc.1"
+version = "0.5.5"
 description = "GrimoireLab script to manage Kibana dashboards from the command line"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `kidash-0.5.4rc1/tests/data/overview-with-index-patterns.json` & `kidash-0.5.5/tests/data/overview-with-index-patterns.json`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/tests/run_tests.py` & `kidash-0.5.5/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/tests/test_export.py` & `kidash-0.5.5/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.4rc1/PKG-INFO` & `kidash-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kidash
-Version: 0.5.4rc1
+Version: 0.5.5
 Summary: GrimoireLab script to manage Kibana dashboards from the command line
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

