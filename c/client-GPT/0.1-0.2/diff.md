# Comparing `tmp/client_GPT-0.1.tar.gz` & `tmp/client_GPT-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-0.1.tar", last modified: Mon Apr 24 12:20:30 2023, max compression
+gzip compressed data, was "client_GPT-0.2.tar", last modified: Thu Apr 27 08:34:22 2023, max compression
```

## Comparing `client_GPT-0.1.tar` & `client_GPT-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:20:30.913521 client_GPT-0.1/
--rw-rw-rw-   0        0        0      359 2023-04-24 12:20:30.912522 client_GPT-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-24 09:17:30.000000 client_GPT-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 12:20:30.910522 client_GPT-0.1/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      359 2023-04-24 12:20:30.000000 client_GPT-0.1/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-24 12:20:30.000000 client_GPT-0.1/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:20:30.000000 client_GPT-0.1/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 12:20:30.000000 client_GPT-0.1/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:20:30.000000 client_GPT-0.1/client_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 12:20:30.913521 client_GPT-0.1/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-04-24 12:20:22.000000 client_GPT-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:34:22.018267 client_GPT-0.2/
+-rw-rw-rw-   0        0        0      417 2023-04-27 08:34:22.018267 client_GPT-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-04-24 09:17:30.000000 client_GPT-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 08:34:22.016270 client_GPT-0.2/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 08:34:21.000000 client_GPT-0.2/client_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 08:34:22.019269 client_GPT-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      589 2023-04-27 08:32:59.000000 client_GPT-0.2/setup.py
```

### Comparing `client_GPT-0.1/setup.py` & `client_GPT-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="0.1",
+    version="0.2",
     author="littleknitsstory",
+    description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python :: 3",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
 )
```

