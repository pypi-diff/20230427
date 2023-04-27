# Comparing `tmp/ucsdasiga-1.0.0a4.tar.gz` & `tmp/ucsdasiga-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucsdasiga-1.0.0a4.tar", last modified: Thu Apr 27 00:17:27 2023, max compression
+gzip compressed data, was "ucsdasiga-1.0.0a5.tar", last modified: Thu Apr 27 00:20:28 2023, max compression
```

## Comparing `ucsdasiga-1.0.0a4.tar` & `ucsdasiga-1.0.0a5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 00:17:27.954477 ucsdasiga-1.0.0a4/
--rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasiga-1.0.0a4/LICENSE
--rw-rw-rw-   0        0        0     2243 2023-04-27 00:17:27.952475 ucsdasiga-1.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-27 00:15:43.000000 ucsdasiga-1.0.0a4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 00:17:27.871457 ucsdasiga-1.0.0a4/asiga/
--rw-rw-rw-   0        0        0     1119 2023-04-27 00:15:28.000000 ucsdasiga-1.0.0a4/asiga/__init__.py
--rw-rw-rw-   0        0        0       64 2023-04-26 03:35:05.000000 ucsdasiga-1.0.0a4/asiga/__main__.py
--rw-rw-rw-   0        0        0     2860 2023-04-26 22:40:41.000000 ucsdasiga-1.0.0a4/asiga/scraper.py
--rw-rw-rw-   0        0        0     1117 2023-04-27 00:16:04.000000 ucsdasiga-1.0.0a4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 00:17:27.954477 ucsdasiga-1.0.0a4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 00:17:27.950474 ucsdasiga-1.0.0a4/ucsdasiga.egg-info/
--rw-rw-rw-   0        0        0     2243 2023-04-27 00:17:27.000000 ucsdasiga-1.0.0a4/ucsdasiga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-27 00:17:27.000000 ucsdasiga-1.0.0a4/ucsdasiga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 00:17:27.000000 ucsdasiga-1.0.0a4/ucsdasiga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 00:17:27.000000 ucsdasiga-1.0.0a4/ucsdasiga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 00:20:28.309195 ucsdasiga-1.0.0a5/
+-rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasiga-1.0.0a5/LICENSE
+-rw-rw-rw-   0        0        0     2243 2023-04-27 00:20:28.309195 ucsdasiga-1.0.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-27 00:15:43.000000 ucsdasiga-1.0.0a5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 00:20:28.295022 ucsdasiga-1.0.0a5/asiga/
+-rw-rw-rw-   0        0        0     1119 2023-04-27 00:15:28.000000 ucsdasiga-1.0.0a5/asiga/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 03:35:05.000000 ucsdasiga-1.0.0a5/asiga/__main__.py
+-rw-rw-rw-   0        0        0     2860 2023-04-26 22:40:41.000000 ucsdasiga-1.0.0a5/asiga/scraper.py
+-rw-rw-rw-   0        0        0     1117 2023-04-27 00:19:34.000000 ucsdasiga-1.0.0a5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 00:20:28.309195 ucsdasiga-1.0.0a5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 00:20:28.305212 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/
+-rw-rw-rw-   0        0        0     2243 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-27 00:20:28.000000 ucsdasiga-1.0.0a5/ucsdasiga.egg-info/top_level.txt
```

### Comparing `ucsdasiga-1.0.0a4/LICENSE` & `ucsdasiga-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ucsdasiga-1.0.0a4/PKG-INFO` & `ucsdasiga-1.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucsdasiga
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: A simple API wrapper and web scraper for the UCSD Associated Students (AS) instructor grade archive.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ucsdasiga-1.0.0a4/asiga/__init__.py` & `ucsdasiga-1.0.0a5/asiga/__init__.py`

 * *Files identical despite different names*

### Comparing `ucsdasiga-1.0.0a4/asiga/scraper.py` & `ucsdasiga-1.0.0a5/asiga/scraper.py`

 * *Files identical despite different names*

### Comparing `ucsdasiga-1.0.0a4/pyproject.toml` & `ucsdasiga-1.0.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ucsdasiga"
-version = "1.0.0-a.4"
+version = "1.0.0-a.5"
 description = "A simple API wrapper and web scraper for the UCSD Associated Students (AS) instructor grade archive."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ucsdasiga-1.0.0a4/ucsdasiga.egg-info/PKG-INFO` & `ucsdasiga-1.0.0a5/ucsdasiga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucsdasiga
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: A simple API wrapper and web scraper for the UCSD Associated Students (AS) instructor grade archive.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

