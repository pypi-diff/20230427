# Comparing `tmp/pystructs3-0.0.3.tar.gz` & `tmp/pystructs3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructs3-0.0.3.tar", last modified: Mon Apr 24 00:11:15 2023, max compression
+gzip compressed data, was "pystructs3-0.0.4.tar", last modified: Thu Apr 27 05:17:19 2023, max compression
```

## Comparing `pystructs3-0.0.3.tar` & `pystructs3-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.3/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-24 00:11:15.760621 pystructs3-0.0.3/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.3/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/pystructs/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      681 2023-04-21 06:27:06.000000 pystructs3-0.0.3/pystructs/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8814 2023-04-23 23:27:43.000000 pystructs3-0.0.3/pystructs/base.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1928 2023-04-19 00:40:15.000000 pystructs3-0.0.3/pystructs/codec.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2798 2023-04-21 06:25:07.000000 pystructs3-0.0.3/pystructs/list.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/pystructs/struct/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      332 2023-04-19 00:33:47.000000 pystructs3-0.0.3/pystructs/struct/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3097 2023-04-19 00:21:42.000000 pystructs3-0.0.3/pystructs/struct/fields.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5133 2023-04-21 07:24:30.000000 pystructs3-0.0.3/pystructs/struct/struct.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/pystructs3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      355 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       30 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-24 00:11:15.760621 pystructs3-0.0.3/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      763 2023-04-24 00:10:56.000000 pystructs3-0.0.3/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.4/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-27 05:17:19.737077 pystructs3-0.0.4/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.4/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/pystructs/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      681 2023-04-21 06:27:06.000000 pystructs3-0.0.4/pystructs/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8814 2023-04-23 23:27:43.000000 pystructs3-0.0.4/pystructs/base.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1928 2023-04-19 00:40:15.000000 pystructs3-0.0.4/pystructs/codec.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2798 2023-04-21 06:25:07.000000 pystructs3-0.0.4/pystructs/list.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/pystructs/struct/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      332 2023-04-19 00:33:47.000000 pystructs3-0.0.4/pystructs/struct/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3060 2023-04-27 05:16:33.000000 pystructs3-0.0.4/pystructs/struct/fields.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5133 2023-04-21 07:24:30.000000 pystructs3-0.0.4/pystructs/struct/struct.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/pystructs3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      355 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       30 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-27 05:17:19.737077 pystructs3-0.0.4/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      763 2023-04-27 05:16:52.000000 pystructs3-0.0.4/setup.py
```

### Comparing `pystructs3-0.0.3/LICENSE` & `pystructs3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.3/PKG-INFO` & `pystructs3-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystructs3-0.0.3/README.md` & `pystructs3-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.3/pystructs/__init__.py` & `pystructs3-0.0.4/pystructs/__init__.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.3/pystructs/base.py` & `pystructs3-0.0.4/pystructs/base.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.3/pystructs/codec.py` & `pystructs3-0.0.4/pystructs/codec.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.3/pystructs/list.py` & `pystructs3-0.0.4/pystructs/list.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.3/pystructs/struct/fields.py` & `pystructs3-0.0.4/pystructs/struct/fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Struct Field Implementation
 """
 from dataclasses import InitVar, MISSING, dataclass
+from dataclasses import field as datafield
 from dataclasses import Field as DataField
 from typing import *
 from typing_extensions import Self
 
 from .. import Codec, Int32
 
 #** Variables **#
@@ -85,23 +86,21 @@
 class Spec:
     default:         Any                         = MISSING
     default_factory: Optional[Callable[[], Any]] = None
     init:            Optional[bool]              = None
     repr:            bool                        = True
     hash:            Optional[bool]              = None
     compare:         bool                        = True
-    metadata:        Optional[Mapping[Any, Any]] = None
-    kw_only:         bool                        = False
- 
+    kwargs:          dict                        = datafield(default_factory=dict)
+
     def compile(self, name: str, anno: Type[Codec]) -> Tuple[Field, DataField]:
         """compile field-spec into official field"""
         init = anno.init if self.init is None else anno.init
-        return (Field(name, anno, init), DataField(
+        return (Field(name, anno, init), datafield(
             default=not_missing(self.default, anno.default),
             default_factory=self.default_factory or MISSING, #type: ignore
             init=init,
             repr=self.repr,
             hash=self.hash,
             compare=self.compare,
-            metadata=self.metadata or {},
-            kw_only=self.kw_only,
+            **self.kwargs,
         ))
```

### Comparing `pystructs3-0.0.3/pystructs/struct/struct.py` & `pystructs3-0.0.4/pystructs/struct/struct.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.3/pystructs3.egg-info/PKG-INFO` & `pystructs3-0.0.4/pystructs3.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystructs3-0.0.3/setup.py` & `pystructs3-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pystructs3',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pystruct',
     description="Dataclass-Like Serialization Helpers for More Complex Data-Types",
     long_description=readme,
     long_description_content_type="text/markdown",
```

