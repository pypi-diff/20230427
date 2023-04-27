# Comparing `tmp/pollstats-0.1.tar.gz` & `tmp/pollstats-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pollstats-0.1.tar", last modified: Thu Apr 27 09:54:14 2023, max compression
+gzip compressed data, was "dist\pollstats-0.2.tar", last modified: Thu Apr 27 10:58:33 2023, max compression
```

## Comparing `pollstats-0.1.tar` & `pollstats-0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 09:54:14.000000 pollstats-0.1/
--rw-rw-rw-   0        0        0     1055 2023-04-27 09:13:20.000000 pollstats-0.1/LICENSE
--rw-rw-rw-   0        0        0     2887 2023-04-27 09:54:14.000000 pollstats-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2168 2023-04-27 09:12:09.000000 pollstats-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 09:54:14.000000 pollstats-0.1/pollstats/
--rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.1/pollstats/__init__.py
--rw-rw-rw-   0        0        0       66 2023-04-27 05:45:06.000000 pollstats-0.1/pollstats/admin.py
--rw-rw-rw-   0        0        0      156 2023-04-27 05:45:06.000000 pollstats-0.1/pollstats/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-27 09:54:14.000000 pollstats-0.1/pollstats/migrations/
--rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.1/pollstats/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-04-27 05:45:06.000000 pollstats-0.1/pollstats/models.py
--rw-rw-rw-   0        0        0       63 2023-04-27 05:45:06.000000 pollstats-0.1/pollstats/tests.py
--rw-rw-rw-   0        0        0      135 2023-04-27 06:34:19.000000 pollstats-0.1/pollstats/urls.py
--rw-rw-rw-   0        0        0      262 2023-04-27 06:52:06.000000 pollstats-0.1/pollstats/views.py
-drwxrwxrwx   0        0        0        0 2023-04-27 09:54:14.000000 pollstats-0.1/pollstats.egg-info/
--rw-rw-rw-   0        0        0     2887 2023-04-27 09:54:14.000000 pollstats-0.1/pollstats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-04-27 09:54:14.000000 pollstats-0.1/pollstats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 09:54:14.000000 pollstats-0.1/pollstats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 09:54:14.000000 pollstats-0.1/pollstats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      546 2023-04-27 09:52:29.000000 pollstats-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 09:54:14.000000 pollstats-0.1/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-04-27 09:50:26.000000 pollstats-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:58:33.000000 pollstats-0.2/
+-rw-rw-rw-   0        0        0     1055 2023-04-27 09:13:20.000000 pollstats-0.2/LICENSE
+-rw-rw-rw-   0        0        0      105 2023-04-27 10:49:49.000000 pollstats-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2887 2023-04-27 10:58:33.000000 pollstats-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2168 2023-04-27 09:12:09.000000 pollstats-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 10:58:33.000000 pollstats-0.2/pollstats/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.2/pollstats/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 05:45:06.000000 pollstats-0.2/pollstats/admin.py
+-rw-rw-rw-   0        0        0      156 2023-04-27 05:45:06.000000 pollstats-0.2/pollstats/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:58:33.000000 pollstats-0.2/pollstats/migrations/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.2/pollstats/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-04-27 05:45:06.000000 pollstats-0.2/pollstats/models.py
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:45:06.000000 pollstats-0.2/pollstats/tests.py
+-rw-rw-rw-   0        0        0      135 2023-04-27 06:34:19.000000 pollstats-0.2/pollstats/urls.py
+-rw-rw-rw-   0        0        0      262 2023-04-27 06:52:06.000000 pollstats-0.2/pollstats/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:58:33.000000 pollstats-0.2/pollstats.egg-info/
+-rw-rw-rw-   0        0        0     2887 2023-04-27 10:58:33.000000 pollstats-0.2/pollstats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-27 10:58:33.000000 pollstats-0.2/pollstats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:58:33.000000 pollstats-0.2/pollstats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 10:58:33.000000 pollstats-0.2/pollstats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      546 2023-04-27 09:52:29.000000 pollstats-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:58:33.000000 pollstats-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-04-27 10:58:01.000000 pollstats-0.2/setup.py
```

### Comparing `pollstats-0.1/LICENSE` & `pollstats-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pollstats-0.1/PKG-INFO` & `pollstats-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollstats
-Version: 0.1
+Version: 0.2
 Summary: A short description of your package
 Home-page: https://github.com/Vijayanand-debug/pollstats
 Author: Vijayanand
 Author-email: vijayanand563@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pollstats-0.1/README.md` & `pollstats-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pollstats-0.1/pollstats.egg-info/PKG-INFO` & `pollstats-0.2/pollstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollstats
-Version: 0.1
+Version: 0.2
 Summary: A short description of your package
 Home-page: https://github.com/Vijayanand-debug/pollstats
 Author: Vijayanand
 Author-email: vijayanand563@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pollstats-0.1/pyproject.toml` & `pollstats-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pollstats-0.1/setup.py` & `pollstats-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pollstats",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     install_requires=[
         # List your package's dependencies here
     ],
     author="Vijayanand",
     author_email="vijayanand563@gmail.com",
     description="A short description of your package",
```

