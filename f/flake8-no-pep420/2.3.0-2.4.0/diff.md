# Comparing `tmp/flake8-no-pep420-2.3.0.tar.gz` & `tmp/flake8_no_pep420-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-no-pep420-2.3.0.tar", last modified: Wed May 11 10:37:44 2022, max compression
+gzip compressed data, was "flake8_no_pep420-2.4.0.tar", last modified: Thu Apr 27 15:42:54 2023, max compression
```

## Comparing `flake8-no-pep420-2.3.0.tar` & `flake8_no_pep420-2.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:37:44.128776 flake8-no-pep420-2.3.0/
--rw-r--r--   0 chainz     (501) staff       (20)     1131 2022-05-11 10:37:35.000000 flake8-no-pep420-2.3.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:28:23.000000 flake8-no-pep420-2.3.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:11.000000 flake8-no-pep420-2.3.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     4365 2022-05-11 10:37:44.128986 flake8-no-pep420-2.3.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     3293 2022-05-11 10:35:25.000000 flake8-no-pep420-2.3.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      635 2022-01-19 11:13:57.000000 flake8-no-pep420-2.3.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1356 2022-05-11 10:37:44.130105 flake8-no-pep420-2.3.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:13:57.000000 flake8-no-pep420-2.3.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:37:44.122105 flake8-no-pep420-2.3.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:37:44.126270 flake8-no-pep420-2.3.0/src/flake8_no_pep420/
--rw-r--r--   0 chainz     (501) staff       (20)      972 2022-01-26 09:24:10.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-13 11:10:08.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:37:44.128524 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     4365 2022-05-11 10:37:43.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      448 2022-05-11 10:37:44.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 10:37:43.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       58 2022-05-11 10:37:43.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 10:37:42.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       66 2022-05-11 10:37:43.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       17 2022-05-11 10:37:44.000000 flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.841275 flake8_no_pep420-2.4.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1203 2023-04-27 15:42:49.000000 flake8_no_pep420-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:25.000000 flake8_no_pep420-2.4.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 flake8_no_pep420-2.4.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4473 2023-04-27 15:42:54.841331 flake8_no_pep420-2.4.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3314 2022-12-26 15:11:06.000000 flake8_no_pep420-2.4.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 flake8_no_pep420-2.4.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1442 2023-04-27 15:42:54.841601 flake8_no_pep420-2.4.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.839185 flake8_no_pep420-2.4.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.840253 flake8_no_pep420-2.4.0/src/flake8_no_pep420/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1062 2023-04-27 15:37:02.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:25.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.841052 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4473 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      472 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       58 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       66 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.841172 flake8_no_pep420-2.4.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2580 2023-04-27 15:37:02.000000 flake8_no_pep420-2.4.0/tests/test_flake8_no_pep420.py
```

### Comparing `flake8-no-pep420-2.3.0/HISTORY.rst` & `flake8_no_pep420-2.4.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-=======
-History
-=======
+=========
+Changelog
+=========
+
+2.4.0 (2023-04-27)
+------------------
+
+* Support ``.pyi`` files.
 
 2.3.0 (2022-05-11)
 ------------------
 
 * Support Python 3.11.
 
 2.2.0 (2022-01-26)
```

### Comparing `flake8-no-pep420-2.3.0/LICENSE` & `flake8_no_pep420-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-no-pep420-2.3.0/PKG-INFO` & `flake8_no_pep420-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
-Name: flake8-no-pep420
-Version: 2.3.0
+Name: flake8_no_pep420
+Version: 2.4.0
 Summary: A flake8 plugin to ban PEP-420 implicit namespace packages.
 Home-page: https://github.com/adamchainz/flake8-no-pep420
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: flake8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 flake8-no-pep420
 ================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/flake8-no-pep420/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/flake8-no-pep420/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/flake8-no-pep420/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/flake8-no-pep420.svg?style=for-the-badge
    :target: https://pypi.org/project/flake8-no-pep420/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
```

### Comparing `flake8-no-pep420-2.3.0/README.rst` & `flake8_no_pep420-2.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ================
 flake8-no-pep420
 ================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/flake8-no-pep420/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/flake8-no-pep420/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/flake8-no-pep420/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/flake8-no-pep420.svg?style=for-the-badge
    :target: https://pypi.org/project/flake8-no-pep420/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
```

### Comparing `flake8-no-pep420-2.3.0/src/flake8_no_pep420/__init__.py` & `flake8_no_pep420-2.4.0/src/flake8_no_pep420/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import ast
 import os
 import sys
-from typing import Any, Generator
+from typing import Any
+from typing import Generator
 
 if sys.version_info >= (3, 8):
     from importlib.metadata import version
 else:
     from importlib_metadata import version
 
 
@@ -20,18 +21,20 @@
 
     def run(self) -> Generator[tuple[int, int, str, type[Any]], None, None]:
         dirname, basename = os.path.split(self._filename)
 
         if basename == "__init__.py":
             return
 
-        init_name = os.path.join(dirname, "__init__.py")
+        ext = os.path.splitext(basename)[1] or ".py"
+        init = f"__init__{ext}"
+        init_name = os.path.join(dirname, init)
         if not os.path.exists(init_name):
             yield (
                 1,
                 0,
                 (
                     "INP001 File is part of an implicit namespace package."
-                    + " Add an __init__.py?"
+                    + f" Add an {init}?"
                 ),
                 type(self),
             )
```

### Comparing `flake8-no-pep420-2.3.0/src/flake8_no_pep420.egg-info/PKG-INFO` & `flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: flake8-no-pep420
-Version: 2.3.0
+Version: 2.4.0
 Summary: A flake8 plugin to ban PEP-420 implicit namespace packages.
 Home-page: https://github.com/adamchainz/flake8-no-pep420
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: flake8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================
 flake8-no-pep420
 ================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/flake8-no-pep420/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/flake8-no-pep420/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/flake8-no-pep420/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/flake8-no-pep420.svg?style=for-the-badge
    :target: https://pypi.org/project/flake8-no-pep420/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
```

