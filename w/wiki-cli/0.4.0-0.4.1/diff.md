# Comparing `tmp/wiki_cli-0.4.0.tar.gz` & `tmp/wiki_cli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiki_cli-0.4.0.tar", max compression
+gzip compressed data, was "wiki_cli-0.4.1.tar", max compression
```

## Comparing `wiki_cli-0.4.0.tar` & `wiki_cli-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1052 2020-12-08 11:50:47.618642 wiki_cli-0.4.0/LICENSE
--rw-r--r--   0        0        0      652 2021-08-16 10:39:37.883647 wiki_cli-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-05-27 16:29:58.657819 wiki_cli-0.4.0/wiki_cli/__init__.py
--rw-r--r--   0        0        0     2129 2021-05-27 17:37:43.446662 wiki_cli-0.4.0/wiki_cli/formatter.py
--rw-r--r--   0        0        0     1357 2021-05-27 17:26:50.035156 wiki_cli-0.4.0/wiki_cli/models.py
--rwxr-xr-x   0        0        0     9022 2021-08-16 10:35:00.421746 wiki_cli-0.4.0/wiki_cli/wiki.py
--rw-r--r--   0        0        0      909 2021-08-16 10:41:26.652236 wiki_cli-0.4.0/setup.py
--rw-r--r--   0        0        0      717 2021-08-16 10:41:26.652515 wiki_cli-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2020-12-08 11:50:47.618642 wiki_cli-0.4.1/LICENSE
+-rw-r--r--   0        0        0      652 2023-04-27 07:26:50.099817 wiki_cli-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-05-27 16:29:58.657819 wiki_cli-0.4.1/wiki_cli/__init__.py
+-rw-r--r--   0        0        0     2129 2021-05-27 17:37:43.446662 wiki_cli-0.4.1/wiki_cli/formatter.py
+-rw-r--r--   0        0        0     1357 2021-05-27 17:26:50.035156 wiki_cli-0.4.1/wiki_cli/models.py
+-rwxr-xr-x   0        0        0     9022 2021-08-16 10:35:00.421746 wiki_cli-0.4.1/wiki_cli/wiki.py
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 wiki_cli-0.4.1/PKG-INFO
```

### Comparing `wiki_cli-0.4.0/LICENSE` & `wiki_cli-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wiki_cli-0.4.0/pyproject.toml` & `wiki_cli-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wiki_cli"
-version = "0.4.0"
+version = "0.4.1"
 description = "Command Line Client for quick lookups on Wikipedia."
 authors = ["sedrubal <dev@sedrubal.de>"]
 repository = "https://gitlab.com/sedrubal/wiki-cli.git"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `wiki_cli-0.4.0/wiki_cli/formatter.py` & `wiki_cli-0.4.1/wiki_cli/formatter.py`

 * *Files identical despite different names*

### Comparing `wiki_cli-0.4.0/wiki_cli/models.py` & `wiki_cli-0.4.1/wiki_cli/models.py`

 * *Files identical despite different names*

### Comparing `wiki_cli-0.4.0/wiki_cli/wiki.py` & `wiki_cli-0.4.1/wiki_cli/wiki.py`

 * *Files identical despite different names*

