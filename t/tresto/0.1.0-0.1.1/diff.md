# Comparing `tmp/tresto-0.1.0.tar.gz` & `tmp/tresto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tresto-0.1.0.tar", last modified: Wed Apr 26 19:03:19 2023, max compression
+gzip compressed data, was "tresto-0.1.1.tar", last modified: Thu Apr 27 01:08:38 2023, max compression
```

## Comparing `tresto-0.1.0.tar` & `tresto-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-26 19:03:19.362825 tresto-0.1.0/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     4276 2023-04-26 19:03:19.362825 tresto-0.1.0/PKG-INFO
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     3773 2023-04-26 18:43:15.000000 tresto-0.1.0/README.md
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)       38 2023-04-26 19:03:19.362825 tresto-0.1.0/setup.cfg
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)      802 2023-04-26 16:23:23.000000 tresto-0.1.0/setup.py
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-26 19:03:19.352825 tresto-0.1.0/tests/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)      362 2023-04-26 17:20:27.000000 tresto-0.1.0/tests/test_hello_world.py
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     2030 2023-04-26 18:39:59.000000 tresto-0.1.0/tests/test_tresto.py
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-26 19:03:19.352825 tresto-0.1.0/tresto/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)       35 2023-04-25 22:49:19.000000 tresto-0.1.0/tresto/__init__.py
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     2156 2023-04-26 15:50:48.000000 tresto-0.1.0/tresto/tresto.py
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-26 19:03:19.362825 tresto-0.1.0/tresto.egg-info/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     4276 2023-04-26 19:03:19.000000 tresto-0.1.0/tresto.egg-info/PKG-INFO
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)      250 2023-04-26 19:03:19.000000 tresto-0.1.0/tresto.egg-info/SOURCES.txt
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)        1 2023-04-26 19:03:19.000000 tresto-0.1.0/tresto.egg-info/dependency_links.txt
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)       18 2023-04-26 19:03:19.000000 tresto-0.1.0/tresto.egg-info/requires.txt
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)        7 2023-04-26 19:03:19.000000 tresto-0.1.0/tresto.egg-info/top_level.txt
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-27 01:08:38.062688 tresto-0.1.1/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     4276 2023-04-27 01:08:38.062688 tresto-0.1.1/PKG-INFO
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     3773 2023-04-26 18:43:15.000000 tresto-0.1.1/README.md
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)       38 2023-04-27 01:08:38.062688 tresto-0.1.1/setup.cfg
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)      794 2023-04-27 01:07:20.000000 tresto-0.1.1/setup.py
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-27 01:08:38.062688 tresto-0.1.1/tests/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)      362 2023-04-26 17:20:27.000000 tresto-0.1.1/tests/test_hello_world.py
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     2030 2023-04-26 18:39:59.000000 tresto-0.1.1/tests/test_tresto.py
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-27 01:08:38.062688 tresto-0.1.1/tresto/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)       35 2023-04-25 22:49:19.000000 tresto-0.1.1/tresto/__init__.py
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     2156 2023-04-26 15:50:48.000000 tresto-0.1.1/tresto/tresto.py
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-27 01:08:38.062688 tresto-0.1.1/tresto.egg-info/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     4276 2023-04-27 01:08:38.000000 tresto-0.1.1/tresto.egg-info/PKG-INFO
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)      250 2023-04-27 01:08:38.000000 tresto-0.1.1/tresto.egg-info/SOURCES.txt
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)        1 2023-04-27 01:08:38.000000 tresto-0.1.1/tresto.egg-info/dependency_links.txt
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)       10 2023-04-27 01:08:38.000000 tresto-0.1.1/tresto.egg-info/requires.txt
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)        7 2023-04-27 01:08:38.000000 tresto-0.1.1/tresto.egg-info/top_level.txt
```

### Comparing `tresto-0.1.0/PKG-INFO` & `tresto-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tresto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python unit testing integrated with Trello, providing visualization of project status, ideal for test-driven development
 Home-page: https://github.com/buanzo/tresto
 Author: Arturo 'Buanzo' Busleiman
 Author-email: buanzo@buanzo.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tresto-0.1.0/README.md` & `tresto-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tresto-0.1.0/setup.py` & `tresto-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="tresto",
-    version="0.1.0",
+    version="0.1.1",
     author="Arturo 'Buanzo' Busleiman",
     author_email="buanzo@buanzo.com.ar",
     description="Python unit testing integrated with Trello, providing visualization of project status, ideal for test-driven development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/buanzo/tresto",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
-        'py-trello>=1.10.0'
+        'py-trello'
     ]
 )
```

### Comparing `tresto-0.1.0/tests/test_tresto.py` & `tresto-0.1.1/tests/test_tresto.py`

 * *Files identical despite different names*

### Comparing `tresto-0.1.0/tresto/tresto.py` & `tresto-0.1.1/tresto/tresto.py`

 * *Files identical despite different names*

### Comparing `tresto-0.1.0/tresto.egg-info/PKG-INFO` & `tresto-0.1.1/tresto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tresto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python unit testing integrated with Trello, providing visualization of project status, ideal for test-driven development
 Home-page: https://github.com/buanzo/tresto
 Author: Arturo 'Buanzo' Busleiman
 Author-email: buanzo@buanzo.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

