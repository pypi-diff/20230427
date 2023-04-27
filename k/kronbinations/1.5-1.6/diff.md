# Comparing `tmp/kronbinations-1.5.tar.gz` & `tmp/kronbinations-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kronbinations-1.5.tar", last modified: Wed Apr 26 15:28:54 2023, max compression
+gzip compressed data, was "kronbinations-1.6.tar", last modified: Thu Apr 27 21:11:01 2023, max compression
```

## Comparing `kronbinations-1.5.tar` & `kronbinations-1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:28:54.650613 kronbinations-1.5/
--rw-rw-rw-   0        0        0     1096 2023-04-26 15:28:44.000000 kronbinations-1.5/LICENSE
--rw-rw-rw-   0        0        0     6252 2023-04-26 15:28:54.650613 kronbinations-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5724 2023-04-26 15:28:44.000000 kronbinations-1.5/README.md
--rw-rw-rw-   0        0        0      523 2023-04-26 15:28:54.656774 kronbinations-1.5/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-04-26 15:28:44.000000 kronbinations-1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:28:54.516639 kronbinations-1.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 15:28:54.556520 kronbinations-1.5/src/kronbinations/
--rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.5/src/kronbinations/JIT_Array.py
--rw-rw-rw-   0        0        0    15680 2023-04-26 15:28:33.000000 kronbinations-1.5/src/kronbinations/JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.5/src/kronbinations/Kron_Array.py
--rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.5/src/kronbinations/Kron_Fun_Modifier.py
--rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.5/src/kronbinations/__init__.py
--rw-rw-rw-   0        0        0    10981 2023-04-24 15:10:06.000000 kronbinations-1.5/src/kronbinations/kronbinations.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:28:54.636804 kronbinations-1.5/src/kronbinations.egg-info/
--rw-rw-rw-   0        0        0     6252 2023-04-26 15:28:53.000000 kronbinations-1.5/src/kronbinations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-04-26 15:28:54.000000 kronbinations-1.5/src/kronbinations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:28:53.000000 kronbinations-1.5/src/kronbinations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 15:28:53.000000 kronbinations-1.5/src/kronbinations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 15:28:53.000000 kronbinations-1.5/src/kronbinations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 15:28:54.636804 kronbinations-1.5/test/
--rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.5/test/test_JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.5/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.290420 kronbinations-1.6/
+-rw-rw-rw-   0        0        0     1096 2023-04-27 18:44:03.000000 kronbinations-1.6/LICENSE
+-rw-rw-rw-   0        0        0     6252 2023-04-27 21:11:01.290420 kronbinations-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5724 2023-04-27 18:44:03.000000 kronbinations-1.6/README.md
+-rw-rw-rw-   0        0        0      523 2023-04-27 21:11:01.306044 kronbinations-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      878 2023-04-27 18:44:03.000000 kronbinations-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.227919 kronbinations-1.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.259170 kronbinations-1.6/src/kronbinations/
+-rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.6/src/kronbinations/JIT_Array.py
+-rw-rw-rw-   0        0        0    17493 2023-04-27 18:49:16.000000 kronbinations-1.6/src/kronbinations/JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.6/src/kronbinations/Kron_Array.py
+-rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.6/src/kronbinations/Kron_Fun_Modifier.py
+-rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.6/src/kronbinations/__init__.py
+-rw-rw-rw-   0        0        0    12896 2023-04-27 18:48:42.000000 kronbinations-1.6/src/kronbinations/kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.290420 kronbinations-1.6/src/kronbinations.egg-info/
+-rw-rw-rw-   0        0        0     6252 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-27 21:11:01.000000 kronbinations-1.6/src/kronbinations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.290420 kronbinations-1.6/test/
+-rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.6/test/test_JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.6/test/test_kronbinations.py
```

### Comparing `kronbinations-1.5/LICENSE` & `kronbinations-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kronbinations-1.5/PKG-INFO` & `kronbinations-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.5
+Version: 1.6
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.5.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.6.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kronbinations-1.5/README.md` & `kronbinations-1.6/README.md`

 * *Files identical despite different names*

### Comparing `kronbinations-1.5/setup.cfg` & `kronbinations-1.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 350d  ..version = 1.5.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 360d  ..version = 1.6.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6b72  description = kr
 00000080: 6f6e 6269 6e61 7469 6f6e 7320 6973 2075  onbinations is u
 00000090: 7365 6420 746f 2072 656d 6f76 6520 6e65  sed to remove ne
@@ -16,15 +16,15 @@
 000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000100: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
 00000110: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
 00000120: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
 00000130: 622e 636f 6d2f 4e74 726f 7069 632f 6b72  b.com/Ntropic/kr
 00000140: 6f6e 6269 6e61 7469 6f6e 732f 6172 6368  onbinations/arch
 00000150: 6976 652f 7265 6673 2f74 6167 732f 7631  ive/refs/tags/v1
-00000160: 2e35 2e74 6172 2e67 7a0d 0a50 726f 6772  .5.tar.gz..Progr
+00000160: 2e36 2e74 6172 2e67 7a0d 0a50 726f 6772  .6.tar.gz..Progr
 00000170: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 00000180: 3d20 3a20 5079 7468 6f6e 203a 3a20 330d  = : Python :: 3.
 00000190: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001a0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
 000001b0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
 000001c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
 000001d0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
```

### Comparing `kronbinations-1.5/setup.py` & `kronbinations-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "kronbinations",
-    version           = "1.5",
+    version            = "1.6",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "kronbinations is used to remove nested loops and perform parameter sweeps.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.5.tar.gz",
+    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.6.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `kronbinations-1.5/src/kronbinations/JIT_Array.py` & `kronbinations-1.6/src/kronbinations/JIT_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.5/src/kronbinations/JIT_kronbinations.py` & `kronbinations-1.6/src/kronbinations/JIT_kronbinations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-import itertools
-from tqdm import tqdm
+from weighted_tqdm import weighted_kronbinations_tqdm, weighted_tqdm
 
 import inspect
 from hashlib import sha1
 import os
 import numpy as np
 import inspect
-import importlib
 
 # import JIT_Array and Kron_Fun_Modifier    
 from .JIT_Array import *
 from .Kron_Fun_Modifier import *
 
 # An array class, that stores an array, and whether it's values have been calculated,
 # and if so, what the values are
 # If values of the array are requested, and they have not been calculated, they are calculated using a function handle passed to the constructor
 class JIT_kronbinations():
     def __init__(self, *values, func=None, other_func=[], import_statements=[], other_arguments=[], checksum=None, autosave=True, data_dir='Cache', redo=False, progress=True, **kwargs):
         # Calculate checksums
+        weights_given = True if 'weights' in kwargs.keys() else False
         if checksum is None:
             checksum = self.checksum(*values, *import_statements, *other_arguments)
         self.checksum = checksum
         # check if data_dir exists
         if not os.path.exists(data_dir):
             os.makedirs(data_dir)
         self.data_dir = data_dir
@@ -39,22 +38,45 @@
             self.other_arguments = other_arguments
 
         # lengths of the values -> ignore the length one arrays, they are not to be iterated over
         # if values is a dictionary, then the keys are the directions, and the values are the arrays
         if isinstance(values[0], dict):
             if len(values) > 1:
                 raise ValueError('If values is a dictionary, it must be the only argument')
-            values = values[0]
-            self.array_vars_all_names = list(values.keys())
-            self.array_vars_all = list(values.values())
+            input_values = values[0]
+            keys = input_values.keys()
+            values = input_values.values()
+            self.array_vars_all_names, self.array_vars_all, self.all_weights = [], [], []
+            for i, (key, value) in enumerate(zip(keys, values)):  
+                # check if value is a dict with value and weight
+                self.array_vars_all_names.append(key)
+                if isinstance(value, dict):
+                    if 'value' in value.keys():
+                        self.array_vars_all.append(value['value'])
+                    else:
+                        raise ValueError('If value is a dictionary, it must have a value key') 
+                    if 'weight' in value.keys():
+                        self.all_weights.append(value['weight'])
+                    else:
+                        self.all_weights.append(None)
+                else: # Normal 
+                    self.array_vars_all.append(value)
+                    if weights_given:
+                        self.all_weights.append(kwargs['weights'][i])
+                    else:
+                        self.all_weights.append(None)
             self.return_as_dict = True
         else:
             self.array_vars_all = list(values)
-            self.array_vars_all_names = None
+            if weights_given:
+                self.all_weights = list(kwargs['weights'])
+            else:
+                self.all_weights = [None] * len(self.array_vars_all)
             self.return_as_dict = False
+            self.array_vars_all_names = None
         for i, arr in enumerate(self.array_vars_all):
             # if does not have length, transform into array
             if not hasattr(arr, '__len__'):
                 self.array_vars_all[i] = np.array([arr])
         # only relevant values in array_directions
         self.array_vars = [arr for arr in self.array_vars_all if len(arr) > 1]
         if isinstance(values, dict):
@@ -77,15 +99,16 @@
         self.size = np.prod(self.array_lengths)
 
         self.do_index = True
         self.do_change = True
         self.do_tqdm = progress
         self.redo = redo
         self.set(**kwargs)   # redo these values if passed as kwargs
-    
+        self.pbar = weighted_kronbinations_tqdm(self.array_vars, self.weights, self.size)
+        
         self.curr_index = -1
         self.func_modifier()
 
     def set(self, **args):
         key_substitution_list = [['index', 'do_index'], ['change', 'do_change'], ['progress', 'do_tqdm']]
         key_list = [v[0] for v in key_substitution_list]
         subs_list = [v[1] for v in key_substitution_list]
@@ -93,14 +116,16 @@
             # Substitute certain keys from substitution list
             if key in key_list:
                 key = subs_list[key_list.index(key)]
             if (key == 'return_as_dict' and value==True) and not isinstance(self.array_vars_all_names, list):
                 raise ValueError('Keys are not defined, must create Object via dictionary in order to set "return_as_dict = True".')
             else:
                 setattr(self, key, value)
+        if self.do_tqdm:
+            self.pbar = weighted_kronbinations_tqdm(self.array_vars, self.weights, self.size)
     def get(self, *args):
         key_substitution_list = [['index', 'do_index'], ['change', 'do_change'], ['progress', 'do_tqdm']]
         key_list = [v[0] for v in key_substitution_list]
         subs_list = [v[1] for v in key_substitution_list]
         x = []
         for key in args:
             if key in key_list:
@@ -246,43 +271,49 @@
             self.last_indexes_all = self.indexes_all
             self.changed_var = changed_var
         return self.last_values, self.last_indexes, self.changed_var
 
     def kronprod(self, **args):
         self.set(**args)
         if self.do_tqdm and self.total_length > 1:
-            self.loop = tqdm(range(self.total_length))
+            self.pbar.init(np.array(list(itertools.product(*self.index_list))))
         if self.do_index:
             if self.do_change:
                 for n in range(self.total_length):
                     v,i,c = next(self)
                     yield tuple(i), v, c
                     if self.do_tqdm and self.total_length > 1:
-                        self.loop.update(1)
+                        self.pbar.increment()
             else:
                 for n in range(self.total_length):
                     v,i,_ = next(self)
                     yield tuple(i), v
                     if self.do_tqdm and self.total_length > 1:
-                        self.loop.update(1)
+                        self.pbar.increment()
         else:
             if self.do_change: 
                 for n in range(self.total_length):
                     v,_,c = next(self)
                     yield v, c
                     if self.do_tqdm and self.total_length > 1:
-                        self.loop.update(1)
+                        self.pbar.increment()
             else:
                 for n in range(self.total_length):
                     v,_,_ = next(self)
                     yield v
                     if self.do_tqdm and self.total_length > 1:
-                        self.loop.update(1)
+                        self.pbar.increment()
         if self.do_tqdm and self.total_length > 1:
-            self.loop.close()
+            self.pbar.close()
+            
+    def tqdm(self, iterator, weights=None, name='', **kwargs):
+        if self.do_tqdm:
+            yield self.pbar.sub_tqdm(iterator, weights=weights, name=name, **kwargs)
+        else:
+            yield weighted_tqdm(iterator, weights=weights, name=name, **kwargs)
 
     def changed(self, elem=None):
         if elem is None:
             return self.changed_var
         elif isinstance(elem, int):
             if self.return_as_dict:
                 string = self.array_vars_all_names[elem]
```

### Comparing `kronbinations-1.5/src/kronbinations/Kron_Array.py` & `kronbinations-1.6/src/kronbinations/Kron_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.5/src/kronbinations/Kron_Fun_Modifier.py` & `kronbinations-1.6/src/kronbinations/Kron_Fun_Modifier.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.5/src/kronbinations/kronbinations.py` & `kronbinations-1.6/src/kronbinations/kronbinations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,67 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 import itertools
-from tqdm import tqdm
+from weighted_tqdm import weighted_kronbinations_tqdm, weighted_tqdm
 from .Kron_Array import *
 
 class kronbinations():
     # A class for scanning parameter landscapes
     # creates iterators over multiple parameters via kronecker products (itertools product), 
     # automatizes the construction of arrays to sotore results on the landscape, simplifies indexing 
     # while keeping the ability to add functions that get only executed in a specific subloop by tracking when a variable is changed
 
     def __init__(self, *values, **kwargs):
         # If values is a dictionary, also store the keys, so that change can be outputted by key
+        weights_given = True if 'weights' in kwargs.keys() else False
         if isinstance(values[0], dict):
             if len(values) > 1:
                 raise ValueError('If values is a dictionary, it must be the only argument')
-            values = values[0]
-            self.array_vars_all_names = list(values.keys())
-            self.array_vars_all = list(values.values())
+            input_values = values[0]
+            keys = input_values.keys()
+            values = input_values.values()
+            self.array_vars_all_names, self.array_vars_all, self.all_weights = [], [], []
+            for i, (key, value) in enumerate(zip(keys, values)):  
+                # check if value is a dict with value and weight
+                self.array_vars_all_names.append(key)
+                if isinstance(value, dict):
+                    if 'value' in value.keys():
+                        self.array_vars_all.append(value['value'])
+                    else:
+                        raise ValueError('If value is a dictionary, it must have a value key') 
+                    if 'weight' in value.keys():
+                        self.all_weights.append(value['weight'])
+                    else:
+                        self.all_weights.append(None)
+                else: # Normal 
+                    self.array_vars_all.append(value)
+                    if weights_given:
+                        self.all_weights.append(kwargs['weights'][i])
+                    else:
+                        self.all_weights.append(None)
             self.return_as_dict = True
         else:
             self.array_vars_all = list(values)
+            if weights_given:
+                self.all_weights = list(kwargs['weights'])
+            else:
+                self.all_weights = [None] * len(self.array_vars_all)
             self.return_as_dict = False
             self.array_vars_all_names = None
         for i, arr in enumerate(self.array_vars_all):
             # if does not have length, transform into array
             if not hasattr(arr, '__len__'):
                 self.array_vars_all[i] = np.array([arr])
         # only relevant values in array_directions
         self.array_vars = [arr for arr in self.array_vars_all if len(arr) > 1]
         if isinstance(values, dict):
             self.array_vars_names = [name for name, arr in zip(self.array_vars_all_names, self.array_vars_all) if len(arr) > 1]
         # add index values of the array vars 
         self.array_vars_indexes = [i for i, arr in enumerate(self.array_vars_all) if len(arr) > 1] 
-        #self.array_vars_indexes += [len(self.array_vars_all) + 1] # add one for the return value
+        self.weights = [w for i, w in enumerate(self.all_weights) if i in self.array_vars_indexes]
 
         if self.return_as_dict:
             self.curr_vals = {key: arr[0] for key, arr in zip(self.array_vars_all_names, self.array_vars_all)}
         else:
             self.curr_vals = [arr[0] for arr in self.array_vars_all]
 
         self.array_lengths_all = [len(arr) for arr in self.array_vars_all]
@@ -45,24 +69,26 @@
         self.shape_all = tuple(self.array_lengths_all)
         self.shape = tuple(self.array_lengths)
         self.ndim_all = len(self.array_lengths_all)
         self.ndim = len(self.array_lengths)
         self.total_length = np.prod(self.array_lengths)
         self.size_all = np.prod(self.array_lengths_all)
         self.size = np.prod(self.array_lengths)
-
+        
         self.index_list = [np.arange(len(v)) for v in self.array_vars]
         self.index_list_all = [np.arange(len(v)) for v in self.array_vars_all]
         # Define the iterators
         self.setup_iterator()
 
         self.do_index = True
         self.do_change = True
         self.do_tqdm = True
         self.set(**kwargs)   # redo these values if passed as kwargs
+        # Initialize tqdm object
+        self.pbar = weighted_kronbinations_tqdm(self.array_vars, self.weights, self.size)
 
 
     def empty(self, *var, **args):
         return Kron_Array(self.array_lengths, 'empty', *var, **args)
     def ones(self, *var, **args):
         return Kron_Array(self.array_lengths, 'ones', *var, **args)
     def zeros(self, *var, **args):
@@ -80,14 +106,16 @@
             # Substitute certain keys from substitution list
             if key in key_list:
                 key = subs_list[key_list.index(key)]
             if (key == 'return_as_dict' and value==True) and not isinstance(self.array_vars_all_names, list):
                 raise ValueError('Keys are not defined, must create Object via dictionary in order to set "return_as_dict = True".')
             else:
                 setattr(self, key, value)
+        if self.do_tqdm:
+            self.pbar = weighted_kronbinations_tqdm(self.array_vars, self.weights, self.size)
     def get(self, *args):
         key_substitution_list = [['index', 'do_index'], ['change', 'do_change'], ['progress', 'do_tqdm']]
         key_list = [v[0] for v in key_substitution_list]
         subs_list = [v[1] for v in key_substitution_list]
         x = []
         for key in args:
             if key in key_list:
@@ -145,44 +173,51 @@
             self.changed_var = changed_var
         
         return self.last_values, self.last_indexes, self.changed_var
 
     def kronprod(self, **args):
         self.set(**args)
         if self.do_tqdm:
-            self.loop = tqdm(range(self.total_length))
+            # get all indexes
+            self.pbar.init(np.array(list(itertools.product(*self.index_list))))
         if self.do_index:
             if self.do_change:
                 for n in range(self.total_length):
                     v,i,c = next(self)
                     yield i, v, c
                     if self.do_tqdm:
-                        self.loop.update(1)
+                        self.pbar.increment()
             else:
                 for n in range(self.total_length):
                     v,i,_ = next(self)
                     yield i, v
                     if self.do_tqdm:
-                        self.loop.update(1)
+                        self.pbar.increment()
         else:
             if self.do_change: 
                 for n in range(self.total_length):
                     v,_,c = next(self)
                     yield v, c
                     if self.do_tqdm:
-                        self.loop.update(1)
+                        self.pbar.increment()
             else:  
                 for n in range(self.total_length):
                     v,_,_ = next(self)
                     yield v
                     if self.do_tqdm:
-                        self.loop.update(1)
+                        self.pbar.increment()
         if self.do_tqdm:
-            self.loop.close()
+            self.pbar.close()
         self.setup_iterator()
+        
+    def tqdm(self, iterator, weights=None, name='', **kwargs):
+        if self.do_tqdm:
+            yield self.pbar.sub_tqdm(iterator, weights=weights, name=name, **kwargs)
+        else:
+            yield weighted_tqdm(iterator, weights=weights, name=name, **kwargs)
 
     def changed(self, elem=None):
         if elem is None:
             return self.changed_var
         elif isinstance(elem, int):
             if self.return_as_dict:
                 string = self.array_vars_all_names[elem]
```

### Comparing `kronbinations-1.5/src/kronbinations.egg-info/PKG-INFO` & `kronbinations-1.6/src/kronbinations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.5
+Version: 1.6
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.5.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.6.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kronbinations-1.5/test/test_JIT_kronbinations.py` & `kronbinations-1.6/test/test_JIT_kronbinations.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.5/test/test_kronbinations.py` & `kronbinations-1.6/test/test_kronbinations.py`

 * *Files identical despite different names*

