# Comparing `tmp/methodism-0.0.2.tar.gz` & `tmp/methodism-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.0.2.tar", last modified: Thu Apr 27 08:01:24 2023, max compression
+gzip compressed data, was "methodism-0.0.3.tar", last modified: Thu Apr 27 08:31:35 2023, max compression
```

## Comparing `methodism-0.0.2.tar` & `methodism-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 08:01:24.531341 methodism-0.0.2/
--rw-rw-rw-   0        0        0     2895 2023-04-27 08:01:24.531341 methodism-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2406 2023-04-27 07:25:46.000000 methodism-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 08:01:24.513329 methodism-0.0.2/base/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.2/base/__init__.py
--rw-rw-rw-   0        0        0     3559 2023-04-27 07:18:17.000000 methodism-0.0.2/base/costumizing.py
--rw-rw-rw-   0        0        0      708 2023-04-26 06:02:02.000000 methodism-0.0.2/base/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.2/base/error_messages.py
--rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.2/base/helper.py
--rw-rw-rw-   0        0        0     3466 2023-04-27 07:09:21.000000 methodism-0.0.2/base/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:01:24.530340 methodism-0.0.2/methodism.egg-info/
--rw-rw-rw-   0        0        0     2895 2023-04-27 08:01:24.000000 methodism-0.0.2/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-27 08:01:24.000000 methodism-0.0.2/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 08:01:24.000000 methodism-0.0.2/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 08:01:24.000000 methodism-0.0.2/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      610 2023-04-27 08:00:50.000000 methodism-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-04-27 08:01:24.542355 methodism-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 08:31:35.269076 methodism-0.0.3/
+-rw-rw-rw-   0        0        0     2881 2023-04-27 08:31:35.269076 methodism-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2399 2023-04-27 08:27:37.000000 methodism-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 08:31:35.253436 methodism-0.0.3/base/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.3/base/__init__.py
+-rw-rw-rw-   0        0        0     3559 2023-04-27 07:18:17.000000 methodism-0.0.3/base/costumizing.py
+-rw-rw-rw-   0        0        0      708 2023-04-26 06:02:02.000000 methodism-0.0.3/base/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.3/base/error_messages.py
+-rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.3/base/helper.py
+-rw-rw-rw-   0        0        0     3466 2023-04-27 07:09:21.000000 methodism-0.0.3/base/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:31:35.269076 methodism-0.0.3/methodism.egg-info/
+-rw-rw-rw-   0        0        0     2881 2023-04-27 08:31:35.000000 methodism-0.0.3/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-27 08:31:35.000000 methodism-0.0.3/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 08:31:35.000000 methodism-0.0.3/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 08:31:35.000000 methodism-0.0.3/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-04-27 08:31:04.000000 methodism-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-04-27 08:31:35.284702 methodism-0.0.3/setup.cfg
```

### Comparing `methodism-0.0.2/PKG-INFO` & `methodism-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.2
+Version: 0.0.3
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
-Project-URL: Homepage, https://github.com/xudoyberdi123/Methodism
+Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Methodism
@@ -73,13 +73,13 @@
             salom.dunyo
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['salom.dunyo']
      """
 ```
 
-## [GitHub](https://github.com/xudoyberdi123/Methodism) Manba 
+## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
```

### Comparing `methodism-0.0.2/README.md` & `methodism-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,13 +59,13 @@
             salom.dunyo
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['salom.dunyo']
      """
 ```
 
-## [GitHub](https://github.com/xudoyberdi123/Methodism) Manba 
+## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
```

### Comparing `methodism-0.0.2/base/costumizing.py` & `methodism-0.0.3/base/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.2/base/decors.py` & `methodism-0.0.3/base/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.2/base/error_messages.py` & `methodism-0.0.3/base/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.2/base/helper.py` & `methodism-0.0.3/base/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.2/base/main.py` & `methodism-0.0.3/base/main.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.2/methodism.egg-info/PKG-INFO` & `methodism-0.0.3/methodism.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.2
+Version: 0.0.3
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
-Project-URL: Homepage, https://github.com/xudoyberdi123/Methodism
+Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Methodism
@@ -73,13 +73,13 @@
             salom.dunyo
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['salom.dunyo']
      """
 ```
 
-## [GitHub](https://github.com/xudoyberdi123/Methodism) Manba 
+## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
```

### Comparing `methodism-0.0.2/pyproject.toml` & `methodism-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/xudoyberdi123/Methodism"
+"Homepage" = "https://github.com/xudikk/Methodism"
```

### Comparing `methodism-0.0.2/setup.cfg` & `methodism-0.0.3/setup.cfg`

 * *Files identical despite different names*

