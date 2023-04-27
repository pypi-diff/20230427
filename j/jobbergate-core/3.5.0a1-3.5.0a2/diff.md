# Comparing `tmp/jobbergate-core-3.5.0a1.tar.gz` & `tmp/jobbergate-core-3.5.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate-core-3.5.0a1.tar", max compression
+gzip compressed data, was "jobbergate-core-3.5.0a2.tar", max compression
```

## Comparing `jobbergate-core-3.5.0a1.tar` & `jobbergate-core-3.5.0a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1082 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/LICENSE
--rw-r--r--   0        0        0      420 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/README.rst
--rw-r--r--   0        0        0      329 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/jobbergate_core/__init__.py
--rw-r--r--   0        0        0      366 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/jobbergate_core/auth/__init__.py
--rw-r--r--   0        0        0      279 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/jobbergate_core/auth/exceptions.py
--rw-r--r--   0        0        0    11813 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/jobbergate_core/auth/handler.py
--rw-r--r--   0        0        0     5534 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/jobbergate_core/auth/token.py
--rw-r--r--   0        0        0      133 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/jobbergate_core/version.py
--rw-r--r--   0        0        0     1769 2023-04-14 17:46:35.339744 jobbergate-core-3.5.0a1/pyproject.toml
--rw-r--r--   0        0        0     1271 2023-04-14 17:46:50.984862 jobbergate-core-3.5.0a1/setup.py
--rw-r--r--   0        0        0     1634 2023-04-14 17:46:50.985195 jobbergate-core-3.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/LICENSE
+-rw-r--r--   0        0        0      420 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/README.rst
+-rw-r--r--   0        0        0      329 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/__init__.py
+-rw-r--r--   0        0        0      366 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/exceptions.py
+-rw-r--r--   0        0        0    11813 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/handler.py
+-rw-r--r--   0        0        0     5534 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/auth/token.py
+-rw-r--r--   0        0        0      133 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/jobbergate_core/version.py
+-rw-r--r--   0        0        0     1769 2023-04-27 21:34:07.112423 jobbergate-core-3.5.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1271 2023-04-27 21:34:29.329498 jobbergate-core-3.5.0a2/setup.py
+-rw-r--r--   0        0        0     1634 2023-04-27 21:34:29.329962 jobbergate-core-3.5.0a2/PKG-INFO
```

### Comparing `jobbergate-core-3.5.0a1/LICENSE` & `jobbergate-core-3.5.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate-core-3.5.0a1/jobbergate_core/auth/handler.py` & `jobbergate-core-3.5.0a2/jobbergate_core/auth/handler.py`

 * *Files identical despite different names*

### Comparing `jobbergate-core-3.5.0a1/jobbergate_core/auth/token.py` & `jobbergate-core-3.5.0a2/jobbergate_core/auth/token.py`

 * *Files identical despite different names*

### Comparing `jobbergate-core-3.5.0a1/pyproject.toml` & `jobbergate-core-3.5.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-core"
-version = "3.5.0-alpha.1"
+version = "3.5.0-alpha.2"
 description = "Jobbergate Core"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate-core-3.5.0a1/setup.py` & `jobbergate-core-3.5.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pendulum>=2.1.2,<3.0.0',
  'py-buzz>=3.1.0,<4.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'python-jose>=3.3.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'jobbergate-core',
-    'version': '3.5.0a1',
+    'version': '3.5.0a2',
     'description': 'Jobbergate Core',
     'long_description': '=================\n Jobbergate Core\n=================\n\nJobbergate-core is a sub-project that contains the key components and logic that is shared among all other sub-projects (CLI, API, and Agent). Additionally, jobbergate-core exists to support custom automation built on top of Jobbergate.\n\nLicense\n-------\n* `MIT <LICENSE>`_\n\n\nCopyright\n---------\n* Copyright (c) 2023 OmniVector Solutions <info@omnivector.solutions>\n\n',
     'author': 'Omnivector Solutions',
     'author_email': 'info@omnivector.solutions',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/omnivector-solutions/jobbergate',
```

### Comparing `jobbergate-core-3.5.0a1/PKG-INFO` & `jobbergate-core-3.5.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-core
-Version: 3.5.0a1
+Version: 3.5.0a2
 Summary: Jobbergate Core
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

