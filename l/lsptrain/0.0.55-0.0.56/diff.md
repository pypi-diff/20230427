# Comparing `tmp/lsptrain-0.0.55.tar.gz` & `tmp/lsptrain-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.55.tar", last modified: Mon Apr 24 03:04:27 2023, max compression
+gzip compressed data, was "lsptrain-0.0.56.tar", last modified: Thu Apr 27 08:10:47 2023, max compression
```

## Comparing `lsptrain-0.0.55.tar` & `lsptrain-0.0.56.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:04:27.131597 lsptrain-0.0.55/
--rw-rw-rw-   0        0        0      492 2023-04-24 03:04:27.131597 lsptrain-0.0.55/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-21 05:10:24.000000 lsptrain-0.0.55/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 03:04:27.111596 lsptrain-0.0.55/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.55/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:04:27.122597 lsptrain-0.0.55/lsptrain/nlp_classification/
--rw-rw-rw-   0        0        0       32 2023-04-23 08:32:50.000000 lsptrain-0.0.55/lsptrain/nlp_classification/__init__.py
--rw-rw-rw-   0        0        0     9714 2023-04-23 09:11:48.000000 lsptrain-0.0.55/lsptrain/nlp_classification/model.py
--rw-rw-rw-   0        0        0     2161 2023-04-23 08:02:20.000000 lsptrain-0.0.55/lsptrain/nlp_classification/train_scripts.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:04:27.125596 lsptrain-0.0.55/lsptrain/nlp_classification_predictor/
--rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.55/lsptrain/nlp_classification_predictor/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.55/lsptrain/nlp_classification_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:04:27.129596 lsptrain-0.0.55/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.55/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.55/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.55/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:04:27.118596 lsptrain-0.0.55/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      492 2023-04-24 03:04:27.000000 lsptrain-0.0.55/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-04-24 03:04:27.000000 lsptrain-0.0.55/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 03:04:27.000000 lsptrain-0.0.55/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-24 03:04:27.000000 lsptrain-0.0.55/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 03:04:27.000000 lsptrain-0.0.55/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 03:04:27.131597 lsptrain-0.0.55/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-04-24 03:03:54.000000 lsptrain-0.0.55/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:10:47.345490 lsptrain-0.0.56/
+-rw-rw-rw-   0        0        0      615 2023-04-27 08:10:47.344490 lsptrain-0.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-04-27 08:10:44.000000 lsptrain-0.0.56/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-27 08:10:47.321490 lsptrain-0.0.56/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.56/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:10:47.332489 lsptrain-0.0.56/lsptrain/nlp_classification/
+-rw-rw-rw-   0        0        0       32 2023-04-23 08:32:50.000000 lsptrain-0.0.56/lsptrain/nlp_classification/__init__.py
+-rw-rw-rw-   0        0        0     9714 2023-04-23 09:11:48.000000 lsptrain-0.0.56/lsptrain/nlp_classification/model.py
+-rw-rw-rw-   0        0        0     2161 2023-04-23 08:02:20.000000 lsptrain-0.0.56/lsptrain/nlp_classification/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:10:47.336490 lsptrain-0.0.56/lsptrain/nlp_classification_predictor/
+-rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.56/lsptrain/nlp_classification_predictor/__init__.py
+-rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.56/lsptrain/nlp_classification_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:10:47.339489 lsptrain-0.0.56/lsptrain/nlp_similarity_predictor/
+-rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.56/lsptrain/nlp_similarity_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2060 2023-04-27 07:49:33.000000 lsptrain-0.0.56/lsptrain/nlp_similarity_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:10:47.343490 lsptrain-0.0.56/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.56/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.56/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.56/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:10:47.328491 lsptrain-0.0.56/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-04-27 08:10:47.000000 lsptrain-0.0.56/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-04-27 08:10:47.000000 lsptrain-0.0.56/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 08:10:47.000000 lsptrain-0.0.56/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-27 08:10:47.000000 lsptrain-0.0.56/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 08:10:47.000000 lsptrain-0.0.56/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 08:10:47.345490 lsptrain-0.0.56/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-04-27 07:52:49.000000 lsptrain-0.0.56/setup.py
```

### Comparing `lsptrain-0.0.55/lsptrain/nlp_classification/model.py` & `lsptrain-0.0.56/lsptrain/nlp_classification/model.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.55/lsptrain/nlp_classification/train_scripts.py` & `lsptrain-0.0.56/lsptrain/nlp_classification/train_scripts.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.55/lsptrain/nlp_classification_predictor/predictor.py` & `lsptrain-0.0.56/lsptrain/nlp_classification_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.55/setup.py` & `lsptrain-0.0.56/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.55',
+      version='0.0.56',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch',
                         'transformers',
```

