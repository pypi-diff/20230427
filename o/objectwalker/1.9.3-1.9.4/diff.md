# Comparing `tmp/objectwalker-1.9.3.tar.gz` & `tmp/objectwalker-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-1.9.3.tar", last modified: Wed Apr 26 19:14:43 2023, max compression
+gzip compressed data, was "objectwalker-1.9.4.tar", last modified: Thu Apr 27 09:34:02 2023, max compression
```

## Comparing `objectwalker-1.9.3.tar` & `objectwalker-1.9.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 19:14:43.035933 objectwalker-1.9.3/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-1.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      457 2023-04-26 19:14:43.035933 objectwalker-1.9.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-26 14:54:45.000000 objectwalker-1.9.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 19:14:43.035933 objectwalker-1.9.3/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-1.9.3/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7861 2023-04-26 19:14:32.000000 objectwalker-1.9.3/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     4604 2023-04-26 19:14:01.000000 objectwalker-1.9.3/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 19:14:43.035933 objectwalker-1.9.3/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)     1343 2023-04-26 18:24:47.000000 objectwalker-1.9.3/objectwalker/filters/EmptyFilter.py
--rw-rw-r--   0 root         (0) root         (0)      969 2023-04-26 18:23:59.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectNameContains.py
--rw-rw-r--   0 root         (0) root         (0)      976 2023-04-26 18:25:13.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectNameEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)      959 2023-04-26 18:27:27.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectNameEquals.py
--rw-rw-r--   0 root         (0) root         (0)      988 2023-04-26 18:27:17.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectNameStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      962 2023-04-26 18:37:26.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectValueContains.py
--rw-rw-r--   0 root         (0) root         (0)      969 2023-04-26 18:37:41.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectValueEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)      952 2023-04-26 18:38:33.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectValueEquals.py
--rw-rw-r--   0 root         (0) root         (0)      981 2023-04-26 18:40:13.000000 objectwalker-1.9.3/objectwalker/filters/FilterObjectValueStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      931 2023-04-26 18:27:17.000000 objectwalker-1.9.3/objectwalker/filters/FilterPathContains.py
--rw-rw-r--   0 root         (0) root         (0)      938 2023-04-26 18:27:08.000000 objectwalker-1.9.3/objectwalker/filters/FilterPathEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)      948 2023-04-26 18:27:04.000000 objectwalker-1.9.3/objectwalker/filters/FilterPathStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      696 2023-04-26 18:26:23.000000 objectwalker-1.9.3/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
--rw-rw-r--   0 root         (0) root         (0)      643 2023-04-26 18:26:48.000000 objectwalker-1.9.3/objectwalker/filters/FilterTypeIsMethodWrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2459 2023-04-26 18:43:39.000000 objectwalker-1.9.3/objectwalker/filters/FilterTypeIsModule.py
--rw-rw-r--   0 root         (0) root         (0)     1190 2023-04-26 18:40:20.000000 objectwalker-1.9.3/objectwalker/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 19:14:43.035933 objectwalker-1.9.3/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      457 2023-04-26 19:14:43.000000 objectwalker-1.9.3/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1050 2023-04-26 19:14:43.000000 objectwalker-1.9.3/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 19:14:43.000000 objectwalker-1.9.3/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-26 19:14:43.000000 objectwalker-1.9.3/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 19:14:43.000000 objectwalker-1.9.3/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-1.9.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 19:14:43.035933 objectwalker-1.9.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1165 2023-04-26 19:14:32.000000 objectwalker-1.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:34:02.951119 objectwalker-1.9.4/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-1.9.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      457 2023-04-27 09:34:02.951119 objectwalker-1.9.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1642 2023-04-26 14:54:45.000000 objectwalker-1.9.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:34:02.947119 objectwalker-1.9.4/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-1.9.4/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7861 2023-04-27 09:33:44.000000 objectwalker-1.9.4/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)    10097 2023-04-27 09:30:28.000000 objectwalker-1.9.4/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:34:02.951119 objectwalker-1.9.4/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1659 2023-04-27 08:56:31.000000 objectwalker-1.9.4/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)      969 2023-04-26 18:23:59.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)      976 2023-04-26 18:25:13.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      959 2023-04-26 18:27:27.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)      988 2023-04-26 18:27:17.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      962 2023-04-26 18:37:26.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectValueContains.py
+-rw-rw-r--   0 root         (0) root         (0)      969 2023-04-26 18:37:41.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectValueEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      952 2023-04-26 18:38:33.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectValueEquals.py
+-rw-rw-r--   0 root         (0) root         (0)      981 2023-04-26 18:40:13.000000 objectwalker-1.9.4/objectwalker/filters/FilterObjectValueStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      931 2023-04-26 18:27:17.000000 objectwalker-1.9.4/objectwalker/filters/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)      938 2023-04-26 18:27:08.000000 objectwalker-1.9.4/objectwalker/filters/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      948 2023-04-26 18:27:04.000000 objectwalker-1.9.4/objectwalker/filters/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      696 2023-04-26 18:26:23.000000 objectwalker-1.9.4/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      643 2023-04-26 18:26:48.000000 objectwalker-1.9.4/objectwalker/filters/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2627 2023-04-27 08:56:53.000000 objectwalker-1.9.4/objectwalker/filters/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)     1190 2023-04-26 18:40:20.000000 objectwalker-1.9.4/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:34:02.947119 objectwalker-1.9.4/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-04-27 09:34:02.000000 objectwalker-1.9.4/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-04-27 09:34:02.000000 objectwalker-1.9.4/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:34:02.000000 objectwalker-1.9.4/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-27 09:34:02.000000 objectwalker-1.9.4/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 09:34:02.000000 objectwalker-1.9.4/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-1.9.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 09:34:02.951119 objectwalker-1.9.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1165 2023-04-27 09:33:39.000000 objectwalker-1.9.4/setup.py
```

### Comparing `objectwalker-1.9.3/README.md` & `objectwalker-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/__main__.py` & `objectwalker-1.9.4/objectwalker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import argparse
 import sys
 import objectwalker
 from objectwalker.filters import *
 
 
-VERSION = "1.9.3"
+VERSION = "1.9.4"
 
 
 banner = r"""
        ____  __      _           __ _       __      ____            
       / __ \/ /_    (_)__  _____/ /| |     / /___ _/ / /_____  _____
      / / / / __ \  / / _ \/ ___/ __/ | /| / / __ `/ / //_/ _ \/ ___/
     / /_/ / /_/ / / /  __/ /__/ /_ | |/ |/ / /_/ / / ,< /  __/ /      v%s
```

### Comparing `objectwalker-1.9.3/objectwalker/filters/EmptyFilter.py` & `objectwalker-1.9.4/objectwalker/filters/EmptyFilter.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,42 +6,51 @@
 
 class EmptyFilter(object):
     """
     Documentation for class EmptyFilter
     """
 
     no_colors = False
-
+    callback = None
     filter_name = "EmptyFilter"
 
     def __init__(self, no_colors=False):
         super(EmptyFilter, self).__init__()
         self.no_colors = no_colors
 
     def check(self, obj, path_to_obj):
         self.print_result(obj, path_to_obj)
         return True
 
     def print_result(self, obj, path_to_obj):
-        # Print the found path
-        obj_value = str(obj)[:50]
-        obj_value = str(bytes(obj_value, 'utf-8'))[2:-1]
-
-        if self.no_colors:
-            print("[%s] [type=%s] [value=%s] | %s" % (
-                    self.filter_name,
-                    str(type(obj)),
-                    obj_value,
-                    '.'.join(path_to_obj)
-                )
-            )
+        if self.callback is not None:
+            self.callback(obj, path_to_obj)
         else:
-            print("[\x1b[95m%s\x1b[0m] [type=\x1b[1;91m%s\x1b[0m] [value=\x1b[94m%s\x1b[0m] | \x1b[1;92m%s\x1b[0m"  % (
-                    self.filter_name,
-                    str(type(obj)),
-                    obj_value,
-                    '.'.join(path_to_obj)
+            # Print the found path
+            obj_value = str(obj)[:50]
+            obj_value = str(bytes(obj_value, 'utf-8'))[2:-1]
+
+            if self.no_colors:
+                print("[%s] [type=%s] [value=%s] | %s" % (
+                        self.filter_name,
+                        str(type(obj)),
+                        obj_value,
+                        '.'.join(path_to_obj)
+                    )
+                )
+            else:
+                print("[\x1b[95m%s\x1b[0m] [type=\x1b[1;91m%s\x1b[0m] [value=\x1b[94m%s\x1b[0m] | \x1b[1;92m%s\x1b[0m"  % (
+                        self.filter_name,
+                        str(type(obj)),
+                        obj_value,
+                        '.'.join(path_to_obj)
+                    )
                 )
-            )
 
     def __repr__(self):
-        return "<%s>" % self.filter_name
+        return "<%s>" % self.filter_name
+
+    def get_callback(self):
+        return self.callback
+
+    def set_callback(self, value):
+        self.callback = value
```

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectNameContains.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectNameContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectNameEndsWith.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectNameEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectNameEquals.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectNameEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectNameStartsWith.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectNameStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectValueContains.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectValueContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectValueEndsWith.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectValueEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectValueEquals.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectValueEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterObjectValueStartsWith.py` & `objectwalker-1.9.4/objectwalker/filters/FilterObjectValueStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterPathContains.py` & `objectwalker-1.9.4/objectwalker/filters/FilterPathContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterPathEndsWith.py` & `objectwalker-1.9.4/objectwalker/filters/FilterPathEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterPathStartsWith.py` & `objectwalker-1.9.4/objectwalker/filters/FilterPathStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py` & `objectwalker-1.9.4/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterTypeIsMethodWrapper.py` & `objectwalker-1.9.4/objectwalker/filters/FilterTypeIsMethodWrapper.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker/filters/FilterTypeIsModule.py` & `objectwalker-1.9.4/objectwalker/filters/FilterTypeIsModule.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,33 +34,36 @@
                     matches_filter = True
 
         if matches_filter:
             self.print_result(obj, path_to_obj)
         return matches_filter
 
     def print_result(self, obj, path_to_obj):
-        # Print the found path
-        module_name, module_type, module_source_file = self.parse_module_name(str(obj))
+        if self.callback is not None:
+            self.callback(obj, path_to_obj)
+        else:
+            # Print the found path
+            module_name, module_type, module_source_file = self.parse_module_name(str(obj))
 
-        if self.no_colors:
-            print("[%s] [module=%s] [module_type=%s] | %s" % (
-                    self.filter_name,
-                    module_name,
-                    module_type,
-                    '.'.join(path_to_obj)
+            if self.no_colors:
+                print("[%s] [module=%s] [module_type=%s] | %s" % (
+                        self.filter_name,
+                        module_name,
+                        module_type,
+                        '.'.join(path_to_obj)
+                    )
                 )
-            )
-        else:
-            print("[\x1b[95m%s\x1b[0m] [module=\x1b[1;91m%s\x1b[0m] [module_type=\x1b[94m%s\x1b[0m] | \x1b[1;92m%s\x1b[0m"  % (
-                    self.filter_name,
-                    module_name,
-                    module_type,
-                    '.'.join(path_to_obj)
+            else:
+                print("[\x1b[95m%s\x1b[0m] [module=\x1b[1;91m%s\x1b[0m] [module_type=\x1b[94m%s\x1b[0m] | \x1b[1;92m%s\x1b[0m"  % (
+                        self.filter_name,
+                        module_name,
+                        module_type,
+                        '.'.join(path_to_obj)
+                    )
                 )
-            )
 
     def parse_module_name(self, module_str):
         module_name, module_type, module_source_file = None, None, None
         matched = re.search("(<module '([^']+)' (\(built-in\)|\(frozen\)|from '([^']+)')>)", module_str)
         if matched is not None:
             _, module_name, module_type, module_source_file = matched.groups()
             if module_type.startswith("from"):
```

### Comparing `objectwalker-1.9.3/objectwalker/filters/__init__.py` & `objectwalker-1.9.4/objectwalker/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/objectwalker.egg-info/SOURCES.txt` & `objectwalker-1.9.4/objectwalker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objectwalker-1.9.3/setup.py` & `objectwalker-1.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 long_description = """e"""
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="objectwalker",
-    version="1.9.3",
+    version="1.9.4",
     description="",
     url="https://github.com/p0dalirius/objectwalker",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=["objectwalker", "objectwalker.filters"],
```

