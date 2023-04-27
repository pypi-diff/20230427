# Comparing `tmp/vijsamplepackage-0.0.2.tar.gz` & `tmp/vijsamplepackage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vijsamplepackage-0.0.2.tar", last modified: Wed Apr 26 09:39:04 2023, max compression
+gzip compressed data, was "vijsamplepackage-0.0.3.tar", last modified: Thu Apr 27 09:25:02 2023, max compression
```

## Comparing `vijsamplepackage-0.0.2.tar` & `vijsamplepackage-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 09:39:04.498401 vijsamplepackage-0.0.2/
--rw-rw-rw-   0        0        0      584 2023-04-26 09:39:04.498401 vijsamplepackage-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-26 09:39:04.498401 vijsamplepackage-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-04-26 09:37:05.000000 vijsamplepackage-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:39:04.491135 vijsamplepackage-0.0.2/vijsamplepackage/
--rw-rw-rw-   0        0        0      180 2023-04-25 07:28:56.000000 vijsamplepackage-0.0.2/vijsamplepackage/__init__.py
--rw-rw-rw-   0        0        0      983 2023-04-25 05:39:12.000000 vijsamplepackage-0.0.2/vijsamplepackage/functions.py
--rw-rw-rw-   0        0        0      318 2023-04-25 07:31:43.000000 vijsamplepackage-0.0.2/vijsamplepackage/greet.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:39:04.496369 vijsamplepackage-0.0.2/vijsamplepackage.egg-info/
--rw-rw-rw-   0        0        0      584 2023-04-26 09:39:04.000000 vijsamplepackage-0.0.2/vijsamplepackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-26 09:39:04.000000 vijsamplepackage-0.0.2/vijsamplepackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 09:39:04.000000 vijsamplepackage-0.0.2/vijsamplepackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-26 09:39:04.000000 vijsamplepackage-0.0.2/vijsamplepackage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 09:25:02.695970 vijsamplepackage-0.0.3/
+-rw-rw-rw-   0        0        0      584 2023-04-27 09:25:02.695970 vijsamplepackage-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-27 09:25:02.695970 vijsamplepackage-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2023-04-27 09:22:45.000000 vijsamplepackage-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:25:02.687777 vijsamplepackage-0.0.3/vijsamplepackage/
+-rw-rw-rw-   0        0        0      180 2023-04-25 07:28:56.000000 vijsamplepackage-0.0.3/vijsamplepackage/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-04-25 05:39:12.000000 vijsamplepackage-0.0.3/vijsamplepackage/functions.py
+-rw-rw-rw-   0        0        0      318 2023-04-26 09:50:23.000000 vijsamplepackage-0.0.3/vijsamplepackage/greet.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:25:02.695970 vijsamplepackage-0.0.3/vijsamplepackage.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-04-27 09:25:02.000000 vijsamplepackage-0.0.3/vijsamplepackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-27 09:25:02.000000 vijsamplepackage-0.0.3/vijsamplepackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 09:25:02.000000 vijsamplepackage-0.0.3/vijsamplepackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-27 09:25:02.000000 vijsamplepackage-0.0.3/vijsamplepackage.egg-info/top_level.txt
```

### Comparing `vijsamplepackage-0.0.2/PKG-INFO` & `vijsamplepackage-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vijsamplepackage
-Version: 0.0.2
+Version: 0.0.3
 Summary: Setting up a sample python package
 Author: Vijai Kannan
 Author-email: vijaik.nd@gmail.com
 License: UNKNOWN
 Keywords: python,sample package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vijsamplepackage-0.0.2/setup.py` & `vijsamplepackage-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'My Sample Python package'
 LONG_DESCRIPTION = 'My Sample Python package for Calculation and Display'
 
 # Setting up
 setup(
        # the name must match the folder name 'vijsamplepackage'
         name="vijsamplepackage",
```

### Comparing `vijsamplepackage-0.0.2/vijsamplepackage/functions.py` & `vijsamplepackage-0.0.3/vijsamplepackage/functions.py`

 * *Files identical despite different names*

### Comparing `vijsamplepackage-0.0.2/vijsamplepackage.egg-info/PKG-INFO` & `vijsamplepackage-0.0.3/vijsamplepackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vijsamplepackage
-Version: 0.0.2
+Version: 0.0.3
 Summary: Setting up a sample python package
 Author: Vijai Kannan
 Author-email: vijaik.nd@gmail.com
 License: UNKNOWN
 Keywords: python,sample package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

