# Comparing `tmp/dask-felleskomponenter-0.0.5.tar.gz` & `tmp/dask-felleskomponenter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jonas/src/dask-felleskomponenter/dist/.tmp-cifv_ohh/dask-felleskomponenter-0.0.5.tar", last modified: Fri Mar 24 10:49:26 2023, max compression
+gzip compressed data, was "/Users/jonas/src/dask-felleskomponenter/beam-components/dist/.tmp-dt4kkupr/dask-felleskomponenter-0.0.6.tar", last modified: Thu Apr 27 12:05:26 2023, max compression
```

## Comparing `dask-felleskomponenter-0.0.5.tar` & `dask-felleskomponenter-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/
--rw-r--r--   0 jonas      (602) staff       (20)     1047 2023-03-23 08:01:02.000000 dask-felleskomponenter-0.0.5/LICENSE.txt
--rw-r--r--   0 jonas      (602) staff       (20)     1202 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/PKG-INFO
--rw-r--r--   0 jonas      (602) staff       (20)      602 2023-03-24 09:33:29.000000 dask-felleskomponenter-0.0.5/README.md
--rw-r--r--   0 jonas      (602) staff       (20)      112 2023-03-23 09:54:58.000000 dask-felleskomponenter-0.0.5/pyproject.toml
--rw-r--r--   0 jonas      (602) staff       (20)       38 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/setup.cfg
--rw-r--r--   0 jonas      (602) staff       (20)      923 2023-03-24 10:48:29.000000 dask-felleskomponenter-0.0.5/setup.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 10:15:30.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/__init__.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/common/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 09:48:20.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/common/__init__.py
--rw-r--r--   0 jonas      (602) staff       (20)      899 2023-03-24 10:47:56.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/common/api_client.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/sources/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 07:45:40.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/sources/__init__.py
--rw-r--r--   0 jonas      (602) staff       (20)     1919 2023-03-24 10:47:51.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/sources/api_source.py
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter.egg-info/
--rw-r--r--   0 jonas      (602) staff       (20)     1202 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter.egg-info/PKG-INFO
--rw-r--r--   0 jonas      (602) staff       (20)      554 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter.egg-info/SOURCES.txt
--rw-r--r--   0 jonas      (602) staff       (20)        1 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter.egg-info/dependency_links.txt
--rw-r--r--   0 jonas      (602) staff       (20)       29 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/dask_felleskomponenter.egg-info/top_level.txt
-drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-03-24 10:49:26.000000 dask-felleskomponenter-0.0.5/src/tests/
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 08:14:30.000000 dask-felleskomponenter-0.0.5/src/tests/__init__.py
--rw-r--r--   0 jonas      (602) staff       (20)      323 2023-03-23 10:16:33.000000 dask-felleskomponenter-0.0.5/src/tests/test_api_client.py
--rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 13:26:55.000000 dask-felleskomponenter-0.0.5/src/tests/test_api_source.py
+drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/
+-rw-r--r--   0 jonas      (602) staff       (20)     1047 2023-03-23 08:01:02.000000 dask-felleskomponenter-0.0.6/LICENSE.txt
+-rw-r--r--   0 jonas      (602) staff       (20)     1202 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/PKG-INFO
+-rw-r--r--   0 jonas      (602) staff       (20)      602 2023-03-24 09:33:29.000000 dask-felleskomponenter-0.0.6/README.md
+-rw-r--r--   0 jonas      (602) staff       (20)      112 2023-03-23 09:54:58.000000 dask-felleskomponenter-0.0.6/pyproject.toml
+-rw-r--r--   0 jonas      (602) staff       (20)       38 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/setup.cfg
+-rw-r--r--   0 jonas      (602) staff       (20)      923 2023-04-27 12:00:29.000000 dask-felleskomponenter-0.0.6/setup.py
+drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/
+drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/
+-rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 10:15:30.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/__init__.py
+drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/common/
+-rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 09:48:20.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/common/__init__.py
+-rw-r--r--   0 jonas      (602) staff       (20)      899 2023-03-24 10:47:56.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/common/api_client.py
+drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/sources/
+-rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 07:45:40.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/sources/__init__.py
+-rw-r--r--   0 jonas      (602) staff       (20)     1919 2023-03-24 12:30:15.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/sources/api_source.py
+drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter.egg-info/
+-rw-r--r--   0 jonas      (602) staff       (20)     1202 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter.egg-info/PKG-INFO
+-rw-r--r--   0 jonas      (602) staff       (20)      554 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas      (602) staff       (20)        1 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas      (602) staff       (20)       29 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/dask_felleskomponenter.egg-info/top_level.txt
+drwxr-xr-x   0 jonas      (602) staff       (20)        0 2023-04-27 12:05:26.000000 dask-felleskomponenter-0.0.6/src/tests/
+-rw-r--r--   0 jonas      (602) staff       (20)        0 2023-03-23 08:14:30.000000 dask-felleskomponenter-0.0.6/src/tests/__init__.py
+-rw-r--r--   0 jonas      (602) staff       (20)      267 2023-03-24 12:38:52.000000 dask-felleskomponenter-0.0.6/src/tests/test_api_client.py
+-rw-r--r--   0 jonas      (602) staff       (20)      941 2023-04-04 14:13:30.000000 dask-felleskomponenter-0.0.6/src/tests/test_api_source.py
```

### Comparing `dask-felleskomponenter-0.0.5/LICENSE.txt` & `dask-felleskomponenter-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.5/PKG-INFO` & `dask-felleskomponenter-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-felleskomponenter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Felleskomponeneter for utvikling av Apache Beam pipelines
 Home-page: https://github.com/kartverket/dask-felleskomponenter
 Author: Dataplattform@Statens Kartverk
 Author-email: dataplattform@kartverket.no
 Project-URL: Bug Tracker, https://github.com/kartverket/dask-felleskomponenter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dask-felleskomponenter-0.0.5/README.md` & `dask-felleskomponenter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.5/setup.py` & `dask-felleskomponenter-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "dask-felleskomponenter",
-    version = "0.0.5",
+    version = "0.0.6",
     author = "Dataplattform@Statens Kartverk",
     author_email = "dataplattform@kartverket.no",
     description = "Felleskomponeneter for utvikling av Apache Beam pipelines",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kartverket/dask-felleskomponenter",
     project_urls = {
```

### Comparing `dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/common/api_client.py` & `dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/common/api_client.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.5/src/dask_felleskomponenter/sources/api_source.py` & `dask-felleskomponenter-0.0.6/src/dask_felleskomponenter/sources/api_source.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.5/src/dask_felleskomponenter.egg-info/PKG-INFO` & `dask-felleskomponenter-0.0.6/src/dask_felleskomponenter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-felleskomponenter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Felleskomponeneter for utvikling av Apache Beam pipelines
 Home-page: https://github.com/kartverket/dask-felleskomponenter
 Author: Dataplattform@Statens Kartverk
 Author-email: dataplattform@kartverket.no
 Project-URL: Bug Tracker, https://github.com/kartverket/dask-felleskomponenter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dask-felleskomponenter-0.0.5/src/dask_felleskomponenter.egg-info/SOURCES.txt` & `dask-felleskomponenter-0.0.6/src/dask_felleskomponenter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

