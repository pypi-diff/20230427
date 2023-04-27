# Comparing `tmp/kthutils-1.0.tar.gz` & `tmp/kthutils-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthutils-1.0.tar", max compression
+gzip compressed data, was "kthutils-1.1.tar", max compression
```

## Comparing `kthutils-1.0.tar` & `kthutils-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.0/LICENSE
--rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.0/README.md
--rw-r--r--   0        0        0      720 2023-03-28 07:05:16.669844 kthutils-1.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.0/src/kthutils/.gitignore
--rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.0/src/kthutils/Makefile
--rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.0/src/kthutils/__init__.py
--rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.0/src/kthutils/cli.nw
--rw-r--r--   0        0        0      281 2023-03-28 06:57:35.072238 kthutils-1.0/src/kthutils/cli.py
--rw-r--r--   0        0        0      770 2023-03-28 06:57:35.076238 kthutils-1.0/src/kthutils/credentials.py
--rw-r--r--   0        0        0    16503 2023-03-28 08:32:20.170796 kthutils-1.0/src/kthutils/ug.nw
--rw-r--r--   0        0        0     8343 2023-03-28 08:32:20.922786 kthutils-1.0/src/kthutils/ug.py
--rw-r--r--   0        0        0      745 2023-03-28 08:50:25.909228 kthutils-1.0/tests/test_ug.py
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 kthutils-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.1/LICENSE
+-rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.1/README.md
+-rw-r--r--   0        0        0      721 2023-04-27 18:35:31.070513 kthutils-1.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.1/src/kthutils/.gitignore
+-rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.1/src/kthutils/Makefile
+-rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.1/src/kthutils/__init__.py
+-rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.1/src/kthutils/cli.nw
+-rw-r--r--   0        0        0      281 2023-04-27 18:36:23.514363 kthutils-1.1/src/kthutils/cli.py
+-rw-r--r--   0        0        0      770 2023-04-27 18:36:23.514363 kthutils-1.1/src/kthutils/credentials.py
+-rw-r--r--   0        0        0    16503 2023-03-28 08:32:20.170796 kthutils-1.1/src/kthutils/ug.nw
+-rw-r--r--   0        0        0     8343 2023-04-27 18:36:23.518363 kthutils-1.1/src/kthutils/ug.py
+-rw-r--r--   0        0        0      745 2023-03-28 08:50:25.909228 kthutils-1.1/tests/test_ug.py
+-rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.1/PKG-INFO
```

### Comparing `kthutils-1.0/LICENSE` & `kthutils-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kthutils-1.0/README.md` & `kthutils-1.1/README.md`

 * *Files identical despite different names*

### Comparing `kthutils-1.0/pyproject.toml` & `kthutils-1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kthutils"
-version = "1.0"
+version = "1.1"
 description = "Various tools for automation at KTH"
 authors = ["Daniel Bosk <dbosk@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/kthutils"
 include = ["*/**/*.py"]
 
@@ -16,15 +16,15 @@
 kthutils = "kthutils.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 weblogin = "^1.5"
 cachetools = "^5.2.0"
 typer = "^0.7.0"
-typerconf = "^1.1"
+typerconf = "^1.10"
 rich = "^13.3.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `kthutils-1.0/src/kthutils/cli.nw` & `kthutils-1.1/src/kthutils/cli.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.0/src/kthutils/credentials.py` & `kthutils-1.1/src/kthutils/credentials.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.0/src/kthutils/ug.nw` & `kthutils-1.1/src/kthutils/ug.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.0/src/kthutils/ug.py` & `kthutils-1.1/src/kthutils/ug.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.0/tests/test_ug.py` & `kthutils-1.1/tests/test_ug.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.0/PKG-INFO` & `kthutils-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthutils
-Version: 1.0
+Version: 1.1
 Summary: Various tools for automation at KTH
 Home-page: https://github.com/dbosk/kthutils
 License: MIT
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: typerconf (>=1.1,<2.0)
+Requires-Dist: typerconf (>=1.10,<2.0)
 Requires-Dist: weblogin (>=1.5,<2.0)
 Project-URL: Bug Tracker, https://github.com/dbosk/kthutils/issues
 Project-URL: Repository, https://github.com/dbosk/kthutils
 Project-URL: Releases, https://github.com/dbosk/kthutils/releases
 Description-Content-Type: text/markdown
 
 This package provides various utilities for automation at KTH. It
```

