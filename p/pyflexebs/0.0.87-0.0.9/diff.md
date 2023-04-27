# Comparing `tmp/pyflexebs-0.0.87.tar.gz` & `tmp/pyflexebs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflexebs-0.0.87.tar", last modified: Thu Apr 27 08:22:02 2023, max compression
+gzip compressed data, was "dist/pyflexebs-0.0.9.tar", last modified: Thu Jul  9 07:36:23 2020, max compression
```

## Comparing `pyflexebs-0.0.87.tar` & `pyflexebs-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:22:02.462866 pyflexebs-0.0.87/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:21:52.000000 pyflexebs-0.0.87/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-04-27 08:22:02.462866 pyflexebs-0.0.87/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      397 2023-04-27 08:21:52.000000 pyflexebs-0.0.87/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:22:02.461866 pyflexebs-0.0.87/pyflexebs/
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2020-07-28 01:37:33.000000 pyflexebs-0.0.87/pyflexebs/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3037 2020-11-16 17:47:31.000000 pyflexebs-0.0.87/pyflexebs/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    12510 2023-04-27 08:21:35.000000 pyflexebs-0.0.87/pyflexebs/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      228 2023-04-27 08:21:52.000000 pyflexebs-0.0.87/pyflexebs/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1965 2021-09-17 18:50:12.000000 pyflexebs-0.0.87/pyflexebs/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:22:02.461866 pyflexebs-0.0.87/pyflexebs.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-04-27 08:22:02.000000 pyflexebs-0.0.87/pyflexebs.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      337 2023-04-27 08:22:02.000000 pyflexebs-0.0.87/pyflexebs.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:22:02.000000 pyflexebs-0.0.87/pyflexebs.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       50 2023-04-27 08:22:02.000000 pyflexebs-0.0.87/pyflexebs.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      114 2023-04-27 08:22:02.000000 pyflexebs-0.0.87/pyflexebs.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       10 2023-04-27 08:22:02.000000 pyflexebs-0.0.87/pyflexebs.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:22:02.462866 pyflexebs-0.0.87/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1726 2023-04-27 08:21:52.000000 pyflexebs-0.0.87/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-09 07:36:23.797051 pyflexebs-0.0.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-07-05 08:09:53.000000 pyflexebs-0.0.9/MANIFEST.in
+-rw-r--r--   0 mark      (1000) mark      (1000)     1439 2020-07-09 07:36:23.797051 pyflexebs-0.0.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      321 2020-07-09 07:36:11.000000 pyflexebs-0.0.9/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-09 07:36:23.796051 pyflexebs-0.0.9/pyflexebs/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-07-05 08:09:53.000000 pyflexebs-0.0.9/pyflexebs/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      796 2020-07-09 06:37:49.000000 pyflexebs-0.0.9/pyflexebs/configs.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-09 07:36:23.797051 pyflexebs-0.0.9/pyflexebs/endpoints/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-07-05 08:09:53.000000 pyflexebs-0.0.9/pyflexebs/endpoints/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2802 2020-07-09 07:35:55.000000 pyflexebs-0.0.9/pyflexebs/endpoints/group_default.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      546 2020-07-05 08:20:08.000000 pyflexebs-0.0.9/pyflexebs/endpoints/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       83 2020-07-09 07:36:11.000000 pyflexebs-0.0.9/pyflexebs/version.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-07-09 07:36:23.797051 pyflexebs-0.0.9/pyflexebs.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1439 2020-07-09 07:36:23.000000 pyflexebs-0.0.9/pyflexebs.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      402 2020-07-09 07:36:23.000000 pyflexebs-0.0.9/pyflexebs.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2020-07-09 07:36:23.000000 pyflexebs-0.0.9/pyflexebs.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       61 2020-07-09 07:36:23.000000 pyflexebs-0.0.9/pyflexebs.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       66 2020-07-09 07:36:23.000000 pyflexebs-0.0.9/pyflexebs.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       10 2020-07-09 07:36:23.000000 pyflexebs-0.0.9/pyflexebs.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2020-07-09 07:36:23.797051 pyflexebs-0.0.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1746 2020-07-09 07:36:11.000000 pyflexebs-0.0.9/setup.py
```

### Comparing `pyflexebs-0.0.87/PKG-INFO` & `pyflexebs-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyflexebs
-Version: 0.0.87
-Summary: Pyflexebs will allow you to monitor and expand/contract you EBS volumes in aws
+Version: 0.0.9
+Summary: pyflexebs will allow you to monitor and expand/contract you ebs in aws
 Home-page: https://veltzer.github.io/pyflexebs
-Download-URL: https://github.com/veltzer/pyflexebs
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
+Download-URL: https://github.com/veltzer/pyflexebs
+Description: ===========
+        *pyflexebs*
+        ===========
+        
+        .. image:: https://img.shields.io/pypi/v/pyflexebs
+        
+        .. image:: https://img.shields.io/github/license/veltzer/pyflexebs
+        
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        
+        project website: https://veltzer.github.io/pyflexebs
+        
+        author: Mark Veltzer
+        
+        version: 0.0.9
+        
+        
+        
 Keywords: aws,ebs
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-===========
-*pyflexebs*
-===========
-
-.. image:: https://img.shields.io/pypi/v/pyflexebs
-
-.. image:: https://img.shields.io/github/license/veltzer/pyflexebs
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-
-project website: https://veltzer.github.io/pyflexebs
-
-author: Mark Veltzer
-
-version: 0.0.87
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyflexebs-0.0.87/pyflexebs.egg-info/PKG-INFO` & `pyflexebs-0.0.9/pyflexebs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyflexebs
-Version: 0.0.87
-Summary: Pyflexebs will allow you to monitor and expand/contract you EBS volumes in aws
+Version: 0.0.9
+Summary: pyflexebs will allow you to monitor and expand/contract you ebs in aws
 Home-page: https://veltzer.github.io/pyflexebs
-Download-URL: https://github.com/veltzer/pyflexebs
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
+Download-URL: https://github.com/veltzer/pyflexebs
+Description: ===========
+        *pyflexebs*
+        ===========
+        
+        .. image:: https://img.shields.io/pypi/v/pyflexebs
+        
+        .. image:: https://img.shields.io/github/license/veltzer/pyflexebs
+        
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        
+        project website: https://veltzer.github.io/pyflexebs
+        
+        author: Mark Veltzer
+        
+        version: 0.0.9
+        
+        
+        
 Keywords: aws,ebs
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-===========
-*pyflexebs*
-===========
-
-.. image:: https://img.shields.io/pypi/v/pyflexebs
-
-.. image:: https://img.shields.io/github/license/veltzer/pyflexebs
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-
-project website: https://veltzer.github.io/pyflexebs
-
-author: Mark Veltzer
-
-version: 0.0.87
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

