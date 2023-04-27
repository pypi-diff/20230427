# Comparing `tmp/pyfoldercheck-0.0.4.tar.gz` & `tmp/pyfoldercheck-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyfoldercheck-0.0.4.tar", last modified: Thu Nov 26 11:53:49 2020, max compression
+gzip compressed data, was "pyfoldercheck-0.0.5.tar", last modified: Thu Apr 27 08:23:10 2023, max compression
```

## Comparing `pyfoldercheck-0.0.4.tar` & `pyfoldercheck-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-11-26 11:53:49.486950 pyfoldercheck-0.0.4/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-05-24 21:46:29.000000 pyfoldercheck-0.0.4/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1458 2020-11-26 11:53:49.486950 pyfoldercheck-0.0.4/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      345 2020-11-26 11:53:28.000000 pyfoldercheck-0.0.4/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-11-26 11:53:49.486950 pyfoldercheck-0.0.4/pyfoldercheck/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2019-02-01 03:34:17.000000 pyfoldercheck-0.0.4/pyfoldercheck/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1254 2020-11-26 11:46:38.000000 pyfoldercheck-0.0.4/pyfoldercheck/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2051 2020-11-26 11:53:03.000000 pyfoldercheck-0.0.4/pyfoldercheck/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      199 2020-11-26 11:53:28.000000 pyfoldercheck-0.0.4/pyfoldercheck/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)      363 2020-11-26 11:48:04.000000 pyfoldercheck-0.0.4/pyfoldercheck/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2020-11-26 11:53:49.486950 pyfoldercheck-0.0.4/pyfoldercheck.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1458 2020-11-26 11:53:49.000000 pyfoldercheck-0.0.4/pyfoldercheck.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      385 2020-11-26 11:53:49.000000 pyfoldercheck-0.0.4/pyfoldercheck.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2020-11-26 11:53:49.000000 pyfoldercheck-0.0.4/pyfoldercheck.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       59 2020-11-26 11:53:49.000000 pyfoldercheck-0.0.4/pyfoldercheck.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       18 2020-11-26 11:53:49.000000 pyfoldercheck-0.0.4/pyfoldercheck.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       14 2020-11-26 11:53:49.000000 pyfoldercheck-0.0.4/pyfoldercheck.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2020-11-26 11:53:49.486950 pyfoldercheck-0.0.4/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1620 2020-11-26 11:53:28.000000 pyfoldercheck-0.0.4/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:23:10.532391 pyfoldercheck-0.0.5/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:23:02.000000 pyfoldercheck-0.0.5/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1409 2023-04-27 08:23:10.532391 pyfoldercheck-0.0.5/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      426 2023-04-27 08:23:02.000000 pyfoldercheck-0.0.5/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:23:10.532391 pyfoldercheck-0.0.5/pyfoldercheck/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2019-02-01 03:34:17.000000 pyfoldercheck-0.0.5/pyfoldercheck/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1254 2020-11-26 11:46:38.000000 pyfoldercheck-0.0.5/pyfoldercheck/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2010 2023-04-27 08:22:41.000000 pyfoldercheck-0.0.5/pyfoldercheck/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      218 2023-04-27 08:23:02.000000 pyfoldercheck-0.0.5/pyfoldercheck/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      363 2020-11-26 11:48:04.000000 pyfoldercheck-0.0.5/pyfoldercheck/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:23:10.532391 pyfoldercheck-0.0.5/pyfoldercheck.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1409 2023-04-27 08:23:10.000000 pyfoldercheck-0.0.5/pyfoldercheck.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      381 2023-04-27 08:23:10.000000 pyfoldercheck-0.0.5/pyfoldercheck.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:23:10.000000 pyfoldercheck-0.0.5/pyfoldercheck.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       58 2023-04-27 08:23:10.000000 pyfoldercheck-0.0.5/pyfoldercheck.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       18 2023-04-27 08:23:10.000000 pyfoldercheck-0.0.5/pyfoldercheck.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       14 2023-04-27 08:23:10.000000 pyfoldercheck-0.0.5/pyfoldercheck.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:23:10.532391 pyfoldercheck-0.0.5/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1559 2023-04-27 08:23:02.000000 pyfoldercheck-0.0.5/setup.py
```

### Comparing `pyfoldercheck-0.0.4/PKG-INFO` & `pyfoldercheck-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyfoldercheck
-Version: 0.0.4
-Summary: apply a set of checks on files in a folder
+Version: 0.0.5
+Summary: Pyfoldercheck will apply a set of checks on files in a folder
 Home-page: https://veltzer.github.io/pyfoldercheck
+Download-URL: https://github.com/veltzer/pyfoldercheck
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyfoldercheck
-Description: ===============
-        *pyfoldercheck*
-        ===============
-        
-        .. image:: https://img.shields.io/pypi/v/pyfoldercheck
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyfoldercheck
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyfoldercheck
-        
-        author: Mark Veltzer
-        
-        version: 0.0.4
-        
-        
-        
 Keywords: mp3,pdf,collection
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
+===============
+*pyfoldercheck*
+===============
+
+.. image:: https://img.shields.io/pypi/v/pyfoldercheck
+
+.. image:: https://img.shields.io/github/license/veltzer/pyfoldercheck
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyfoldercheck
+
+author: Mark Veltzer
+
+version: 0.0.5
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2019, 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfoldercheck-0.0.4/pyfoldercheck/configs.py` & `pyfoldercheck-0.0.5/pyfoldercheck/configs.py`

 * *Files identical despite different names*

### Comparing `pyfoldercheck-0.0.4/pyfoldercheck/main.py` & `pyfoldercheck-0.0.5/pyfoldercheck/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 
 import pylogconf.core
 from pytconf import register_endpoint, register_main, config_arg_parse_and_launch
 
 from pyfoldercheck.configs import ConfigRepository, ConfigNames, Authorized
-from pyfoldercheck.static import APP_NAME, VERSION_STR
+from pyfoldercheck.static import APP_NAME, VERSION_STR, DESCRIPTION
 from pyfoldercheck.utils import is_ascii, add_non_ascii
 
 
 def scan_files():
     bad_characters = set()
     count = 0
     for root, directories, files in os.walk(ConfigRepository.folder):
@@ -21,28 +21,28 @@
             if not is_ascii(file, Authorized.chars_ok_for_files):
                 # full = os.path.join(root, file)
                 # print(file, full)
                 add_non_ascii(bad_characters, file)
         for directory in directories:
             if not is_ascii(directory, Authorized.chars_ok_for_folders):
                 full = os.path.join(root, directory)
-                print('folder [{}]'.format(full))
+                print(f"folder [{full}]")
     return bad_characters, count
 
 
 @register_endpoint(
     description="Scan the folder",
     configs=[
         ConfigRepository,
     ],
 )
 def scan() -> None:
     bad_characters, count = scan_files()
     print(bad_characters)
-    print("found [{}] appearances".format(count))
+    print(f"found [{count}] appearances")
 
 
 @register_endpoint(
     description="Authorize words with non ascii in them",
     configs=[
         ConfigRepository,
         ConfigNames,
@@ -58,15 +58,15 @@
     scan_files()
     # write the repository back
     with open(ConfigNames.repository, "w") as f:
         json.dump(repository, f)
 
 
 @register_main(
-    main_description="A program to help you out with your mp3 library",
+    main_description=DESCRIPTION,
     app_name=APP_NAME,
     version=VERSION_STR,
 )
 def main():
     pylogconf.core.setup()
     config_arg_parse_and_launch()
```

### Comparing `pyfoldercheck-0.0.4/pyfoldercheck.egg-info/PKG-INFO` & `pyfoldercheck-0.0.5/pyfoldercheck.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyfoldercheck
-Version: 0.0.4
-Summary: apply a set of checks on files in a folder
+Version: 0.0.5
+Summary: Pyfoldercheck will apply a set of checks on files in a folder
 Home-page: https://veltzer.github.io/pyfoldercheck
+Download-URL: https://github.com/veltzer/pyfoldercheck
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyfoldercheck
-Description: ===============
-        *pyfoldercheck*
-        ===============
-        
-        .. image:: https://img.shields.io/pypi/v/pyfoldercheck
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyfoldercheck
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyfoldercheck
-        
-        author: Mark Veltzer
-        
-        version: 0.0.4
-        
-        
-        
 Keywords: mp3,pdf,collection
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
+===============
+*pyfoldercheck*
+===============
+
+.. image:: https://img.shields.io/pypi/v/pyfoldercheck
+
+.. image:: https://img.shields.io/github/license/veltzer/pyfoldercheck
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyfoldercheck
+
+author: Mark Veltzer
+
+version: 0.0.5
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2019, 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfoldercheck-0.0.4/setup.py` & `pyfoldercheck-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,56 +5,51 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyfoldercheck",
-    version="0.0.4",
+    version="0.0.5",
     packages=[
-        'pyfoldercheck',
+        "pyfoldercheck",
     ],
     # from here all is optional
-    description="apply a set of checks on files in a folder",
+    description="Pyfoldercheck will apply a set of checks on files in a folder",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'mp3',
-        'pdf',
-        'collection',
+        "mp3",
+        "pdf",
+        "collection",
     ],
     url="https://veltzer.github.io/pyfoldercheck",
     download_url="https://github.com/veltzer/pyfoldercheck",
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
-        'pyfoldercheck=pyfoldercheck.main:main',
+        "pyfoldercheck=pyfoldercheck.main:main",
     ]},
-    python_requires=">=3.6",
 )
```

