# Comparing `tmp/enhancedocs-0.5.0a1.tar.gz` & `tmp/enhancedocs-0.5.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.0a1.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.0a2.tar", max compression
```

## Comparing `enhancedocs-0.5.0a1.tar` & `enhancedocs-0.5.0a2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-03-27 07:32:26.636816 enhancedocs-0.5.0a1/LICENSE
--rw-r--r--   0        0        0      833 2023-04-27 11:58:01.160797 enhancedocs-0.5.0a1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 10:19:37.805831 enhancedocs-0.5.0a1/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 09:59:17.547934 enhancedocs-0.5.0a1/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0      787 2023-04-27 10:19:37.800385 enhancedocs-0.5.0a1/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0      928 2023-04-27 10:21:38.943135 enhancedocs-0.5.0a1/enhancedocs/commands/build.py
--rw-r--r--   0        0        0      986 2023-04-27 10:20:31.857527 enhancedocs-0.5.0a1/enhancedocs/commands/push.py
--rw-r--r--   0        0        0      399 2023-04-27 10:28:48.381221 enhancedocs-0.5.0a1/enhancedocs/config.py
--rw-r--r--   0        0        0      446 2023-04-27 10:28:48.384720 enhancedocs-0.5.0a1/enhancedocs/main.py
--rw-r--r--   0        0        0      311 2023-04-27 10:06:38.828657 enhancedocs-0.5.0a1/enhancedocs/utils.py
--rw-r--r--   0        0        0      432 2023-04-27 12:00:31.567657 enhancedocs-0.5.0a1/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 enhancedocs-0.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-03-27 07:32:26.636816 enhancedocs-0.5.0a2/LICENSE
+-rw-r--r--   0        0        0      833 2023-04-27 11:58:01.160797 enhancedocs-0.5.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 10:19:37.805831 enhancedocs-0.5.0a2/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:59:17.547934 enhancedocs-0.5.0a2/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0      787 2023-04-27 10:19:37.800385 enhancedocs-0.5.0a2/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0      928 2023-04-27 10:21:38.943135 enhancedocs-0.5.0a2/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0      986 2023-04-27 10:20:31.857527 enhancedocs-0.5.0a2/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0      399 2023-04-27 10:28:48.381221 enhancedocs-0.5.0a2/enhancedocs/config.py
+-rw-r--r--   0        0        0      446 2023-04-27 10:28:48.384720 enhancedocs-0.5.0a2/enhancedocs/main.py
+-rw-r--r--   0        0        0      311 2023-04-27 10:06:38.828657 enhancedocs-0.5.0a2/enhancedocs/utils.py
+-rw-r--r--   0        0        0      435 2023-04-27 12:01:56.324733 enhancedocs-0.5.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 enhancedocs-0.5.0a2/PKG-INFO
```

### Comparing `enhancedocs-0.5.0a1/LICENSE` & `enhancedocs-0.5.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a1/README.md` & `enhancedocs-0.5.0a2/README.md`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a1/enhancedocs/commands/ask.py` & `enhancedocs-0.5.0a2/enhancedocs/commands/ask.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a1/enhancedocs/commands/build.py` & `enhancedocs-0.5.0a2/enhancedocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a1/enhancedocs/commands/push.py` & `enhancedocs-0.5.0a2/enhancedocs/commands/push.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a1/PKG-INFO` & `enhancedocs-0.5.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.0a1
+Version: 0.5.0a2
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

