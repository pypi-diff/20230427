# Comparing `tmp/hafez-0.1.0.tar.gz` & `tmp/hafez-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hafez-0.1.0.tar", last modified: Thu Apr 27 00:41:49 2023, max compression
+gzip compressed data, was "hafez-0.1.1.tar", last modified: Thu Apr 27 04:16:51 2023, max compression
```

## Comparing `hafez-0.1.0.tar` & `hafez-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.333198 hafez-0.1.0/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1073 2023-04-25 23:36:29.000000 hafez-0.1.0/LICENSE
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       40 2023-03-28 05:39:02.000000 hafez-0.1.0/MANIFEST.in
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 00:41:49.333025 hafez-0.1.0/PKG-INFO
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     2563 2023-04-26 03:17:25.000000 hafez-0.1.0/README.md
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.331322 hafez-0.1.0/hafez/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      130 2023-04-26 02:31:37.000000 hafez-0.1.0/hafez/__init__.py
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1281 2023-04-26 03:08:57.000000 hafez-0.1.0/hafez/main.py
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.332383 hafez-0.1.0/hafez/utils/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-26 01:48:50.000000 hafez-0.1.0/hafez/utils/__init__.py
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1229 2023-04-27 00:30:32.000000 hafez-0.1.0/hafez/utils/db.py
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      792 2023-04-26 02:32:50.000000 hafez-0.1.0/hafez/utils/formating.py
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 00:41:49.331991 hafez-0.1.0/hafez.egg-info/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/PKG-INFO
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      313 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/SOURCES.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        1 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/dependency_links.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/requires.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        6 2023-04-27 00:41:49.000000 hafez-0.1.0/hafez.egg-info/top_level.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      465 2023-04-26 02:35:56.000000 hafez-0.1.0/pyproject.toml
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-26 02:13:01.000000 hafez-0.1.0/requirements.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       38 2023-04-27 00:41:49.333243 hafez-0.1.0/setup.cfg
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      365 2023-03-28 05:53:03.000000 hafez-0.1.0/setup.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:16:51.454100 hafez-0.1.1/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1073 2023-04-25 23:36:29.000000 hafez-0.1.1/LICENSE
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       40 2023-03-28 05:39:02.000000 hafez-0.1.1/MANIFEST.in
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 04:16:51.453833 hafez-0.1.1/PKG-INFO
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     2563 2023-04-26 03:17:25.000000 hafez-0.1.1/README.md
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:16:51.452590 hafez-0.1.1/hafez/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      130 2023-04-26 02:31:37.000000 hafez-0.1.1/hafez/__init__.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1281 2023-04-26 03:08:57.000000 hafez-0.1.1/hafez/main.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:16:51.453619 hafez-0.1.1/hafez/utils/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-26 01:48:50.000000 hafez-0.1.1/hafez/utils/__init__.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1229 2023-04-27 04:14:50.000000 hafez-0.1.1/hafez/utils/db.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      792 2023-04-26 02:32:50.000000 hafez-0.1.1/hafez/utils/formating.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:16:51.453269 hafez-0.1.1/hafez.egg-info/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 04:16:51.000000 hafez-0.1.1/hafez.egg-info/PKG-INFO
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      313 2023-04-27 04:16:51.000000 hafez-0.1.1/hafez.egg-info/SOURCES.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        1 2023-04-27 04:16:51.000000 hafez-0.1.1/hafez.egg-info/dependency_links.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-27 04:16:51.000000 hafez-0.1.1/hafez.egg-info/requires.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        6 2023-04-27 04:16:51.000000 hafez-0.1.1/hafez.egg-info/top_level.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      465 2023-04-27 04:16:16.000000 hafez-0.1.1/pyproject.toml
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-26 02:13:01.000000 hafez-0.1.1/requirements.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       38 2023-04-27 04:16:51.454161 hafez-0.1.1/setup.cfg
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      365 2023-03-28 05:53:03.000000 hafez-0.1.1/setup.py
```

### Comparing `hafez-0.1.0/LICENSE` & `hafez-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hafez-0.1.0/PKG-INFO` & `hafez-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hafez
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hafez Poems
 Author-email: Kaveh Bakhtiyari <kbakhtiyari@yahoo.com>
 Project-URL: Homepage, https://github.com/kavehbc/hafez
 Project-URL: Bug Tracker, https://github.com/kavehbc/hafez
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hafez-0.1.0/README.md` & `hafez-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hafez-0.1.0/hafez/main.py` & `hafez-0.1.1/hafez/main.py`

 * *Files identical despite different names*

### Comparing `hafez-0.1.0/hafez/utils/db.py` & `hafez-0.1.1/hafez/utils/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import sqlite3
 from sqlite3 import Connection
 import pathlib
 
-URI_SQLITE_DB = str(pathlib.Path(__file__).parents[2].resolve()) + "/data/hafez.db"
+URI_SQLITE_DB = str(pathlib.Path(__file__).parents[1].resolve()) + "/data/hafez.db"
 
 
 def get_data(id: int = None):
     conn = get_connection()
     if id is None:
         sql_query = "SELECT * FROM poems"
     else:
```

### Comparing `hafez-0.1.0/hafez/utils/formating.py` & `hafez-0.1.1/hafez/utils/formating.py`

 * *Files identical despite different names*

### Comparing `hafez-0.1.0/hafez.egg-info/PKG-INFO` & `hafez-0.1.1/hafez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hafez
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hafez Poems
 Author-email: Kaveh Bakhtiyari <kbakhtiyari@yahoo.com>
 Project-URL: Homepage, https://github.com/kavehbc/hafez
 Project-URL: Bug Tracker, https://github.com/kavehbc/hafez
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

