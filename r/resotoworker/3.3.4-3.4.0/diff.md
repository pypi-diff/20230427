# Comparing `tmp/resotoworker-3.3.4.tar.gz` & `tmp/resotoworker-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.3.4.tar", last modified: Wed Apr 26 16:52:38 2023, max compression
+gzip compressed data, was "resotoworker-3.4.0.tar", last modified: Thu Apr 27 11:24:42 2023, max compression
```

## Comparing `resotoworker-3.3.4.tar` & `resotoworker-3.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:38.437504 resotoworker-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:49:36.000000 resotoworker-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-26 16:52:38.437504 resotoworker-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-26 16:49:36.000000 resotoworker-3.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-26 16:49:36.000000 resotoworker-3.3.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:38.433504 resotoworker-3.3.4/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-26 16:49:36.000000 resotoworker-3.3.4/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:38.437504 resotoworker-3.3.4/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-26 16:52:38.000000 resotoworker-3.3.4/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-26 16:52:38.000000 resotoworker-3.3.4/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:38.000000 resotoworker-3.3.4/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 16:52:38.000000 resotoworker-3.3.4/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:52:38.000000 resotoworker-3.3.4/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 16:52:38.000000 resotoworker-3.3.4/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 16:52:38.000000 resotoworker-3.3.4/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:52:38.441504 resotoworker-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-26 16:49:36.000000 resotoworker-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:52:38.437504 resotoworker-3.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:49:36.000000 resotoworker-3.3.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 16:49:36.000000 resotoworker-3.3.4/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-26 16:49:36.000000 resotoworker-3.3.4/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-26 16:49:36.000000 resotoworker-3.3.4/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-26 16:49:36.000000 resotoworker-3.3.4/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-26 16:49:36.000000 resotoworker-3.3.4/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.280683 resotoworker-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:22:30.000000 resotoworker-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-27 11:24:42.280683 resotoworker-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-27 11:22:30.000000 resotoworker-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-27 11:22:30.000000 resotoworker-3.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.272683 resotoworker-3.4.0/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-27 11:22:30.000000 resotoworker-3.4.0/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.276683 resotoworker-3.4.0/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 11:24:42.000000 resotoworker-3.4.0/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:24:42.280683 resotoworker-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-27 11:22:30.000000 resotoworker-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:42.280683 resotoworker-3.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-27 11:22:30.000000 resotoworker-3.4.0/test/test_utils.py
```

### Comparing `resotoworker-3.3.4/PKG-INFO` & `resotoworker-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.3.4
+Version: 3.4.0
 Summary: Runs collector plugins and sends the result to resotocore.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoworker-3.3.4/README.md` & `resotoworker-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/__main__.py` & `resotoworker-3.4.0/resotoworker/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/cleanup.py` & `resotoworker-3.4.0/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/collect.py` & `resotoworker-3.4.0/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/config.py` & `resotoworker-3.4.0/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/pluginloader.py` & `resotoworker-3.4.0/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/resotocore.py` & `resotoworker-3.4.0/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/tag.py` & `resotoworker-3.4.0/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker/utils.py` & `resotoworker-3.4.0/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.4.0/resotoworker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.3.4
+Version: 3.4.0
 Summary: Runs collector plugins and sends the result to resotocore.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoworker-3.3.4/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.4.0/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/setup.py` & `resotoworker-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/test/test_collect.py` & `resotoworker-3.4.0/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/test/test_resotocore.py` & `resotoworker-3.4.0/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.3.4/test/test_utils.py` & `resotoworker-3.4.0/test/test_utils.py`

 * *Files identical despite different names*

