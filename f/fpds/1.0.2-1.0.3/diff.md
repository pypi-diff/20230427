# Comparing `tmp/fpds-1.0.2.tar.gz` & `tmp/fpds-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpds-1.0.2.tar", last modified: Thu Jan  5 20:22:55 2023, max compression
+gzip compressed data, was "fpds-1.0.3.tar", last modified: Wed Apr 26 22:19:23 2023, max compression
```

## Comparing `fpds-1.0.2.tar` & `fpds-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.717194 fpds-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-05 20:21:59.000000 fpds-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-05 20:21:59.000000 fpds-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-01-05 20:22:55.717194 fpds-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-01-05 20:21:59.000000 fpds-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-05 20:22:55.717194 fpds-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 20:21:59.000000 fpds-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.713194 fpds-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.717194 fpds-1.0.2/src/fpds/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.717194 fpds-1.0.2/src/fpds/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/cli/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.717194 fpds-1.0.2/src/fpds/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/constants/fields.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.717194 fpds-1.0.2/src/fpds/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/core/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.717194 fpds-1.0.2/src/fpds/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-01-05 20:21:59.000000 fpds-1.0.2/src/fpds/utilities/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:22:55.717194 fpds-1.0.2/src/fpds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-01-05 20:22:55.000000 fpds-1.0.2/src/fpds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-01-05 20:22:55.000000 fpds-1.0.2/src/fpds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:22:55.000000 fpds-1.0.2/src/fpds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 20:22:55.000000 fpds-1.0.2/src/fpds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-01-05 20:22:55.000000 fpds-1.0.2/src/fpds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-05 20:22:55.000000 fpds-1.0.2/src/fpds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.297100 fpds-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 22:18:26.000000 fpds-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 22:18:26.000000 fpds-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-26 22:19:23.297100 fpds-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-26 22:18:26.000000 fpds-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 22:19:23.297100 fpds-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:18:26.000000 fpds-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.285099 fpds-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.289100 fpds-1.0.3/src/fpds/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/cli/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/constants/fields.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/core/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/utilities/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.297100 fpds-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 22:18:26.000000 fpds-1.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-26 22:18:26.000000 fpds-1.0.3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-26 22:18:26.000000 fpds-1.0.3/tests/test_xml.py
```

### Comparing `fpds-1.0.2/LICENSE` & `fpds-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fpds-1.0.2/PKG-INFO` & `fpds-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpds
-Version: 1.0.2
+Version: 1.0.3
 Summary: A parser for the Federal Procurement Data System (FPDS) Atom feed
 Author: Derek Herincx
 Author-email: derek663@gmail.com
 Keywords: fpds python atom cli
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `fpds-1.0.2/README.md` & `fpds-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fpds-1.0.2/setup.cfg` & `fpds-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = fpds
 author = Derek Herincx
 author_email = derek663@gmail.com
-version = 1.0.2
+version = 1.0.3
 description = A parser for the Federal Procurement Data System (FPDS) Atom feed
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = fpds python atom cli
 classifiers = 
 	Intended Audience :: Developers
 	Natural Language :: English
```

### Comparing `fpds-1.0.2/src/fpds/cli/parse.py` & `fpds-1.0.3/src/fpds/cli/parse.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.2/src/fpds/config.py` & `fpds-1.0.3/src/fpds/config.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.2/src/fpds/constants/fields.json` & `fpds-1.0.3/src/fpds/constants/fields.json`

 * *Files identical despite different names*

### Comparing `fpds-1.0.2/src/fpds/core/parser.py` & `fpds-1.0.3/src/fpds/core/parser.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.2/src/fpds/utilities/params.py` & `fpds-1.0.3/src/fpds/utilities/params.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.2/src/fpds.egg-info/PKG-INFO` & `fpds-1.0.3/src/fpds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpds
-Version: 1.0.2
+Version: 1.0.3
 Summary: A parser for the Federal Procurement Data System (FPDS) Atom feed
 Author: Derek Herincx
 Author-email: derek663@gmail.com
 Keywords: fpds python atom cli
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

