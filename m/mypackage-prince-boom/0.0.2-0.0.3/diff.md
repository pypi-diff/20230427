# Comparing `tmp/mypackage_prince_boom-0.0.2.tar.gz` & `tmp/mypackage_prince_boom-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackage_prince_boom-0.0.2.tar", last modified: Thu Apr 27 10:00:42 2023, max compression
+gzip compressed data, was "mypackage_prince_boom-0.0.3.tar", last modified: Thu Apr 27 11:09:03 2023, max compression
```

## Comparing `mypackage_prince_boom-0.0.2.tar` & `mypackage_prince_boom-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 10:00:42.340364 mypackage_prince_boom-0.0.2/
--rw-rw-r--   0 studio45  (1000) studio45  (1000)     1073 2023-04-26 11:26:19.000000 mypackage_prince_boom-0.0.2/LICENSE
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-04-27 10:00:42.340364 mypackage_prince_boom-0.0.2/PKG-INFO
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      170 2023-04-26 11:26:08.000000 mypackage_prince_boom-0.0.2/README.md
-drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 10:00:42.336364 mypackage_prince_boom-0.0.2/mypackage_prince_boom/
--rw-rw-r--   0 studio45  (1000) studio45  (1000)       43 2023-04-27 09:59:28.000000 mypackage_prince_boom-0.0.2/mypackage_prince_boom/__init__.py
-drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 10:00:42.340364 mypackage_prince_boom-0.0.2/mypackage_prince_boom.egg-info/
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-04-27 10:00:42.000000 mypackage_prince_boom-0.0.2/mypackage_prince_boom.egg-info/PKG-INFO
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      332 2023-04-27 10:00:42.000000 mypackage_prince_boom-0.0.2/mypackage_prince_boom.egg-info/SOURCES.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)        1 2023-04-27 10:00:42.000000 mypackage_prince_boom-0.0.2/mypackage_prince_boom.egg-info/dependency_links.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)       79 2023-04-27 10:00:42.000000 mypackage_prince_boom-0.0.2/mypackage_prince_boom.egg-info/entry_points.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)        9 2023-04-27 10:00:42.000000 mypackage_prince_boom-0.0.2/mypackage_prince_boom.egg-info/requires.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)       22 2023-04-27 10:00:42.000000 mypackage_prince_boom-0.0.2/mypackage_prince_boom.egg-info/top_level.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)       38 2023-04-27 10:00:42.340364 mypackage_prince_boom-0.0.2/setup.cfg
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      686 2023-04-27 09:59:57.000000 mypackage_prince_boom-0.0.2/setup.py
+drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 11:09:03.942336 mypackage_prince_boom-0.0.3/
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)     1073 2023-04-26 11:26:19.000000 mypackage_prince_boom-0.0.3/LICENSE
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-04-27 11:09:03.942336 mypackage_prince_boom-0.0.3/PKG-INFO
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      170 2023-04-27 11:08:59.000000 mypackage_prince_boom-0.0.3/README.md
+drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 11:09:03.938336 mypackage_prince_boom-0.0.3/mypackage_prince_boom/
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)       43 2023-04-27 11:08:46.000000 mypackage_prince_boom-0.0.3/mypackage_prince_boom/__init__.py
+drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 11:09:03.942336 mypackage_prince_boom-0.0.3/mypackage_prince_boom.egg-info/
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-04-27 11:09:03.000000 mypackage_prince_boom-0.0.3/mypackage_prince_boom.egg-info/PKG-INFO
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      332 2023-04-27 11:09:03.000000 mypackage_prince_boom-0.0.3/mypackage_prince_boom.egg-info/SOURCES.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)        1 2023-04-27 11:09:03.000000 mypackage_prince_boom-0.0.3/mypackage_prince_boom.egg-info/dependency_links.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)       79 2023-04-27 11:09:03.000000 mypackage_prince_boom-0.0.3/mypackage_prince_boom.egg-info/entry_points.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)        9 2023-04-27 11:09:03.000000 mypackage_prince_boom-0.0.3/mypackage_prince_boom.egg-info/requires.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)       22 2023-04-27 11:09:03.000000 mypackage_prince_boom-0.0.3/mypackage_prince_boom.egg-info/top_level.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)       38 2023-04-27 11:09:03.942336 mypackage_prince_boom-0.0.3/setup.cfg
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      686 2023-04-27 11:08:55.000000 mypackage_prince_boom-0.0.3/setup.py
```

### Comparing `mypackage_prince_boom-0.0.2/LICENSE` & `mypackage_prince_boom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypackage_prince_boom-0.0.2/setup.py` & `mypackage_prince_boom-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mypackage_prince_boom',
-    version='0.0.2',
+    version='0.0.3',
     packages=['mypackage_prince_boom'],
     install_requires=[
         'requests',
     ],
     entry_points={
         'console_scripts': [
             'mypackage_prince_boom = mypackage_prince_boom.__main__:main'
```

