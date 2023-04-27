# Comparing `tmp/enhancedocs-0.5.0a3.tar.gz` & `tmp/enhancedocs-0.5.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedocs-0.5.0a3.tar", max compression
+gzip compressed data, was "enhancedocs-0.5.0a4.tar", max compression
```

## Comparing `enhancedocs-0.5.0a3.tar` & `enhancedocs-0.5.0a4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-03-27 07:32:26.636816 enhancedocs-0.5.0a3/LICENSE
--rw-r--r--   0        0        0      847 2023-04-27 12:22:55.344998 enhancedocs-0.5.0a3/README.md
--rw-r--r--   0        0        0        0 2023-04-27 10:19:37.805831 enhancedocs-0.5.0a3/enhancedocs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 09:59:17.547934 enhancedocs-0.5.0a3/enhancedocs/commands/__init__.py
--rw-r--r--   0        0        0      787 2023-04-27 10:19:37.800385 enhancedocs-0.5.0a3/enhancedocs/commands/ask.py
--rw-r--r--   0        0        0      928 2023-04-27 10:21:38.943135 enhancedocs-0.5.0a3/enhancedocs/commands/build.py
--rw-r--r--   0        0        0      986 2023-04-27 10:20:31.857527 enhancedocs-0.5.0a3/enhancedocs/commands/push.py
--rw-r--r--   0        0        0      399 2023-04-27 10:28:48.381221 enhancedocs-0.5.0a3/enhancedocs/config.py
--rw-r--r--   0        0        0      446 2023-04-27 10:28:48.384720 enhancedocs-0.5.0a3/enhancedocs/main.py
--rw-r--r--   0        0        0      311 2023-04-27 10:06:38.828657 enhancedocs-0.5.0a3/enhancedocs/utils.py
--rw-r--r--   0        0        0      432 2023-04-27 12:22:38.560003 enhancedocs-0.5.0a3/pyproject.toml
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 enhancedocs-0.5.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/LICENSE
+-rw-r--r--   0        0        0      846 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/commands/__init__.py
+-rw-r--r--   0        0        0      787 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/commands/ask.py
+-rw-r--r--   0        0        0      928 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/commands/build.py
+-rw-r--r--   0        0        0      986 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/commands/push.py
+-rw-r--r--   0        0        0      399 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/config.py
+-rw-r--r--   0        0        0      446 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/main.py
+-rw-r--r--   0        0        0      311 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/enhancedocs/utils.py
+-rw-r--r--   0        0        0      432 2023-04-27 13:08:29.556229 enhancedocs-0.5.0a4/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 enhancedocs-0.5.0a4/PKG-INFO
```

### Comparing `enhancedocs-0.5.0a3/LICENSE` & `enhancedocs-0.5.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a3/README.md` & `enhancedocs-0.5.0a4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # EnhanceDocs CLI
 
 EnhanceDocs Command Line Interface (CLI)
 
 [![pypi version](https://img.shields.io/pypi/v/enhancedocs.svg)](https://pypi.org/pypi/enhancedocs/)
-[![Downloads](https://img.shields.io/pypi/dm/enhancedocs.svg)](https://pypi.org/project/enhancedocs/)
+[![Downloads](https://static.pepy.tech/badge/enhancedocs/month)](https://pypi.org/pypi/enhancedocs/)
 [![License: MIT](https://img.shields.io/badge/license-Apache--2.0-yellow)](https://www.apache.org/licenses/LICENSE-2.0)
  [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/enhancedocs.svg?style=social&label=Follow%20%40EnhanceDocs)](https://twitter.com/enhancedocs)
 [![](https://dcbadge.vercel.app/api/server/AUDa3KZavw?compact=true&style=flat)](https://discord.gg/AUDa3KZavw)
 
 ## Requirements
 - [Python 3.11.2](https://www.python.org/downloads/)
```

### Comparing `enhancedocs-0.5.0a3/enhancedocs/commands/ask.py` & `enhancedocs-0.5.0a4/enhancedocs/commands/ask.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a3/enhancedocs/commands/build.py` & `enhancedocs-0.5.0a4/enhancedocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a3/enhancedocs/commands/push.py` & `enhancedocs-0.5.0a4/enhancedocs/commands/push.py`

 * *Files identical despite different names*

### Comparing `enhancedocs-0.5.0a3/PKG-INFO` & `enhancedocs-0.5.0a4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhancedocs
-Version: 0.5.0a3
+Version: 0.5.0a4
 Summary: EnhanceDocs Command Line Interface (CLI)
 License: Apache-2.0
 Author: Alvaro Molina
 Author-email: alw3ys@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 
 # EnhanceDocs CLI
 
 EnhanceDocs Command Line Interface (CLI)
 
 [![pypi version](https://img.shields.io/pypi/v/enhancedocs.svg)](https://pypi.org/pypi/enhancedocs/)
-[![Downloads](https://img.shields.io/pypi/dm/enhancedocs.svg)](https://pypi.org/project/enhancedocs/)
+[![Downloads](https://static.pepy.tech/badge/enhancedocs/month)](https://pypi.org/pypi/enhancedocs/)
 [![License: MIT](https://img.shields.io/badge/license-Apache--2.0-yellow)](https://www.apache.org/licenses/LICENSE-2.0)
  [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/enhancedocs.svg?style=social&label=Follow%20%40EnhanceDocs)](https://twitter.com/enhancedocs)
 [![](https://dcbadge.vercel.app/api/server/AUDa3KZavw?compact=true&style=flat)](https://discord.gg/AUDa3KZavw)
 
 ## Requirements
 - [Python 3.11.2](https://www.python.org/downloads/)
```

