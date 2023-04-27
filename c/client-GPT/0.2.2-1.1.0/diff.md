# Comparing `tmp/client_GPT-0.2.2.tar.gz` & `tmp/client_GPT-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-0.2.2.tar", last modified: Thu Apr 27 12:40:20 2023, max compression
+gzip compressed data, was "client_GPT-1.1.0.tar", last modified: Thu Apr 27 13:20:56 2023, max compression
```

## Comparing `client_GPT-0.2.2.tar` & `client_GPT-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:40:20.307367 client_GPT-0.2.2/
--rw-rw-rw-   0        0        0      419 2023-04-27 12:40:20.306377 client_GPT-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-24 09:17:30.000000 client_GPT-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:40:20.301364 client_GPT-0.2.2/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-27 12:40:20.000000 client_GPT-0.2.2/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-27 12:40:20.000000 client_GPT-0.2.2/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:40:20.000000 client_GPT-0.2.2/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 12:40:20.000000 client_GPT-0.2.2/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 12:40:20.000000 client_GPT-0.2.2/client_GPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 12:40:20.304384 client_GPT-0.2.2/client_gpt/
--rw-rw-rw-   0        0        0        0 2023-04-10 12:34:12.000000 client_GPT-0.2.2/client_gpt/__init__.py
--rw-rw-rw-   0        0        0     3891 2023-04-24 10:31:04.000000 client_GPT-0.2.2/client_gpt/client.py
--rw-rw-rw-   0        0        0       42 2023-04-27 12:40:20.307367 client_GPT-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-04-27 12:37:15.000000 client_GPT-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:20:56.287430 client_GPT-1.1.0/
+-rw-rw-rw-   0        0        0      419 2023-04-27 13:20:56.285429 client_GPT-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-04-24 09:17:30.000000 client_GPT-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 13:20:56.284429 client_GPT-1.1.0/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-27 13:20:56.000000 client_GPT-1.1.0/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-27 13:20:56.000000 client_GPT-1.1.0/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:20:56.000000 client_GPT-1.1.0/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 13:20:56.000000 client_GPT-1.1.0/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:20:56.000000 client_GPT-1.1.0/client_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:20:56.287430 client_GPT-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-04-27 13:20:48.000000 client_GPT-1.1.0/setup.py
```

### Comparing `client_GPT-0.2.2/setup.py` & `client_GPT-1.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="0.2.2",
+    version="1.1.0",
     author="littleknitsstory",
     description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
```

