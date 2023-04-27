# Comparing `tmp/client_GPT-0.2.tar.gz` & `tmp/client_GPT-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-0.2.tar", last modified: Thu Apr 27 08:34:22 2023, max compression
+gzip compressed data, was "client_GPT-0.2.1.tar", last modified: Thu Apr 27 09:24:40 2023, max compression
```

## Comparing `client_GPT-0.2.tar` & `client_GPT-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 08:34:22.018267 client_GPT-0.2/
--rw-rw-rw-   0        0        0      417 2023-04-27 08:34:22.018267 client_GPT-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-24 09:17:30.000000 client_GPT-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 08:34:22.016270 client_GPT-0.2/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      417 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 08:34:22.019269 client_GPT-0.2/setup.cfg
--rw-rw-rw-   0        0        0      589 2023-04-27 08:32:59.000000 client_GPT-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:24:40.480283 client_GPT-0.2.1/
+-rw-rw-rw-   0        0        0      419 2023-04-27 09:24:40.479285 client_GPT-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-04-24 09:17:30.000000 client_GPT-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 09:24:40.478282 client_GPT-0.2.1/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-27 09:24:40.000000 client_GPT-0.2.1/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-27 09:24:40.000000 client_GPT-0.2.1/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 09:24:40.000000 client_GPT-0.2.1/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 09:24:40.000000 client_GPT-0.2.1/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 09:24:40.000000 client_GPT-0.2.1/client_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 09:24:40.480283 client_GPT-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-04-27 09:22:18.000000 client_GPT-0.2.1/setup.py
```

### Comparing `client_GPT-0.2/setup.py` & `client_GPT-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="0.2",
+    version="0.2.1",
     author="littleknitsstory",
     description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
```

