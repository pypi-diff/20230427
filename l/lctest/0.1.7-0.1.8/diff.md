# Comparing `tmp/lctest-0.1.7.tar.gz` & `tmp/lctest-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctest-0.1.7.tar", last modified: Sun Aug 14 01:56:06 2022, max compression
+gzip compressed data, was "lctest-0.1.8.tar", last modified: Wed Apr 26 22:37:46 2023, max compression
```

## Comparing `lctest-0.1.7.tar` & `lctest-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2022-08-14 01:56:06.083226 lctest-0.1.7/
--rw-r--r--   0 tuanchau   (503) staff       (20)      918 2022-08-14 01:56:06.082904 lctest-0.1.7/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      252 2022-07-22 10:51:15.000000 lctest-0.1.7/README.md
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2022-08-14 01:56:06.081477 lctest-0.1.7/lctest/
--rw-r--r--   0 tuanchau   (503) staff       (20)      499 2022-08-14 01:47:19.000000 lctest-0.1.7/lctest/__init__.py
--rw-r--r--   0 tuanchau   (503) staff       (20)      704 2022-07-22 10:51:15.000000 lctest-0.1.7/lctest/arguments.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     3795 2022-08-01 23:49:59.000000 lctest-0.1.7/lctest/lib.py
--rw-r--r--   0 tuanchau   (503) staff       (20)      332 2022-07-22 10:51:15.000000 lctest-0.1.7/lctest/stdlib.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     2136 2022-08-01 23:47:00.000000 lctest-0.1.7/lctest/test.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     9218 2022-08-14 00:10:34.000000 lctest-0.1.7/lctest/testcase.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     1340 2022-08-01 23:42:18.000000 lctest-0.1.7/lctest/text_format.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2022-08-14 01:56:06.082619 lctest-0.1.7/lctest.egg-info/
--rw-r--r--   0 tuanchau   (503) staff       (20)      918 2022-08-14 01:56:05.000000 lctest-0.1.7/lctest.egg-info/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      264 2022-08-14 01:56:06.000000 lctest-0.1.7/lctest.egg-info/SOURCES.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        1 2022-08-14 01:56:05.000000 lctest-0.1.7/lctest.egg-info/dependency_links.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        7 2022-08-14 01:56:06.000000 lctest-0.1.7/lctest.egg-info/top_level.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       38 2022-08-14 01:56:06.083270 lctest-0.1.7/setup.cfg
--rw-r--r--   0 tuanchau   (503) staff       (20)     1268 2022-08-14 01:49:49.000000 lctest-0.1.7/setup.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-04-26 22:37:46.825358 lctest-0.1.8/
+-rw-r--r--   0 tuanchau   (503) staff       (20)      918 2023-04-26 22:37:46.825167 lctest-0.1.8/PKG-INFO
+-rw-r--r--   0 tuanchau   (503) staff       (20)      252 2023-04-26 22:36:06.000000 lctest-0.1.8/README.md
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-04-26 22:37:46.823619 lctest-0.1.8/lctest/
+-rw-r--r--   0 tuanchau   (503) staff       (20)      499 2022-08-14 01:47:19.000000 lctest-0.1.8/lctest/__init__.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)      704 2022-07-22 10:51:15.000000 lctest-0.1.8/lctest/arguments.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     3795 2022-08-01 23:49:59.000000 lctest-0.1.8/lctest/lib.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)      332 2022-07-22 10:51:15.000000 lctest-0.1.8/lctest/stdlib.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     2136 2022-08-01 23:47:00.000000 lctest-0.1.8/lctest/test.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     9218 2022-08-14 00:10:34.000000 lctest-0.1.8/lctest/testcase.py
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1340 2022-08-01 23:42:18.000000 lctest-0.1.8/lctest/text_format.py
+drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-04-26 22:37:46.824873 lctest-0.1.8/lctest.egg-info/
+-rw-r--r--   0 tuanchau   (503) staff       (20)      918 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/PKG-INFO
+-rw-r--r--   0 tuanchau   (503) staff       (20)      264 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/SOURCES.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)        1 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/dependency_links.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)        7 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/top_level.txt
+-rw-r--r--   0 tuanchau   (503) staff       (20)       38 2023-04-26 22:37:46.825403 lctest-0.1.8/setup.cfg
+-rw-r--r--   0 tuanchau   (503) staff       (20)     1268 2023-04-26 22:37:36.000000 lctest-0.1.8/setup.py
```

### Comparing `lctest-0.1.7/PKG-INFO` & `lctest-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctest
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simulate leetcode runner
 Home-page: https://lctest.readthedocs.io/
 Author: Tuan Chau
 Author-email: tuanchaujp@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,13 +25,13 @@
 from lctest import *
 
 @testcase(
     (Expected, Parameters)
 )
 class Solution:
     @solution
-    fun doSomething(self, params):
+    def doSomething(self, params):
         pass
 
     def sol(self, params):
         pass
 ```
```

### Comparing `lctest-0.1.7/lctest/arguments.py` & `lctest-0.1.8/lctest/arguments.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.7/lctest/lib.py` & `lctest-0.1.8/lctest/lib.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.7/lctest/test.py` & `lctest-0.1.8/lctest/test.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.7/lctest/testcase.py` & `lctest-0.1.8/lctest/testcase.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.7/lctest/text_format.py` & `lctest-0.1.8/lctest/text_format.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.7/lctest.egg-info/PKG-INFO` & `lctest-0.1.8/lctest.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctest
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simulate leetcode runner
 Home-page: https://lctest.readthedocs.io/
 Author: Tuan Chau
 Author-email: tuanchaujp@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,13 +25,13 @@
 from lctest import *
 
 @testcase(
     (Expected, Parameters)
 )
 class Solution:
     @solution
-    fun doSomething(self, params):
+    def doSomething(self, params):
         pass
 
     def sol(self, params):
         pass
 ```
```

### Comparing `lctest-0.1.7/setup.py` & `lctest-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="lctest",
-    version="0.1.7",
+    version="0.1.8",
     description="Simulate leetcode runner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://lctest.readthedocs.io/",
     author="Tuan Chau",
     author_email="tuanchaujp@gmail.com",
     license="MIT",
```

