# Comparing `tmp/aioxmlrpc-0.6.4.tar.gz` & `tmp/aioxmlrpc-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxmlrpc-0.6.4.tar", max compression
+gzip compressed data, was "aioxmlrpc-0.6.5.tar", max compression
```

## Comparing `aioxmlrpc-0.6.4.tar` & `aioxmlrpc-0.6.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1525 2022-06-02 06:43:48.349040 aioxmlrpc-0.6.4/LICENSE
--rw-r--r--   0        0        0     1390 2022-06-02 06:43:48.349040 aioxmlrpc-0.6.4/README.rst
--rw-r--r--   0        0        0      508 2022-06-02 06:52:52.504178 aioxmlrpc-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      129 2022-06-02 06:43:48.352373 aioxmlrpc-0.6.4/src/aioxmlrpc/__init__.py
--rw-r--r--   0        0        0     4741 2022-06-02 06:43:48.352373 aioxmlrpc-0.6.4/src/aioxmlrpc/client.py
--rw-r--r--   0        0        0     2176 2022-06-02 06:52:56.079730 aioxmlrpc-0.6.4/setup.py
--rw-r--r--   0        0        0     2032 2022-06-02 06:52:56.079970 aioxmlrpc-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1525 2022-06-02 06:43:48.349040 aioxmlrpc-0.6.5/LICENSE
+-rw-r--r--   0        0        0     1390 2022-06-02 06:43:48.349040 aioxmlrpc-0.6.5/README.rst
+-rw-r--r--   0        0        0      498 2023-04-27 08:33:37.381595 aioxmlrpc-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      129 2022-06-02 06:43:48.352373 aioxmlrpc-0.6.5/src/aioxmlrpc/__init__.py
+-rw-r--r--   0        0        0     4741 2022-06-02 06:43:48.352373 aioxmlrpc-0.6.5/src/aioxmlrpc/client.py
+-rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 aioxmlrpc-0.6.5/PKG-INFO
```

### Comparing `aioxmlrpc-0.6.4/LICENSE` & `aioxmlrpc-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxmlrpc-0.6.4/README.rst` & `aioxmlrpc-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `aioxmlrpc-0.6.4/src/aioxmlrpc/client.py` & `aioxmlrpc-0.6.5/src/aioxmlrpc/client.py`

 * *Files identical despite different names*

### Comparing `aioxmlrpc-0.6.4/PKG-INFO` & `aioxmlrpc-0.6.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aioxmlrpc
-Version: 0.6.4
-Summary: Source code of Sequoia API TLDPublic
+Version: 0.6.5
+Summary: XML-RPC client for asyncio
 Home-page: https://github.com/mardiros/aioxmlrpc
 License: BSD-3-Clause License
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Description-Content-Type: text/x-rst
 
 =========
 aioxmlrpc
 =========
 
 .. image:: https://github.com/mardiros/aioxmlrpc/actions/workflows/main.yml/badge.svg
```

