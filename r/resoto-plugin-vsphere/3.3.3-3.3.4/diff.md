# Comparing `tmp/resoto-plugin-vsphere-3.3.3.tar.gz` & `tmp/resoto-plugin-vsphere-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-vsphere-3.3.3.tar", last modified: Fri Apr 21 14:36:49 2023, max compression
+gzip compressed data, was "resoto-plugin-vsphere-3.3.4.tar", last modified: Wed Apr 26 16:54:45 2023, max compression
```

## Comparing `resoto-plugin-vsphere-3.3.3.tar` & `resoto-plugin-vsphere-3.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:49.778390 resoto-plugin-vsphere-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 14:36:49.778390 resoto-plugin-vsphere-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:49.774390 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/vsphere_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:49.778390 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 14:36:49.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-21 14:36:49.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:36:49.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 14:36:49.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:36:49.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 14:36:49.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 14:36:49.000000 resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:36:49.778390 resoto-plugin-vsphere-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:49.778390 resoto-plugin-vsphere-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-21 14:35:04.000000 resoto-plugin-vsphere-3.3.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:45.624503 resoto-plugin-vsphere-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 16:54:45.624503 resoto-plugin-vsphere-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:45.620503 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/vsphere_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:45.624503 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 16:54:45.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-26 16:54:45.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:54:45.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 16:54:45.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:54:45.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 16:54:45.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 16:54:45.000000 resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:54:45.624503 resoto-plugin-vsphere-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:45.624503 resoto-plugin-vsphere-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-26 16:52:36.000000 resoto-plugin-vsphere-3.3.4/test/test_config.py
```

### Comparing `resoto-plugin-vsphere-3.3.3/PKG-INFO` & `resoto-plugin-vsphere-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.3.3
+Version: 3.3.4
 Summary: Resoto VSphere Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/vsphere
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/__init__.py` & `resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/config.py` & `resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/resources.py` & `resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere/vsphere_client.py` & `resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere/vsphere_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/PKG-INFO` & `resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-vsphere
-Version: 3.3.3
+Version: 3.3.4
 Summary: Resoto VSphere Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/vsphere
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-vsphere-3.3.3/resoto_plugin_vsphere.egg-info/SOURCES.txt` & `resoto-plugin-vsphere-3.3.4/resoto_plugin_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-vsphere-3.3.3/setup.py` & `resoto-plugin-vsphere-3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-vsphere",
-    version="3.3.3",
+    version="3.3.4",
     description="Resoto VSphere Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["vsphere = resoto_plugin_vsphere:VSphereCollectorPlugin"]},
     include_package_data=True,
```

