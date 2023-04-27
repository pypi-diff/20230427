# Comparing `tmp/CommonlyTools-2.0.9.tar.gz` & `tmp/CommonlyTools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-2.0.9.tar", last modified: Thu Apr 27 02:50:02 2023, max compression
+gzip compressed data, was "CommonlyTools-2.1.0.tar", last modified: Thu Apr 27 03:02:10 2023, max compression
```

## Comparing `CommonlyTools-2.0.9.tar` & `CommonlyTools-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 02:50:02.975760 CommonlyTools-2.0.9/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 02:50:02.975760 CommonlyTools-2.0.9/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 02:50:02.000000 CommonlyTools-2.0.9/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      301 2023-04-27 02:50:02.000000 CommonlyTools-2.0.9/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-27 02:50:02.000000 CommonlyTools-2.0.9/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-27 02:50:02.000000 CommonlyTools-2.0.9/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-27 02:50:02.000000 CommonlyTools-2.0.9/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.9/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 02:50:02.975760 CommonlyTools-2.0.9/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:35:28.000000 CommonlyTools-2.0.9/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 02:50:02.975760 CommonlyTools-2.0.9/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.9/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     3299 2023-04-27 02:49:35.000000 CommonlyTools-2.0.9/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      266 2023-04-27 02:29:07.000000 CommonlyTools-2.0.9/commonlytools/error.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-27 02:50:02.975760 CommonlyTools-2.0.9/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      735 2023-04-27 02:49:52.000000 CommonlyTools-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 03:02:10.123052 CommonlyTools-2.1.0/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 03:02:10.115052 CommonlyTools-2.1.0/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 03:02:09.000000 CommonlyTools-2.1.0/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      301 2023-04-27 03:02:10.000000 CommonlyTools-2.1.0/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-27 03:02:09.000000 CommonlyTools-2.1.0/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-27 03:02:09.000000 CommonlyTools-2.1.0/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-27 03:02:09.000000 CommonlyTools-2.1.0/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 03:02:10.123052 CommonlyTools-2.1.0/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:35:28.000000 CommonlyTools-2.1.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 03:02:10.115052 CommonlyTools-2.1.0/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.1.0/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     3340 2023-04-27 03:00:07.000000 CommonlyTools-2.1.0/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      266 2023-04-27 02:56:49.000000 CommonlyTools-2.1.0/commonlytools/error.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-27 03:02:10.131052 CommonlyTools-2.1.0/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-04-27 03:00:17.000000 CommonlyTools-2.1.0/setup.py
```

### Comparing `CommonlyTools-2.0.9/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.1.0/CommonlyTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.9
+Version: 2.1.0
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.9/LICENSE` & `CommonlyTools-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.9/PKG-INFO` & `CommonlyTools-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.9
+Version: 2.1.0
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.9/README.md` & `CommonlyTools-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.9/commonlytools/discohook.py` & `CommonlyTools-2.1.0/commonlytools/discohook.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 class Embed:
     def __init__(self, title:str=None, description:str=None, timestamp:datetime.datetime=None, color=0xffffff, colour=0xffffff):
         self._title=title
         self._description=description
         _colour=str(color) or str(colour)
         if _colour.startswith("#" or "0x"):
-            _colour.replace("#", "0x", 1)
+            if _colour.startswith("#"):
+                _colour.replace("#", "0x")
         else:
             raise ColourError("Invalid color hex!\n")
         self._colour=int(_colour, 10)
         if timestamp != None:
             self._timestamp=f"{timestamp.year}-{timestamp.month}-{timestamp.day}T{timestamp.hour}:{timestamp.minute}:{timestamp.second}.{timestamp.microsecond}Z"
         else:
             self._timestamp=None
```

### Comparing `CommonlyTools-2.0.9/setup.py` & `CommonlyTools-2.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="2.0.9",
+    version="2.1.0",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```

