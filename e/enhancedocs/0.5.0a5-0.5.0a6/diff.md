# Comparing `tmp/enhancedocs-0.5.0a5.tar.gz` & `tmp/enhancedocs-0.5.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.0a5.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.0a6.tar", max compression
```

## Comparing `enhancedocs-0.5.0a5.tar` & `enhancedocs-0.5.0a6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/LICENSE
--rw-r--r--   0        0        0      846 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/README.md
--rw-r--r--   0        0        0      432 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0      777 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0      918 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/commands/build.py
--rw-r--r--   0        0        0      976 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/commands/push.py
--rw-r--r--   0        0        0      369 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/config.py
--rw-r--r--   0        0        0      370 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/main.py
--rw-r--r--   0        0        0      311 2023-04-27 13:45:10.177908 enhancedocs-0.5.0a5/src/enhancedocs/utils.py
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 enhancedocs-0.5.0a5/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/LICENSE
+-rw-r--r--   0        0        0      846 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/README.md
+-rw-r--r--   0        0        0      455 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0      777 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0      940 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0     1838 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0      817 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/config.py
+-rw-r--r--   0        0        0      370 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/main.py
+-rw-r--r--   0        0        0      311 2023-04-27 16:53:38.448109 enhancedocs-0.5.0a6/src/enhancedocs/utils.py
+-rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 enhancedocs-0.5.0a6/PKG-INFO
```

### Comparing `enhancedocs-0.5.0a5/LICENSE` & `enhancedocs-0.5.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a5/README.md` & `enhancedocs-0.5.0a6/README.md`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a5/src/enhancedocs/commands/ask.py` & `enhancedocs-0.5.0a6/src/enhancedocs/commands/ask.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a5/src/enhancedocs/commands/build.py` & `enhancedocs-0.5.0a6/src/enhancedocs/commands/build.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,8 +25,8 @@
         for path in paths:
             files = get_files(path)
             for file in files:
                 file_data = read_file(file)
                 if file_data is not None:
                     output_file.write(json.dumps(file_data) + '\n')
 
-    return True
+    click.echo("🔨 Build finished")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `enhancedocs-0.5.0a5/PKG-INFO` & `enhancedocs-0.5.0a6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.0a5
+Version: 0.5.0a6
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: sentry-sdk (>=1.21.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # EnhanceDocs CLI
 
 EnhanceDocs Command Line Interface (CLI)
 
 [![pypi version](https://img.shields.io/pypi/v/enhancedocs.svg)](https://pypi.org/pypi/enhancedocs/)
```

