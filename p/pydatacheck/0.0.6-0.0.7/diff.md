# Comparing `tmp/pydatacheck-0.0.6.tar.gz` & `tmp/pydatacheck-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatacheck-0.0.6.tar", last modified: Fri Oct  7 19:08:01 2022, max compression
+gzip compressed data, was "pydatacheck-0.0.7.tar", last modified: Thu Apr 27 08:20:38 2023, max compression
```

## Comparing `pydatacheck-0.0.6.tar` & `pydatacheck-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-07 19:08:01.110918 pydatacheck-0.0.6/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2022-10-07 19:07:46.000000 pydatacheck-0.0.6/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2022-08-31 07:28:07.000000 pydatacheck-0.0.6/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1451 2022-10-07 19:08:01.110918 pydatacheck-0.0.6/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      390 2022-10-07 19:07:46.000000 pydatacheck-0.0.6/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-07 19:08:01.109918 pydatacheck-0.0.6/pydatacheck/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-08-31 07:28:07.000000 pydatacheck-0.0.6/pydatacheck/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      143 2022-10-07 18:10:34.000000 pydatacheck-0.0.6/pydatacheck/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3547 2022-10-07 19:03:20.000000 pydatacheck-0.0.6/pydatacheck/data_check_books.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1224 2022-10-07 19:03:24.000000 pydatacheck-0.0.6/pydatacheck/data_check_videos.py
--rw-r--r--   0 mark      (1000) mark      (1000)      873 2022-10-07 19:07:23.000000 pydatacheck-0.0.6/pydatacheck/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)       34 2022-08-31 07:28:07.000000 pydatacheck-0.0.6/pydatacheck/route.py
--rw-r--r--   0 mark      (1000) mark      (1000)      187 2022-10-07 19:07:46.000000 pydatacheck-0.0.6/pydatacheck/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-07 19:08:01.110918 pydatacheck-0.0.6/pydatacheck.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1451 2022-10-07 19:08:01.000000 pydatacheck-0.0.6/pydatacheck.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      436 2022-10-07 19:08:01.000000 pydatacheck-0.0.6/pydatacheck.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-10-07 19:08:01.000000 pydatacheck-0.0.6/pydatacheck.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       55 2022-10-07 19:08:01.000000 pydatacheck-0.0.6/pydatacheck.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       34 2022-10-07 19:08:01.000000 pydatacheck-0.0.6/pydatacheck.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       12 2022-10-07 19:08:01.000000 pydatacheck-0.0.6/pydatacheck.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-10-07 19:08:01.110918 pydatacheck-0.0.6/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1665 2022-10-07 19:07:46.000000 pydatacheck-0.0.6/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:20:38.575294 pydatacheck-0.0.7/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:20:27.000000 pydatacheck-0.0.7/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1355 2023-04-27 08:20:38.575294 pydatacheck-0.0.7/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      396 2023-04-27 08:20:27.000000 pydatacheck-0.0.7/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:20:38.575294 pydatacheck-0.0.7/pydatacheck/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-08-31 07:28:07.000000 pydatacheck-0.0.7/pydatacheck/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      143 2022-10-07 18:10:34.000000 pydatacheck-0.0.7/pydatacheck/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3547 2022-10-07 19:03:20.000000 pydatacheck-0.0.7/pydatacheck/data_check_books.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1224 2022-10-07 19:03:24.000000 pydatacheck-0.0.7/pydatacheck/data_check_videos.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      849 2023-04-27 08:20:06.000000 pydatacheck-0.0.7/pydatacheck/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       34 2022-08-31 07:28:07.000000 pydatacheck-0.0.7/pydatacheck/route.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-27 08:20:27.000000 pydatacheck-0.0.7/pydatacheck/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:20:38.575294 pydatacheck-0.0.7/pydatacheck.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1355 2023-04-27 08:20:38.000000 pydatacheck-0.0.7/pydatacheck.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      424 2023-04-27 08:20:38.000000 pydatacheck-0.0.7/pydatacheck.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:20:38.000000 pydatacheck-0.0.7/pydatacheck.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       54 2023-04-27 08:20:38.000000 pydatacheck-0.0.7/pydatacheck.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       34 2023-04-27 08:20:38.000000 pydatacheck-0.0.7/pydatacheck.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       12 2023-04-27 08:20:38.000000 pydatacheck-0.0.7/pydatacheck.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:20:38.576294 pydatacheck-0.0.7/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1567 2023-04-27 08:20:27.000000 pydatacheck-0.0.7/setup.py
```

### Comparing `pydatacheck-0.0.6/LICENSE` & `pydatacheck-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatacheck-0.0.6/PKG-INFO` & `pydatacheck-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pydatacheck
-Version: 0.0.6
-Summary: pydatacheck checks yaml data files
+Version: 0.0.7
+Summary: Pydatacheck checks yaml data files
 Home-page: https://veltzer.github.io/pydatacheck
+Download-URL: https://github.com/veltzer/pydatacheck
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pydatacheck
 Keywords: yaml,imdb,simania,goodreads
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
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -37,12 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydatacheck
 
 author: Mark Veltzer
 
-version: 0.0.6
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2022
-
+version: 0.0.7
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2022, 2023
```

### Comparing `pydatacheck-0.0.6/pydatacheck/data_check_books.py` & `pydatacheck-0.0.7/pydatacheck/data_check_books.py`

 * *Files identical despite different names*

### Comparing `pydatacheck-0.0.6/pydatacheck/data_check_videos.py` & `pydatacheck-0.0.7/pydatacheck/data_check_videos.py`

 * *Files identical despite different names*

### Comparing `pydatacheck-0.0.6/pydatacheck/main.py` & `pydatacheck-0.0.7/pydatacheck/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pylogconf.core
 from pytconf import register_endpoint, register_main, config_arg_parse_and_launch, get_free_args
 
 
-from pydatacheck.static import APP_NAME, VERSION_STR
+from pydatacheck.static import APP_NAME, VERSION_STR, DESCRIPTION
 from pydatacheck.data_check_books import do_check_books
 from pydatacheck.data_check_videos import do_check_videos
 
 
 @register_endpoint(
     description="check videos",
     allow_free_args=True,
@@ -22,15 +22,15 @@
     min_free_args=1,
 )
 def check_books() -> None:
     do_check_books(get_free_args())
 
 
 @register_main(
-    main_description="pydatacheck will check your yaml files for you",
+    main_description=DESCRIPTION,
     app_name=APP_NAME,
     version=VERSION_STR,
 )
 def main():
     pylogconf.core.setup()
     config_arg_parse_and_launch()
```

### Comparing `pydatacheck-0.0.6/pydatacheck.egg-info/PKG-INFO` & `pydatacheck-0.0.7/pydatacheck.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pydatacheck
-Version: 0.0.6
-Summary: pydatacheck checks yaml data files
+Version: 0.0.7
+Summary: Pydatacheck checks yaml data files
 Home-page: https://veltzer.github.io/pydatacheck
+Download-URL: https://github.com/veltzer/pydatacheck
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pydatacheck
 Keywords: yaml,imdb,simania,goodreads
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
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -37,12 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydatacheck
 
 author: Mark Veltzer
 
-version: 0.0.6
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2022
-
+version: 0.0.7
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2022, 2023
```

### Comparing `pydatacheck-0.0.6/setup.py` & `pydatacheck-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,55 +5,53 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pydatacheck",
-    version="0.0.6",
+    version="0.0.7",
     packages=[
-        'pydatacheck',
+        "pydatacheck",
     ],
     # from here all is optional
-    description="pydatacheck checks yaml data files",
+    description="Pydatacheck checks yaml data files",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'yaml',
-        'imdb',
-        'simania',
-        'goodreads',
+        "yaml",
+        "imdb",
+        "simania",
+        "goodreads",
     ],
     url="https://veltzer.github.io/pydatacheck",
     download_url="https://github.com/veltzer/pydatacheck",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'pytconf',
-        'cinemagoer',
-        'beautifulsoup4',
+        "pytconf",
+        "cinemagoer",
+        "beautifulsoup4",
     ],
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
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
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
-        'pydatacheck=pydatacheck.main:main',
+        "pydatacheck=pydatacheck.main:main",
     ]},
 )
```

