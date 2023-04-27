# Comparing `tmp/pycmdtools-0.0.79.tar.gz` & `tmp/pycmdtools-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmdtools-0.0.79.tar", last modified: Sat Jul  2 09:39:08 2022, max compression
+gzip compressed data, was "pycmdtools-0.0.80.tar", last modified: Thu Apr 27 06:50:46 2023, max compression
```

## Comparing `pycmdtools-0.0.79.tar` & `pycmdtools-0.0.80.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-07-02 09:39:08.718548 pycmdtools-0.0.79/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2022-07-02 09:38:45.000000 pycmdtools-0.0.79/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2017-11-26 05:03:51.000000 pycmdtools-0.0.79/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1518 2022-07-02 09:39:08.718548 pycmdtools-0.0.79/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      415 2022-07-02 09:38:45.000000 pycmdtools-0.0.79/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-07-02 09:39:08.717548 pycmdtools-0.0.79/pycmdtools/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-21 07:37:10.000000 pycmdtools-0.0.79/pycmdtools/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2300 2022-04-28 05:14:39.000000 pycmdtools-0.0.79/pycmdtools/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     9505 2022-07-02 09:38:19.000000 pycmdtools-0.0.79/pycmdtools/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      216 2022-07-02 09:38:45.000000 pycmdtools-0.0.79/pycmdtools/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4612 2022-06-29 15:12:56.000000 pycmdtools-0.0.79/pycmdtools/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-07-02 09:39:08.718548 pycmdtools-0.0.79/pycmdtools.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1518 2022-07-02 09:39:08.000000 pycmdtools-0.0.79/pycmdtools.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      360 2022-07-02 09:39:08.000000 pycmdtools-0.0.79/pycmdtools.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-07-02 09:39:08.000000 pycmdtools-0.0.79/pycmdtools.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       53 2022-07-02 09:39:08.000000 pycmdtools-0.0.79/pycmdtools.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      118 2022-07-02 09:39:08.000000 pycmdtools-0.0.79/pycmdtools.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2022-07-02 09:39:08.000000 pycmdtools-0.0.79/pycmdtools.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-07-02 09:39:08.718548 pycmdtools-0.0.79/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1909 2022-07-02 09:38:45.000000 pycmdtools-0.0.79/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 06:50:46.617669 pycmdtools-0.0.80/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 06:50:37.000000 pycmdtools-0.0.80/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1422 2023-04-27 06:50:46.618669 pycmdtools-0.0.80/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      421 2023-04-27 06:50:37.000000 pycmdtools-0.0.80/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 06:50:46.617669 pycmdtools-0.0.80/pycmdtools/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-21 07:37:10.000000 pycmdtools-0.0.80/pycmdtools/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2300 2022-04-28 05:14:39.000000 pycmdtools-0.0.80/pycmdtools/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     9769 2023-04-27 06:48:33.000000 pycmdtools-0.0.80/pycmdtools/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1376 2023-04-27 06:48:09.000000 pycmdtools-0.0.80/pycmdtools/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      216 2023-04-27 06:50:37.000000 pycmdtools-0.0.80/pycmdtools/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4632 2023-03-08 23:00:20.000000 pycmdtools-0.0.80/pycmdtools/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 06:50:46.617669 pycmdtools-0.0.80/pycmdtools.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1422 2023-04-27 06:50:46.000000 pycmdtools-0.0.80/pycmdtools.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      369 2023-04-27 06:50:46.000000 pycmdtools-0.0.80/pycmdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 06:50:46.000000 pycmdtools-0.0.80/pycmdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-27 06:50:46.000000 pycmdtools-0.0.80/pycmdtools.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      118 2023-04-27 06:50:46.000000 pycmdtools-0.0.80/pycmdtools.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-04-27 06:50:46.000000 pycmdtools-0.0.80/pycmdtools.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 06:50:46.618669 pycmdtools-0.0.80/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1811 2023-04-27 06:50:37.000000 pycmdtools-0.0.80/setup.py
```

### Comparing `pycmdtools-0.0.79/LICENSE` & `pycmdtools-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `pycmdtools-0.0.79/PKG-INFO` & `pycmdtools-0.0.80/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pycmdtools
-Version: 0.0.79
+Version: 0.0.80
 Summary: pycmdtools is set of useful command line tools written in python
 Home-page: https://veltzer.github.io/pycmdtools
+Download-URL: https://github.com/veltzer/pycmdtools
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pycmdtools
 Keywords: utils,command line,python,shell,utilities
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
 
 project website: https://veltzer.github.io/pycmdtools
 
 author: Mark Veltzer
 
-version: 0.0.79
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022
-
+version: 0.0.80
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pycmdtools-0.0.79/pycmdtools/configs.py` & `pycmdtools-0.0.80/pycmdtools/configs.py`

 * *Files identical despite different names*

### Comparing `pycmdtools-0.0.79/pycmdtools/main.py` & `pycmdtools-0.0.80/pycmdtools/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from lxml import etree
 
 from pycmdtools.configs import ConfigFolder, ConfigUseStandardExceptions, ConfigChangeLine, ConfigProgress, \
     ConfigAlgorithm, ConfigDownloadGoogleDrive, ConfigCopy, ConfigDownloadGdriveURL, ConfigOutput
 from pycmdtools.static import DESCRIPTION, APP_NAME, VERSION_STR
 from pycmdtools.utils import yield_bad_symlinks, diamond_lines, checksum, download_file_from_google_drive, error, \
     remove_bad_symlinks, gdrive_download_link
+from pycmdtools.python import do_python_check_syntax
 
 
 @register_endpoint(
     description="Find all bad symbolic links in a folder",
     configs=[
         ConfigFolder,
         ConfigUseStandardExceptions
@@ -105,14 +106,23 @@
     for line in diamond_lines(get_free_args()):
         if line not in saw:
             saw.add(line)
             print(line, end='')
 
 
 @register_endpoint(
+    description="check python files for syntax",
+    allow_free_args=True
+)
+def python_check_syntax() -> None:
+    for filename in get_free_args():
+        do_python_check_syntax(filename)
+
+
+@register_endpoint(
     description="print all command line arguments",
     allow_free_args=True
 )
 def print_all_args() -> None:
     print(f"number of command line arguments is {len(get_free_args())}")
     for i, s in enumerate(get_free_args()):
         print(f"{i}: {s}")
```

### Comparing `pycmdtools-0.0.79/pycmdtools/utils.py` & `pycmdtools-0.0.80/pycmdtools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 import hashlib
 import logging
 import os
 import os.path
 import sys
-from typing import Callable, List
+from typing import Callable, List, Optional
 
 # These are symbolic links used for locks in standard users directories
 __standard_exceptions__ = {
     'lock',  # firefox lock, $HOME/.mozilla/firefox/[XXX].default/lock
     'SingletonCookie',  # chrome lock, /home/mark/.config/google-chrome/SingletonCookie
     'SingletonLock',  # chrome lock, /home/mark/.config/google-chrome/SingletonLock
     'SingletonSocket',  # chrome lock, /home/mark/.config/google-chrome/SingletonSocket
@@ -17,15 +17,15 @@
 import requests
 from bs4 import BeautifulSoup
 
 
 def yield_bad_symlinks(
     folder: str = ".",
     use_standard_exceptions: bool = True,
-    onerror: Callable = None,
+    onerror: Optional[Callable] = None,
 ):
     """
     remove bad symbolic links from a folder.
 
     Control this functions verbosity using the python logging framework
     :param folder:
     :param use_standard_exceptions:
```

### Comparing `pycmdtools-0.0.79/pycmdtools.egg-info/PKG-INFO` & `pycmdtools-0.0.80/pycmdtools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pycmdtools
-Version: 0.0.79
+Version: 0.0.80
 Summary: pycmdtools is set of useful command line tools written in python
 Home-page: https://veltzer.github.io/pycmdtools
+Download-URL: https://github.com/veltzer/pycmdtools
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pycmdtools
 Keywords: utils,command line,python,shell,utilities
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
 
 project website: https://veltzer.github.io/pycmdtools
 
 author: Mark Veltzer
 
-version: 0.0.79
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022
-
+version: 0.0.80
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

