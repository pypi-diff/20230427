# Comparing `tmp/test-push-swap-0.2.tar.gz` & `tmp/test-push-swap-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-push-swap-0.2.tar", last modified: Thu Apr 27 16:38:57 2023, max compression
+gzip compressed data, was "test-push-swap-0.3.tar", last modified: Thu Apr 27 16:44:34 2023, max compression
```

## Comparing `test-push-swap-0.2.tar` & `test-push-swap-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        0 2023-04-27 16:38:57.165467 test-push-swap-0.2/
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       40 2023-04-27 16:29:54.000000 test-push-swap-0.2/MANIFEST.in
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      416 2023-04-27 16:38:57.164944 test-push-swap-0.2/PKG-INFO
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      434 2023-04-27 15:45:45.000000 test-push-swap-0.2/README.md
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       38 2023-04-27 16:38:57.165638 test-push-swap-0.2/setup.cfg
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      634 2023-04-27 16:38:27.000000 test-push-swap-0.2/setup.py
-drwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        0 2023-04-27 16:38:57.157521 test-push-swap-0.2/test_push_swap/
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       22 2023-04-27 15:54:16.000000 test-push-swap-0.2/test_push_swap/__init__.py
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      637 2023-04-27 16:36:12.000000 test-push-swap-0.2/test_push_swap/post_install.py
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)     5104 2023-04-27 15:45:45.000000 test-push-swap-0.2/test_push_swap/pstester.py
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      634 2023-04-27 16:38:27.000000 test-push-swap-0.2/test_push_swap/setup.py
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)     5104 2023-04-27 15:45:45.000000 test-push-swap-0.2/test_push_swap/test-push-swap.py
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)     5104 2023-04-27 15:45:45.000000 test-push-swap-0.2/test_push_swap/test_push_swap.py
-drwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        0 2023-04-27 16:38:57.163736 test-push-swap-0.2/test_push_swap.egg-info/
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      416 2023-04-27 16:38:56.000000 test-push-swap-0.2/test_push_swap.egg-info/PKG-INFO
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      398 2023-04-27 16:38:56.000000 test-push-swap-0.2/test_push_swap.egg-info/SOURCES.txt
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        1 2023-04-27 16:38:56.000000 test-push-swap-0.2/test_push_swap.egg-info/dependency_links.txt
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       59 2023-04-27 16:38:56.000000 test-push-swap-0.2/test_push_swap.egg-info/entry_points.txt
--rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       15 2023-04-27 16:38:56.000000 test-push-swap-0.2/test_push_swap.egg-info/top_level.txt
+drwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        0 2023-04-27 16:44:34.673575 test-push-swap-0.3/
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       40 2023-04-27 16:29:54.000000 test-push-swap-0.3/MANIFEST.in
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      416 2023-04-27 16:44:34.673064 test-push-swap-0.3/PKG-INFO
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      434 2023-04-27 15:45:45.000000 test-push-swap-0.3/README.md
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       38 2023-04-27 16:44:34.673752 test-push-swap-0.3/setup.cfg
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      640 2023-04-27 16:41:39.000000 test-push-swap-0.3/setup.py
+drwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        0 2023-04-27 16:44:34.665690 test-push-swap-0.3/test_push_swap/
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       32 2023-04-27 16:44:07.000000 test-push-swap-0.3/test_push_swap/__init__.py
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      637 2023-04-27 16:36:12.000000 test-push-swap-0.3/test_push_swap/post_install.py
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)     5104 2023-04-27 15:45:45.000000 test-push-swap-0.3/test_push_swap/pstester.py
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      640 2023-04-27 16:41:33.000000 test-push-swap-0.3/test_push_swap/setup.py
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)     5104 2023-04-27 15:45:45.000000 test-push-swap-0.3/test_push_swap/test-push-swap.py
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)     5104 2023-04-27 15:45:45.000000 test-push-swap-0.3/test_push_swap/test_push_swap.py
+drwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        0 2023-04-27 16:44:34.671818 test-push-swap-0.3/test_push_swap.egg-info/
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      416 2023-04-27 16:44:34.000000 test-push-swap-0.3/test_push_swap.egg-info/PKG-INFO
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)      398 2023-04-27 16:44:34.000000 test-push-swap-0.3/test_push_swap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)        1 2023-04-27 16:44:34.000000 test-push-swap-0.3/test_push_swap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       65 2023-04-27 16:44:34.000000 test-push-swap-0.3/test_push_swap.egg-info/entry_points.txt
+-rwxrwxrwx   0 huaydin  (101028) 2022_vienna  (4222)       15 2023-04-27 16:44:34.000000 test-push-swap-0.3/test_push_swap.egg-info/top_level.txt
```

### Comparing `test-push-swap-0.2/setup.py` & `test-push-swap-0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='test-push-swap',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'pstester = test_push_swap.pstester:main'
+            'test_push_swap = test_push_swap.pstester:main'
         ]
     },
     install_requires=[],
     author='hueseyin kaya aydin',
     author_email='huaydin@student.42vienna.com',
     description='A tester for the push swap project',
     url='https://github.com/hu8813/tester_push_swap',
```

### Comparing `test-push-swap-0.2/test_push_swap/post_install.py` & `test-push-swap-0.3/test_push_swap/post_install.py`

 * *Files identical despite different names*

### Comparing `test-push-swap-0.2/test_push_swap/pstester.py` & `test-push-swap-0.3/test_push_swap/pstester.py`

 * *Files identical despite different names*

### Comparing `test-push-swap-0.2/test_push_swap/setup.py` & `test-push-swap-0.3/test_push_swap/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='test-push-swap',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'pstester = test_push_swap.pstester:main'
+            'test_push_swap = test_push_swap.pstester:main'
         ]
     },
     install_requires=[],
     author='hueseyin kaya aydin',
     author_email='huaydin@student.42vienna.com',
     description='A tester for the push swap project',
     url='https://github.com/hu8813/tester_push_swap',
```

### Comparing `test-push-swap-0.2/test_push_swap/test-push-swap.py` & `test-push-swap-0.3/test_push_swap/test-push-swap.py`

 * *Files identical despite different names*

### Comparing `test-push-swap-0.2/test_push_swap/test_push_swap.py` & `test-push-swap-0.3/test_push_swap/test_push_swap.py`

 * *Files identical despite different names*

