# Comparing `tmp/pypmed-0.1.3.tar.gz` & `tmp/pypmed-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypmed-0.1.3.tar", max compression
+gzip compressed data, was "pypmed-0.1.4.tar", max compression
```

## Comparing `pypmed-0.1.3.tar` & `pypmed-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-04-25 22:13:48.316316 pypmed-0.1.3/LICENSE
--rw-r--r--   0        0        0     1014 2023-04-26 22:01:22.828431 pypmed-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-25 22:13:48.316772 pypmed-0.1.3/pypmed/__init__.py
--rw-r--r--   0        0        0     5661 2023-04-26 21:46:35.212017 pypmed-0.1.3/pypmed/apis.py
--rw-r--r--   0        0        0      946 2023-04-26 21:54:47.967620 pypmed-0.1.3/pypmed/checks.py
--rw-r--r--   0        0        0     1684 2023-04-26 21:48:02.476714 pypmed-0.1.3/pypmed/filters.py
--rw-r--r--   0        0        0     1296 2023-04-26 21:47:46.415870 pypmed-0.1.3/pypmed/parsers.py
--rw-r--r--   0        0        0      669 2023-04-26 22:05:53.857612 pypmed-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 pypmed-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-26 22:14:11.967803 pypmed-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1014 2023-04-26 22:14:11.967803 pypmed-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 22:14:11.967803 pypmed-0.1.4/pypmed/__init__.py
+-rw-r--r--   0        0        0     5661 2023-04-26 22:14:11.967803 pypmed-0.1.4/pypmed/apis.py
+-rw-r--r--   0        0        0      946 2023-04-26 22:14:11.967803 pypmed-0.1.4/pypmed/checks.py
+-rw-r--r--   0        0        0     1684 2023-04-26 22:14:11.967803 pypmed-0.1.4/pypmed/filters.py
+-rw-r--r--   0        0        0     1296 2023-04-26 22:14:11.967803 pypmed-0.1.4/pypmed/parsers.py
+-rw-r--r--   0        0        0      669 2023-04-26 22:14:11.967803 pypmed-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 pypmed-0.1.4/PKG-INFO
```

### Comparing `pypmed-0.1.3/LICENSE` & `pypmed-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.3/README.md` & `pypmed-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.3/pypmed/apis.py` & `pypmed-0.1.4/pypmed/apis.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.3/pypmed/checks.py` & `pypmed-0.1.4/pypmed/checks.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.3/pypmed/filters.py` & `pypmed-0.1.4/pypmed/filters.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.3/pypmed/parsers.py` & `pypmed-0.1.4/pypmed/parsers.py`

 * *Files identical despite different names*

### Comparing `pypmed-0.1.3/pyproject.toml` & `pypmed-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypmed"
-version = "0.1.3"
+version = "0.1.4"
 description = "python wrapper for pubmed apis --> https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi/"
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pypmed"}]
 
 license = "MIT"
```

### Comparing `pypmed-0.1.3/PKG-INFO` & `pypmed-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypmed
-Version: 0.1.3
+Version: 0.1.4
 Summary: python wrapper for pubmed apis --> https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi/
 Home-page: https://github.com/jermwatt/pypmed
 License: MIT
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

