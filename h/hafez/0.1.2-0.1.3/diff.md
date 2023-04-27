# Comparing `tmp/hafez-0.1.2.tar.gz` & `tmp/hafez-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hafez-0.1.2.tar", last modified: Thu Apr 27 04:36:25 2023, max compression
+gzip compressed data, was "hafez-0.1.3.tar", last modified: Thu Apr 27 04:59:05 2023, max compression
```

## Comparing `hafez-0.1.2.tar` & `hafez-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:36:25.613316 hafez-0.1.2/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1073 2023-04-25 23:36:29.000000 hafez-0.1.2/LICENSE
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       40 2023-03-28 05:39:02.000000 hafez-0.1.2/MANIFEST.in
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 04:36:25.613174 hafez-0.1.2/PKG-INFO
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     2563 2023-04-26 03:17:25.000000 hafez-0.1.2/README.md
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:36:25.611918 hafez-0.1.2/hafez/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      130 2023-04-26 02:31:37.000000 hafez-0.1.2/hafez/__init__.py
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1281 2023-04-26 03:08:57.000000 hafez-0.1.2/hafez/main.py
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:36:25.613014 hafez-0.1.2/hafez/utils/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-26 01:48:50.000000 hafez-0.1.2/hafez/utils/__init__.py
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1274 2023-04-27 04:34:33.000000 hafez-0.1.2/hafez/utils/db.py
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      792 2023-04-26 02:32:50.000000 hafez-0.1.2/hafez/utils/formating.py
-drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:36:25.612651 hafez-0.1.2/hafez.egg-info/
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 04:36:25.000000 hafez-0.1.2/hafez.egg-info/PKG-INFO
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      313 2023-04-27 04:36:25.000000 hafez-0.1.2/hafez.egg-info/SOURCES.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        1 2023-04-27 04:36:25.000000 hafez-0.1.2/hafez.egg-info/dependency_links.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-27 04:36:25.000000 hafez-0.1.2/hafez.egg-info/requires.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        6 2023-04-27 04:36:25.000000 hafez-0.1.2/hafez.egg-info/top_level.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      465 2023-04-27 04:35:37.000000 hafez-0.1.2/pyproject.toml
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-26 02:13:01.000000 hafez-0.1.2/requirements.txt
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       38 2023-04-27 04:36:25.613352 hafez-0.1.2/setup.cfg
--rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      365 2023-03-28 05:53:03.000000 hafez-0.1.2/setup.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:59:05.803080 hafez-0.1.3/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1073 2023-04-25 23:36:29.000000 hafez-0.1.3/LICENSE
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       40 2023-03-28 05:39:02.000000 hafez-0.1.3/MANIFEST.in
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 04:59:05.802930 hafez-0.1.3/PKG-INFO
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     2563 2023-04-26 03:17:25.000000 hafez-0.1.3/README.md
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:59:05.800812 hafez-0.1.3/hafez/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      130 2023-04-26 02:31:37.000000 hafez-0.1.3/hafez/__init__.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:59:05.801570 hafez-0.1.3/hafez/data/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)   954368 2023-04-26 01:40:38.000000 hafez-0.1.3/hafez/data/hafez.db
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1281 2023-04-26 03:08:57.000000 hafez-0.1.3/hafez/main.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:59:05.802769 hafez-0.1.3/hafez/utils/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-26 01:48:50.000000 hafez-0.1.3/hafez/utils/__init__.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     1274 2023-04-27 04:58:34.000000 hafez-0.1.3/hafez/utils/db.py
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      792 2023-04-26 02:32:50.000000 hafez-0.1.3/hafez/utils/formating.py
+drwxr-xr-x   0 kaveh.bakhtiyari   (503) staff       (20)        0 2023-04-27 04:59:05.801434 hafez-0.1.3/hafez.egg-info/
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)     3035 2023-04-27 04:59:05.000000 hafez-0.1.3/hafez.egg-info/PKG-INFO
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      333 2023-04-27 04:59:05.000000 hafez-0.1.3/hafez.egg-info/SOURCES.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        1 2023-04-27 04:59:05.000000 hafez-0.1.3/hafez.egg-info/dependency_links.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-27 04:59:05.000000 hafez-0.1.3/hafez.egg-info/requires.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)        6 2023-04-27 04:59:05.000000 hafez-0.1.3/hafez.egg-info/top_level.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      465 2023-04-27 04:58:44.000000 hafez-0.1.3/pyproject.toml
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       14 2023-04-26 02:13:01.000000 hafez-0.1.3/requirements.txt
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)       38 2023-04-27 04:59:05.803115 hafez-0.1.3/setup.cfg
+-rw-r--r--   0 kaveh.bakhtiyari   (503) staff       (20)      434 2023-04-27 04:50:17.000000 hafez-0.1.3/setup.py
```

### Comparing `hafez-0.1.2/LICENSE` & `hafez-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hafez-0.1.2/PKG-INFO` & `hafez-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hafez
-Version: 0.1.2
+Version: 0.1.3
 Summary: Hafez Poems
 Author-email: Kaveh Bakhtiyari <kbakhtiyari@yahoo.com>
 Project-URL: Homepage, https://github.com/kavehbc/hafez
 Project-URL: Bug Tracker, https://github.com/kavehbc/hafez
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hafez-0.1.2/README.md` & `hafez-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hafez-0.1.2/hafez/main.py` & `hafez-0.1.3/hafez/main.py`

 * *Files identical despite different names*

### Comparing `hafez-0.1.2/hafez/utils/db.py` & `hafez-0.1.3/hafez/utils/db.py`

 * *Files identical despite different names*

### Comparing `hafez-0.1.2/hafez/utils/formating.py` & `hafez-0.1.3/hafez/utils/formating.py`

 * *Files identical despite different names*

### Comparing `hafez-0.1.2/hafez.egg-info/PKG-INFO` & `hafez-0.1.3/hafez.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hafez
-Version: 0.1.2
+Version: 0.1.3
 Summary: Hafez Poems
 Author-email: Kaveh Bakhtiyari <kbakhtiyari@yahoo.com>
 Project-URL: Homepage, https://github.com/kavehbc/hafez
 Project-URL: Bug Tracker, https://github.com/kavehbc/hafez
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

