# Comparing `tmp/SDTcloud-0.0.1.tar.gz` & `tmp/SDTcloud-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.0.1.tar", last modified: Thu Apr 27 00:38:21 2023, max compression
+gzip compressed data, was "SDTcloud-0.0.2.tar", last modified: Thu Apr 27 00:52:36 2023, max compression
```

## Comparing `SDTcloud-0.0.1.tar` & `SDTcloud-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:38:21.441410 SDTcloud-0.0.1/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-27 00:38:21.441264 SDTcloud-0.0.1/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.1/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:38:21.440209 SDTcloud-0.0.1/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.1/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)     4394 2023-04-27 00:36:40.000000 SDTcloud-0.0.1/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:38:21.441025 SDTcloud-0.0.1/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-27 00:38:21.000000 SDTcloud-0.0.1/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-04-27 00:38:21.000000 SDTcloud-0.0.1/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-04-27 00:38:21.000000 SDTcloud-0.0.1/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-04-27 00:38:21.000000 SDTcloud-0.0.1/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-04-27 00:38:21.441448 SDTcloud-0.0.1/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-04-27 00:38:20.000000 SDTcloud-0.0.1/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:52:36.027404 SDTcloud-0.0.2/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-27 00:52:36.027257 SDTcloud-0.0.2/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.2/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:52:36.026272 SDTcloud-0.0.2/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.2/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)     4394 2023-04-27 00:52:06.000000 SDTcloud-0.0.2/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-27 00:52:36.027053 SDTcloud-0.0.2/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-04-27 00:52:35.000000 SDTcloud-0.0.2/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-04-27 00:52:36.000000 SDTcloud-0.0.2/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-04-27 00:52:35.000000 SDTcloud-0.0.2/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-04-27 00:52:35.000000 SDTcloud-0.0.2/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-04-27 00:52:36.027442 SDTcloud-0.0.2/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-04-27 00:52:15.000000 SDTcloud-0.0.2/setup.py
```

### Comparing `SDTcloud-0.0.1/SDTcloud/sdtcloud.py` & `SDTcloud-0.0.2/SDTcloud/sdtcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import pandas as pd 
 import getpass
 
 
 class SDTcloud():
     def __init__(self):
-        self.url = "http://10.110.31.15:31779"
+        self.url = "http://25.10.133.65:31779"
         self.userId = input("ID: ")
         self.userPassword = getpass.getpass("PW: ")
         self.userToken = f"Bearer {self.login(self.userId, self.userPassword)}"
 
     # 로그인
     def login(self, 
             id: str,
```

### Comparing `SDTcloud-0.0.1/setup.py` & `SDTcloud-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.0.1",
+    version="0.0.2",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

