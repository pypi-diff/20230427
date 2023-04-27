# Comparing `tmp/rssfixer-0.1.2.tar.gz` & `tmp/rssfixer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.1.2.tar", last modified: Wed Apr 26 18:22:47 2023, max compression
+gzip compressed data, was "rssfixer-0.1.3.tar", last modified: Wed Apr 26 18:45:41 2023, max compression
```

## Comparing `rssfixer-0.1.2.tar` & `rssfixer-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.494967 rssfixer-0.1.2/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.2/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:22:47.494778 rssfixer-0.1.2/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     8682 2023-04-26 18:07:49.000000 rssfixer-0.1.2/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-26 18:21:32.000000 rssfixer-0.1.2/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-26 18:22:47.495013 rssfixer-0.1.2/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.491680 rssfixer-0.1.2/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.493028 rssfixer-0.1.2/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.2/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)    12431 2023-04-26 18:06:57.000000 rssfixer-0.1.2/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.494007 rssfixer-0.1.2/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      371 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-26 18:22:47.000000 rssfixer-0.1.2/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:22:47.494548 rssfixer-0.1.2/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-26 16:32:08.000000 rssfixer-0.1.2/src/tests/test_rss.py
--rw-r--r--   0 reuteras   (501) staff       (20)     4141 2023-04-26 18:16:41.000000 rssfixer-0.1.2/src/tests/test_rss_args.py
--rw-r--r--   0 reuteras   (501) staff       (20)     1980 2023-04-26 16:34:02.000000 rssfixer-0.1.2/src/tests/test_rss_main.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.082135 rssfixer-0.1.3/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.3/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:45:41.081919 rssfixer-0.1.3/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     8682 2023-04-26 18:07:49.000000 rssfixer-0.1.3/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-26 18:44:42.000000 rssfixer-0.1.3/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-26 18:45:41.082197 rssfixer-0.1.3/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.077840 rssfixer-0.1.3/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.079056 rssfixer-0.1.3/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.3/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)    12618 2023-04-26 18:40:18.000000 rssfixer-0.1.3/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.080498 rssfixer-0.1.3/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     9508 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      371 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-26 18:45:41.000000 rssfixer-0.1.3/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-26 18:45:41.081480 rssfixer-0.1.3/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-26 16:32:08.000000 rssfixer-0.1.3/src/tests/test_rss.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     4141 2023-04-26 18:16:41.000000 rssfixer-0.1.3/src/tests/test_rss_args.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     1980 2023-04-26 16:34:02.000000 rssfixer-0.1.3/src/tests/test_rss_main.py
```

### Comparing `rssfixer-0.1.2/LICENSE` & `rssfixer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.2/PKG-INFO` & `rssfixer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rssfixer-0.1.2/README.md` & `rssfixer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.2/pyproject.toml` & `rssfixer-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rssfixer"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
 description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `rssfixer-0.1.2/src/rssfixer/rss.py` & `rssfixer-0.1.3/src/rssfixer/rss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Generate rss feed for "blogs" without rss feed."""
 import argparse
+import hashlib
 import importlib.metadata
 import json
 import re
 import sys
 
 import requests
 from bs4 import BeautifulSoup
@@ -174,15 +175,18 @@
     links = []
     unique_titles = set()
 
     # Iterate through all the elements of type html_entries in the page
     for entry in soup.find_all(arguments.release_entries):
         try:
             title = entry.text.strip()
-            url = arguments.release_url
+            title_bytes = title.encode("utf-8")
+            title_hash = hashlib.sha256(title_bytes)
+            title_sha256 = title_hash.hexdigest()
+            url = arguments.release_url + "?" + title_sha256
         except (KeyError, AttributeError):
             print("ERROR: Unable to title in HTML element")
             sys.exit(1)
         description = ""
         if title not in unique_titles:
             unique_titles.add(title)
             links.append((url, title, description))
```

### Comparing `rssfixer-0.1.2/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.1.3/src/rssfixer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rssfixer-0.1.2/src/tests/test_rss.py` & `rssfixer-0.1.3/src/tests/test_rss.py`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.2/src/tests/test_rss_args.py` & `rssfixer-0.1.3/src/tests/test_rss_args.py`

 * *Files identical despite different names*

### Comparing `rssfixer-0.1.2/src/tests/test_rss_main.py` & `rssfixer-0.1.3/src/tests/test_rss_main.py`

 * *Files identical despite different names*

