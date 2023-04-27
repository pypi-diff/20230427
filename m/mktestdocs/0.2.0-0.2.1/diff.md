# Comparing `tmp/mktestdocs-0.2.0.tar.gz` & `tmp/mktestdocs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktestdocs-0.2.0.tar", last modified: Thu May 26 16:51:08 2022, max compression
+gzip compressed data, was "mktestdocs-0.2.1.tar", last modified: Thu Apr 27 06:01:47 2023, max compression
```

## Comparing `mktestdocs-0.2.0.tar` & `mktestdocs-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-05-26 16:51:08.134235 mktestdocs-0.2.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      159 2022-05-26 16:51:08.134235 mktestdocs-0.2.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4697 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-05-26 16:51:08.130235 mktestdocs-0.2.0/mktestdocs/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      371 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/mktestdocs/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4508 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/mktestdocs/__main__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-05-26 16:51:08.134235 mktestdocs-0.2.0/mktestdocs.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      159 2022-05-26 16:51:07.000000 mktestdocs-0.2.0/mktestdocs.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      401 2022-05-26 16:51:08.000000 mktestdocs-0.2.0/mktestdocs.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-05-26 16:51:07.000000 mktestdocs-0.2.0/mktestdocs.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2022-05-26 16:51:07.000000 mktestdocs-0.2.0/mktestdocs.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2022-05-26 16:51:07.000000 mktestdocs-0.2.0/mktestdocs.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2022-05-26 16:51:08.134235 mktestdocs-0.2.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      307 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-05-26 16:51:08.134235 mktestdocs-0.2.0/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      214 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/tests/conftest.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      940 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/tests/test_actual_docstrings.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/tests/test_class.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      903 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/tests/test_codeblock.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2656 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/tests/test_markdown.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      235 2022-05-26 16:46:26.000000 mktestdocs-0.2.0/tests/test_mktestdocs.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 06:01:47.245277 mktestdocs-0.2.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       97 2023-04-27 06:01:47.245277 mktestdocs-0.2.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4759 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 06:01:47.237277 mktestdocs-0.2.1/mktestdocs/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      371 2023-04-27 06:01:16.000000 mktestdocs-0.2.1/mktestdocs/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4508 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/mktestdocs/__main__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 06:01:47.241277 mktestdocs-0.2.1/mktestdocs.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       97 2023-04-27 06:01:47.000000 mktestdocs-0.2.1/mktestdocs.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      365 2023-04-27 06:01:47.000000 mktestdocs-0.2.1/mktestdocs.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-27 06:01:47.000000 mktestdocs-0.2.1/mktestdocs.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-04-27 06:01:47.000000 mktestdocs-0.2.1/mktestdocs.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-04-27 06:01:47.000000 mktestdocs-0.2.1/mktestdocs.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-27 06:01:47.245277 mktestdocs-0.2.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      303 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 06:01:47.245277 mktestdocs-0.2.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      940 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/tests/test_actual_docstrings.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/tests/test_class.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      903 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/tests/test_codeblock.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2656 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/tests/test_markdown.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      235 2023-04-27 05:59:46.000000 mktestdocs-0.2.1/tests/test_mktestdocs.py
```

### Comparing `mktestdocs-0.2.0/LICENSE` & `mktestdocs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mktestdocs-0.2.0/README.md` & `mktestdocs-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 
 ```
 pip install mktestdocs
 ```
 
 ## Usage 
 
-Let's say that you're using [mkdocs](https://squidfunk.github.io/mkdocs-material/getting-started/) for your documentation. Then you're 
-writing down markdown to explain how your python packages works. It'd be 
-great if you could run your unit tests against them. You can use this package
-to write unit-tests for that. 
+Let's say that you're using [mkdocs](https://squidfunk.github.io/mkdocs-material/getting-started/) 
+for your documentation. Then you're writing down markdown to explain how your Python packages work. 
+It'd be a shame if a codeblock had an error in it, so it'd be 
+great if you could run your unit tests against them. 
+
+This package allows you to do _just that_. Here's an example:
 
 ```python
 import pathlib
 import pytest
 
 from mktestdocs import check_md_file
```

### Comparing `mktestdocs-0.2.0/mktestdocs/__main__.py` & `mktestdocs-0.2.1/mktestdocs/__main__.py`

 * *Files identical despite different names*

### Comparing `mktestdocs-0.2.0/tests/test_actual_docstrings.py` & `mktestdocs-0.2.1/tests/test_actual_docstrings.py`

 * *Files identical despite different names*

### Comparing `mktestdocs-0.2.0/tests/test_class.py` & `mktestdocs-0.2.1/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `mktestdocs-0.2.0/tests/test_codeblock.py` & `mktestdocs-0.2.1/tests/test_codeblock.py`

 * *Files identical despite different names*

### Comparing `mktestdocs-0.2.0/tests/test_markdown.py` & `mktestdocs-0.2.1/tests/test_markdown.py`

 * *Files identical despite different names*

