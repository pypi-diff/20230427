# Comparing `tmp/gulistandb-0.0.6.tar.gz` & `tmp/gulistandb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulistandb-0.0.6.tar", last modified: Thu Apr 27 05:52:13 2023, max compression
+gzip compressed data, was "gulistandb-0.0.7.tar", last modified: Thu Apr 27 10:56:58 2023, max compression
```

## Comparing `gulistandb-0.0.6.tar` & `gulistandb-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 05:52:13.699483 gulistandb-0.0.6/
--rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.6/License
--rw-rw-rw-   0        0        0     6646 2023-04-27 05:52:13.695485 gulistandb-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    11850 2023-04-27 05:46:19.000000 gulistandb-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 05:52:13.699483 gulistandb-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-04-27 05:46:56.000000 gulistandb-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 05:52:13.548548 gulistandb-0.0.6/src/
--rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.6/src/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-04-27 04:58:22.000000 gulistandb-0.0.6/src/editor.py
-drwxrwxrwx   0        0        0        0 2023-04-27 05:52:13.692488 gulistandb-0.0.6/src/gulistandb.egg-info/
--rw-rw-rw-   0        0        0     6646 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 05:52:13.000000 gulistandb-0.0.6/src/gulistandb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6270 2023-04-27 05:01:44.000000 gulistandb-0.0.6/src/gulistandb.py
--rw-rw-rw-   0        0        0     1361 2023-04-26 11:39:19.000000 gulistandb-0.0.6/src/reader.py
--rw-rw-rw-   0        0        0     1766 2023-04-27 04:59:45.000000 gulistandb-0.0.6/src/writter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:58.553211 gulistandb-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.7/License
+-rw-rw-rw-   0        0        0    10082 2023-04-27 10:56:58.550213 gulistandb-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    18722 2023-04-27 10:52:57.000000 gulistandb-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:56:58.554211 gulistandb-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-04-27 10:56:12.000000 gulistandb-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:58.443281 gulistandb-0.0.7/src/
+-rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.7/src/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-04-27 04:58:22.000000 gulistandb-0.0.7/src/editor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:56:58.543218 gulistandb-0.0.7/src/gulistandb.egg-info/
+-rw-rw-rw-   0        0        0    10082 2023-04-27 10:56:57.000000 gulistandb-0.0.7/src/gulistandb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-27 10:56:58.000000 gulistandb-0.0.7/src/gulistandb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:56:57.000000 gulistandb-0.0.7/src/gulistandb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 10:56:57.000000 gulistandb-0.0.7/src/gulistandb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:56:58.000000 gulistandb-0.0.7/src/gulistandb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6382 2023-04-27 10:52:43.000000 gulistandb-0.0.7/src/gulistandb.py
+-rw-rw-rw-   0        0        0     1361 2023-04-26 11:39:19.000000 gulistandb-0.0.7/src/reader.py
+-rw-rw-rw-   0        0        0     1766 2023-04-27 04:59:45.000000 gulistandb-0.0.7/src/writter.py
```

### Comparing `gulistandb-0.0.6/License` & `gulistandb-0.0.7/License`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.6/setup.py` & `gulistandb-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-16') as f:
     long_description = f.read()
 
 setup(
     name='gulistandb',
-    version='0.0.6',
+    version='0.0.7',
     install_requires=[
         'pandas',
         # add more dependencies as needed
     ],
     package_dir={'': 'src'},
 
     # metadata
```

### Comparing `gulistandb-0.0.6/src/editor.py` & `gulistandb-0.0.7/src/editor.py`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.6/src/gulistandb.py` & `gulistandb-0.0.7/src/gulistandb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from editor import fileInit
 from reader import reader
 from writter import writter
+# from src.gulistandb import BOOK_LIB
 
 
 SUPPORTED_DATA_TYPES = ['csv',   'json']
 
 
 class Table:
 
@@ -149,16 +150,18 @@
         data = t.get()
     """
 
         with open(self.file_path, 'r') as file:
             data = file.read()
             return (data)
 
-    def clear(self):
+    def clear(self, ClrTable):
         fileInit(self.fileType, self.file_path, self.column)
+        if ClrTable == True:
+            self.TableName = ""
         return 0
 
     def insert(self, *datas):
         """
     Inserts new data into the table file.
 
     Args:
```

### Comparing `gulistandb-0.0.6/src/reader.py` & `gulistandb-0.0.7/src/reader.py`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.6/src/writter.py` & `gulistandb-0.0.7/src/writter.py`

 * *Files identical despite different names*

