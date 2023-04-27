# Comparing `tmp/pytagimg-0.0.1.tar.gz` & `tmp/pytagimg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytagimg-0.0.1.tar", last modified: Fri Aug 28 05:04:59 2020, max compression
+gzip compressed data, was "pytagimg-0.0.3.tar", last modified: Thu Apr 27 08:24:21 2023, max compression
```

## Comparing `pytagimg-0.0.1.tar` & `pytagimg-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-28 05:04:59.282791 pytagimg-0.0.1/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-08-28 01:05:25.000000 pytagimg-0.0.1/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1393 2020-08-28 05:04:59.282791 pytagimg-0.0.1/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      315 2020-08-28 01:13:02.000000 pytagimg-0.0.1/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-28 05:04:59.281790 pytagimg-0.0.1/pytagimg/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-08-28 01:05:25.000000 pytagimg-0.0.1/pytagimg/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1029 2020-08-28 01:12:08.000000 pytagimg-0.0.1/pytagimg/configs.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-28 05:04:59.281790 pytagimg-0.0.1/pytagimg/endpoints/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-08-28 01:05:25.000000 pytagimg-0.0.1/pytagimg/endpoints/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3480 2020-08-28 01:12:15.000000 pytagimg-0.0.1/pytagimg/endpoints/group_default.py
--rw-r--r--   0 mark      (1000) mark      (1000)      539 2020-08-28 01:12:22.000000 pytagimg-0.0.1/pytagimg/endpoints/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)       83 2020-08-28 01:08:20.000000 pytagimg-0.0.1/pytagimg/version.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-08-28 05:04:59.281790 pytagimg-0.0.1/pytagimg.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1393 2020-08-28 05:04:59.000000 pytagimg-0.0.1/pytagimg.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      390 2020-08-28 05:04:59.000000 pytagimg-0.0.1/pytagimg.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2020-08-28 05:04:59.000000 pytagimg-0.0.1/pytagimg.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       59 2020-08-28 05:04:59.000000 pytagimg-0.0.1/pytagimg.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       18 2020-08-28 05:04:59.000000 pytagimg-0.0.1/pytagimg.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2020-08-28 05:04:59.000000 pytagimg-0.0.1/pytagimg.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2020-08-28 05:04:59.282791 pytagimg-0.0.1/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1599 2020-08-28 01:13:02.000000 pytagimg-0.0.1/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:24:21.231910 pytagimg-0.0.3/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:24:05.000000 pytagimg-0.0.3/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1326 2023-04-27 08:24:21.231910 pytagimg-0.0.3/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      390 2023-04-27 08:24:05.000000 pytagimg-0.0.3/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:24:21.231910 pytagimg-0.0.3/pytagimg/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-08-28 01:05:25.000000 pytagimg-0.0.3/pytagimg/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      225 2022-08-15 14:22:43.000000 pytagimg-0.0.3/pytagimg/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      497 2023-04-27 08:23:48.000000 pytagimg-0.0.3/pytagimg/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      181 2023-04-27 08:24:05.000000 pytagimg-0.0.3/pytagimg/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:24:21.231910 pytagimg-0.0.3/pytagimg.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1326 2023-04-27 08:24:21.000000 pytagimg-0.0.3/pytagimg.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      308 2023-04-27 08:24:21.000000 pytagimg-0.0.3/pytagimg.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:24:21.000000 pytagimg-0.0.3/pytagimg.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-27 08:24:21.000000 pytagimg-0.0.3/pytagimg.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       18 2023-04-27 08:24:21.000000 pytagimg-0.0.3/pytagimg.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-27 08:24:21.000000 pytagimg-0.0.3/pytagimg.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:24:21.231910 pytagimg-0.0.3/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1486 2023-04-27 08:24:05.000000 pytagimg-0.0.3/setup.py
```

### Comparing `pytagimg-0.0.1/PKG-INFO` & `pytagimg-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pytagimg
-Version: 0.0.1
-Summary: pytagimg helps tag images fast
+Version: 0.0.3
+Summary: Pytagimg helps you tag images fast
 Home-page: https://veltzer.github.io/pytagimg
+Download-URL: https://github.com/veltzer/pytagimg
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pytagimg
-Description: ==========
-        *pytagimg*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pytagimg
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pytagimg
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pytagimg
-        
-        author: Mark Veltzer
-        
-        version: 0.0.1
-        
-        
-        
-Keywords: make,scons
+Keywords: images,photos
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========
+*pytagimg*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pytagimg
+
+.. image:: https://img.shields.io/github/license/veltzer/pytagimg
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pytagimg
+
+author: Mark Veltzer
+
+version: 0.0.3
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytagimg-0.0.1/pytagimg.egg-info/PKG-INFO` & `pytagimg-0.0.3/pytagimg.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pytagimg
-Version: 0.0.1
-Summary: pytagimg helps tag images fast
+Version: 0.0.3
+Summary: Pytagimg helps you tag images fast
 Home-page: https://veltzer.github.io/pytagimg
+Download-URL: https://github.com/veltzer/pytagimg
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pytagimg
-Description: ==========
-        *pytagimg*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pytagimg
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pytagimg
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pytagimg
-        
-        author: Mark Veltzer
-        
-        version: 0.0.1
-        
-        
-        
-Keywords: make,scons
+Keywords: images,photos
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========
+*pytagimg*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pytagimg
+
+.. image:: https://img.shields.io/github/license/veltzer/pytagimg
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pytagimg
+
+author: Mark Veltzer
+
+version: 0.0.3
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytagimg-0.0.1/setup.py` & `pytagimg-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,56 +5,50 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pytagimg",
-    version="0.0.1",
+    version="0.0.3",
     packages=[
-        'pytagimg',
-        'pytagimg.endpoints',
+        "pytagimg",
     ],
     # from here all is optional
-    description="pytagimg helps tag images fast",
+    description="Pytagimg helps you tag images fast",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'make',
-        'scons',
+        "images",
+        "photos",
     ],
     url="https://veltzer.github.io/pytagimg",
     download_url="https://github.com/veltzer/pytagimg",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'pytconf',
-        'pylogconf',
+        "pytconf",
+        "pylogconf",
     ],
-    extras_require={
-    },
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
-    ],
-    data_files=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
     ],
     entry_points={"console_scripts": [
-        'pytagimg=pytagimg.endpoints.main:main',
+        "pytagimg=pytagimg.main:main",
     ]},
-    python_requires=">=3.6",
 )
```

