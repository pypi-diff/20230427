# Comparing `tmp/alida-arg-parser-0.0.8.tar.gz` & `tmp/alida-arg-parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alida-arg-parser-0.0.8.tar", last modified: Wed Mar 30 08:22:14 2022, max compression
+gzip compressed data, was "dist/alida-arg-parser-0.0.9.tar", last modified: Tue Apr 12 15:39:26 2022, max compression
```

## Comparing `alida-arg-parser-0.0.8.tar` & `alida-arg-parser-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-30 08:22:14.085716 alida-arg-parser-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      425 2022-03-30 08:22:14.085716 alida-arg-parser-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-30 08:22:14.084716 alida-arg-parser-0.0.8/alida_arg_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      425 2022-03-30 08:22:13.000000 alida-arg-parser-0.0.8/alida_arg_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      568 2022-03-30 08:22:14.000000 alida-arg-parser-0.0.8/alida_arg_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-30 08:22:13.000000 alida-arg-parser-0.0.8/alida_arg_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-03-30 08:22:13.000000 alida-arg-parser-0.0.8/alida_arg_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-03-30 08:22:13.000000 alida-arg-parser-0.0.8/alida_arg_parser.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-30 08:22:14.084716 alida-arg-parser-0.0.8/alidaargparser/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/generator.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/model.py
--rw-rw-rw-   0 root         (0) root         (0)     6459 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/property.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-30 08:22:14.085716 alida-arg-parser-0.0.8/alidaargparser/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15372 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/templates/spark_3_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)     4835 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/templates/template.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/translation_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/alidaargparser/type_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-03-30 08:22:14.085716 alida-arg-parser-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2022-03-30 08:22:05.000000 alida-arg-parser-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 15:39:26.084878 alida-arg-parser-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      425 2022-04-12 15:39:26.084878 alida-arg-parser-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       45 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 15:39:26.083878 alida-arg-parser-0.0.9/alida_arg_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      425 2022-04-12 15:39:25.000000 alida-arg-parser-0.0.9/alida_arg_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      568 2022-04-12 15:39:26.000000 alida-arg-parser-0.0.9/alida_arg_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-12 15:39:25.000000 alida-arg-parser-0.0.9/alida_arg_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-04-12 15:39:25.000000 alida-arg-parser-0.0.9/alida_arg_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-04-12 15:39:25.000000 alida-arg-parser-0.0.9/alida_arg_parser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 15:39:26.083878 alida-arg-parser-0.0.9/alidaargparser/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     6459 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/property.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 15:39:26.084878 alida-arg-parser-0.0.9/alidaargparser/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15372 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/templates/spark_3_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/templates/template.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/translation_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/alidaargparser/type_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2022-04-12 15:39:26.084878 alida-arg-parser-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2022-04-12 15:39:14.000000 alida-arg-parser-0.0.9/setup.py
```

### Comparing `alida-arg-parser-0.0.8/alida_arg_parser.egg-info/SOURCES.txt` & `alida-arg-parser-0.0.9/alida_arg_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alida-arg-parser-0.0.8/alidaargparser/generator.py` & `alida-arg-parser-0.0.9/alidaargparser/generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from jinja2 import Template, defaults
 import jinja2
 import json
 from .translation_dictionary import translation
 import os
 
 
-templates = {"default": "template.py", "spark:3.2.0":"spark_3_2_0.py"}
+templates = {   "default": "template.py", 
+                "spark:3.2.0":"spark_3_2_0.py", 
+                "spark:3.2.1":"spark_3_2_0.py"}
 
 # Load jinja template
 def get_template(path):
     path = os.path.join(os.path.dirname(os.path.realpath(__file__)), path)
     templateLoader = jinja2.FileSystemLoader(os.path.dirname(path))
     templateEnv = jinja2.Environment(loader=templateLoader)
     return templateEnv.get_template(name=os.path.basename(path))
```

### Comparing `alida-arg-parser-0.0.8/alidaargparser/parser.py` & `alida-arg-parser-0.0.9/alidaargparser/parser.py`

 * *Files identical despite different names*

### Comparing `alida-arg-parser-0.0.8/alidaargparser/property.py` & `alida-arg-parser-0.0.9/alidaargparser/property.py`

 * *Files identical despite different names*

### Comparing `alida-arg-parser-0.0.8/alidaargparser/templates/spark_3_2_0.py` & `alida-arg-parser-0.0.9/alidaargparser/templates/spark_3_2_0.py`

 * *Files identical despite different names*

### Comparing `alida-arg-parser-0.0.8/alidaargparser/templates/template.py` & `alida-arg-parser-0.0.9/alidaargparser/templates/template.py`

 * *Files identical despite different names*

### Comparing `alida-arg-parser-0.0.8/setup.py` & `alida-arg-parser-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="alida-arg-parser",
-    version="0.0.8",
+    version="0.0.9",
     author="Alida research team",
     author_email="salvatore.cipolla@eng.it",
     description="Python argparser modified for Alida services",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

