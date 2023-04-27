# Comparing `tmp/kk-plugins-0.0.3.tar.gz` & `tmp/kk-plugins-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-plugins-0.0.3.tar", last modified: Wed Apr 26 16:11:45 2023, max compression
+gzip compressed data, was "kk-plugins-0.0.4.tar", last modified: Wed Apr 26 16:17:42 2023, max compression
```

## Comparing `kk-plugins-0.0.3.tar` & `kk-plugins-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:11:45.659168 kk-plugins-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 16:11:45.659168 kk-plugins-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 16:11:24.000000 kk-plugins-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:11:45.659168 kk-plugins-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-26 16:11:24.000000 kk-plugins-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:11:45.659168 kk-plugins-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:11:45.659168 kk-plugins-0.0.3/src/kk-plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:11:24.000000 kk-plugins-0.0.3/src/kk-plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:11:45.659168 kk-plugins-0.0.3/src/kk_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 16:11:45.000000 kk-plugins-0.0.3/src/kk_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 16:11:45.000000 kk-plugins-0.0.3/src/kk_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:11:45.000000 kk-plugins-0.0.3/src/kk_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-26 16:11:45.000000 kk-plugins-0.0.3/src/kk_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 16:11:45.000000 kk-plugins-0.0.3/src/kk_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.635626 kk-plugins-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.635626 kk-plugins-0.0.4/src/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/cmd/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.635626 kk-plugins-0.0.4/src/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/filter/bloomfilter_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/filter/cuckoofilter_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/src/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/github/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/src/kk_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 16:17:42.000000 kk-plugins-0.0.4/src/kk_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:42.639626 kk-plugins-0.0.4/src/scrapy_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:17:22.000000 kk-plugins-0.0.4/src/scrapy_plugins/__init__.py
```

### Comparing `kk-plugins-0.0.3/PKG-INFO` & `kk-plugins-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.0.3
+Version: 0.0.4
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kk-plugins-0.0.3/setup.py` & `kk-plugins-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.0.3/src/kk_plugins.egg-info/PKG-INFO` & `kk-plugins-0.0.4/src/kk_plugins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.0.3
+Version: 0.0.4
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

