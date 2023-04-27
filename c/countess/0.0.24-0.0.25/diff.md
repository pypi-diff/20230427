# Comparing `tmp/countess-0.0.24.tar.gz` & `tmp/countess-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.24.tar", last modified: Thu Apr 27 04:26:41 2023, max compression
+gzip compressed data, was "countess-0.0.25.tar", last modified: Thu Apr 27 04:51:42 2023, max compression
```

## Comparing `countess-0.0.24.tar` & `countess-0.0.25.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.24/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:26:41.596055 countess-0.0.24/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-04-26 02:32:05.000000 countess-0.0.24/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-04-26 02:31:56.000000 countess-0.0.24/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.24/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15736 2023-04-26 23:25:45.000000 countess-0.0.24/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5024 2023-04-21 06:08:37.000000 countess-0.0.24/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13178 2023-04-26 23:25:45.000000 countess-0.0.24/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.24/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    21779 2023-04-26 02:38:33.000000 countess-0.0.24/countess/gui/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-04-26 02:29:55.000000 countess-0.0.24/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    33190 2023-04-26 23:25:45.000000 countess-0.0.24/countess/gui/main.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.24/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5795 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1194 2023-04-26 02:29:55.000000 countess-0.0.24/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2038 2023-04-26 03:33:35.000000 countess-0.0.24/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4145 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-04-26 02:29:55.000000 countess-0.0.24/countess/plugins/hdf5.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-04-26 02:29:55.000000 countess-0.0.24/countess/plugins/log_score.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6776 2023-04-26 23:25:45.000000 countess-0.0.24/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2200 2023-04-26 02:38:33.000000 countess-0.0.24/countess/plugins/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.24/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     9717 2023-04-26 02:29:55.000000 countess-0.0.24/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.592055 countess-0.0.24/countess.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      906 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      784 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      237 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-04-27 04:26:41.000000 countess-0.0.24/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2415 2023-04-27 04:26:35.000000 countess-0.0.24/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-04-27 04:26:41.596055 countess-0.0.24/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-04-21 06:08:37.000000 countess-0.0.24/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:26:41.596055 countess-0.0.24/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-04-21 06:08:37.000000 countess-0.0.24/tests/test_gui.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2022-12-12 02:15:43.000000 countess-0.0.25/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       26 2023-04-27 04:47:23.000000 countess-0.0.25/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:51:42.905179 countess-0.0.25/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2877 2023-04-27 04:50:53.000000 countess-0.0.25/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2023-04-27 04:51:00.000000 countess-0.0.25/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.25/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      736 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4271 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1910 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15736 2023-04-26 23:25:45.000000 countess-0.0.25/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5024 2023-04-21 06:08:37.000000 countess-0.0.25/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13178 2023-04-26 23:25:45.000000 countess-0.0.25/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.25/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    21779 2023-04-26 02:38:33.000000 countess-0.0.25/countess/gui/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5947 2023-04-26 02:29:55.000000 countess-0.0.25/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    33190 2023-04-26 23:25:45.000000 countess-0.0.25/countess/gui/main.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-04-21 06:08:37.000000 countess-0.0.25/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5795 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1194 2023-04-26 02:29:55.000000 countess-0.0.25/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2038 2023-04-26 03:33:35.000000 countess-0.0.25/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4145 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1744 2023-04-26 02:29:55.000000 countess-0.0.25/countess/plugins/hdf5.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3051 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      347 2023-04-26 02:29:55.000000 countess-0.0.25/countess/plugins/log_score.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5520 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6776 2023-04-26 23:25:45.000000 countess-0.0.25/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2200 2023-04-26 02:38:33.000000 countess-0.0.25/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.25/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.25/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     9717 2023-04-26 02:29:55.000000 countess-0.0.25/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/countess.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3528 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      936 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      784 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      237 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2023-04-27 04:51:42.000000 countess-0.0.25/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2414 2023-04-27 04:49:11.000000 countess-0.0.25/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1444 2023-04-27 04:51:42.909180 countess-0.0.25/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-04-21 06:08:37.000000 countess-0.0.25/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-27 04:51:42.905179 countess-0.0.25/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      636 2023-04-21 06:08:37.000000 countess-0.0.25/tests/test_gui.py
```

### Comparing `countess-0.0.24/LICENSE.txt` & `countess-0.0.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/PKG-INFO` & `countess-0.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.24
+Version: 0.0.25
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.24
+# CountESS 0.0.25
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.24/README.md` & `countess-0.0.25/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.24
+# CountESS 0.0.25
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.24/countess/core/cmd.py` & `countess-0.0.25/countess/core/cmd.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/core/config.py` & `countess-0.0.25/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/core/logger.py` & `countess-0.0.25/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/core/parameters.py` & `countess-0.0.25/countess/core/parameters.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/core/pipeline.py` & `countess-0.0.25/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/core/plugins.py` & `countess-0.0.25/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/gui/config.py` & `countess-0.0.25/countess/gui/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/gui/logger.py` & `countess-0.0.25/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/gui/main.py` & `countess-0.0.25/countess/gui/main.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/csv.py` & `countess-0.0.25/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/expression.py` & `countess-0.0.25/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/fastq.py` & `countess-0.0.25/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/group_by.py` & `countess-0.0.25/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/hdf5.py` & `countess-0.0.25/countess/plugins/hdf5.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/join.py` & `countess-0.0.25/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/pivot.py` & `countess-0.0.25/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/regex.py` & `countess-0.0.25/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/plugins/variant.py` & `countess-0.0.25/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess/utils/variant.py` & `countess-0.0.25/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/countess.egg-info/PKG-INFO` & `countess-0.0.25/countess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.24
+Version: 0.0.25
 Summary: CountESS
 Author: CountESS Developers
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer: Nick Moore
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: hdf
 License-File: LICENSE.txt
 
-# CountESS 0.0.24
+# CountESS 0.0.25
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.24/countess.egg-info/SOURCES.txt` & `countess-0.0.25/countess.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE.txt
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 countess/__init__.py
+countess/py.typed
 countess.egg-info/PKG-INFO
 countess.egg-info/SOURCES.txt
 countess.egg-info/dependency_links.txt
 countess.egg-info/entry_points.txt
 countess.egg-info/requires.txt
 countess.egg-info/top_level.txt
 countess/core/__init__.py
```

### Comparing `countess-0.0.24/countess.egg-info/entry_points.txt` & `countess-0.0.25/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/pyproject.toml` & `countess-0.0.25/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     'pandas~=2.0.0',
     'rapidfuzz~=2.15.1',
     'ttkthemes~=3.2.2',
 ]
 
 [project.optional-dependencies]
 dev = [
-    'black<24', 
+    'black<24',
     'build==0.10.0',
     'mypy~=1.0.1',
     'pylint~=2.16',
     'types-ttkthemes~=3.2',
     'twine==4.0.2',
     'pandas-stubs~=1.4',
     'pytest~=7.2',
```

### Comparing `countess-0.0.24/setup.cfg` & `countess-0.0.25/setup.cfg`

 * *Files identical despite different names*

### Comparing `countess-0.0.24/tests/test_gui.py` & `countess-0.0.25/tests/test_gui.py`

 * *Files identical despite different names*

