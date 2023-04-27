# Comparing `tmp/pycookie-0.0.1.tar.gz` & `tmp/pycookie-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycookie-0.0.1.tar", last modified: Fri May 21 01:57:06 2021, max compression
+gzip compressed data, was "pycookie-0.0.2.tar", last modified: Thu Apr 27 08:19:25 2023, max compression
```

## Comparing `pycookie-0.0.1.tar` & `pycookie-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-05-21 01:57:06.477382 pycookie-0.0.1/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2021-05-17 11:07:24.000000 pycookie-0.0.1/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1406 2021-05-21 01:57:06.477382 pycookie-0.0.1/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      315 2021-05-21 01:55:07.000000 pycookie-0.0.1/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-05-21 01:57:06.476382 pycookie-0.0.1/pycookie/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2021-05-21 01:46:48.000000 pycookie-0.0.1/pycookie/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      282 2021-05-21 01:47:36.000000 pycookie-0.0.1/pycookie/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      459 2021-05-21 01:54:18.000000 pycookie-0.0.1/pycookie/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      170 2021-05-21 01:55:07.000000 pycookie-0.0.1/pycookie/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-05-21 01:57:06.477382 pycookie-0.0.1/pycookie.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1406 2021-05-21 01:57:06.000000 pycookie-0.0.1/pycookie.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      312 2021-05-21 01:57:06.000000 pycookie-0.0.1/pycookie.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-05-21 01:57:06.000000 pycookie-0.0.1/pycookie.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       49 2021-05-21 01:57:06.000000 pycookie-0.0.1/pycookie.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       32 2021-05-21 01:57:06.000000 pycookie-0.0.1/pycookie.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2021-05-21 01:57:06.000000 pycookie-0.0.1/pycookie.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2021-05-21 01:57:06.477382 pycookie-0.0.1/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1619 2021-05-21 01:55:07.000000 pycookie-0.0.1/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:19:25.674991 pycookie-0.0.2/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:19:03.000000 pycookie-0.0.2/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1340 2023-04-27 08:19:25.674991 pycookie-0.0.2/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      384 2023-04-27 08:19:03.000000 pycookie-0.0.2/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:19:25.674991 pycookie-0.0.2/pycookie/
+-rw-r--r--   0 mark      (1000) mark      (1000)       25 2021-05-21 01:46:48.000000 pycookie-0.0.2/pycookie/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      282 2021-05-21 01:47:36.000000 pycookie-0.0.2/pycookie/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      957 2023-04-27 08:18:36.000000 pycookie-0.0.2/pycookie/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      184 2023-04-27 08:19:03.000000 pycookie-0.0.2/pycookie/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:19:25.674991 pycookie-0.0.2/pycookie.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1340 2023-04-27 08:19:25.000000 pycookie-0.0.2/pycookie.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      308 2023-04-27 08:19:25.000000 pycookie-0.0.2/pycookie.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:19:25.000000 pycookie-0.0.2/pycookie.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-27 08:19:25.000000 pycookie-0.0.2/pycookie.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       32 2023-04-27 08:19:25.000000 pycookie-0.0.2/pycookie.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-27 08:19:25.000000 pycookie-0.0.2/pycookie.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:19:25.674991 pycookie-0.0.2/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1553 2023-04-27 08:19:03.000000 pycookie-0.0.2/setup.py
```

### Comparing `pycookie-0.0.1/PKG-INFO` & `pycookie-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pycookie
-Version: 0.0.1
-Summary: help you handle cookies
+Version: 0.0.2
+Summary: Pycookie will help you handle cookies
 Home-page: https://veltzer.github.io/pycookie
+Download-URL: https://github.com/veltzer/pycookie
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pycookie
-Description: ==========
-        *pycookie*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pycookie
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pycookie
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pycookie
-        
-        author: Mark Veltzer
-        
-        version: 0.0.1
-        
-        
-        
 Keywords: cookies,browser,chrome,firefox
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
+*pycookie*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pycookie
+
+.. image:: https://img.shields.io/github/license/veltzer/pycookie
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pycookie
+
+author: Mark Veltzer
+
+version: 0.0.2
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycookie-0.0.1/pycookie.egg-info/PKG-INFO` & `pycookie-0.0.2/pycookie.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pycookie
-Version: 0.0.1
-Summary: help you handle cookies
+Version: 0.0.2
+Summary: Pycookie will help you handle cookies
 Home-page: https://veltzer.github.io/pycookie
+Download-URL: https://github.com/veltzer/pycookie
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pycookie
-Description: ==========
-        *pycookie*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pycookie
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pycookie
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pycookie
-        
-        author: Mark Veltzer
-        
-        version: 0.0.1
-        
-        
-        
 Keywords: cookies,browser,chrome,firefox
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
+*pycookie*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pycookie
+
+.. image:: https://img.shields.io/github/license/veltzer/pycookie
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pycookie
+
+author: Mark Veltzer
+
+version: 0.0.2
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycookie-0.0.1/setup.py` & `pycookie-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,58 +5,53 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pycookie",
-    version="0.0.1",
+    version="0.0.2",
     packages=[
-        'pycookie',
+        "pycookie",
     ],
     # from here all is optional
-    description="help you handle cookies",
+    description="Pycookie will help you handle cookies",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'cookies',
-        'browser',
-        'chrome',
-        'firefox',
+        "cookies",
+        "browser",
+        "chrome",
+        "firefox",
     ],
     url="https://veltzer.github.io/pycookie",
     download_url="https://github.com/veltzer/pycookie",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'pytconf',
-        'pylogconf',
-        'browsercookie',
+        "pytconf",
+        "pylogconf",
+        "browsercookie",
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
-        'pycookie=pycookie.main:main',
+        "pycookie=pycookie.main:main",
     ]},
-    python_requires=">=3.6",
 )
```

