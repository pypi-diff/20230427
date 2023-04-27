# Comparing `tmp/sortinghat_openinfra-0.1.0.tar.gz` & `tmp/sortinghat_openinfra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat_openinfra-0.1.0.tar", max compression
+gzip compressed data, was "sortinghat_openinfra-0.1.1.tar", max compression
```

## Comparing `sortinghat_openinfra-0.1.0.tar` & `sortinghat_openinfra-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-24 16:31:53.884965 sortinghat_openinfra-0.1.0/LICENSE
--rw-r--r--   0        0        0     2244 2023-04-24 16:31:53.884965 sortinghat_openinfra-0.1.0/README.md
--rw-r--r--   0        0        0     1248 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/sortinghat/core/importer/backends/_version.py
--rw-r--r--   0        0        0     7864 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/sortinghat/core/importer/backends/openinfra.py
--rw-r--r--   0        0        0        0 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     6403 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/tests/data/openinfra_page_1.json
--rw-r--r--   0        0        0     5073 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/tests/data/openinfra_page_2.json
--rw-r--r--   0        0        0     2595 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/tests/data/openinfra_private.json
--rw-r--r--   0        0        0    17771 2023-04-24 16:31:53.888965 sortinghat_openinfra-0.1.0/tests/test_openinfra.py
--rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2244 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/README.md
+-rw-r--r--   0        0        0     1248 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/sortinghat/core/importer/backends/_version.py
+-rw-r--r--   0        0        0     7864 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/sortinghat/core/importer/backends/openinfra.py
+-rw-r--r--   0        0        0        0 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     6403 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/tests/data/openinfra_page_1.json
+-rw-r--r--   0        0        0     5073 2023-04-27 12:20:41.004426 sortinghat_openinfra-0.1.1/tests/data/openinfra_page_2.json
+-rw-r--r--   0        0        0     2595 2023-04-27 12:20:41.004426 sortinghat_openinfra-0.1.1/tests/data/openinfra_private.json
+-rw-r--r--   0        0        0    17771 2023-04-27 12:20:41.004426 sortinghat_openinfra-0.1.1/tests/test_openinfra.py
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.1/PKG-INFO
```

### Comparing `sortinghat_openinfra-0.1.0/LICENSE` & `sortinghat_openinfra-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.0/README.md` & `sortinghat_openinfra-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.0/pyproject.toml` & `sortinghat_openinfra-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat-openinfra"
-version = "0.1.0"
+version = "0.1.1"
 description = "SortingHat backend to import identities from OpenInfraID"
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sortinghat_openinfra-0.1.0/sortinghat/core/importer/backends/openinfra.py` & `sortinghat_openinfra-0.1.1/sortinghat/core/importer/backends/openinfra.py`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.0/tests/data/openinfra_page_1.json` & `sortinghat_openinfra-0.1.1/tests/data/openinfra_page_1.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.0/tests/data/openinfra_page_2.json` & `sortinghat_openinfra-0.1.1/tests/data/openinfra_page_2.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.0/tests/data/openinfra_private.json` & `sortinghat_openinfra-0.1.1/tests/data/openinfra_private.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.0/tests/test_openinfra.py` & `sortinghat_openinfra-0.1.1/tests/test_openinfra.py`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.0/PKG-INFO` & `sortinghat_openinfra-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat-openinfra
-Version: 0.1.0
+Version: 0.1.1
 Summary: SortingHat backend to import identities from OpenInfraID
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab,sortinghat
 Author: Bitergia Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

