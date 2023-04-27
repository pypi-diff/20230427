# Comparing `tmp/lftk-1.0b5.tar.gz` & `tmp/lftk-1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lftk-1.0b5.tar", last modified: Mon Mar  6 02:52:26 2023, max compression
+gzip compressed data, was "lftk-1.0b6.tar", last modified: Mon Mar  6 03:13:17 2023, max compression
```

## Comparing `lftk-1.0b5.tar` & `lftk-1.0b6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 02:52:26.478144 lftk-1.0b5/
--rw-r--r--   0 root         (0) root         (0)      306 2023-03-06 02:52:26.479144 lftk-1.0b5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 02:52:26.315143 lftk-1.0b5/lftk/
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-05 22:32:35.000000 lftk-1.0b5/lftk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 02:52:26.338143 lftk-1.0b5/lftk/derivation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-05 22:01:09.000000 lftk-1.0b5/lftk/derivation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-02-28 03:22:01.000000 lftk-1.0b5/lftk/derivation/avgentity.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-05 21:16:55.000000 lftk-1.0b5/lftk/derivation/avgpartofspeech.py
--rw-r--r--   0 root         (0) root         (0)     4735 2023-03-05 21:20:07.000000 lftk-1.0b5/lftk/derivation/avgworddiff.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-02-26 21:10:41.000000 lftk-1.0b5/lftk/derivation/avgwordsent.py
--rw-r--r--   0 root         (0) root         (0)      268 2023-03-05 21:44:07.000000 lftk-1.0b5/lftk/derivation/foundation_collector.py
--rw-r--r--   0 root         (0) root         (0)     7191 2023-03-02 20:12:26.000000 lftk-1.0b5/lftk/derivation/typetokenratio.py
--rw-r--r--   0 root         (0) root         (0)      302 2023-03-05 22:18:28.000000 lftk-1.0b5/lftk/derivation_collector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 02:52:26.347143 lftk-1.0b5/lftk/foundation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-05 22:01:27.000000 lftk-1.0b5/lftk/foundation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-02-28 03:21:20.000000 lftk-1.0b5/lftk/foundation/entity.py
--rw-r--r--   0 root         (0) root         (0)     6311 2023-03-05 21:10:37.000000 lftk-1.0b5/lftk/foundation/partofspeech.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-03-02 19:49:10.000000 lftk-1.0b5/lftk/foundation/worddiff.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-03-02 20:09:58.000000 lftk-1.0b5/lftk/foundation/wordsent.py
--rw-r--r--   0 root         (0) root         (0)     4120 2023-03-06 02:52:17.000000 lftk-1.0b5/lftk/lftk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 02:52:26.396143 lftk-1.0b5/lftk/resources/
--rw-r--r--   0 root         (0) root         (0)  2117809 2023-02-26 19:43:15.000000 lftk-1.0b5/lftk/resources/AoA_ratings_bry.csv
--rw-r--r--   0 root         (0) root         (0)  1143304 2023-02-26 19:41:48.000000 lftk-1.0b5/lftk/resources/AoA_ratings_kup.csv
--rw-r--r--   0 root         (0) root         (0)     6491 2023-03-05 21:43:26.000000 lftk-1.0b5/lftk/resources/feature_map.json
--rw-r--r--   0 root         (0) root         (0)  6058161 2023-02-27 00:07:37.000000 lftk-1.0b5/lftk/resources/subtlex_us.csv
--rw-r--r--   0 root         (0) root         (0)      662 2023-03-05 22:18:47.000000 lftk-1.0b5/lftk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 02:52:26.327143 lftk-1.0b5/lftk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      306 2023-03-06 02:52:26.000000 lftk-1.0b5/lftk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-06 02:52:26.000000 lftk-1.0b5/lftk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 02:52:26.000000 lftk-1.0b5/lftk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-06 02:52:26.000000 lftk-1.0b5/lftk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-06 02:52:26.000000 lftk-1.0b5/lftk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    13319 2023-03-05 21:50:01.000000 lftk-1.0b5/license.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-06 02:52:26.484144 lftk-1.0b5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      591 2023-03-06 02:51:33.000000 lftk-1.0b5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 03:13:17.378107 lftk-1.0b6/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-03-06 03:13:17.379107 lftk-1.0b6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 03:13:17.241106 lftk-1.0b6/lftk/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-03-06 03:12:53.000000 lftk-1.0b6/lftk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 03:13:17.262106 lftk-1.0b6/lftk/derivation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-05 22:01:09.000000 lftk-1.0b6/lftk/derivation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-02-28 03:22:01.000000 lftk-1.0b6/lftk/derivation/avgentity.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-05 21:16:55.000000 lftk-1.0b6/lftk/derivation/avgpartofspeech.py
+-rw-r--r--   0 root         (0) root         (0)     4735 2023-03-05 21:20:07.000000 lftk-1.0b6/lftk/derivation/avgworddiff.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-02-26 21:10:41.000000 lftk-1.0b6/lftk/derivation/avgwordsent.py
+-rw-r--r--   0 root         (0) root         (0)      268 2023-03-05 21:44:07.000000 lftk-1.0b6/lftk/derivation/foundation_collector.py
+-rw-r--r--   0 root         (0) root         (0)     7191 2023-03-02 20:12:26.000000 lftk-1.0b6/lftk/derivation/typetokenratio.py
+-rw-r--r--   0 root         (0) root         (0)      302 2023-03-05 22:18:28.000000 lftk-1.0b6/lftk/derivation_collector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 03:13:17.270106 lftk-1.0b6/lftk/foundation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-05 22:01:27.000000 lftk-1.0b6/lftk/foundation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-02-28 03:21:20.000000 lftk-1.0b6/lftk/foundation/entity.py
+-rw-r--r--   0 root         (0) root         (0)     6311 2023-03-05 21:10:37.000000 lftk-1.0b6/lftk/foundation/partofspeech.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-03-02 19:49:10.000000 lftk-1.0b6/lftk/foundation/worddiff.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-03-02 20:09:58.000000 lftk-1.0b6/lftk/foundation/wordsent.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2023-03-06 02:52:17.000000 lftk-1.0b6/lftk/lftk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 03:13:17.314106 lftk-1.0b6/lftk/resources/
+-rw-r--r--   0 root         (0) root         (0)  2117809 2023-02-26 19:43:15.000000 lftk-1.0b6/lftk/resources/AoA_ratings_bry.csv
+-rw-r--r--   0 root         (0) root         (0)  1143304 2023-02-26 19:41:48.000000 lftk-1.0b6/lftk/resources/AoA_ratings_kup.csv
+-rw-r--r--   0 root         (0) root         (0)     6491 2023-03-05 21:43:26.000000 lftk-1.0b6/lftk/resources/feature_map.json
+-rw-r--r--   0 root         (0) root         (0)  6058161 2023-02-27 00:07:37.000000 lftk-1.0b6/lftk/resources/subtlex_us.csv
+-rw-r--r--   0 root         (0) root         (0)      662 2023-03-05 22:18:47.000000 lftk-1.0b6/lftk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 03:13:17.252106 lftk-1.0b6/lftk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-03-06 03:13:17.000000 lftk-1.0b6/lftk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-06 03:13:17.000000 lftk-1.0b6/lftk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 03:13:17.000000 lftk-1.0b6/lftk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-03-06 03:13:17.000000 lftk-1.0b6/lftk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-03-06 03:13:17.000000 lftk-1.0b6/lftk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    13319 2023-03-05 21:50:01.000000 lftk-1.0b6/license.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-03-06 03:13:17.381107 lftk-1.0b6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      591 2023-03-06 03:13:14.000000 lftk-1.0b6/setup.py
```

### Comparing `lftk-1.0b5/lftk/derivation/avgentity.py` & `lftk-1.0b6/lftk/derivation/avgentity.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/derivation/avgworddiff.py` & `lftk-1.0b6/lftk/derivation/avgworddiff.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/derivation/avgwordsent.py` & `lftk-1.0b6/lftk/derivation/avgwordsent.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/derivation/typetokenratio.py` & `lftk-1.0b6/lftk/derivation/typetokenratio.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/foundation/partofspeech.py` & `lftk-1.0b6/lftk/foundation/partofspeech.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/foundation/worddiff.py` & `lftk-1.0b6/lftk/foundation/worddiff.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/foundation/wordsent.py` & `lftk-1.0b6/lftk/foundation/wordsent.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/lftk.py` & `lftk-1.0b6/lftk/lftk.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/resources/AoA_ratings_bry.csv` & `lftk-1.0b6/lftk/resources/AoA_ratings_bry.csv`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/resources/AoA_ratings_kup.csv` & `lftk-1.0b6/lftk/resources/AoA_ratings_kup.csv`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/resources/feature_map.json` & `lftk-1.0b6/lftk/resources/feature_map.json`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/resources/subtlex_us.csv` & `lftk-1.0b6/lftk/resources/subtlex_us.csv`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk/utils.py` & `lftk-1.0b6/lftk/utils.py`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/lftk.egg-info/SOURCES.txt` & `lftk-1.0b6/lftk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/license.txt` & `lftk-1.0b6/license.txt`

 * *Files identical despite different names*

### Comparing `lftk-1.0b5/setup.py` & `lftk-1.0b6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 from setuptools import find_packages
 setup(
     name = 'lftk',  
-    version='1.0-beta-5',
+    version='1.0-beta-6',
     license='CC BY-NC 4.0',   
     description = 'Comprehensive Multilingual Linguistic Features Extraction in Python',
     author = 'Bruce W. Lee',
     author_email = 'brucelws@seas.upenn.edu', 
     packages=find_packages(),
     url='https://github.com/brucewlee/lftk',
     keywords='linguistic feature',
```

