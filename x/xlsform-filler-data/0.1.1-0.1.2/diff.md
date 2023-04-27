# Comparing `tmp/xlsform_filler_data-0.1.1.tar.gz` & `tmp/xlsform_filler_data-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlsform_filler_data-0.1.1.tar", max compression
+gzip compressed data, was "xlsform_filler_data-0.1.2.tar", max compression
```

## Comparing `xlsform_filler_data-0.1.1.tar` & `xlsform_filler_data-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       76 2023-04-26 05:46:10.327908 xlsform_filler_data-0.1.1/README.md
--rw-r--r--   0        0        0      557 2023-04-26 06:03:30.905260 xlsform_filler_data-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-18 18:35:03.705672 xlsform_filler_data-0.1.1/xlsform_filler_data/__init__.py
--rw-r--r--   0        0        0     2043 2023-04-25 20:01:24.661693 xlsform_filler_data-0.1.1/xlsform_filler_data/xlsform_filler_data.py
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.1/setup.py
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      905 2023-04-27 21:19:14.799272 xlsform_filler_data-0.1.2/README.md
+-rw-r--r--   0        0        0      557 2023-04-27 21:21:36.966735 xlsform_filler_data-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-18 18:35:03.705672 xlsform_filler_data-0.1.2/xlsform_filler_data/__init__.py
+-rw-r--r--   0        0        0     2043 2023-04-25 20:01:24.661693 xlsform_filler_data-0.1.2/xlsform_filler_data/xlsform_filler_data.py
+-rw-r--r--   0        0        0     1844 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.2/setup.py
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 xlsform_filler_data-0.1.2/PKG-INFO
```

### Comparing `xlsform_filler_data-0.1.1/pyproject.toml` & `xlsform_filler_data-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xlsform-filler-data"
-version = "0.1.1"
+version = "0.1.2"
 description = "A tool for generating fake testing data based on an XLSform. "
 authors = ["Brian Mc Donald <brian@brianmcdonald.me>"]
 readme = "README.md"
 packages = [{include = "xlsform_filler_data"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `xlsform_filler_data-0.1.1/xlsform_filler_data/xlsform_filler_data.py` & `xlsform_filler_data-0.1.2/xlsform_filler_data/xlsform_filler_data.py`

 * *Files identical despite different names*

