# Comparing `tmp/autocalver-2023.4.26.84995rc1.tar.gz` & `tmp/autocalver-2023.4.26.85833.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocalver-2023.4.26.84995rc1.tar", last modified: Wed Apr 26 23:37:47 2023, max compression
+gzip compressed data, was "autocalver-2023.4.26.85833.tar", last modified: Wed Apr 26 23:50:56 2023, max compression
```

## Comparing `autocalver-2023.4.26.84995rc1.tar` & `autocalver-2023.4.26.85833.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:37:47.302847 autocalver-2023.4.26.84995rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-26 23:37:32.000000 autocalver-2023.4.26.84995rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 23:37:32.000000 autocalver-2023.4.26.84995rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-26 23:37:47.302847 autocalver-2023.4.26.84995rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-26 23:37:32.000000 autocalver-2023.4.26.84995rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-26 23:37:46.000000 autocalver-2023.4.26.84995rc1/git-log-head
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 23:37:32.000000 autocalver-2023.4.26.84995rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 23:37:47.302847 autocalver-2023.4.26.84995rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:37:47.298847 autocalver-2023.4.26.84995rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:37:47.298847 autocalver-2023.4.26.84995rc1/src/autocalver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-26 23:37:32.000000 autocalver-2023.4.26.84995rc1/src/autocalver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-26 23:37:32.000000 autocalver-2023.4.26.84995rc1/src/autocalver/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:37:47.298847 autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-26 23:37:47.000000 autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 23:37:47.000000 autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 23:37:47.000000 autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 23:37:47.000000 autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 23:37:47.000000 autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 23:37:47.000000 autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:37:47.302847 autocalver-2023.4.26.84995rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-26 23:37:32.000000 autocalver-2023.4.26.84995rc1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:50:56.970949 autocalver-2023.4.26.85833/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-26 23:50:44.000000 autocalver-2023.4.26.85833/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 23:50:44.000000 autocalver-2023.4.26.85833/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-26 23:50:56.970949 autocalver-2023.4.26.85833/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-26 23:50:44.000000 autocalver-2023.4.26.85833/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-26 23:50:56.000000 autocalver-2023.4.26.85833/git-log-head
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 23:50:44.000000 autocalver-2023.4.26.85833/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 23:50:56.970949 autocalver-2023.4.26.85833/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:50:56.970949 autocalver-2023.4.26.85833/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:50:56.970949 autocalver-2023.4.26.85833/src/autocalver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-26 23:50:44.000000 autocalver-2023.4.26.85833/src/autocalver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-26 23:50:44.000000 autocalver-2023.4.26.85833/src/autocalver/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:50:56.970949 autocalver-2023.4.26.85833/src/autocalver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-26 23:50:56.000000 autocalver-2023.4.26.85833/src/autocalver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 23:50:56.000000 autocalver-2023.4.26.85833/src/autocalver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 23:50:56.000000 autocalver-2023.4.26.85833/src/autocalver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 23:50:56.000000 autocalver-2023.4.26.85833/src/autocalver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 23:50:56.000000 autocalver-2023.4.26.85833/src/autocalver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 23:50:56.000000 autocalver-2023.4.26.85833/src/autocalver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:50:56.970949 autocalver-2023.4.26.85833/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-26 23:50:44.000000 autocalver-2023.4.26.85833/tests/test_integration.py
```

### Comparing `autocalver-2023.4.26.84995rc1/LICENSE` & `autocalver-2023.4.26.85833/LICENSE`

 * *Files identical despite different names*

### Comparing `autocalver-2023.4.26.84995rc1/PKG-INFO` & `autocalver-2023.4.26.85833/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocalver
-Version: 2023.4.26.84995rc1
+Version: 2023.4.26.85833
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: lint
 Provides-Extra: mypy
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `autocalver-2023.4.26.84995rc1/README.md` & `autocalver-2023.4.26.85833/README.md`

 * *Files identical despite different names*

### Comparing `autocalver-2023.4.26.84995rc1/pyproject.toml` & `autocalver-2023.4.26.85833/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autocalver-2023.4.26.84995rc1/src/autocalver/integration.py` & `autocalver-2023.4.26.85833/src/autocalver/integration.py`

 * *Files identical despite different names*

### Comparing `autocalver-2023.4.26.84995rc1/src/autocalver.egg-info/PKG-INFO` & `autocalver-2023.4.26.85833/src/autocalver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocalver
-Version: 2023.4.26.84995rc1
+Version: 2023.4.26.85833
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: lint
 Provides-Extra: mypy
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `autocalver-2023.4.26.84995rc1/tests/test_integration.py` & `autocalver-2023.4.26.85833/tests/test_integration.py`

 * *Files identical despite different names*

