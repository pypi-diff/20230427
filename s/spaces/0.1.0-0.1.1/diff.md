# Comparing `tmp/spaces-0.1.0.tar.gz` & `tmp/spaces-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.1.0.tar", max compression
+gzip compressed data, was "spaces-0.1.1.tar", max compression
```

## Comparing `spaces-0.1.0.tar` & `spaces-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0       61 2021-08-10 11:39:42.028906 spaces-0.1.0/README.md
--rw-r--r--   0        0        0      464 2021-08-10 11:43:34.845731 spaces-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-08-10 11:40:31.077526 spaces-0.1.0/spaces/__init__.py
--rw-r--r--   0        0        0      616 2021-08-10 11:43:40.034202 spaces-0.1.0/setup.py
--rw-r--r--   0        0        0      573 2021-08-10 11:43:40.034352 spaces-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-04-27 15:34:16.931108 spaces-0.1.1/README.md
+-rw-r--r--   0        0        0      482 2023-04-27 15:42:40.879626 spaces-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-27 15:40:38.868471 spaces-0.1.1/spaces/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-27 15:40:23.864577 spaces-0.1.1/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0      539 2023-04-27 15:36:02.266379 spaces-0.1.1/spaces/gpu/client.py
+-rw-r--r--   0        0        0     5396 2023-04-27 15:36:02.266379 spaces-0.1.1/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     1183 2023-04-27 15:39:25.436982 spaces-0.1.1/spaces/gpu/patching.py
+-rw-r--r--   0        0        0      312 2023-04-27 15:34:16.931108 spaces-0.1.1/spaces/utils.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 spaces-0.1.1/PKG-INFO
```

### Comparing `spaces-0.1.0/PKG-INFO` & `spaces-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Project-URL: Repository, https://github.com/huggingface/huggingface_hub
 Description-Content-Type: text/markdown
 
 # Hugging Face Spaces
 
 ## Installation
```

