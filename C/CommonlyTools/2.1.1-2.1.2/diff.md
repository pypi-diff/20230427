# Comparing `tmp/CommonlyTools-2.1.1.tar.gz` & `tmp/CommonlyTools-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-2.1.1.tar", last modified: Thu Apr 27 03:08:35 2023, max compression
+gzip compressed data, was "CommonlyTools-2.1.2.tar", last modified: Thu Apr 27 04:38:33 2023, max compression
```

## Comparing `CommonlyTools-2.1.1.tar` & `CommonlyTools-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 03:08:35.058677 CommonlyTools-2.1.1/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 03:08:35.058677 CommonlyTools-2.1.1/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 03:08:34.000000 CommonlyTools-2.1.1/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      301 2023-04-27 03:08:34.000000 CommonlyTools-2.1.1/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-27 03:08:34.000000 CommonlyTools-2.1.1/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-27 03:08:34.000000 CommonlyTools-2.1.1/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-27 03:08:34.000000 CommonlyTools-2.1.1/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.1.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 03:08:35.058677 CommonlyTools-2.1.1/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:35:28.000000 CommonlyTools-2.1.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 03:08:35.058677 CommonlyTools-2.1.1/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.1.1/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     3359 2023-04-27 03:08:14.000000 CommonlyTools-2.1.1/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      266 2023-04-27 02:56:49.000000 CommonlyTools-2.1.1/commonlytools/error.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-27 03:08:35.058677 CommonlyTools-2.1.1/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      735 2023-04-27 03:08:26.000000 CommonlyTools-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 04:38:33.852852 CommonlyTools-2.1.2/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 04:38:33.840852 CommonlyTools-2.1.2/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 04:38:33.000000 CommonlyTools-2.1.2/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      301 2023-04-27 04:38:33.000000 CommonlyTools-2.1.2/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-27 04:38:33.000000 CommonlyTools-2.1.2/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-27 04:38:33.000000 CommonlyTools-2.1.2/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-27 04:38:33.000000 CommonlyTools-2.1.2/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-27 04:38:33.852852 CommonlyTools-2.1.2/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:35:28.000000 CommonlyTools-2.1.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-27 04:38:33.852852 CommonlyTools-2.1.2/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.1.2/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     3379 2023-04-27 04:36:57.000000 CommonlyTools-2.1.2/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      266 2023-04-27 02:56:49.000000 CommonlyTools-2.1.2/commonlytools/error.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-27 04:38:33.852852 CommonlyTools-2.1.2/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-04-27 04:37:04.000000 CommonlyTools-2.1.2/setup.py
```

### Comparing `CommonlyTools-2.1.1/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.1.2/CommonlyTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.1.1
+Version: 2.1.2
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.1.1/LICENSE` & `CommonlyTools-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.1.1/PKG-INFO` & `CommonlyTools-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.1.1
+Version: 2.1.2
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.1.1/README.md` & `CommonlyTools-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.1.1/commonlytools/discohook.py` & `CommonlyTools-2.1.2/commonlytools/discohook.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class Embed:
     def __init__(self, title:str=None, description:str=None, timestamp:datetime.datetime=None, color=0xffffff, colour=0xffffff):
         self._title=title
         self._description=description
         _colour=color or colour
         _colour=str(_colour)
-        if _colour.startswith("#" or "0x"):
+        if _colour.startswith("#") or _colour.startswith("0x"):
             if _colour.startswith("#"):
                 _colour.replace("#", "0x")
         else:
             raise ColourError("Invalid color hex!\n")
         self._colour=int(_colour, 10)
         if timestamp != None:
             self._timestamp=f"{timestamp.year}-{timestamp.month}-{timestamp.day}T{timestamp.hour}:{timestamp.minute}:{timestamp.second}.{timestamp.microsecond}Z"
```

### Comparing `CommonlyTools-2.1.1/setup.py` & `CommonlyTools-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="2.1.1",
+    version="2.1.2",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```

