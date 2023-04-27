# Comparing `tmp/hpdb-4.0.5.tar.gz` & `tmp/hpdb-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpdb-4.0.5.tar", last modified: Sun Feb 26 09:08:22 2023, max compression
+gzip compressed data, was "hpdb-4.0.7.tar", last modified: Thu Apr 27 21:24:48 2023, max compression
```

## Comparing `hpdb-4.0.5.tar` & `hpdb-4.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-02-26 09:08:22.358782 hpdb-4.0.5/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2022-10-05 15:05:32.000000 hpdb-4.0.5/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     2824 2023-02-26 09:08:22.358460 hpdb-4.0.5/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      979 2023-02-26 09:08:14.000000 hpdb-4.0.5/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-02-26 09:08:22.355427 hpdb-4.0.5/hpdb/
--rw-r--r--   0 hp         (501) staff       (20)       29 2022-10-05 15:18:03.000000 hpdb-4.0.5/hpdb/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     7520 2023-02-26 09:03:54.000000 hpdb-4.0.5/hpdb/dbclass.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-02-26 09:08:22.357911 hpdb-4.0.5/hpdb.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     2824 2023-02-26 09:08:22.000000 hpdb-4.0.5/hpdb.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      204 2023-02-26 09:08:22.000000 hpdb-4.0.5/hpdb.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-02-26 09:08:22.000000 hpdb-4.0.5/hpdb.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)       52 2023-02-26 09:08:22.000000 hpdb-4.0.5/hpdb.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        5 2023-02-26 09:08:22.000000 hpdb-4.0.5/hpdb.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1039 2023-02-26 09:08:14.000000 hpdb-4.0.5/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-02-26 09:08:22.358904 hpdb-4.0.5/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-04-27 21:24:48.759468 hpdb-4.0.7/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2022-10-05 15:05:32.000000 hpdb-4.0.7/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     2824 2023-04-27 21:24:48.758966 hpdb-4.0.7/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      979 2023-04-27 21:24:34.000000 hpdb-4.0.7/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-04-27 21:24:48.753093 hpdb-4.0.7/hpdb/
+-rw-r--r--   0 hp         (501) staff       (20)       29 2022-10-05 15:18:03.000000 hpdb-4.0.7/hpdb/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     7520 2023-02-26 09:03:54.000000 hpdb-4.0.7/hpdb/dbclass.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-04-27 21:24:48.758213 hpdb-4.0.7/hpdb.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     2824 2023-04-27 21:24:48.000000 hpdb-4.0.7/hpdb.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      204 2023-04-27 21:24:48.000000 hpdb-4.0.7/hpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-04-27 21:24:48.000000 hpdb-4.0.7/hpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)       52 2023-04-27 21:24:48.000000 hpdb-4.0.7/hpdb.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        5 2023-04-27 21:24:48.000000 hpdb-4.0.7/hpdb.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1039 2023-04-27 21:24:34.000000 hpdb-4.0.7/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-04-27 21:24:48.759628 hpdb-4.0.7/setup.cfg
```

### Comparing `hpdb-4.0.5/LICENSE` & `hpdb-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hpdb-4.0.5/PKG-INFO` & `hpdb-4.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpdb
-Version: 4.0.5
+Version: 4.0.7
 Summary: Makes working with existing sql databases super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -35,15 +35,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # HPDB
 
-Current version: 4.0.5
+Current version: 4.0.7
 ## dbClass
 ### installation
 python -m pip install hpdb
 
 ### usage
 
 #### settings.ini
```

### Comparing `hpdb-4.0.5/README.md` & `hpdb-4.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HPDB
 
-Current version: 4.0.5
+Current version: 4.0.7
 ## dbClass
 ### installation
 python -m pip install hpdb
 
 ### usage
 
 #### settings.ini
```

### Comparing `hpdb-4.0.5/hpdb/dbclass.py` & `hpdb-4.0.7/hpdb/dbclass.py`

 * *Files identical despite different names*

### Comparing `hpdb-4.0.5/hpdb.egg-info/PKG-INFO` & `hpdb-4.0.7/hpdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpdb
-Version: 4.0.5
+Version: 4.0.7
 Summary: Makes working with existing sql databases super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -35,15 +35,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # HPDB
 
-Current version: 4.0.5
+Current version: 4.0.7
 ## dbClass
 ### installation
 python -m pip install hpdb
 
 ### usage
 
 #### settings.ini
```

### Comparing `hpdb-4.0.5/pyproject.toml` & `hpdb-4.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hpdb"
-version = "4.0.5"
+version = "4.0.7"
 description = "Makes working with existing sql databases super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

