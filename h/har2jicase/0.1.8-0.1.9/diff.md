# Comparing `tmp/har2jicase-0.1.8.tar.gz` & `tmp/har2jicase-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2jicase-0.1.8.tar", last modified: Sun Apr 23 10:37:34 2023, max compression
+gzip compressed data, was "har2jicase-0.1.9.tar", last modified: Thu Apr 27 01:31:28 2023, max compression
```

## Comparing `har2jicase-0.1.8.tar` & `har2jicase-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.276045 har2jicase-0.1.8/
--rw-rw-rw-   0        0        0      518 2023-04-23 10:37:34.276045 har2jicase-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.271043 har2jicase-0.1.8/har2jicase.egg-info/
--rw-rw-rw-   0        0        0      518 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har2jicase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.8/har2jicase.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.274046 har2jicase-0.1.8/har_to_case/
--rw-rw-rw-   0        0        0      260 2023-04-23 10:37:34.000000 har2jicase-0.1.8/har_to_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:37:34.275046 har2jicase-0.1.8/har_to_case/common/
--rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.8/har_to_case/common/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.8/har_to_case/common/tools.py
--rw-rw-rw-   0        0        0     1383 2023-04-21 09:06:51.000000 har2jicase-0.1.8/har_to_case/main.py
--rw-rw-rw-   0        0        0     8756 2023-04-23 10:36:59.000000 har2jicase-0.1.8/har_to_case/parse_har.py
--rw-rw-rw-   0        0        0       42 2023-04-23 10:37:34.277045 har2jicase-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     4102 2023-04-23 10:37:23.000000 har2jicase-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:31:28.413615 har2jicase-0.1.9/
+-rw-rw-rw-   0        0        0      518 2023-04-27 01:31:28.413615 har2jicase-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-04-21 03:08:02.000000 har2jicase-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 01:31:28.407902 har2jicase-0.1.9/har2jicase.egg-info/
+-rw-rw-rw-   0        0        0      518 2023-04-27 01:31:28.000000 har2jicase-0.1.9/har2jicase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-27 01:31:28.000000 har2jicase-0.1.9/har2jicase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 01:31:28.000000 har2jicase-0.1.9/har2jicase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-27 01:31:28.000000 har2jicase-0.1.9/har2jicase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-27 01:31:28.000000 har2jicase-0.1.9/har2jicase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 01:31:28.000000 har2jicase-0.1.9/har2jicase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 04:57:38.000000 har2jicase-0.1.9/har2jicase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-27 01:31:28.411045 har2jicase-0.1.9/har_to_case/
+-rw-rw-rw-   0        0        0      260 2023-04-27 01:31:28.000000 har2jicase-0.1.9/har_to_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 01:31:28.412599 har2jicase-0.1.9/har_to_case/common/
+-rw-rw-rw-   0        0        0      204 2022-10-26 08:00:20.000000 har2jicase-0.1.9/har_to_case/common/__init__.py
+-rw-rw-rw-   0        0        0     3070 2023-04-20 06:19:26.000000 har2jicase-0.1.9/har_to_case/common/tools.py
+-rw-rw-rw-   0        0        0     1383 2023-04-21 09:06:51.000000 har2jicase-0.1.9/har_to_case/main.py
+-rw-rw-rw-   0        0        0     8756 2023-04-27 01:30:02.000000 har2jicase-0.1.9/har_to_case/parse_har.py
+-rw-rw-rw-   0        0        0       42 2023-04-27 01:31:28.413615 har2jicase-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     4102 2023-04-27 01:31:27.000000 har2jicase-0.1.9/setup.py
```

### Comparing `har2jicase-0.1.8/PKG-INFO` & `har2jicase-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.8
+Version: 0.1.9
 Summary: 将浏览器录制的har文件转换为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.8/har2jicase.egg-info/PKG-INFO` & `har2jicase-0.1.9/har2jicase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2jicase
-Version: 0.1.8
+Version: 0.1.9
 Summary: 将浏览器录制的har文件转换为极星测试框架的YAML测试用例
 Home-page: 
 Author: Captain Ji
 Author-email: qing.ji@extremevision.com.cn
 License: MIT
 Keywords: har json compare comparison case yaml yml
 Requires-Python: >=3.6.13
```

### Comparing `har2jicase-0.1.8/har_to_case/common/tools.py` & `har2jicase-0.1.9/har_to_case/common/tools.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.8/har_to_case/main.py` & `har2jicase-0.1.9/har_to_case/main.py`

 * *Files identical despite different names*

### Comparing `har2jicase-0.1.8/har_to_case/parse_har.py` & `har2jicase-0.1.9/har_to_case/parse_har.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             validate_contains = ''
             if isinstance(data, dict):
                 for key in data.keys():
                     if validate_contains == '':
                         validate_contains = key
                     else:
                         validate_contains = validate_contains + '-' + key
-            elif isinstance(data, str):
+            elif len(data.keys()) <= 1:
                 validate_contains = 'data'
             else:
                 for item in data:
                     # todo: data中的data继续解析，后续看需求再定
                     if isinstance(item, dict):
                         pass
                     else:
```

### Comparing `har2jicase-0.1.8/setup.py` & `har2jicase-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import io
 import os
 import sys
 from shutil import rmtree
 from setuptools import find_packages, setup, Command
 
 # 写入自己的内容
-VERSION = '0.1.8'  # 为项目指定目前的版本号
+VERSION = '0.1.9'  # 为项目指定目前的版本号
 # 项目目录
 PROJECT_PATH = 'har_to_case'
 
 NAME = 'har2jicase'  # 项目名
 DESCRIPTION = '将浏览器录制的har文件转换为极星测试框架的YAML测试用例'
 KEYWORDS = 'har json compare comparison case yaml yml'
 AUTHOR = 'Captain Ji'
```

