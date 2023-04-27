# Comparing `tmp/openz-0.1.0.tar.gz` & `tmp/openz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openz-0.1.0.tar", max compression
+gzip compressed data, was "openz-0.1.1.tar", max compression
```

## Comparing `openz-0.1.0.tar` & `openz-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2023-04-27 13:14:20.771065 openz-0.1.0/LICENSE
--rw-r--r--   0        0        0      231 2023-04-27 14:47:34.718102 openz-0.1.0/openz/__init__.py
--rw-r--r--   0        0        0     3980 2023-04-27 15:45:33.710543 openz-0.1.0/openz/_core.py
--rw-r--r--   0        0        0      552 2023-04-27 15:54:05.556018 openz-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      714 2023-04-27 15:50:55.554663 openz-0.1.0/README.md
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 openz-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-27 13:14:20.771065 openz-0.1.1/LICENSE
+-rw-r--r--   0        0        0      231 2023-04-27 14:47:34.718102 openz-0.1.1/openz/__init__.py
+-rw-r--r--   0        0        0     3980 2023-04-27 15:45:33.710543 openz-0.1.1/openz/_core.py
+-rw-r--r--   0        0        0      606 2023-04-27 15:55:36.060885 openz-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-04-27 15:50:55.554663 openz-0.1.1/README.md
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 openz-0.1.1/PKG-INFO
```

### Comparing `openz-0.1.0/LICENSE` & `openz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openz-0.1.0/openz/_core.py` & `openz-0.1.1/openz/_core.py`

 * *Files identical despite different names*

### Comparing `openz-0.1.0/pyproject.toml` & `openz-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "openz"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Cologler <skyoflw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "openz"}]
+homepage = "https://github.com/Cologler/openz-python"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 filelock = "^3.12.0"
 portalocker = "^2.7.0"
 nanoid = "^2.0.0"
```

### Comparing `openz-0.1.0/README.md` & `openz-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openz-0.1.0/PKG-INFO` & `openz-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: openz
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
+Home-page: https://github.com/Cologler/openz-python
 License: MIT
 Author: Cologler
 Author-email: skyoflw@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

