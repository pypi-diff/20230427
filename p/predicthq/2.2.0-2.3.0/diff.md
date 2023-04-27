# Comparing `tmp/predicthq-2.2.0.tar.gz` & `tmp/predicthq-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predicthq-2.2.0.tar", last modified: Wed Feb  8 02:01:33 2023, max compression
+gzip compressed data, was "predicthq-2.3.0.tar", last modified: Thu Apr 27 21:15:33 2023, max compression
```

## Comparing `predicthq-2.2.0.tar` & `predicthq-2.3.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-08 02:01:26.000000 predicthq-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-08 02:01:26.000000 predicthq-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-02-08 02:01:33.892872 predicthq-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-02-08 02:01:26.000000 predicthq-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.888872 predicthq-2.2.0/predicthq/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/oauth2/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/oauth2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/v1/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/accounts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/accounts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/v1/broadcasts/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/broadcasts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/broadcasts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/broadcasts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/v1/events/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/events/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/v1/features/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/features/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/features/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/v1/places/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/places/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/places/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/places/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq/endpoints/v1/radius/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/radius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/radius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/endpoints/v1/radius/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-08 02:01:26.000000 predicthq-2.2.0/predicthq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/predicthq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-02-08 02:01:33.000000 predicthq-2.2.0/predicthq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-08 02:01:33.000000 predicthq-2.2.0/predicthq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 02:01:33.000000 predicthq-2.2.0/predicthq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-08 02:01:33.000000 predicthq-2.2.0/predicthq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-08 02:01:33.000000 predicthq-2.2.0/predicthq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-08 02:01:33.892872 predicthq-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-08 02:01:26.000000 predicthq-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:01:33.892872 predicthq-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-02-08 02:01:26.000000 predicthq-2.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-02-08 02:01:26.000000 predicthq-2.2.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 21:15:23.000000 predicthq-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-27 21:15:23.000000 predicthq-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-27 21:15:33.252367 predicthq-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-27 21:15:23.000000 predicthq-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/oauth2/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/oauth2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/accounts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/accounts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/events/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/features/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/features/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/places/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/places/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/places/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/places/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq/endpoints/v1/radius/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/radius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/radius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/endpoints/v1/radius/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 21:15:23.000000 predicthq-2.3.0/predicthq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/predicthq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 21:15:33.000000 predicthq-2.3.0/predicthq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 21:15:33.256367 predicthq-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-27 21:15:23.000000 predicthq-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:15:33.252367 predicthq-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-27 21:15:23.000000 predicthq-2.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-27 21:15:23.000000 predicthq-2.3.0/tests/test_config.py
```

### Comparing `predicthq-2.2.0/LICENSE` & `predicthq-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/PKG-INFO` & `predicthq-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 2.2.0
+Version: 2.3.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-2.2.0/README.md` & `predicthq-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/client.py` & `predicthq-2.3.0/predicthq/client.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/config.py` & `predicthq-2.3.0/predicthq/config.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/base.py` & `predicthq-2.3.0/predicthq/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/decorators.py` & `predicthq-2.3.0/predicthq/endpoints/decorators.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/oauth2/endpoint.py` & `predicthq-2.3.0/predicthq/endpoints/oauth2/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/oauth2/schemas.py` & `predicthq-2.3.0/predicthq/endpoints/oauth2/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/schemas.py` & `predicthq-2.3.0/predicthq/endpoints/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,37 @@
 
     import_format = r"@(?P<latitude>-?\d+(\.\d+)?),(?P<longitude>-?\d+(\.\d+)?)"
     export_format = "@{latitude},{longitude}"
 
     latitude = FloatType(required=True)
     longitude = FloatType(required=True)
 
+# see https://github.com/predicthq/sdk-py/pull/84#discussion_r1163399743
+# ParentType requires either the value to be a boolean value or an enum value
+# therefore, we need to create a custom type that allows both
+class BooleanOrEnumType(BooleanType):
+    def __init__(self, *args, **kwargs):
+        self.enum_values = kwargs.pop("choices")
+        super().__init__(*args, **kwargs)
+
+    def to_native(self, value, context=None):
+        try:
+            return super().to_native(value, context)
+        except ConversionError:
+            if value not in self.enum_values:
+                raise ConversionError(u"Must be either a boolean or any of: {}.".format([x for x in self.enum_values]))
+            return value
+
+
+class ParentType(Model):
+    class Options:
+        serialize_when_none = False
+
+    include = BooleanOrEnumType(choices=("only",))
+
 
 class Place(Model):
     class Options:
         serialize_when_none = False
 
     scope = ListType(StringType)
     exact = ListType(StringType)
```

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/broadcasts/endpoint.py` & `predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/broadcasts/schemas.py` & `predicthq-2.3.0/predicthq/endpoints/v1/broadcasts/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/events/endpoint.py` & `predicthq-2.3.0/predicthq/endpoints/v1/events/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/events/schemas.py` & `predicthq-2.3.0/predicthq/endpoints/v1/events/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     IntRange,
     IntType,
     ListType,
     LocationAround,
     Model,
     ModelType,
     PaginatedMixin,
+    ParentType,
     Place,
     PolyModelType,
     ResultSet,
     ResultType,
     SortableMixin,
     StringListType,
     StringModelType,
@@ -40,22 +41,23 @@
     country = ListType(StringType)
     deleted_reason = ListType(StringType(choices=("cancelled", "duplicate", "invalid", "postponed")))
     end = ModelType(DateTimeRange)
     end_around = ModelType(DateAround)
     id = ListType(StringType)
     label = ListType(StringType)
     location_around = ModelType(LocationAround)
+    parent = ModelType(ParentType)
     place = ModelType(Place)
     placekey = StringType()
     postponed = ModelType(DateTimeRange)
     q = StringType()
     relevance = ListType(StringType)
     start = ModelType(DateTimeRange)
     start_around = ModelType(DateAround)
-    state = ListType(StringType(choices=("active", "deleted"), default="active"))
+    state = ListType(StringType(choices=("active", "deleted", "predicted"), default="active"))
     updated = ModelType(DateTimeRange)
     within = StringListType(StringModelType(Area), separator="+")
 
     # The below parameters are only available if they are enabled in your plan.
     # If you are not subscribed to a feature, using the parameter will have no
     # effect on your search results.
     aviation_rank = ModelType(IntRange)
```

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/features/endpoint.py` & `predicthq-2.3.0/predicthq/endpoints/v1/features/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/features/schemas.py` & `predicthq-2.3.0/predicthq/endpoints/v1/features/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/places/schemas.py` & `predicthq-2.3.0/predicthq/endpoints/v1/places/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/radius/endpoint.py` & `predicthq-2.3.0/predicthq/endpoints/v1/radius/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq/endpoints/v1/radius/schemas.py` & `predicthq-2.3.0/predicthq/endpoints/v1/radius/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/predicthq.egg-info/PKG-INFO` & `predicthq-2.3.0/predicthq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 2.2.0
+Version: 2.3.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-2.2.0/predicthq.egg-info/SOURCES.txt` & `predicthq-2.3.0/predicthq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/setup.py` & `predicthq-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/tests/test_client.py` & `predicthq-2.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `predicthq-2.2.0/tests/test_config.py` & `predicthq-2.3.0/tests/test_config.py`

 * *Files identical despite different names*

