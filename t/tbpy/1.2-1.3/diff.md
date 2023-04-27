# Comparing `tmp/tbpy-1.2.tar.gz` & `tmp/tbpy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbpy-1.2.tar", last modified: Tue Apr 25 21:49:27 2023, max compression
+gzip compressed data, was "tbpy-1.3.tar", last modified: Thu Apr 27 20:39:16 2023, max compression
```

## Comparing `tbpy-1.2.tar` & `tbpy-1.3.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.790647 tbpy-1.2/
--rw-rw-rw-   0        0        0     1091 2022-11-08 18:13:24.000000 tbpy-1.2/LICENSE
--rw-rw-rw-   0        0        0      830 2023-04-25 21:49:27.789649 tbpy-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-25 21:35:19.000000 tbpy-1.2/README.md
--rw-rw-rw-   0        0        0      506 2023-04-25 21:48:33.000000 tbpy-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 21:49:27.790647 tbpy-1.2/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-04-25 21:48:38.000000 tbpy-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.699295 tbpy-1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.735033 tbpy-1.2/src/tbpy/
--rw-rw-rw-   0        0        0    10628 2023-04-25 21:46:44.000000 tbpy-1.2/src/tbpy/__init__.py
--rw-rw-rw-   0        0        0     1254 2023-04-25 21:47:51.000000 tbpy-1.2/src/tbpy/test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.778653 tbpy-1.2/src/tbpy.egg-info/
--rw-rw-rw-   0        0        0      830 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.786684 tbpy-1.2/tests/
--rw-rw-rw-   0        0        0       88 2023-04-25 20:57:58.000000 tbpy-1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 20:39:16.497121 tbpy-1.3/
+-rw-rw-rw-   0        0        0     1091 2022-11-08 18:13:24.000000 tbpy-1.3/LICENSE
+-rw-rw-rw-   0        0        0      830 2023-04-27 20:39:16.495120 tbpy-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-25 21:35:19.000000 tbpy-1.3/README.md
+-rw-rw-rw-   0        0        0      506 2023-04-27 17:08:51.000000 tbpy-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 20:39:16.498121 tbpy-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-27 20:34:18.000000 tbpy-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 20:39:16.407801 tbpy-1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 20:39:16.449329 tbpy-1.3/src/tbpy/
+-rw-rw-rw-   0        0        0    12399 2023-04-27 20:27:02.000000 tbpy-1.3/src/tbpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 20:39:16.484733 tbpy-1.3/src/tbpy.egg-info/
+-rw-rw-rw-   0        0        0      830 2023-04-27 20:39:16.000000 tbpy-1.3/src/tbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-04-27 20:39:16.000000 tbpy-1.3/src/tbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 20:39:16.000000 tbpy-1.3/src/tbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 20:39:16.000000 tbpy-1.3/src/tbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 20:39:16.486733 tbpy-1.3/tests/
+-rw-rw-rw-   0        0        0       88 2023-04-25 20:57:58.000000 tbpy-1.3/tests/test.py
```

### Comparing `tbpy-1.2/LICENSE` & `tbpy-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tbpy-1.2/PKG-INFO` & `tbpy-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbpy
-Version: 1.2
+Version: 1.3
 Summary: Welcome to terminalbreaker
 Home-page: https://github.com/Ellicode/terminalbreaker
 Author: Ellicode
 Author-email: Ellicode <ellicode22@gmail.com>
 Project-URL: Homepage, https://github.com/Ellicode/terminalbreaker
 Project-URL: Bug Tracker, https://github.com/Ellicode/terminalbreaker/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tbpy-1.2/setup.py` & `tbpy-1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "tbpy",
-    version = "1.2",
+    version = "1.3",
     author = "Ellicode",
     author_email = "ellicode22@gmail.com",
     description = "Welcome to terminalbreaker!",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Ellicode/terminalbreaker",
     project_urls = {
         "Bug Tracker": "https://github.com/Ellicode/terminalbreaker/issues",
     },
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[
-        'colorama',
-    ],
     package_dir = {"": "src"},
     packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.6"
 )
```

### Comparing `tbpy-1.2/src/tbpy.egg-info/PKG-INFO` & `tbpy-1.3/src/tbpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbpy
-Version: 1.2
+Version: 1.3
 Summary: Welcome to terminalbreaker
 Home-page: https://github.com/Ellicode/terminalbreaker
 Author: Ellicode
 Author-email: Ellicode <ellicode22@gmail.com>
 Project-URL: Homepage, https://github.com/Ellicode/terminalbreaker
 Project-URL: Bug Tracker, https://github.com/Ellicode/terminalbreaker/issues
 Classifier: Programming Language :: Python :: 3
```

