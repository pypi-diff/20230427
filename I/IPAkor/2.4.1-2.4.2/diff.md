# Comparing `tmp/IPAkor-2.4.1.tar.gz` & `tmp/IPAkor-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPAkor-2.4.1.tar", last modified: Thu Apr 27 20:49:47 2023, max compression
+gzip compressed data, was "IPAkor-2.4.2.tar", last modified: Thu Apr 27 21:18:01 2023, max compression
```

## Comparing `IPAkor-2.4.1.tar` & `IPAkor-2.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:49:47.285339 IPAkor-2.4.1/
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:49:47.280365 IPAkor-2.4.1/IPAkor/
--rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.4.1/IPAkor/__init__.py
--rw-r--r--   0 eneminova   (501) staff       (20)     3969 2023-04-27 20:40:43.000000 IPAkor-2.4.1/IPAkor/border_maker.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:49:47.282864 IPAkor-2.4.1/IPAkor/static/
--rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.4.1/IPAkor/static/final_trans.csv
--rw-r--r--   0 eneminova   (501) staff       (20)    14930 2023-04-27 20:49:40.000000 IPAkor-2.4.1/IPAkor/transcription.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 20:49:47.282549 IPAkor-2.4.1/IPAkor.egg-info/
--rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 20:49:47.000000 IPAkor-2.4.1/IPAkor.egg-info/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 20:49:47.000000 IPAkor-2.4.1/IPAkor.egg-info/SOURCES.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 20:49:47.000000 IPAkor-2.4.1/IPAkor.egg-info/dependency_links.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 20:49:47.000000 IPAkor-2.4.1/IPAkor.egg-info/requires.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 20:49:47.000000 IPAkor-2.4.1/IPAkor.egg-info/top_level.txt
--rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.4.1/MANIFEST.in
--rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 20:49:47.285465 IPAkor-2.4.1/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.4.1/README.md
--rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 20:49:47.285952 IPAkor-2.4.1/setup.cfg
--rw-r--r--   0 eneminova   (501) staff       (20)      580 2023-04-27 20:49:40.000000 IPAkor-2.4.1/setup.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:18:01.179643 IPAkor-2.4.2/
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:18:01.174143 IPAkor-2.4.2/IPAkor/
+-rw-r--r--   0 eneminova   (501) staff       (20)       85 2023-04-27 20:00:43.000000 IPAkor-2.4.2/IPAkor/__init__.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     3969 2023-04-27 20:40:43.000000 IPAkor-2.4.2/IPAkor/border_maker.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:18:01.176826 IPAkor-2.4.2/IPAkor/static/
+-rw-r--r--   0 eneminova   (501) staff       (20)   187060 2023-04-26 18:39:38.000000 IPAkor-2.4.2/IPAkor/static/final_trans.csv
+-rw-r--r--   0 eneminova   (501) staff       (20)    15015 2023-04-27 21:08:11.000000 IPAkor-2.4.2/IPAkor/transcription.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-27 21:18:01.176432 IPAkor-2.4.2/IPAkor.egg-info/
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 21:18:01.000000 IPAkor-2.4.2/IPAkor.egg-info/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)      285 2023-04-27 21:18:01.000000 IPAkor-2.4.2/IPAkor.egg-info/SOURCES.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-27 21:18:01.000000 IPAkor-2.4.2/IPAkor.egg-info/dependency_links.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-27 21:18:01.000000 IPAkor-2.4.2/IPAkor.egg-info/requires.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-27 21:18:01.000000 IPAkor-2.4.2/IPAkor.egg-info/top_level.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       23 2023-04-27 20:32:18.000000 IPAkor-2.4.2/MANIFEST.in
+-rw-r--r--   0 eneminova   (501) staff       (20)      246 2023-04-27 21:18:01.179759 IPAkor-2.4.2/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.4.2/README.md
+-rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-27 21:18:01.180370 IPAkor-2.4.2/setup.cfg
+-rw-r--r--   0 eneminova   (501) staff       (20)      585 2023-04-27 21:17:56.000000 IPAkor-2.4.2/setup.py
```

### Comparing `IPAkor-2.4.1/IPAkor/border_maker.py` & `IPAkor-2.4.2/IPAkor/border_maker.py`

 * *Files identical despite different names*

### Comparing `IPAkor-2.4.1/IPAkor/static/final_trans.csv` & `IPAkor-2.4.2/IPAkor/static/final_trans.csv`

 * *Files identical despite different names*

### Comparing `IPAkor-2.4.1/IPAkor/transcription.py` & `IPAkor-2.4.2/IPAkor/transcription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import re
 from konlpy.tag import Twitter
 from konlpy.tag import Kkma
 import csv
 import wget
-
+import os
 
 class BorderMaker:
 
     def __init__(self):
         self.twitter = Twitter()
         self.kkma = Kkma()
 
         self.final_trans = dict()
-        self.filename = 'IPAkor/static/final_trans.csv'
-        with open(self.filename, 'r', encoding='utf-8') as ft_file:
+        self.path_to_module = os.path.dirname(__file__)
+        self.weight_path = os.path.join(self.path_to_module, "static", "final_trans.csv")
+        with open(self.weight_path, 'rb') as ft_file:
             spamreader = csv.reader(ft_file)
 
             for row in spamreader:
                 self.final_trans[row[0]] = row[2]
 
     def intruser(self, word: str) -> str:
         ready_word = ''
```

### Comparing `IPAkor-2.4.1/README.md` & `IPAkor-2.4.2/README.md`

 * *Files identical despite different names*

