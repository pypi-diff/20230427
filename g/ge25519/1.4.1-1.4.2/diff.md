# Comparing `tmp/ge25519-1.4.1.tar.gz` & `tmp/ge25519-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ge25519-1.4.1.tar", last modified: Wed Apr 26 19:36:01 2023, max compression
+gzip compressed data, was "ge25519-1.4.2.tar", last modified: Wed Apr 26 22:41:24 2023, max compression
```

## Comparing `ge25519-1.4.1.tar` & `ge25519-1.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.186356 ge25519-1.4.1/
--rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-25 14:57:02.000000 ge25519-1.4.1/LICENSE
--rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-26 19:36:01.186433 ge25519-1.4.1/PKG-INFO
--rw-r--r--   0 alapets    (502) staff       (20)     5258 2023-04-15 14:00:02.000000 ge25519-1.4.1/README.rst
--rw-r--r--   0 alapets    (502) staff       (20)     1034 2023-04-26 19:27:36.000000 ge25519-1.4.1/pyproject.toml
--rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-26 19:36:01.186660 ge25519-1.4.1/setup.cfg
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.183544 ge25519-1.4.1/src/
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.184723 ge25519-1.4.1/src/ge25519/
--rw-r--r--   0 alapets    (502) staff       (20)      166 2023-04-25 14:57:02.000000 ge25519-1.4.1/src/ge25519/__init__.py
--rw-r--r--   0 alapets    (502) staff       (20)   121618 2023-04-25 14:57:02.000000 ge25519-1.4.1/src/ge25519/ge25519.py
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.186065 ge25519-1.4.1/src/ge25519.egg-info/
--rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/PKG-INFO
--rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/SOURCES.txt
--rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/dependency_links.txt
--rw-r--r--   0 alapets    (502) staff       (20)      234 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/requires.txt
--rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/top_level.txt
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.186203 ge25519-1.4.1/test/
--rw-r--r--   0 alapets    (502) staff       (20)     8605 2023-04-25 14:57:02.000000 ge25519-1.4.1/test/test_ge25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:41:24.609966 ge25519-1.4.2/
+-rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-25 14:57:02.000000 ge25519-1.4.2/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)     5792 2023-04-26 22:41:24.610021 ge25519-1.4.2/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)     5256 2023-04-26 22:36:48.000000 ge25519-1.4.2/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)     1034 2023-04-26 22:39:41.000000 ge25519-1.4.2/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-26 22:41:24.610219 ge25519-1.4.2/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:41:24.607547 ge25519-1.4.2/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:41:24.608601 ge25519-1.4.2/src/ge25519/
+-rw-r--r--   0 alapets    (502) staff       (20)      166 2023-04-25 14:57:02.000000 ge25519-1.4.2/src/ge25519/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)   121618 2023-04-25 14:57:02.000000 ge25519-1.4.2/src/ge25519/ge25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:41:24.609653 ge25519-1.4.2/src/ge25519.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)     5792 2023-04-26 22:41:24.000000 ge25519-1.4.2/src/ge25519.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-26 22:41:24.000000 ge25519-1.4.2/src/ge25519.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-26 22:41:24.000000 ge25519-1.4.2/src/ge25519.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      234 2023-04-26 22:41:24.000000 ge25519-1.4.2/src/ge25519.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-26 22:41:24.000000 ge25519-1.4.2/src/ge25519.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 22:41:24.609800 ge25519-1.4.2/test/
+-rw-r--r--   0 alapets    (502) staff       (20)     8605 2023-04-25 14:57:02.000000 ge25519-1.4.2/test/test_ge25519.py
```

### Comparing `ge25519-1.4.1/LICENSE` & `ge25519-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ge25519-1.4.1/PKG-INFO` & `ge25519-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ge25519
-Version: 1.4.1
+Version: 1.4.2
 Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/ge25519
 Project-URL: Documentation, https://ge25519.readthedocs.io
 Requires-Python: >=3.7
@@ -42,16 +42,16 @@
 
 Purpose
 -------
 This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
 
 The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
 
-PInstallation and Usage
------------------------
+Installation and Usage
+----------------------
 This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__:
 
 .. code-block:: bash
 
     python -m pip install ge25519
 
 The library can be imported in the usual ways:
```

### Comparing `ge25519-1.4.1/README.rst` & `ge25519-1.4.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 Purpose
 -------
 This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
 
 The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
 
-PInstallation and Usage
------------------------
+Installation and Usage
+----------------------
 This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__:
 
 .. code-block:: bash
 
     python -m pip install ge25519
 
 The library can be imported in the usual ways:
```

### Comparing `ge25519-1.4.1/pyproject.toml` & `ge25519-1.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ge25519"
-version = "1.4.1"
+version = "1.4.2"
 description = """\
     Pure-Python data structure for working with Ed25519 \
     (and Ristretto) group elements and operations.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
```

### Comparing `ge25519-1.4.1/src/ge25519/ge25519.py` & `ge25519-1.4.2/src/ge25519/ge25519.py`

 * *Files identical despite different names*

### Comparing `ge25519-1.4.1/src/ge25519.egg-info/PKG-INFO` & `ge25519-1.4.2/src/ge25519.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ge25519
-Version: 1.4.1
+Version: 1.4.2
 Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/ge25519
 Project-URL: Documentation, https://ge25519.readthedocs.io
 Requires-Python: >=3.7
@@ -42,16 +42,16 @@
 
 Purpose
 -------
 This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
 
 The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
 
-PInstallation and Usage
------------------------
+Installation and Usage
+----------------------
 This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__:
 
 .. code-block:: bash
 
     python -m pip install ge25519
 
 The library can be imported in the usual ways:
```

### Comparing `ge25519-1.4.1/test/test_ge25519.py` & `ge25519-1.4.2/test/test_ge25519.py`

 * *Files identical despite different names*

