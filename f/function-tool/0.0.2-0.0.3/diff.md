# Comparing `tmp/function_tool-0.0.2.tar.gz` & `tmp/function_tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function_tool-0.0.2.tar", last modified: Mon Apr 17 06:54:07 2023, max compression
+gzip compressed data, was "function_tool-0.0.3.tar", last modified: Thu Apr 27 02:54:34 2023, max compression
```

## Comparing `function_tool-0.0.2.tar` & `function_tool-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:54:07.416174 function_tool-0.0.2/
--rw-r--r--   0 fhss       (501) staff       (20)     1086 2023-04-17 06:09:13.000000 function_tool-0.0.2/LICENSE
--rw-r--r--   0 fhss       (501) staff       (20)     1220 2023-04-17 06:54:07.415857 function_tool-0.0.2/PKG-INFO
--rw-r--r--   0 fhss       (501) staff       (20)      271 2023-04-17 06:12:41.000000 function_tool-0.0.2/README.md
-drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:54:07.414581 function_tool-0.0.2/function_tool.egg-info/
--rw-r--r--   0 fhss       (501) staff       (20)     1220 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/PKG-INFO
--rw-r--r--   0 fhss       (501) staff       (20)      243 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/SOURCES.txt
--rw-r--r--   0 fhss       (501) staff       (20)        1 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/dependency_links.txt
--rw-r--r--   0 fhss       (501) staff       (20)       22 2023-04-17 06:54:07.000000 function_tool-0.0.2/function_tool.egg-info/top_level.txt
-drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-17 06:54:07.415330 function_tool-0.0.2/function_tool_derrick/
--rw-r--r--   0 fhss       (501) staff       (20)     1721 2023-04-17 05:58:22.000000 function_tool-0.0.2/function_tool_derrick/UsualTool.py
--rw-r--r--   0 fhss       (501) staff       (20)      151 2023-04-17 04:54:21.000000 function_tool-0.0.2/function_tool_derrick/__init__.py
--rw-r--r--   0 fhss       (501) staff       (20)       38 2023-04-17 06:54:07.416324 function_tool-0.0.2/setup.cfg
--rw-r--r--   0 fhss       (501) staff       (20)     1341 2023-04-17 06:53:38.000000 function_tool-0.0.2/setup.py
+drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-27 02:54:34.438014 function_tool-0.0.3/
+-rw-r--r--   0 fhss       (501) staff       (20)     1086 2023-04-27 02:28:56.000000 function_tool-0.0.3/LICENSE
+-rw-r--r--   0 fhss       (501) staff       (20)     2029 2023-04-27 02:54:34.437739 function_tool-0.0.3/PKG-INFO
+-rw-r--r--   0 fhss       (501) staff       (20)      936 2023-04-27 02:46:55.000000 function_tool-0.0.3/README.md
+drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-27 02:54:34.436349 function_tool-0.0.3/function_tool.egg-info/
+-rw-r--r--   0 fhss       (501) staff       (20)     2029 2023-04-27 02:54:34.000000 function_tool-0.0.3/function_tool.egg-info/PKG-INFO
+-rw-r--r--   0 fhss       (501) staff       (20)      243 2023-04-27 02:54:34.000000 function_tool-0.0.3/function_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 fhss       (501) staff       (20)        1 2023-04-27 02:54:34.000000 function_tool-0.0.3/function_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 fhss       (501) staff       (20)       22 2023-04-27 02:54:34.000000 function_tool-0.0.3/function_tool.egg-info/top_level.txt
+drwxr-xr-x   0 fhss       (501) staff       (20)        0 2023-04-27 02:54:34.437272 function_tool-0.0.3/function_tool_derrick/
+-rw-r--r--   0 fhss       (501) staff       (20)     3108 2023-04-27 02:48:20.000000 function_tool-0.0.3/function_tool_derrick/UsualTool.py
+-rw-r--r--   0 fhss       (501) staff       (20)      151 2023-04-27 02:29:02.000000 function_tool-0.0.3/function_tool_derrick/__init__.py
+-rw-r--r--   0 fhss       (501) staff       (20)       38 2023-04-27 02:54:34.438123 function_tool-0.0.3/setup.cfg
+-rw-r--r--   0 fhss       (501) staff       (20)     1341 2023-04-27 02:49:12.000000 function_tool-0.0.3/setup.py
```

### Comparing `function_tool-0.0.2/LICENSE` & `function_tool-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `function_tool-0.0.2/setup.py` & `function_tool-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="function_tool",
-    version='0.0.2',
+    version='0.0.3',
     author="DerrickChiu",
     author_email="chiull@foxmail.com",
     description="some usual tool with class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://gitee.com/DerrickChiu/function_tool.git",
```

