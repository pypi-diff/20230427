# Comparing `tmp/hyperfetch-1.0.7.tar.gz` & `tmp/hyperfetch-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfetch-1.0.7.tar", last modified: Thu Apr 27 12:57:39 2023, max compression
+gzip compressed data, was "hyperfetch-1.0.8.tar", last modified: Thu Apr 27 13:00:19 2023, max compression
```

## Comparing `hyperfetch-1.0.7.tar` & `hyperfetch-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:39.874173 hyperfetch-1.0.7/
--rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.7/LICENSE
--rw-rw-rw-   0        0        0    10466 2023-04-27 12:57:39.874173 hyperfetch-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.7/README.md
--rw-rw-rw-   0        0        0     1689 2023-04-27 12:57:07.000000 hyperfetch-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 12:57:39.874173 hyperfetch-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:39.834463 hyperfetch-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:39.839997 hyperfetch-1.0.7/src/hyperfetch/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:48:32.000000 hyperfetch-1.0.7/src/hyperfetch/__init__.py
--rw-rw-rw-   0        0        0    10569 2023-04-27 12:48:32.000000 hyperfetch-1.0.7/src/hyperfetch/alg_samplers.py
--rw-rw-rw-   0        0        0      654 2023-04-27 12:48:32.000000 hyperfetch-1.0.7/src/hyperfetch/auth_connection.py
--rw-rw-rw-   0        0        0     2118 2023-04-27 12:48:32.000000 hyperfetch-1.0.7/src/hyperfetch/callbacks.py
--rw-rw-rw-   0        0        0    34085 2023-04-27 12:55:49.000000 hyperfetch-1.0.7/src/hyperfetch/manager.py
--rw-rw-rw-   0        0        0     4994 2023-04-27 12:48:32.000000 hyperfetch-1.0.7/src/hyperfetch/tuning.py
--rw-rw-rw-   0        0        0      825 2023-04-27 12:48:32.000000 hyperfetch-1.0.7/src/hyperfetch/util.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:39.872182 hyperfetch-1.0.7/src/hyperfetch.egg-info/
--rw-rw-rw-   0        0        0    10466 2023-04-27 12:57:39.000000 hyperfetch-1.0.7/src/hyperfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-27 12:57:39.000000 hyperfetch-1.0.7/src/hyperfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:57:39.000000 hyperfetch-1.0.7/src/hyperfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-27 12:57:39.000000 hyperfetch-1.0.7/src/hyperfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      211 2023-04-27 12:57:39.000000 hyperfetch-1.0.7/src/hyperfetch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 12:57:39.000000 hyperfetch-1.0.7/src/hyperfetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.731766 hyperfetch-1.0.8/
+-rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0    10466 2023-04-27 13:00:19.731766 hyperfetch-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7935 2023-04-25 16:34:58.000000 hyperfetch-1.0.8/README.md
+-rw-rw-rw-   0        0        0     1689 2023-04-27 13:00:05.000000 hyperfetch-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:00:19.731766 hyperfetch-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.702104 hyperfetch-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.710359 hyperfetch-1.0.8/src/hyperfetch/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/alg_samplers.py
+-rw-rw-rw-   0        0        0      654 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/auth_connection.py
+-rw-rw-rw-   0        0        0     2118 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/callbacks.py
+-rw-rw-rw-   0        0        0    34085 2023-04-27 12:55:49.000000 hyperfetch-1.0.8/src/hyperfetch/manager.py
+-rw-rw-rw-   0        0        0     4994 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/tuning.py
+-rw-rw-rw-   0        0        0      825 2023-04-27 12:48:32.000000 hyperfetch-1.0.8/src/hyperfetch/util.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:00:19.731260 hyperfetch-1.0.8/src/hyperfetch.egg-info/
+-rw-rw-rw-   0        0        0    10466 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      211 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 13:00:19.000000 hyperfetch-1.0.8/src/hyperfetch.egg-info/top_level.txt
```

### Comparing `hyperfetch-1.0.7/LICENSE` & `hyperfetch-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/PKG-INFO` & `hyperfetch-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.7
+Version: 1.0.8
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```

### Comparing `hyperfetch-1.0.7/README.md` & `hyperfetch-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/pyproject.toml` & `hyperfetch-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["hyperfetch"]
 
 [project]
 name = "hyperfetch"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Karoline Sund Wahl", email="karolines.wahl@gmail.com" },
 ]
 description = "HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application."
 readme = "README.md"
 requires-python = ">=3.9, <3.11.0"
 license = {file = "LICENSE"}
```

### Comparing `hyperfetch-1.0.7/src/hyperfetch/alg_samplers.py` & `hyperfetch-1.0.8/src/hyperfetch/alg_samplers.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/src/hyperfetch/auth_connection.py` & `hyperfetch-1.0.8/src/hyperfetch/auth_connection.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/src/hyperfetch/callbacks.py` & `hyperfetch-1.0.8/src/hyperfetch/callbacks.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/src/hyperfetch/manager.py` & `hyperfetch-1.0.8/src/hyperfetch/manager.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/src/hyperfetch/tuning.py` & `hyperfetch-1.0.8/src/hyperfetch/tuning.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/src/hyperfetch/util.py` & `hyperfetch-1.0.8/src/hyperfetch/util.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.7/src/hyperfetch.egg-info/PKG-INFO` & `hyperfetch-1.0.8/src/hyperfetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.7
+Version: 1.0.8
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```

