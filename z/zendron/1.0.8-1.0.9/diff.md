# Comparing `tmp/zendron-1.0.8.tar.gz` & `tmp/zendron-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.0.8.tar", last modified: Wed Apr 26 08:21:23 2023, max compression
+gzip compressed data, was "zendron-1.0.9.tar", last modified: Wed Apr 26 08:29:22 2023, max compression
```

## Comparing `zendron-1.0.8.tar` & `zendron-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:21:23.081493 zendron-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 08:21:08.000000 zendron-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 08:21:08.000000 zendron-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-26 08:21:23.081493 zendron-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-26 08:21:08.000000 zendron-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:21:23.077493 zendron-1.0.8/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:21:08.000000 zendron-1.0.8/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 08:21:08.000000 zendron-1.0.8/conf/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 08:21:08.000000 zendron-1.0.8/conf/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 08:21:08.000000 zendron-1.0.8/conf/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 08:21:08.000000 zendron-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:21:23.081493 zendron-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:21:23.077493 zendron-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:21:23.081493 zendron-1.0.8/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/comments_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-26 08:21:08.000000 zendron-1.0.8/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:21:23.081493 zendron-1.0.8/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-26 08:21:23.000000 zendron-1.0.8/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 08:21:23.000000 zendron-1.0.8/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:21:23.000000 zendron-1.0.8/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 08:21:23.000000 zendron-1.0.8/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 08:21:23.000000 zendron-1.0.8/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 08:21:23.000000 zendron-1.0.8/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.953232 zendron-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 08:28:56.000000 zendron-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 08:28:56.000000 zendron-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-26 08:29:22.953232 zendron-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-26 08:28:56.000000 zendron-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.949232 zendron-1.0.9/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 08:28:56.000000 zendron-1.0.9/conf/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 08:28:56.000000 zendron-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:29:22.953232 zendron-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.949232 zendron-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.949232 zendron-1.0.9/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/comments_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-26 08:28:56.000000 zendron-1.0.9/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:29:22.953232 zendron-1.0.9/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 08:29:22.000000 zendron-1.0.9/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.0.8/LICENSE` & `zendron-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/PKG-INFO` & `zendron-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.0.8
+Version: 1.0.9
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
-Version: 1.0.8
+Version: 1.0.9
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
```

### Comparing `zendron-1.0.8/README.md` & `zendron-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Zendron
 
-Version: 1.0.8
+Version: 1.0.9
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
```

### Comparing `zendron-1.0.8/pyproject.toml` & `zendron-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=65.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.0.8"
+version = "1.0.9"
 description = "Import Zotero annotations with Dendron integration"
 readme = "README.md"
 authors = [{ name = "Michael Volk", email = "michaeljvolk7@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zendron-1.0.8/src/zendron/__main__.py` & `zendron-1.0.9/src/zendron/__main__.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/annotations.py` & `zendron-1.0.9/src/zendron/annotations.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/bibtex.py` & `zendron-1.0.9/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/cache.py` & `zendron-1.0.9/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/cache_deprecated.py` & `zendron-1.0.9/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/comments.py` & `zendron-1.0.9/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/comments_deprecated.py` & `zendron-1.0.9/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/config.py` & `zendron-1.0.9/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/front.py` & `zendron-1.0.9/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/init.py` & `zendron-1.0.9/src/zendron/init.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/items.py` & `zendron-1.0.9/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/load.py` & `zendron-1.0.9/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/metadata.py` & `zendron-1.0.9/src/zendron/metadata.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/read_md.py` & `zendron-1.0.9/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/remove.py` & `zendron-1.0.9/src/zendron/remove.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/scratch.py` & `zendron-1.0.9/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/sync.py` & `zendron-1.0.9/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron/user_citation_key.py` & `zendron-1.0.9/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.0.8/src/zendron.egg-info/PKG-INFO` & `zendron-1.0.9/src/zendron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.0.8
+Version: 1.0.9
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Zendron
 
-Version: 1.0.8
+Version: 1.0.9
 
 ## Introduction
 
 - This package was developed for porting Zotero annotations and metadata to markdown. These markdown notes are then brought into a [Dendron](https://www.dendron.so/) hierarchy for integration with vault notes. We recommend using the package within [Visual Studio Code](https://code.visualstudio.com/).The end goal is to get a two way sync between notes in Zotero and notes in Dendron, but this has some difficulties and limitations that are taking some time to address. For now only a one way sync from Zotero to Dendron is supported.
 
 ## Install Instructions
```

### Comparing `zendron-1.0.8/src/zendron.egg-info/SOURCES.txt` & `zendron-1.0.9/src/zendron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

