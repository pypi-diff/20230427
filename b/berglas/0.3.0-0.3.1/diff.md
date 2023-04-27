# Comparing `tmp/berglas-0.3.0.tar.gz` & `tmp/berglas-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berglas-0.3.0.tar", last modified: Tue Apr 18 21:02:58 2023, max compression
+gzip compressed data, was "berglas-0.3.1.tar", last modified: Thu Apr 27 18:48:21 2023, max compression
```

## Comparing `berglas-0.3.0.tar` & `berglas-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-18 21:02:58.533967 berglas-0.3.0/
--rw-r--r--   0 maru       (501) staff       (20)    11345 2023-04-11 20:34:42.000000 berglas-0.3.0/LICENSE
--rw-r--r--   0 maru       (501) staff       (20)     4406 2023-04-18 21:02:58.534024 berglas-0.3.0/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)     3476 2023-04-18 20:55:34.000000 berglas-0.3.0/README.rst
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-18 21:02:58.533240 berglas-0.3.0/berglas/
--rw-r--r--   0 maru       (501) staff       (20)       87 2023-04-18 21:02:57.000000 berglas-0.3.0/berglas/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     1255 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/auto.py
--rw-r--r--   0 maru       (501) staff       (20)      271 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/constants.py
--rw-r--r--   0 maru       (501) staff       (20)       41 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)     4610 2023-04-18 20:43:05.000000 berglas-0.3.0/berglas/resolver.py
--rw-r--r--   0 maru       (501) staff       (20)     4616 2023-04-11 20:34:42.000000 berglas-0.3.0/berglas/runtime.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-18 21:02:58.533868 berglas-0.3.0/berglas.egg-info/
--rw-r--r--   0 maru       (501) staff       (20)     4406 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)      324 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/SOURCES.txt
--rw-r--r--   0 maru       (501) staff       (20)        1 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/dependency_links.txt
--rw-r--r--   0 maru       (501) staff       (20)      190 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/requires.txt
--rw-r--r--   0 maru       (501) staff       (20)        8 2023-04-18 21:02:58.000000 berglas-0.3.0/berglas.egg-info/top_level.txt
--rw-r--r--   0 maru       (501) staff       (20)      211 2023-04-11 20:34:42.000000 berglas-0.3.0/pyproject.toml
--rw-r--r--   0 maru       (501) staff       (20)      256 2023-04-18 21:02:58.534263 berglas-0.3.0/setup.cfg
--rw-r--r--   0 maru       (501) staff       (20)     2626 2023-04-18 20:43:05.000000 berglas-0.3.0/setup.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-27 18:48:21.675211 berglas-0.3.1/
+-rw-r--r--   0 maru       (501) staff       (20)    11345 2023-04-11 20:34:42.000000 berglas-0.3.1/LICENSE
+-rw-r--r--   0 maru       (501) staff       (20)     4406 2023-04-27 18:48:21.675282 berglas-0.3.1/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)     3476 2023-04-18 20:55:34.000000 berglas-0.3.1/README.rst
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-27 18:48:21.674420 berglas-0.3.1/berglas/
+-rw-r--r--   0 maru       (501) staff       (20)       87 2023-04-27 18:48:21.000000 berglas-0.3.1/berglas/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     1255 2023-04-11 20:34:42.000000 berglas-0.3.1/berglas/auto.py
+-rw-r--r--   0 maru       (501) staff       (20)      271 2023-04-11 20:34:42.000000 berglas-0.3.1/berglas/constants.py
+-rw-r--r--   0 maru       (501) staff       (20)       41 2023-04-11 20:34:42.000000 berglas-0.3.1/berglas/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)     4609 2023-04-27 18:46:43.000000 berglas-0.3.1/berglas/resolver.py
+-rw-r--r--   0 maru       (501) staff       (20)     4616 2023-04-11 20:34:42.000000 berglas-0.3.1/berglas/runtime.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-04-27 18:48:21.675074 berglas-0.3.1/berglas.egg-info/
+-rw-r--r--   0 maru       (501) staff       (20)     4406 2023-04-27 18:48:21.000000 berglas-0.3.1/berglas.egg-info/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)      324 2023-04-27 18:48:21.000000 berglas-0.3.1/berglas.egg-info/SOURCES.txt
+-rw-r--r--   0 maru       (501) staff       (20)        1 2023-04-27 18:48:21.000000 berglas-0.3.1/berglas.egg-info/dependency_links.txt
+-rw-r--r--   0 maru       (501) staff       (20)      190 2023-04-27 18:48:21.000000 berglas-0.3.1/berglas.egg-info/requires.txt
+-rw-r--r--   0 maru       (501) staff       (20)        8 2023-04-27 18:48:21.000000 berglas-0.3.1/berglas.egg-info/top_level.txt
+-rw-r--r--   0 maru       (501) staff       (20)      211 2023-04-11 20:34:42.000000 berglas-0.3.1/pyproject.toml
+-rw-r--r--   0 maru       (501) staff       (20)      256 2023-04-27 18:48:21.675507 berglas-0.3.1/setup.cfg
+-rw-r--r--   0 maru       (501) staff       (20)     2626 2023-04-18 20:43:05.000000 berglas-0.3.1/setup.py
```

### Comparing `berglas-0.3.0/LICENSE` & `berglas-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `berglas-0.3.0/PKG-INFO` & `berglas-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berglas
-Version: 0.3.0
+Version: 0.3.1
 Summary: Berglas Python Library
 Home-page: https://github.com/maroux/berglas-python
 Author: Aniruddha Maru
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: secrets gcs gcp
```

### Comparing `berglas-0.3.0/README.rst` & `berglas-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `berglas-0.3.0/berglas/auto.py` & `berglas-0.3.1/berglas/auto.py`

 * *Files identical despite different names*

### Comparing `berglas-0.3.0/berglas/resolver.py` & `berglas-0.3.1/berglas/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         if not blob:
             raise AutoException("secret object not found")
 
         if not blob.metadata or not blob.metadata.get(METADATA_KMS_KEY):
             raise AutoException("missing kms key in secret metadata")
 
         key = blob.metadata[METADATA_KMS_KEY]
-        data = blob.download_as_string()
+        data = blob.download_as_bytes()
         parts = data.split(b":", maxsplit=1)
         if len(parts) < 2:
             raise AutoException("invalid ciphertext: not enough parts")
 
         try:
             enc_dek = base64.decodebytes(parts[0])
         except binascii.Error:
```

### Comparing `berglas-0.3.0/berglas/runtime.py` & `berglas-0.3.1/berglas/runtime.py`

 * *Files identical despite different names*

### Comparing `berglas-0.3.0/berglas.egg-info/PKG-INFO` & `berglas-0.3.1/berglas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berglas
-Version: 0.3.0
+Version: 0.3.1
 Summary: Berglas Python Library
 Home-page: https://github.com/maroux/berglas-python
 Author: Aniruddha Maru
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: secrets gcs gcp
```

### Comparing `berglas-0.3.0/setup.py` & `berglas-0.3.1/setup.py`

 * *Files identical despite different names*

