# Comparing `tmp/enhancedocs-0.5.1.tar.gz` & `tmp/enhancedocs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.1.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.2.tar", max compression
```

## Comparing `enhancedocs-0.5.1.tar` & `enhancedocs-0.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/LICENSE
--rw-r--r--   0        0        0      846 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/README.md
--rw-r--r--   0        0        0      453 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0      777 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0      940 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/commands/build.py
--rw-r--r--   0        0        0     1838 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/commands/push.py
--rw-r--r--   0        0        0      817 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/config.py
--rw-r--r--   0        0        0      370 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/main.py
--rw-r--r--   0        0        0      311 2023-04-27 18:44:38.364222 enhancedocs-0.5.1/src/enhancedocs/utils.py
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 enhancedocs-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1031 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/README.md
+-rw-r--r--   0        0        0      453 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0      777 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0      940 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0     1838 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0     1151 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/config.py
+-rw-r--r--   0        0        0      611 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/main.py
+-rw-r--r--   0        0        0      311 2023-04-27 19:25:43.287299 enhancedocs-0.5.2/src/enhancedocs/utils.py
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 enhancedocs-0.5.2/PKG-INFO
```

### Comparing `enhancedocs-0.5.1/LICENSE` & `enhancedocs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.1/README.md` & `enhancedocs-0.5.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -13,7 +13,13 @@
 
 ## Getting Started
 
 You can install and configure EnhanceDocs using this command:
 ```bash
 pip install -U enhancedocs
 ```
+
+## Running EnhanceDocs CLI on Github Actions
+
+Set up your GitHub Actions workflow with a specific version of EnhanceDocs CLI.
+
+https://github.com/marketplace/actions/setup-enhancedocs
```

### Comparing `enhancedocs-0.5.1/src/enhancedocs/commands/ask.py` & `enhancedocs-0.5.2/src/enhancedocs/commands/ask.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.1/src/enhancedocs/commands/build.py` & `enhancedocs-0.5.2/src/enhancedocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.1/src/enhancedocs/commands/push.py` & `enhancedocs-0.5.2/src/enhancedocs/commands/push.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.1/PKG-INFO` & `enhancedocs-0.5.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.1
+Version: 0.5.2
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -30,7 +30,13 @@
 ## Getting Started
 
 You can install and configure EnhanceDocs using this command:
 ```bash
 pip install -U enhancedocs
 ```
 
+## Running EnhanceDocs CLI on Github Actions
+
+Set up your GitHub Actions workflow with a specific version of EnhanceDocs CLI.
+
+https://github.com/marketplace/actions/setup-enhancedocs
+
```

