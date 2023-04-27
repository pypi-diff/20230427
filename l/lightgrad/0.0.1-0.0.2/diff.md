# Comparing `tmp/lightgrad-0.0.1.tar.gz` & `tmp/lightgrad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightgrad-0.0.1.tar", last modified: Thu Apr 27 11:38:50 2023, max compression
+gzip compressed data, was "lightgrad-0.0.2.tar", last modified: Thu Apr 27 11:42:45 2023, max compression
```

## Comparing `lightgrad-0.0.1.tar` & `lightgrad-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:38:50.468771 lightgrad-0.0.1/
--rw-rw-rw-   0        0        0     1077 2020-04-20 16:05:24.000000 lightgrad-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      659 2023-04-27 11:38:50.462772 lightgrad-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-27 11:37:50.000000 lightgrad-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 11:38:50.418238 lightgrad-0.0.1/lightgrad/
--rw-rw-rw-   0        0        0      128 2023-04-27 11:33:06.000000 lightgrad-0.0.1/lightgrad/__init__.py
--rw-rw-rw-   0        0        0     8659 2020-04-20 16:05:24.000000 lightgrad-0.0.1/lightgrad/engine.c
--rw-rw-rw-   0        0        0     1654 2020-04-20 16:05:24.000000 lightgrad-0.0.1/lightgrad/nn.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:38:50.448756 lightgrad-0.0.1/lightgrad.egg-info/
--rw-rw-rw-   0        0        0      659 2023-04-27 11:38:50.000000 lightgrad-0.0.1/lightgrad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-27 11:38:50.000000 lightgrad-0.0.1/lightgrad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:38:50.000000 lightgrad-0.0.1/lightgrad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 11:38:50.000000 lightgrad-0.0.1/lightgrad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 11:38:50.469771 lightgrad-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-04-27 11:34:54.000000 lightgrad-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:38:50.454769 lightgrad-0.0.1/test/
--rw-rw-rw-   0        0        0     1541 2020-04-20 16:05:24.000000 lightgrad-0.0.1/test/test_engine.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:42:45.881429 lightgrad-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2020-04-20 16:05:24.000000 lightgrad-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      708 2023-04-27 11:42:45.879428 lightgrad-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-27 11:37:50.000000 lightgrad-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 11:42:45.847429 lightgrad-0.0.2/lightgrad/
+-rw-rw-rw-   0        0        0      130 2023-04-27 11:42:10.000000 lightgrad-0.0.2/lightgrad/__init__.py
+-rw-rw-rw-   0        0        0     8659 2020-04-20 16:05:24.000000 lightgrad-0.0.2/lightgrad/engine.c
+-rw-rw-rw-   0        0        0     1655 2023-04-27 11:40:46.000000 lightgrad-0.0.2/lightgrad/nn.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:42:45.871428 lightgrad-0.0.2/lightgrad.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-04-27 11:42:45.000000 lightgrad-0.0.2/lightgrad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-27 11:42:45.000000 lightgrad-0.0.2/lightgrad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:42:45.000000 lightgrad-0.0.2/lightgrad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 11:42:45.000000 lightgrad-0.0.2/lightgrad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 11:42:45.881429 lightgrad-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      955 2023-04-27 11:42:02.000000 lightgrad-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:42:45.875429 lightgrad-0.0.2/test/
+-rw-rw-rw-   0        0        0     1542 2023-04-27 11:40:45.000000 lightgrad-0.0.2/test/test_engine.py
```

### Comparing `lightgrad-0.0.1/LICENSE` & `lightgrad-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightgrad-0.0.1/PKG-INFO` & `lightgrad-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lightgrad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Autograd Engine written in Python C-API
-Home-page: 
+Home-page: https://github.com/marcosalvalaggio-bip/lightgrad
 Author: Marco S.
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lightgrad-0.0.1/lightgrad/engine.c` & `lightgrad-0.0.2/lightgrad/engine.c`

 * *Files identical despite different names*

### Comparing `lightgrad-0.0.1/lightgrad/nn.py` & `lightgrad-0.0.2/lightgrad/nn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from minigrad.engine import Value
+from lightgrad.engine import Value
 
 # https://github.com/karpathy/micrograd/
 
 class Module:
 
     def zero_grad(self):
         for p in self.parameters():
```

### Comparing `lightgrad-0.0.1/lightgrad.egg-info/PKG-INFO` & `lightgrad-0.0.2/lightgrad.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lightgrad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Autograd Engine written in Python C-API
-Home-page: 
+Home-page: https://github.com/marcosalvalaggio-bip/lightgrad
 Author: Marco S.
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lightgrad-0.0.1/setup.py` & `lightgrad-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from setuptools.extension import Extension
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='lightgrad',
-      version='0.0.1',
+      version='0.0.2',
       description='Autograd Engine written in Python C-API',
       author='Marco S.',
       author_email='mar.salvalaggio@gmail.com',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      url='',
+      url='https://github.com/marcosalvalaggio-bip/lightgrad',
       packages = ['lightgrad'],
       ext_modules = [Extension('lightgrad.engine', sources = ['lightgrad/engine.c'])],
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
```

### Comparing `lightgrad-0.0.1/test/test_engine.py` & `lightgrad-0.0.2/test/test_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from minigrad.engine import Value
+from lightgrad.engine import Value
 
 def test_sanity_check():
 
     x = Value(-4.0)
     z = Value(2.0) * x + Value(2.0) + x
     q = z.relu() + z * x
     h = (z * z).relu()
```

