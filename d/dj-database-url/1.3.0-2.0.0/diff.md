# Comparing `tmp/dj-database-url-1.3.0.tar.gz` & `tmp/dj-database-url-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-database-url-1.3.0.tar", last modified: Mon Mar 27 20:56:35 2023, max compression
+gzip compressed data, was "dj-database-url-2.0.0.tar", last modified: Thu Apr 27 15:31:20 2023, max compression
```

## Comparing `dj-database-url-1.3.0.tar` & `dj-database-url-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:56:35.978649 dj-database-url-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-27 20:56:26.000000 dj-database-url-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 20:56:26.000000 dj-database-url-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-03-27 20:56:35.978649 dj-database-url-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-03-27 20:56:26.000000 dj-database-url-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:56:35.978649 dj-database-url-1.3.0/dj_database_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-03-27 20:56:35.000000 dj-database-url-1.3.0/dj_database_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-27 20:56:35.000000 dj-database-url-1.3.0/dj_database_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:56:35.000000 dj-database-url-1.3.0/dj_database_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:56:35.000000 dj-database-url-1.3.0/dj_database_url.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 20:56:35.000000 dj-database-url-1.3.0/dj_database_url.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 20:56:35.000000 dj-database-url-1.3.0/dj_database_url.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-27 20:56:26.000000 dj-database-url-1.3.0/dj_database_url.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:56:26.000000 dj-database-url-1.3.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-27 20:56:26.000000 dj-database-url-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:56:35.978649 dj-database-url-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-27 20:56:26.000000 dj-database-url-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/dj_database_url/
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/dj_database_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/dj_database_url/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/dj_database_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 15:31:20.000000 dj-database-url-2.0.0/dj_database_url.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:31:20.092095 dj-database-url-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-04-27 15:31:00.000000 dj-database-url-2.0.0/tests/test_dj_database_url.py
```

### Comparing `dj-database-url-1.3.0/LICENSE` & `dj-database-url-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-database-url-1.3.0/PKG-INFO` & `dj-database-url-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dj-database-url
-Version: 1.3.0
+Version: 2.0.0
 Summary: Use Database URLs in your Django Application.
 Home-page: https://github.com/jazzband/dj-database-url
 Author: Original Author: Kenneth Reitz, Maintained by: JazzBand Community
 License: BSD
+Project-URL: GitHub, https://github.com/jazzband/dj-database-url/
+Project-URL: Release log, https://github.com/jazzband/dj-database-url/blob/master/CHANGELOG.md
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
```

### Comparing `dj-database-url-1.3.0/README.rst` & `dj-database-url-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `dj-database-url-1.3.0/dj_database_url.egg-info/PKG-INFO` & `dj-database-url-2.0.0/dj_database_url.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dj-database-url
-Version: 1.3.0
+Version: 2.0.0
 Summary: Use Database URLs in your Django Application.
 Home-page: https://github.com/jazzband/dj-database-url
 Author: Original Author: Kenneth Reitz, Maintained by: JazzBand Community
 License: BSD
+Project-URL: GitHub, https://github.com/jazzband/dj-database-url/
+Project-URL: Release log, https://github.com/jazzband/dj-database-url/blob/master/CHANGELOG.md
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
```

### Comparing `dj-database-url-1.3.0/dj_database_url.py` & `dj-database-url-2.0.0/dj_database_url/__init__.py`

 * *Files identical despite different names*

### Comparing `dj-database-url-1.3.0/setup.py` & `dj-database-url-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from setuptools import setup
 
 readme = Path("README.rst").read_text()
 
 setup(
     name="dj-database-url",
-    version="1.3.0",
+    version="2.0.0",
     url="https://github.com/jazzband/dj-database-url",
     license="BSD",
     author="Original Author: Kenneth Reitz, Maintained by: JazzBand Community",
     description="Use Database URLs in your Django Application.",
     long_description=readme,
     long_description_content_type="text/x-rst",
-    py_modules=["dj_database_url"],
+    packages=["dj_database_url"],
     install_requires=["Django>=3.2", "typing_extensions >= 3.10.0.0"],
-    zip_safe=False,
     include_package_data=True,
+    package_data={
+        "dj_database_url": ["py.typed"],
+    },
     platforms="any",
-    project_links={
+    project_urls={
         "GitHub": "https://github.com/jazzband/dj-database-url/",
         "Release log": (
             "https://github.com/jazzband/dj-database-url/blob/master/CHANGELOG.md"
         ),
     },
     classifiers=[
         "Environment :: Web Environment",
```

