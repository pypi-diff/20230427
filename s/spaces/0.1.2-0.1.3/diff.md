# Comparing `tmp/spaces-0.1.2.tar.gz` & `tmp/spaces-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.1.2.tar", max compression
+gzip compressed data, was "spaces-0.1.3.tar", max compression
```

## Comparing `spaces-0.1.2.tar` & `spaces-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       61 2023-04-27 15:34:16.931108 spaces-0.1.2/README.md
--rw-r--r--   0        0        0      532 2023-04-27 15:53:52.142978 spaces-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-27 15:40:38.868471 spaces-0.1.2/spaces/__init__.py
--rw-r--r--   0        0        0      103 2023-04-27 15:40:23.864577 spaces-0.1.2/spaces/gpu/__init__.py
--rw-r--r--   0        0        0      539 2023-04-27 15:36:02.266379 spaces-0.1.2/spaces/gpu/client.py
--rw-r--r--   0        0        0     5396 2023-04-27 15:36:02.266379 spaces-0.1.2/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     1183 2023-04-27 15:39:25.436982 spaces-0.1.2/spaces/gpu/patching.py
--rw-r--r--   0        0        0      312 2023-04-27 15:34:16.931108 spaces-0.1.2/spaces/utils.py
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 spaces-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-04-27 15:34:16.931108 spaces-0.1.3/README.md
+-rw-r--r--   0        0        0      532 2023-04-27 16:28:17.320678 spaces-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-27 15:40:38.868471 spaces-0.1.3/spaces/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-27 15:40:23.864577 spaces-0.1.3/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0      612 2023-04-27 16:27:32.868982 spaces-0.1.3/spaces/gpu/client.py
+-rw-r--r--   0        0        0     5396 2023-04-27 15:36:02.266379 spaces-0.1.3/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     1183 2023-04-27 15:39:25.436982 spaces-0.1.3/spaces/gpu/patching.py
+-rw-r--r--   0        0        0      362 2023-04-27 16:25:15.393923 spaces-0.1.3/spaces/utils.py
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 spaces-0.1.3/PKG-INFO
```

### Comparing `spaces-0.1.2/pyproject.toml` & `spaces-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.1.2"
+version = "0.1.3"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
```

### Comparing `spaces-0.1.2/spaces/gpu/decorator.py` & `spaces-0.1.3/spaces/gpu/decorator.py`

 * *Files identical despite different names*

### Comparing `spaces-0.1.2/spaces/gpu/patching.py` & `spaces-0.1.3/spaces/gpu/patching.py`

 * *Files identical despite different names*

### Comparing `spaces-0.1.2/PKG-INFO` & `spaces-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

