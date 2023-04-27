# Comparing `tmp/dtrx-8.5.0.tar.gz` & `tmp/dtrx-8.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtrx-8.5.0.tar", last modified: Wed Nov 16 14:54:47 2022, max compression
+gzip compressed data, was "dtrx-8.5.1.tar", last modified: Thu Apr 27 19:18:05 2023, max compression
```

## Comparing `dtrx-8.5.0.tar` & `dtrx-8.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2022-11-16 14:54:47.307850 dtrx-8.5.0/
--rw-rw-r--   0 noah      (1000) noah      (1000)    35147 2021-11-24 20:34:36.000000 dtrx-8.5.0/COPYING
--rw-rw-r--   0 noah      (1000) noah      (1000)     6689 2022-11-16 14:54:47.307850 dtrx-8.5.0/PKG-INFO
--rw-rw-r--   0 noah      (1000) noah      (1000)     5571 2022-11-16 14:51:03.000000 dtrx-8.5.0/README.md
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2022-11-16 14:54:47.307850 dtrx-8.5.0/dtrx/
--rw-rw-r--   0 noah      (1000) noah      (1000)        0 2022-03-29 02:05:22.000000 dtrx-8.5.0/dtrx/__init__.py
--rwxrwxr-x   0 noah      (1000) noah      (1000)    61923 2022-11-16 14:51:47.000000 dtrx-8.5.0/dtrx/dtrx.py
-drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2022-11-16 14:54:47.307850 dtrx-8.5.0/dtrx.egg-info/
--rw-rw-r--   0 noah      (1000) noah      (1000)     6689 2022-11-16 14:54:47.000000 dtrx-8.5.0/dtrx.egg-info/PKG-INFO
--rw-rw-r--   0 noah      (1000) noah      (1000)      251 2022-11-16 14:54:47.000000 dtrx-8.5.0/dtrx.egg-info/SOURCES.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)        1 2022-11-16 14:54:47.000000 dtrx-8.5.0/dtrx.egg-info/dependency_links.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)       40 2022-11-16 14:54:47.000000 dtrx-8.5.0/dtrx.egg-info/entry_points.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)       95 2022-11-16 14:54:47.000000 dtrx-8.5.0/dtrx.egg-info/requires.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)        5 2022-11-16 14:54:47.000000 dtrx-8.5.0/dtrx.egg-info/top_level.txt
--rw-rw-r--   0 noah      (1000) noah      (1000)      240 2022-03-29 02:05:22.000000 dtrx-8.5.0/pyproject.toml
--rw-rw-r--   0 noah      (1000) noah      (1000)     1307 2022-11-16 14:54:47.307850 dtrx-8.5.0/setup.cfg
--rw-rw-r--   0 noah      (1000) noah      (1000)       88 2022-11-16 14:51:03.000000 dtrx-8.5.0/setup.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-04-27 19:18:05.088180 dtrx-8.5.1/
+-rw-rw-r--   0 noah      (1000) noah      (1000)    35147 2021-11-24 20:34:36.000000 dtrx-8.5.1/COPYING
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6689 2023-04-27 19:18:05.088180 dtrx-8.5.1/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)     5571 2022-11-16 14:51:03.000000 dtrx-8.5.1/README.md
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-04-27 19:18:05.088180 dtrx-8.5.1/dtrx/
+-rw-rw-r--   0 noah      (1000) noah      (1000)        0 2022-03-29 02:05:22.000000 dtrx-8.5.1/dtrx/__init__.py
+-rwxrwxr-x   0 noah      (1000) noah      (1000)    61917 2023-04-27 19:16:07.000000 dtrx-8.5.1/dtrx/dtrx.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2023-04-27 19:18:05.088180 dtrx-8.5.1/dtrx.egg-info/
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6689 2023-04-27 19:18:05.000000 dtrx-8.5.1/dtrx.egg-info/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)      251 2023-04-27 19:18:05.000000 dtrx-8.5.1/dtrx.egg-info/SOURCES.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        1 2023-04-27 19:18:05.000000 dtrx-8.5.1/dtrx.egg-info/dependency_links.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       40 2023-04-27 19:18:05.000000 dtrx-8.5.1/dtrx.egg-info/entry_points.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       99 2023-04-27 19:18:05.000000 dtrx-8.5.1/dtrx.egg-info/requires.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        5 2023-04-27 19:18:05.000000 dtrx-8.5.1/dtrx.egg-info/top_level.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)      240 2022-03-29 02:05:22.000000 dtrx-8.5.1/pyproject.toml
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1311 2023-04-27 19:18:05.088180 dtrx-8.5.1/setup.cfg
+-rw-rw-r--   0 noah      (1000) noah      (1000)       88 2022-11-16 14:51:03.000000 dtrx-8.5.1/setup.py
```

### Comparing `dtrx-8.5.0/COPYING` & `dtrx-8.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `dtrx-8.5.0/PKG-INFO` & `dtrx-8.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrx
-Version: 8.5.0
+Version: 8.5.1
 Summary: Script to intelligently extract multiple archive types
 Download-URL: https://github.com/dtrx-py/dtrx
 Author: Brett Smith
 Author-email: brettcsmith@brettcsmith.org
 License: GNU General Public License version 3 or later
 Project-URL: homepage, http://www.brettcsmith.org/2007/dtrx/
 Project-URL: code, https://github.com/dtrx-py/dtrx
```

### Comparing `dtrx-8.5.0/README.md` & `dtrx-8.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dtrx-8.5.0/dtrx/dtrx.py` & `dtrx-8.5.1/dtrx/dtrx.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,31 +63,29 @@
     get_input = raw_input  # noqa: F821
 
 try:
     set
 except NameError:
     from sets import Set as set
 
-VERSION = "8.5.0"
+VERSION = "8.5.1"
 VERSION_BANNER = """dtrx version %s
 Copyright © 2006-2011 Brett Smith <brettcsmith@brettcsmith.org>
 Copyright © 2008 Peter Kelemen <Peter.Kelemen@gmail.com>
 Copyright © 2011 Ville Skyttä <ville.skytta@iki.fi>
 
 This program is free software; you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
 Free Software Foundation; either version 3 of the License, or (at your
 option) any later version.
 
 This program is distributed in the hope that it will be useful, but
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
-Public License for more details.""" % (
-    VERSION,
-)
+Public License for more details.""" % (VERSION,)
 
 # Python3.6 optparse has a hard time parsing this, so ascii transform it
 if sys.version_info[:2] == (3, 6):
     VERSION_BANNER = VERSION_BANNER.encode("ascii", errors="ignore").decode("ascii")
 
 
 MATCHING_DIRECTORY = 1
```

### Comparing `dtrx-8.5.0/dtrx.egg-info/PKG-INFO` & `dtrx-8.5.1/dtrx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrx
-Version: 8.5.0
+Version: 8.5.1
 Summary: Script to intelligently extract multiple archive types
 Download-URL: https://github.com/dtrx-py/dtrx
 Author: Brett Smith
 Author-email: brettcsmith@brettcsmith.org
 License: GNU General Public License version 3 or later
 Project-URL: homepage, http://www.brettcsmith.org/2007/dtrx/
 Project-URL: code, https://github.com/dtrx-py/dtrx
```

### Comparing `dtrx-8.5.0/setup.cfg` & `dtrx-8.5.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 project_urls = 
 	homepage = http://www.brettcsmith.org/2007/dtrx/
 	code = https://github.com/dtrx-py/dtrx
 
 [options]
 packages = dtrx
 install_requires = 
-	platform==unsupported;platform_system=="Windows"
 	subprocess32;python_version < '3.3'
+	unsupported-python==1.0.0;platform_system=="Windows"
 python_requires = >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
 
 [options.entry_points]
 console_scripts = 
 	dtrx = dtrx.dtrx:main
 
 [bdist_wheel]
```

