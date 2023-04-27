# Comparing `tmp/boston-1.0.1.tar.gz` & `tmp/boston-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boston-1.0.1.tar", last modified: Thu Apr 27 15:25:18 2023, max compression
+gzip compressed data, was "boston-1.0.2.tar", last modified: Thu Apr 27 15:31:01 2023, max compression
```

## Comparing `boston-1.0.1.tar` & `boston-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:25:18.186164 boston-1.0.1/
--rw-rw-rw-   0        0        0      451 2023-04-27 15:25:18.184164 boston-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 15:25:18.162205 boston-1.0.1/boston/
--rw-rw-rw-   0        0        0       19 2023-04-27 15:24:12.000000 boston-1.0.1/boston/__init__.py
--rw-rw-rw-   0        0        0      338 2023-04-27 15:13:35.000000 boston-1.0.1/boston/boston.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:25:18.181163 boston-1.0.1/boston.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-27 15:25:17.000000 boston-1.0.1/boston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-27 15:25:18.000000 boston-1.0.1/boston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:25:17.000000 boston-1.0.1/boston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 15:25:17.000000 boston-1.0.1/boston.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 15:25:17.000000 boston-1.0.1/boston.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:25:18.186164 boston-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-04-27 15:24:16.000000 boston-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:31:01.372792 boston-1.0.2/
+-rw-rw-rw-   0        0        0      451 2023-04-27 15:31:01.371797 boston-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 15:31:01.335787 boston-1.0.2/boston/
+-rw-rw-rw-   0        0        0      338 2023-04-27 15:30:45.000000 boston-1.0.2/boston/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-04-27 15:13:35.000000 boston-1.0.2/boston/boston.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:31:01.368786 boston-1.0.2/boston.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-04-27 15:31:01.000000 boston-1.0.2/boston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 15:31:00.000000 boston-1.0.2/boston.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 15:31:01.373787 boston-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-04-27 15:30:48.000000 boston-1.0.2/setup.py
```

### Comparing `boston-1.0.1/setup.py` & `boston-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="boston", # Replace with your own username
-    version="1.0.1",
+    version="1.0.2",
     author="julmubm",
     author_email="dltpdn@gmail.com",
     description="loading boston housing price dataset like sklearn.datasets.load_boston() style.",
     long_description_content_type="text/markdown",
     url="https://github.com/dltpdn/boston",
     install_requires=['pandas'],
     packages=setuptools.find_packages(),
```

