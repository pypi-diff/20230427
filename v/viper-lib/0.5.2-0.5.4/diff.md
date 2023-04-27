# Comparing `tmp/viper_lib-0.5.2.tar.gz` & `tmp/viper_lib-0.5.4.tar.gz`

## Comparing `viper_lib-0.5.2.tar` & `viper_lib-0.5.4.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/__init__.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/async_utils.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/better_threading.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/cucumber.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/cucumber_main.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/exceptions.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/format.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/frozendict.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/interactive.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/persistent.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/pickle_utils.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/test_client.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/test_server.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/warnings.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/abc/__init__.py
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/abc/connection.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/abc/flux.py
--rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/abc/io.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/building/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/building/cy_clean.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/building/cy_compile.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/building/module_tools.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/compress/__init__.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/compress/flux.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/crypto/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/crypto/exceptions.py
--rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/crypto/flux.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/crypto/session.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/crypto/utils.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/debugging/__init__.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/debugging/chrono.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/debugging/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/evolve/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/evolve/primitives.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/evolve/types/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/evolve/types/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/contextual.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/decorators.py
--rw-r--r--   0        0        0    16443 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/iterable.py
--rw-r--r--   0        0        0    17389 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/procedural.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/prototype.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/secret.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/specialized.py
--rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/static.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/meta/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/partition/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/partition/memory.py
--rw-r--r--   0        0        0    14044 2020-02-02 00:00:00.000000 viper_lib-0.5.2/Viper/partition/primitives.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.5.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.5.2/LICENSE
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.5.2/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 viper_lib-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper.pth
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/__init__.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/async_utils.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/better_threading.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/cucumber.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/cucumber_main.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/exceptions.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/format.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/frozendict.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/interactive.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/persistent.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/pickle_utils.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/test_client.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/test_server.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/warnings.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/__init__.py
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/connection.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/flux.py
+-rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/io.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/cy_clean.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/cy_compile.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/module_tools.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/compress/__init__.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/compress/flux.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/exceptions.py
+-rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/flux.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/session.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/utils.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/debugging/__init__.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/debugging/chrono.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/debugging/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/primitives.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/types/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/types/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/contextual.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/decorators.py
+-rw-r--r--   0        0        0    16443 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/iterable.py
+-rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/procedural.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/prototype.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/secret.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/specialized.py
+-rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/static.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/partition/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/partition/memory.py
+-rw-r--r--   0        0        0    14044 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/partition/primitives.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.5.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.5.4/LICENSE
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.5.4/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 viper_lib-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.5.4/PKG-INFO
```

### Comparing `viper_lib-0.5.2/Viper/async_utils.py` & `viper_lib-0.5.4/Viper/async_utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/better_threading.py` & `viper_lib-0.5.4/Viper/better_threading.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/cucumber_main.py` & `viper_lib-0.5.4/Viper/cucumber_main.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/format.py` & `viper_lib-0.5.4/Viper/format.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/frozendict.py` & `viper_lib-0.5.4/Viper/frozendict.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/interactive.py` & `viper_lib-0.5.4/Viper/interactive.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/persistent.py` & `viper_lib-0.5.4/Viper/persistent.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/pickle_utils.py` & `viper_lib-0.5.4/Viper/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/test_client.py` & `viper_lib-0.5.4/Viper/test_client.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/test_server.py` & `viper_lib-0.5.4/Viper/test_server.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/warnings.py` & `viper_lib-0.5.4/Viper/warnings.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/abc/connection.py` & `viper_lib-0.5.4/Viper/abc/connection.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/abc/flux.py` & `viper_lib-0.5.4/Viper/abc/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/abc/io.py` & `viper_lib-0.5.4/Viper/abc/io.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/building/cy_clean.py` & `viper_lib-0.5.4/Viper/building/cy_clean.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/building/cy_compile.py` & `viper_lib-0.5.4/Viper/building/cy_compile.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/building/module_tools.py` & `viper_lib-0.5.4/Viper/building/module_tools.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/compress/flux.py` & `viper_lib-0.5.4/Viper/compress/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/crypto/exceptions.py` & `viper_lib-0.5.4/Viper/crypto/exceptions.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/crypto/flux.py` & `viper_lib-0.5.4/Viper/crypto/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/crypto/session.py` & `viper_lib-0.5.4/Viper/crypto/session.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/crypto/utils.py` & `viper_lib-0.5.4/Viper/crypto/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/debugging/chrono.py` & `viper_lib-0.5.4/Viper/debugging/chrono.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/debugging/utils.py` & `viper_lib-0.5.4/Viper/debugging/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/evolve/primitives.py` & `viper_lib-0.5.4/Viper/evolve/primitives.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/meta/contextual.py` & `viper_lib-0.5.4/Viper/meta/contextual.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/meta/decorators.py` & `viper_lib-0.5.4/Viper/meta/decorators.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/meta/iterable.py` & `viper_lib-0.5.4/Viper/meta/iterable.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/meta/procedural.py` & `viper_lib-0.5.4/Viper/meta/procedural.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,34 +228,39 @@
             return ProceduralImporter.__cache[fullname]
 
         package, _, module = fullname.rpartition(".")
         spec = super().find_spec(fullname, path, target)
 
         if spec:
 
-            # print("Trying to import '{}', got '{}'".format(fullname, spec))
-
-            spec.loader = cls(spec.loader)
+            special = False
                     
             from pathlib import Path
             import sys
             directories = [Path(p) for p in (sys.path if path is None else path)]
             
             for dir in directories:
                 package_dir = dir / module
                 if package_dir.is_dir():
                     for file in package_dir.iterdir():
-                        if file.name == "__proc__.py":
-                            # print("Got a special package")
+                        if file.name == "__proc__.py":      # This is a procedural package
                             ProceduralImporter.__loading_packages[fullname] = file
+                            special = True
                             break
             
-            ProceduralImporter.__cache[fullname] = spec
+            if package and package in ProceduralImporter.__loaded_packages:     # Parent is procedural
+                special = True
+            
+            if special:
+                spec.loader = cls(spec.loader)
+                ProceduralImporter.__cache[fullname] = spec
 
-        return spec
+                return spec
+        
+        return None
     
 
     @staticmethod
     def invalidate_caches():
         ProceduralImporter.__cache.clear()
 
 
@@ -400,10 +405,10 @@
                 exec(code, parent_package.__dict__)
                 ProceduralImporter.__package_all_remaining.pop(parent_name)
                     
 
 
 
 
-sys.meta_path[-1] = ProceduralImporter      # Replace the source finder
+sys.meta_path.insert(0, ProceduralImporter)
 
 del Loader, ModuleSpec, PathFinder, Path, sys, ModuleType, Sequence, WeakValueDictionary
```

### Comparing `viper_lib-0.5.2/Viper/meta/secret.py` & `viper_lib-0.5.4/Viper/meta/secret.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/meta/specialized.py` & `viper_lib-0.5.4/Viper/meta/specialized.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/meta/static.py` & `viper_lib-0.5.4/Viper/meta/static.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/meta/utils.py` & `viper_lib-0.5.4/Viper/meta/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/Viper/partition/primitives.py` & `viper_lib-0.5.4/Viper/partition/primitives.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/.gitignore` & `viper_lib-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/LICENSE` & `viper_lib-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/README.md` & `viper_lib-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.2/pyproject.toml` & `viper_lib-0.5.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "viper_lib"
-version = "0.5.2"
+version = "0.5.4"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin.n7@gmail.com" },
 ]
 description = "A Python library full of useful Python tools."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
@@ -16,8 +16,11 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Repository" = "https://github.com/MrVoustache/Viper"
-"Bug Tracker" = "https://github.com/MrVoustache/Viper/issues"
+"Bug Tracker" = "https://github.com/MrVoustache/Viper/issues"
+
+[tool.hatch.build.targets.wheel.force-include]
+"./Viper.pth" = "./Viper.pth"
```

### Comparing `viper_lib-0.5.2/PKG-INFO` & `viper_lib-0.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viper_lib
-Version: 0.5.2
+Version: 0.5.4
 Summary: A Python library full of useful Python tools.
 Project-URL: Repository, https://github.com/MrVoustache/Viper
 Project-URL: Bug Tracker, https://github.com/MrVoustache/Viper/issues
 Author-email: Vincent Raulin <vincent.raulin.n7@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Vincent Raulin
```

