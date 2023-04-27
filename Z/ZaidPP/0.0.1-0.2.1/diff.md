# Comparing `tmp/ZaidPP-0.0.1.tar.gz` & `tmp/ZaidPP-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZaidPP-0.0.1.tar", last modified: Sat Apr 22 22:41:23 2023, max compression
+gzip compressed data, was "ZaidPP-0.2.1.tar", last modified: Thu Apr 27 12:01:42 2023, max compression
```

## Comparing `ZaidPP-0.0.1.tar` & `ZaidPP-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 22:41:23.799951 ZaidPP-0.0.1/
--rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPP-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      842 2023-04-22 22:41:23.797953 ZaidPP-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPP-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 22:41:23.799951 ZaidPP-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-04-22 22:39:05.000000 ZaidPP-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:41:23.769322 ZaidPP-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-22 22:41:23.777321 ZaidPP-0.0.1/src/ZaidPP/
--rw-rw-rw-   0        0        0     5438 2023-04-22 22:01:40.000000 ZaidPP-0.0.1/src/ZaidPP/ZaidPP.py
--rw-rw-rw-   0        0        0       24 2023-04-22 22:35:06.000000 ZaidPP-0.0.1/src/ZaidPP/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:41:23.795950 ZaidPP-0.0.1/src/ZaidPP.egg-info/
--rw-rw-rw-   0        0        0      842 2023-04-22 22:41:23.000000 ZaidPP-0.0.1/src/ZaidPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-22 22:41:23.000000 ZaidPP-0.0.1/src/ZaidPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 22:41:23.000000 ZaidPP-0.0.1/src/ZaidPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-22 22:41:23.000000 ZaidPP-0.0.1/src/ZaidPP.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.763763 ZaidPP-0.2.1/
+-rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPP-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      842 2023-04-27 12:01:42.763763 ZaidPP-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPP-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 12:01:42.764763 ZaidPP-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-04-27 11:59:03.000000 ZaidPP-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.728177 ZaidPP-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.743169 ZaidPP-0.2.1/src/ZaidPP/
+-rw-rw-rw-   0        0        0    11990 2023-04-27 11:55:22.000000 ZaidPP-0.2.1/src/ZaidPP/ZaidPP.py
+-rw-rw-rw-   0        0        0       24 2023-04-22 22:35:06.000000 ZaidPP-0.2.1/src/ZaidPP/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:01:42.761761 ZaidPP-0.2.1/src/ZaidPP.egg-info/
+-rw-rw-rw-   0        0        0      842 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 12:01:42.000000 ZaidPP-0.2.1/src/ZaidPP.egg-info/top_level.txt
```

### Comparing `ZaidPP-0.0.1/PKG-INFO` & `ZaidPP-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPP
-Version: 0.0.1
+Version: 0.2.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ZaidPP-0.0.1/setup.py` & `ZaidPP-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('instaloder\nuser_agent\nrequests\nuuid')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="ZaidPP",
-    version="0.0.1",
+    version="0.2.1",
     author="Zaid",
     author_email="www710700@gmail.com",
     description="• Scrape Instagram Profile and login Instagram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `ZaidPP-0.0.1/src/ZaidPP.egg-info/PKG-INFO` & `ZaidPP-0.2.1/src/ZaidPP.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPP
-Version: 0.0.1
+Version: 0.2.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

