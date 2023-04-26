# Comparing `tmp/settngs-0.6.2.tar.gz` & `tmp/settngs-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settngs-0.6.2.tar", last modified: Mon Feb 20 10:09:57 2023, max compression
+gzip compressed data, was "settngs-0.6.3.tar", last modified: Tue Apr 25 07:16:12 2023, max compression
```

## Comparing `settngs-0.6.2.tar` & `settngs-0.6.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:09:57.789595 settngs-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-20 10:09:48.000000 settngs-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-20 10:09:57.789595 settngs-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-02-20 10:09:48.000000 settngs-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:09:57.789595 settngs-0.6.2/settngs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-20 10:09:57.000000 settngs-0.6.2/settngs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-20 10:09:57.000000 settngs-0.6.2/settngs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 10:09:57.000000 settngs-0.6.2/settngs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-20 10:09:57.000000 settngs-0.6.2/settngs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-20 10:09:57.000000 settngs-0.6.2/settngs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-02-20 10:09:48.000000 settngs-0.6.2/settngs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-20 10:09:57.789595 settngs-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-20 10:09:48.000000 settngs-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:12.033409 settngs-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 07:16:03.000000 settngs-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-25 07:16:12.033409 settngs-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-25 07:16:03.000000 settngs-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:12.033409 settngs-0.6.3/settngs/
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-04-25 07:16:03.000000 settngs-0.6.3/settngs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 07:16:03.000000 settngs-0.6.3/settngs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:03.000000 settngs-0.6.3/settngs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:12.033409 settngs-0.6.3/settngs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-25 07:16:12.037409 settngs-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 07:16:03.000000 settngs-0.6.3/setup.py
```

### Comparing `settngs-0.6.2/LICENSE` & `settngs-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `settngs-0.6.2/PKG-INFO` & `settngs-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.6.2/README.md` & `settngs-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `settngs-0.6.2/settngs.egg-info/PKG-INFO` & `settngs-0.6.3/settngs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.6.2/settngs.py` & `settngs-0.6.3/settngs/__init__.py`

 * *Files identical despite different names*

