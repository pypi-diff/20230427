# Comparing `tmp/datatable-faker-0.1.3.tar.gz` & `tmp/datatable-faker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable-faker-0.1.3.tar", last modified: Wed Apr 26 05:09:09 2023, max compression
+gzip compressed data, was "datatable-faker-0.1.4.tar", last modified: Thu Apr 27 07:03:16 2023, max compression
```

## Comparing `datatable-faker-0.1.3.tar` & `datatable-faker-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/
--rw-rw-r--   0 root         (0) root         (0)     1070 2023-04-25 12:48:19.000000 datatable-faker-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1751 2023-04-26 05:06:25.000000 datatable-faker-0.1.3/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      982 2023-04-26 05:07:45.000000 datatable-faker-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/src/datatable_faker/
--rw-rw-r--   0 root         (0) root         (0)     1819 2023-04-26 05:06:16.000000 datatable-faker-0.1.3/src/datatable_faker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1410 2023-04-26 05:03:55.000000 datatable-faker-0.1.3/src/datatable_faker/check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:09:09.257793 datatable-faker-0.1.3/src/datatable_faker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      302 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-26 05:09:09.000000 datatable-faker-0.1.3/src/datatable_faker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/
+-rw-rw-r--   0 root         (0) root         (0)     1070 2023-04-25 12:48:19.000000 datatable-faker-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1751 2023-04-26 05:06:25.000000 datatable-faker-0.1.4/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      982 2023-04-27 07:01:46.000000 datatable-faker-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/src/datatable_faker/
+-rw-rw-r--   0 root         (0) root         (0)     4964 2023-04-27 06:59:33.000000 datatable-faker-0.1.4/src/datatable_faker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-04-26 05:03:55.000000 datatable-faker-0.1.4/src/datatable_faker/check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:03:16.235128 datatable-faker-0.1.4/src/datatable_faker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      302 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 07:03:16.000000 datatable-faker-0.1.4/src/datatable_faker.egg-info/top_level.txt
```

### Comparing `datatable-faker-0.1.3/LICENSE` & `datatable-faker-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.3/PKG-INFO` & `datatable-faker-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `datatable-faker-0.1.3/README.rst` & `datatable-faker-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.3/setup.py` & `datatable-faker-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="datatable-faker",
     author="Prince Roshan",
-    version='0.1.3',
+    version='0.1.4',
     author_email="princekrroshan01@gmail.com",
     url="https://github.com/Agent-Hellboy/datatable-faker",
     description="Library to generate fake datatable for unittest ",
     long_description=read("README.rst"),
     license="MIT",
     package_dir={'': 'src'},
     packages=['datatable_faker'],
```

### Comparing `datatable-faker-0.1.3/src/datatable_faker/check.py` & `datatable-faker-0.1.4/src/datatable_faker/check.py`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.3/src/datatable_faker.egg-info/PKG-INFO` & `datatable-faker-0.1.4/src/datatable_faker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
```

