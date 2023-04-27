# Comparing `tmp/pyweblight-0.0.4.tar.gz` & `tmp/pyweblight-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweblight-0.0.4.tar", last modified: Sat Apr 30 01:35:02 2022, max compression
+gzip compressed data, was "pyweblight-0.0.5.tar", last modified: Thu Apr 27 08:11:51 2023, max compression
```

## Comparing `pyweblight-0.0.4.tar` & `pyweblight-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-30 01:35:02.555374 pyweblight-0.0.4/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2020-05-24 13:27:22.000000 pyweblight-0.0.4/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1474 2022-04-30 01:35:02.555374 pyweblight-0.0.4/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      327 2022-04-30 01:34:41.000000 pyweblight-0.0.4/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-30 01:35:02.555374 pyweblight-0.0.4/pyweblight/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-21 07:52:41.000000 pyweblight-0.0.4/pyweblight/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      503 2020-07-25 10:55:20.000000 pyweblight-0.0.4/pyweblight/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      639 2020-11-15 21:23:32.000000 pyweblight-0.0.4/pyweblight/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      211 2022-04-30 01:34:41.000000 pyweblight-0.0.4/pyweblight/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     6340 2021-09-17 18:27:11.000000 pyweblight-0.0.4/pyweblight/webserver_start.py
--rw-r--r--   0 mark      (1000) mark      (1000)      159 2021-09-17 18:27:36.000000 pyweblight-0.0.4/pyweblight/webserver_stop.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-30 01:35:02.555374 pyweblight-0.0.4/pyweblight.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1474 2022-04-30 01:35:02.000000 pyweblight-0.0.4/pyweblight.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      391 2022-04-30 01:35:02.000000 pyweblight-0.0.4/pyweblight.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-04-30 01:35:02.000000 pyweblight-0.0.4/pyweblight.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       53 2022-04-30 01:35:02.000000 pyweblight-0.0.4/pyweblight.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       32 2022-04-30 01:35:02.000000 pyweblight-0.0.4/pyweblight.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2022-04-30 01:35:02.000000 pyweblight-0.0.4/pyweblight.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-04-30 01:35:02.556374 pyweblight-0.0.4/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1714 2022-04-30 01:34:41.000000 pyweblight-0.0.4/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:11:51.008166 pyweblight-0.0.5/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 08:11:40.000000 pyweblight-0.0.5/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1400 2023-04-27 08:11:51.008166 pyweblight-0.0.5/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      402 2023-04-27 08:11:40.000000 pyweblight-0.0.5/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:11:51.008166 pyweblight-0.0.5/pyweblight/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-21 07:52:41.000000 pyweblight-0.0.5/pyweblight/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      503 2020-07-25 10:55:20.000000 pyweblight-0.0.5/pyweblight/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      613 2023-04-27 08:11:27.000000 pyweblight-0.0.5/pyweblight/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-27 08:11:40.000000 pyweblight-0.0.5/pyweblight/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     6376 2023-04-22 07:38:30.000000 pyweblight-0.0.5/pyweblight/webserver_start.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      159 2021-09-17 18:27:36.000000 pyweblight-0.0.5/pyweblight/webserver_stop.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 08:11:51.008166 pyweblight-0.0.5/pyweblight.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1400 2023-04-27 08:11:50.000000 pyweblight-0.0.5/pyweblight.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      387 2023-04-27 08:11:50.000000 pyweblight-0.0.5/pyweblight.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 08:11:50.000000 pyweblight-0.0.5/pyweblight.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-27 08:11:50.000000 pyweblight-0.0.5/pyweblight.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       32 2023-04-27 08:11:50.000000 pyweblight-0.0.5/pyweblight.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-04-27 08:11:50.000000 pyweblight-0.0.5/pyweblight.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 08:11:51.009166 pyweblight-0.0.5/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1634 2023-04-27 08:11:40.000000 pyweblight-0.0.5/setup.py
```

### Comparing `pyweblight-0.0.4/PKG-INFO` & `pyweblight-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyweblight
-Version: 0.0.4
-Summary: pyweblight is a small configurable web server for developers
+Version: 0.0.5
+Summary: Pyweblight is a small configurable web server for developers
 Home-page: https://veltzer.github.io/pyweblight
+Download-URL: https://github.com/veltzer/pyweblight
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyweblight
-Description: ============
-        *pyweblight*
-        ============
-        
-        .. image:: https://img.shields.io/pypi/v/pyweblight
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyweblight
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyweblight
-        
-        author: Mark Veltzer
-        
-        version: 0.0.4
-        
-        
-        
 Keywords: http,https,apache,python,python3,server,web
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
-Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+============
+*pyweblight*
+============
+
+.. image:: https://img.shields.io/pypi/v/pyweblight
+
+.. image:: https://img.shields.io/github/license/veltzer/pyweblight
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyweblight
+
+author: Mark Veltzer
+
+version: 0.0.5
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyweblight-0.0.4/pyweblight/main.py` & `pyweblight-0.0.5/pyweblight/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 main entry point to the program
 """
 
 
 import pylogconf.core
 from pytconf import register_main, config_arg_parse_and_launch, register_endpoint
 
-from pyweblight.static import APP_NAME, VERSION_STR
+from pyweblight.static import APP_NAME, VERSION_STR, DESCRIPTION
 
 
 @register_endpoint(
     description="Start the web server",
 )
 def start() -> None:
     pass
@@ -20,15 +20,15 @@
     description="Stop the web server",
 )
 def stop() -> None:
     pass
 
 
 @register_main(
-    main_description="pyweblight is a lightweight web server in python",
+    main_description=DESCRIPTION,
     app_name=APP_NAME,
     version=VERSION_STR,
 )
 def main():
     pylogconf.core.setup()
     config_arg_parse_and_launch()
```

### Comparing `pyweblight-0.0.4/pyweblight/webserver_start.py` & `pyweblight-0.0.5/pyweblight/webserver_start.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - /favicon.ico return 500 and should return 404.
 - make the search path much more elaborate so that I can easy searching for files inside
 libraries.
 - make the transport of requests be UTF-8 so that the browser will shut up about
 the fact that all my documents do not have ending in them.
 """
 
+# pylint: disable=deprecated-module
 import cgi
 import os
 import time
 import http.server
 import mimetypes
 import daemon
```

### Comparing `pyweblight-0.0.4/pyweblight.egg-info/PKG-INFO` & `pyweblight-0.0.5/pyweblight.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyweblight
-Version: 0.0.4
-Summary: pyweblight is a small configurable web server for developers
+Version: 0.0.5
+Summary: Pyweblight is a small configurable web server for developers
 Home-page: https://veltzer.github.io/pyweblight
+Download-URL: https://github.com/veltzer/pyweblight
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyweblight
-Description: ============
-        *pyweblight*
-        ============
-        
-        .. image:: https://img.shields.io/pypi/v/pyweblight
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyweblight
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyweblight
-        
-        author: Mark Veltzer
-        
-        version: 0.0.4
-        
-        
-        
 Keywords: http,https,apache,python,python3,server,web
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
-Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+============
+*pyweblight*
+============
+
+.. image:: https://img.shields.io/pypi/v/pyweblight
+
+.. image:: https://img.shields.io/github/license/veltzer/pyweblight
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyweblight
+
+author: Mark Veltzer
+
+version: 0.0.5
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyweblight-0.0.4/setup.py` & `pyweblight-0.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,61 +5,56 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyweblight",
-    version="0.0.4",
+    version="0.0.5",
     packages=[
-        'pyweblight',
+        "pyweblight",
     ],
     # from here all is optional
-    description="pyweblight is a small configurable web server for developers",
+    description="Pyweblight is a small configurable web server for developers",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'http',
-        'https',
-        'apache',
-        'python',
-        'python3',
-        'server',
-        'web',
+        "http",
+        "https",
+        "apache",
+        "python",
+        "python3",
+        "server",
+        "web",
     ],
     url="https://veltzer.github.io/pyweblight",
     download_url="https://github.com/veltzer/pyweblight",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'python-daemon',
-        'pytconf',
-        'pylogconf',
+        "python-daemon",
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
-        'pyweblight=pyweblight.main:main',
+        "pyweblight=pyweblight.main:main",
     ]},
-    python_requires=">=3.7",
 )
```

