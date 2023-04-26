# Comparing `tmp/settngs-0.6.3.tar.gz` & `tmp/settngs-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settngs-0.6.3.tar", last modified: Tue Apr 25 07:16:12 2023, max compression
+gzip compressed data, was "settngs-0.6.5.tar", last modified: Wed Apr 26 22:34:48 2023, max compression
```

## Comparing `settngs-0.6.3.tar` & `settngs-0.6.5.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:12.033409 settngs-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 07:16:03.000000 settngs-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-25 07:16:12.033409 settngs-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-25 07:16:03.000000 settngs-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:12.033409 settngs-0.6.3/settngs/
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-04-25 07:16:03.000000 settngs-0.6.3/settngs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 07:16:03.000000 settngs-0.6.3/settngs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:03.000000 settngs-0.6.3/settngs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:16:12.033409 settngs-0.6.3/settngs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 07:16:12.000000 settngs-0.6.3/settngs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-25 07:16:12.037409 settngs-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 07:16:03.000000 settngs-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.051508 settngs-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-26 22:34:34.000000 settngs-0.6.5/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-26 22:34:34.000000 settngs-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 22:34:34.000000 settngs-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-26 22:34:34.000000 settngs-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-26 22:34:48.055508 settngs-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-26 22:34:34.000000 settngs-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 22:34:34.000000 settngs-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:34:34.000000 settngs-0.6.5/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/settngs/
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-04-26 22:34:34.000000 settngs-0.6.5/settngs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 22:34:34.000000 settngs-0.6.5/settngs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:34.000000 settngs-0.6.5/settngs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/settngs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 22:34:48.000000 settngs-0.6.5/settngs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-26 22:34:48.055508 settngs-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 22:34:34.000000 settngs-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:34.000000 settngs-0.6.5/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-26 22:34:34.000000 settngs-0.6.5/testing/settngs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:34.000000 settngs-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-04-26 22:34:34.000000 settngs-0.6.5/tests/settngs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:34:48.055508 settngs-0.6.5/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-26 22:34:34.000000 settngs-0.6.5/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-26 22:34:34.000000 settngs-0.6.5/workflows/package.yaml
```

### Comparing `settngs-0.6.3/LICENSE` & `settngs-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `settngs-0.6.3/PKG-INFO` & `settngs-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.6.3
+Version: 0.6.5
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.6.3/README.md` & `settngs-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `settngs-0.6.3/settngs/__init__.py` & `settngs-0.6.5/settngs/__init__.py`

 * *Files identical despite different names*

### Comparing `settngs-0.6.3/settngs.egg-info/PKG-INFO` & `settngs-0.6.5/settngs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.6.3
+Version: 0.6.5
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.6.3/setup.cfg` & `settngs-0.6.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = settngs
-version = 0.6.3
 description = A library for managing settings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lordwelch/settngs
 author = Timmy Welch
 author_email = timmy@narnian.us
 license = MIT
@@ -15,15 +14,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 install_requires = 
-	typing-extensions;python_version < '3.11'
+	typing-extensions>=4.3.0;python_version < '3.11'
 python_requires = >=3.8
 include_package_data = True
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
```

