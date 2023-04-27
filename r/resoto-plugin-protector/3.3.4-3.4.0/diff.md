# Comparing `tmp/resoto-plugin-protector-3.3.4.tar.gz` & `tmp/resoto-plugin-protector-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-protector-3.3.4.tar", last modified: Wed Apr 26 16:51:17 2023, max compression
+gzip compressed data, was "resoto-plugin-protector-3.4.0.tar", last modified: Thu Apr 27 11:22:01 2023, max compression
```

## Comparing `resoto-plugin-protector-3.3.4.tar` & `resoto-plugin-protector-3.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.197383 resoto-plugin-protector-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:49:29.000000 resoto-plugin-protector-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-26 16:51:17.197383 resoto-plugin-protector-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 16:49:29.000000 resoto-plugin-protector-3.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:49:29.000000 resoto-plugin-protector-3.3.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.193383 resoto-plugin-protector-3.3.4/resoto_plugin_protector/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-26 16:49:29.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-26 16:49:29.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.197383 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-26 16:51:17.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 16:51:17.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:17.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 16:51:17.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:17.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 16:51:17.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 16:51:17.000000 resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:51:17.197383 resoto-plugin-protector-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 16:49:29.000000 resoto-plugin-protector-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:17.197383 resoto-plugin-protector-3.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-26 16:49:29.000000 resoto-plugin-protector-3.3.4/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:01.870856 resoto-plugin-protector-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:19:58.000000 resoto-plugin-protector-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-27 11:22:01.870856 resoto-plugin-protector-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-27 11:19:58.000000 resoto-plugin-protector-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:19:58.000000 resoto-plugin-protector-3.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:01.866855 resoto-plugin-protector-3.4.0/resoto_plugin_protector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-27 11:19:58.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-27 11:19:58.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:01.870856 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-27 11:22:01.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-27 11:22:01.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:01.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 11:22:01.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:22:01.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 11:22:01.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 11:22:01.000000 resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 11:22:01.870856 resoto-plugin-protector-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-27 11:19:58.000000 resoto-plugin-protector-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:22:01.870856 resoto-plugin-protector-3.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 11:19:58.000000 resoto-plugin-protector-3.4.0/test/test_config.py
```

### Comparing `resoto-plugin-protector-3.3.4/PKG-INFO` & `resoto-plugin-protector-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.3.4
+Version: 3.4.0
 Summary: Resoto Protector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/protector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-protector-3.3.4/README.md` & `resoto-plugin-protector-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.3.4/resoto_plugin_protector/__init__.py` & `resoto-plugin-protector-3.4.0/resoto_plugin_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.3.4/resoto_plugin_protector/config.py` & `resoto-plugin-protector-3.4.0/resoto_plugin_protector/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.3.4/resoto_plugin_protector.egg-info/PKG-INFO` & `resoto-plugin-protector-3.4.0/resoto_plugin_protector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.3.4
+Version: 3.4.0
 Summary: Resoto Protector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/protector
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-protector-3.3.4/setup.py` & `resoto-plugin-protector-3.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-protector",
-    version="3.3.4",
+    version="3.4.0",
     description="Resoto Protector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["protector = resoto_plugin_protector:ProtectorPlugin"]},
     include_package_data=True,
```

