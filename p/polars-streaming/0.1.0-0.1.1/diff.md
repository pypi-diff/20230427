# Comparing `tmp/polars-streaming-0.1.0.tar.gz` & `tmp/polars-streaming-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alchemist/Desktop/OpenSource/polars-streaming/dist/.tmp-pryrjy9h/polars-streaming-0.1.0.tar", last modified: Wed Apr 26 17:49:49 2023, max compression
+gzip compressed data, was "/home/alchemist/Desktop/OpenSource/polars-streaming/dist/.tmp-84p19d52/polars-streaming-0.1.1.tar", last modified: Thu Apr 27 13:15:25 2023, max compression
```

## Comparing `polars-streaming-0.1.0.tar` & `polars-streaming-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11357 2023-04-19 18:26:51.000000 polars-streaming-0.1.0/LICENSE
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    13597 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       50 2023-04-19 18:26:51.000000 polars-streaming-0.1.0/README.md
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/polars_streaming/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      200 2023-04-26 17:06:45.000000 polars-streaming-0.1.0/polars_streaming/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1035 2023-04-26 13:05:53.000000 polars-streaming-0.1.0/polars_streaming/core.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      436 2023-04-26 17:25:44.000000 polars-streaming-0.1.0/polars_streaming/exceptions.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2135 2023-04-26 13:31:16.000000 polars-streaming-0.1.0/polars_streaming/fileProcessor.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2820 2023-04-26 17:45:17.000000 polars-streaming-0.1.0/polars_streaming/kafkaProcessor.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1715 2023-04-26 13:32:40.000000 polars-streaming-0.1.0/polars_streaming/readwriter.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      917 2023-04-26 12:58:37.000000 polars-streaming-0.1.0/polars_streaming/utils.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/polars_streaming.egg-info/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    13597 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/polars_streaming.egg-info/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      442 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/polars_streaming.egg-info/SOURCES.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/polars_streaming.egg-info/dependency_links.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      128 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/polars_streaming.egg-info/requires.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       17 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/polars_streaming.egg-info/top_level.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1281 2023-04-26 17:41:07.000000 polars-streaming-0.1.0/pyproject.toml
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-26 17:49:49.000000 polars-streaming-0.1.0/setup.cfg
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11357 2023-04-19 18:26:51.000000 polars-streaming-0.1.1/LICENSE
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    13953 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      406 2023-04-26 18:01:15.000000 polars-streaming-0.1.1/README.md
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/polars_streaming/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      200 2023-04-27 13:14:56.000000 polars-streaming-0.1.1/polars_streaming/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1035 2023-04-26 13:05:53.000000 polars-streaming-0.1.1/polars_streaming/core.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      436 2023-04-26 17:25:44.000000 polars-streaming-0.1.1/polars_streaming/exceptions.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2135 2023-04-26 13:31:16.000000 polars-streaming-0.1.1/polars_streaming/fileProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     2820 2023-04-26 17:45:17.000000 polars-streaming-0.1.1/polars_streaming/kafkaProcessor.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1715 2023-04-26 13:32:40.000000 polars-streaming-0.1.1/polars_streaming/readwriter.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      917 2023-04-26 12:58:37.000000 polars-streaming-0.1.1/polars_streaming/utils.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/polars_streaming.egg-info/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    13953 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/polars_streaming.egg-info/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      442 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/polars_streaming.egg-info/SOURCES.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/polars_streaming.egg-info/dependency_links.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      128 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/polars_streaming.egg-info/requires.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       17 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/polars_streaming.egg-info/top_level.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1228 2023-04-27 13:14:56.000000 polars-streaming-0.1.1/pyproject.toml
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-27 13:15:25.000000 polars-streaming-0.1.1/setup.cfg
```

### Comparing `polars-streaming-0.1.0/LICENSE` & `polars-streaming-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.0/PKG-INFO` & `polars-streaming-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-streaming
-Version: 0.1.0
+Version: 0.1.1
 Summary: Stream Processing Library using Polars
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,9 +212,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 Provides-Extra: dev
 License-File: LICENSE
 
+<div align="center">
+
 # polars-streaming
-Stream Processing using Polars
+
+<div align="left">
+
+This library helps to process streaming data using Polars.
+
+## Installation
+```bash
+pip install polars-streaming
+```
+**Install from sources**
+
+Alternatively, you can also clone the latest version from the [repository](https://github.com/VinishUchiha/polars-streaming) and install it directly from the source code:
+
+```bash
+pip install -e .
+```
```

### Comparing `polars-streaming-0.1.0/polars_streaming/core.py` & `polars-streaming-0.1.1/polars_streaming/core.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.0/polars_streaming/fileProcessor.py` & `polars-streaming-0.1.1/polars_streaming/fileProcessor.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.0/polars_streaming/kafkaProcessor.py` & `polars-streaming-0.1.1/polars_streaming/kafkaProcessor.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.0/polars_streaming/readwriter.py` & `polars-streaming-0.1.1/polars_streaming/readwriter.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.0/polars_streaming/utils.py` & `polars-streaming-0.1.1/polars_streaming/utils.py`

 * *Files identical despite different names*

### Comparing `polars-streaming-0.1.0/polars_streaming.egg-info/PKG-INFO` & `polars-streaming-0.1.1/polars_streaming.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-streaming
-Version: 0.1.0
+Version: 0.1.1
 Summary: Stream Processing Library using Polars
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,9 +212,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 Provides-Extra: dev
 License-File: LICENSE
 
+<div align="center">
+
 # polars-streaming
-Stream Processing using Polars
+
+<div align="left">
+
+This library helps to process streaming data using Polars.
+
+## Installation
+```bash
+pip install polars-streaming
+```
+**Install from sources**
+
+Alternatively, you can also clone the latest version from the [repository](https://github.com/VinishUchiha/polars-streaming) and install it directly from the source code:
+
+```bash
+pip install -e .
+```
```

### Comparing `polars-streaming-0.1.0/pyproject.toml` & `polars-streaming-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polars-streaming"
-version = "0.1.0"
+version = "0.1.1"
 description = "Stream Processing Library using Polars"
 readme = "README.md"
 authors = [{ name = "Vinish M", email = "vinishuchiha@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -23,22 +23,19 @@
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 kafka = ["confluent-kafka"]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
-[tool.setuptools]
-py-modules = ["polars_streaming"]
-
 [project.urls]
 Homepage = "https://github.com/VinishUchiha/polars-streaming"
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

