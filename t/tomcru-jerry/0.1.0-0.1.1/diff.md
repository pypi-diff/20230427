# Comparing `tmp/tomcru_jerry-0.1.0.tar.gz` & `tmp/tomcru_jerry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru_jerry-0.1.0.tar", max compression
+gzip compressed data, was "tomcru_jerry-0.1.1.tar", max compression
```

## Comparing `tomcru_jerry-0.1.0.tar` & `tomcru_jerry-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.0/LICENSE
--rw-r--r--   0        0        0      124 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.0/README.md
--rw-r--r--   0        0        0      370 2023-04-09 01:05:06.921873 tomcru_jerry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 01:02:24.722671 tomcru_jerry-0.1.0/tomcru_jerry/__init__.py
--rw-r--r--   0        0        0       47 2023-04-09 00:57:52.392152 tomcru_jerry-0.1.0/tomcru_jerry/cloneself/__init__.py
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 tomcru_jerry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.1/LICENSE
+-rw-r--r--   0        0        0      124 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.1/README.md
+-rw-r--r--   0        0        0      391 2023-04-27 01:02:40.831876 tomcru_jerry-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1978 2023-04-17 23:54:18.705910 tomcru_jerry-0.1.1/tomcru_jerry/__init__.py
+-rw-r--r--   0        0        0     3084 2023-04-25 23:25:52.640719 tomcru_jerry-0.1.1/tomcru_jerry/cli.py
+-rw-r--r--   0        0        0     3859 2023-04-23 14:49:50.811637 tomcru_jerry-0.1.1/tomcru_jerry/controllers.py
+-rw-r--r--   0        0        0     2422 2023-04-17 23:28:38.922059 tomcru_jerry-0.1.1/tomcru_jerry/flask_jerry.py
+-rw-r--r--   0        0        0     3617 2023-04-17 23:34:56.509211 tomcru_jerry-0.1.1/tomcru_jerry/mockapi.py
+-rw-r--r--   0        0        0     5494 2023-04-18 00:07:35.193927 tomcru_jerry-0.1.1/tomcru_jerry/static.py
+-rw-r--r--   0        0        0     2268 2023-04-24 16:07:40.404928 tomcru_jerry-0.1.1/tomcru_jerry/utils.py
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 tomcru_jerry-0.1.1/PKG-INFO
```

### Comparing `tomcru_jerry-0.1.0/LICENSE` & `tomcru_jerry-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.0/PKG-INFO` & `tomcru_jerry-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: tomcru-jerry
-Version: 0.1.0
+Version: 0.1.1
 Summary: General purpose web library
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (==3.1.7)
+Requires-Dist: gitpython (==3.1.31)
 Description-Content-Type: text/markdown
 
 # tomcru-jerry
 Reusable library snippets that can be used in any framework. Aimed for flask, fastapi &amp; tomcru projects.
```

