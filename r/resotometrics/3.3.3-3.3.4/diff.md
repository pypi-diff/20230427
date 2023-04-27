# Comparing `tmp/resotometrics-3.3.3.tar.gz` & `tmp/resotometrics-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotometrics-3.3.3.tar", last modified: Fri Apr 21 14:33:10 2023, max compression
+gzip compressed data, was "resotometrics-3.3.4.tar", last modified: Wed Apr 26 16:51:17 2023, max compression
```

## Comparing `resotometrics-3.3.3.tar` & `resotometrics-3.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:10.674027 resotometrics-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 14:31:33.000000 resotometrics-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-21 14:33:10.674027 resotometrics-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-21 14:31:33.000000 resotometrics-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:31:33.000000 resotometrics-3.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:10.670027 resotometrics-3.3.3/resotometrics/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-21 14:31:33.000000 resotometrics-3.3.3/resotometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-21 14:31:33.000000 resotometrics-3.3.3/resotometrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-21 14:31:33.000000 resotometrics-3.3.3/resotometrics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-21 14:31:33.000000 resotometrics-3.3.3/resotometrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-21 14:31:33.000000 resotometrics-3.3.3/resotometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-21 14:31:33.000000 resotometrics-3.3.3/resotometrics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:10.674027 resotometrics-3.3.3/resotometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-21 14:33:10.000000 resotometrics-3.3.3/resotometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-21 14:33:10.000000 resotometrics-3.3.3/resotometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:33:10.000000 resotometrics-3.3.3/resotometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 14:33:10.000000 resotometrics-3.3.3/resotometrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:33:10.000000 resotometrics-3.3.3/resotometrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 14:33:10.000000 resotometrics-3.3.3/resotometrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 14:33:10.000000 resotometrics-3.3.3/resotometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:33:10.674027 resotometrics-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-21 14:31:33.000000 resotometrics-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:10.674027 resotometrics-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-21 14:31:33.000000 resotometrics-3.3.3/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.832252 resotometrics-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 16:49:32.000000 resotometrics-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-26 16:51:17.832252 resotometrics-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-26 16:49:32.000000 resotometrics-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:49:32.000000 resotometrics-3.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.828252 resotometrics-3.3.4/resotometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 16:49:32.000000 resotometrics-3.3.4/resotometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-26 16:49:32.000000 resotometrics-3.3.4/resotometrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-26 16:49:32.000000 resotometrics-3.3.4/resotometrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-04-26 16:49:32.000000 resotometrics-3.3.4/resotometrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-26 16:49:32.000000 resotometrics-3.3.4/resotometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-26 16:49:32.000000 resotometrics-3.3.4/resotometrics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.832252 resotometrics-3.3.4/resotometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-26 16:51:17.000000 resotometrics-3.3.4/resotometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 16:51:17.000000 resotometrics-3.3.4/resotometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:17.000000 resotometrics-3.3.4/resotometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 16:51:17.000000 resotometrics-3.3.4/resotometrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:17.000000 resotometrics-3.3.4/resotometrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:51:17.000000 resotometrics-3.3.4/resotometrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 16:51:17.000000 resotometrics-3.3.4/resotometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:51:17.832252 resotometrics-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-26 16:49:32.000000 resotometrics-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.832252 resotometrics-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 16:49:32.000000 resotometrics-3.3.4/test/test_args.py
```

### Comparing `resotometrics-3.3.3/PKG-INFO` & `resotometrics-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.3.3
+Version: 3.3.4
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.3.3/README.md` & `resotometrics-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.3/resotometrics/__main__.py` & `resotometrics-3.3.4/resotometrics/__main__.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.3/resotometrics/config.py` & `resotometrics-3.3.4/resotometrics/config.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.3/resotometrics/default_metrics.yaml` & `resotometrics-3.3.4/resotometrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.3/resotometrics/metrics.py` & `resotometrics-3.3.4/resotometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.3/resotometrics/search.py` & `resotometrics-3.3.4/resotometrics/search.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.3/resotometrics.egg-info/PKG-INFO` & `resotometrics-3.3.4/resotometrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.3.3
+Version: 3.3.4
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.3.3/setup.py` & `resotometrics-3.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.3.3/test/test_args.py` & `resotometrics-3.3.4/test/test_args.py`

 * *Files identical despite different names*

