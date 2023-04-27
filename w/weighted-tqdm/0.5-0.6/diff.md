# Comparing `tmp/weighted_tqdm-0.5.tar.gz` & `tmp/weighted_tqdm-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_tqdm-0.5.tar", last modified: Thu Apr 27 15:18:54 2023, max compression
+gzip compressed data, was "weighted_tqdm-0.6.tar", last modified: Thu Apr 27 21:16:28 2023, max compression
```

## Comparing `weighted_tqdm-0.5.tar` & `weighted_tqdm-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.725123 weighted_tqdm-0.5/
--rw-rw-rw-   0        0        0     1096 2023-04-27 15:18:36.000000 weighted_tqdm-0.5/LICENSE
--rw-rw-rw-   0        0        0     2967 2023-04-27 15:18:54.725123 weighted_tqdm-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2023-04-27 15:18:36.000000 weighted_tqdm-0.5/README.md
--rw-rw-rw-   0        0        0      516 2023-04-27 15:18:54.732197 weighted_tqdm-0.5/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-04-27 15:18:36.000000 weighted_tqdm-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.621787 weighted_tqdm-0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.640404 weighted_tqdm-0.5/src/weighted_tqdm/
--rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.5/src/weighted_tqdm/__init__.py
--rw-rw-rw-   0        0        0    10990 2023-04-27 15:06:20.000000 weighted_tqdm-0.5/src/weighted_tqdm/weighted_tqdm.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.691858 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/
--rw-rw-rw-   0        0        0     2967 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.725123 weighted_tqdm-0.5/test/
--rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 weighted_tqdm-0.5/test/test_JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 weighted_tqdm-0.5/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.288491 weighted_tqdm-0.6/
+-rw-rw-rw-   0        0        0     1096 2023-04-27 21:16:24.000000 weighted_tqdm-0.6/LICENSE
+-rw-rw-rw-   0        0        0     2967 2023-04-27 21:16:28.289490 weighted_tqdm-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-04-27 21:16:24.000000 weighted_tqdm-0.6/README.md
+-rw-rw-rw-   0        0        0      516 2023-04-27 21:16:28.290489 weighted_tqdm-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-04-27 21:16:24.000000 weighted_tqdm-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.260590 weighted_tqdm-0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.267574 weighted_tqdm-0.6/src/weighted_tqdm/
+-rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.6/src/weighted_tqdm/__init__.py
+-rw-rw-rw-   0        0        0    14675 2023-04-27 18:40:16.000000 weighted_tqdm-0.6/src/weighted_tqdm/weighted_tqdm.py
+drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.282490 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/
+-rw-rw-rw-   0        0        0     2967 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-27 21:16:28.000000 weighted_tqdm-0.6/src/weighted_tqdm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 21:16:28.287491 weighted_tqdm-0.6/test/
+-rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 weighted_tqdm-0.6/test/test_JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 weighted_tqdm-0.6/test/test_kronbinations.py
```

### Comparing `weighted_tqdm-0.5/LICENSE` & `weighted_tqdm-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.5/PKG-INFO` & `weighted_tqdm-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: weighted_tqdm
-Version: 0.5
+Version: 0.6
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.5.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.6.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # weighted_tqdm
 
 Install via 
-`pip install weighted_tqdm`
+`pip install weighted-tqdm`
 
 Import via
 `from weighted_tqdm import *`
 
 ## Description
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
 ```
```

### Comparing `weighted_tqdm-0.5/README.md` & `weighted_tqdm-0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # weighted_tqdm
 
 Install via 
-`pip install weighted_tqdm`
+`pip install weighted-tqdm`
 
 Import via
 `from weighted_tqdm import *`
 
 ## Description
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
 ```
```

### Comparing `weighted_tqdm-0.5/setup.cfg` & `weighted_tqdm-0.6/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 350d  ..version = 0.5.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 360d  ..version = 0.6.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 7765  description = we
 00000080: 6967 6874 6564 5f74 7164 6d20 616c 6c6f  ighted_tqdm allo
 00000090: 7773 2066 6f72 2077 6569 6768 7465 6420  ws for weighted 
@@ -15,15 +15,15 @@
 000000e0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 000000f0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
 00000100: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
 00000110: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
 00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
 00000130: 7472 6f70 6963 2f77 6569 6768 7465 645f  tropic/weighted_
 00000140: 7471 646d 2f61 7263 6869 7665 2f72 6566  tqdm/archive/ref
-00000150: 732f 7461 6773 2f76 302e 352e 7461 722e  s/tags/v0.5.tar.
+00000150: 732f 7461 6773 2f76 302e 362e 7461 722e  s/tags/v0.6.tar.
 00000160: 677a 0d0a 5072 6f67 7261 6d6d 696e 6720  gz..Programming 
 00000170: 4c61 6e67 7561 6765 203d 203a 2050 7974  Language = : Pyt
 00000180: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
 00000190: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
 000001a0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
 000001b0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
 000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
```

### Comparing `weighted_tqdm-0.5/setup.py` & `weighted_tqdm-0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "weighted_tqdm",
-    version     = "0.5",
+    version      = "0.6",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "weighted_tqdm allows for weighted iterations in tqdm progress bars.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.5.tar.gz",
+    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.6.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `weighted_tqdm-0.5/src/weighted_tqdm/weighted_tqdm.py` & `weighted_tqdm-0.6/src/weighted_tqdm/weighted_tqdm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 # A function that modifies tqdm progress bars to estimate the remaining time, by allowing the user to specify how much time a step takes with respect to the others
 # adds input weights=[1,2,4,8,16] for a progress bar that takes into account that iteration 2 takes twice as long as iteration 1, and iteration 3 takes 4 times as long as iteration 1, etc.
 import time
 from tqdm import tqdm
+import itertools
+import numpy as np
 
 def determine_length_of_iterable(iterable, weights, **kwargs):
     # calulcate the total number of iterations
     if hasattr(iterable, '__len__'):
         total = len(iterable)
     elif 'total' in kwargs:
         total = kwargs['total']
@@ -126,17 +128,17 @@
             elem = next(iterator)
             if my_level == self.levels: # no sub-call -> update pbar
                 self.current_count_float += self.weight_by_level[-1][ind]
                 ind += 1
                 new_count = round(self.current_count_float*self.total)
                 diff_count = new_count - self.current_count
                 if self.print_val:
-                    self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind+1) + '/' + str(how_many) + ')')
+                    self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind) + '/' + str(how_many) + ')')
                 else:
-                    self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
+                    self.pbar.set_description(self.names[-1]+'(' +str(ind) + '/' + str(how_many) + ')')
                 self.pbar.update(diff_count)
                 self.current_count = new_count
                 destroyed_subcall_last = 0
             else: # there was a subcall -> destroy it
                 ind += 1
                 self.levels -= 1
                 self.weight_by_level.pop()
@@ -160,62 +162,142 @@
             self.pbar.close()
             self.pbar = None
             self.current_count = 0
             self.current_count_float = 0.0
             self.weight_by_level = []
             self.names = []
             self.levels = 0    
+            if self.print_val:
+                self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind+1) + '/' + str(how_many) + ')')
+            else:
+                self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
+
             
     def tqdm(self, iterable, **kwargs):
         return self.weighted_tqdm(iterable, **kwargs)
     
     def qudit_tqdm(self, iterable, dit=2, exp=3, **kwargs):
         return self.weighted_tqdm(iterable, weights=lambda i: (dit**i)**exp, **kwargs)
       
 #p = progress(total=1000)
 #for i in p.weighted_tqdm(range(5), weights=lambda i: (i+1), name='outer'):
 #    for j in p.tqdm((1,2,3,4,5), name='inner'):
 #        time.sleep(0.1*(i+1))      
 
-
 class weighted_kronbinations_tqdm:
-    def __init__(self, list_of_iterators, list_of_weights, total=1000, **kwargs):
+    def __init__(self, list_of_iterators, list_of_weights, total=1000, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', **kwargs):
         # this function takes a list of iterators and weights and returns a generator that iterates through the kronecker product of the iterators
         # Prepare data
         lengths = []
         weights = []
         for i, w in zip(list_of_iterators, list_of_weights):
             lengths.append(determine_length_of_iterable(i, w, **kwargs))
             weights_var, sum_weights = make_weight_list(i, lengths[-1], w)
             weights.append([j/sum_weights for j in weights_var])
         self.lengths = lengths
         self.weights = weights
         self.total = total
+        # Variables for subincrements 
+        # similar to progress class but lowest level is kronbinations level and 
+        # treated differently
+        self.levels = 0
+        self.weight_by_level = []
+        self.ind_by_level = []
+        self.names = []
+        self.bar_format = bar_format
+        
     def init(self, indexes, **kwargs):
         # indexes is a 2d array of indexes, where each row is an index and each column is an iterator
         # Construct a pbar object, and find the total weight  of all indexes to renormalize for the pbar
         # find sum_of_weights = sum([weight of every index]), with weight of an index being the product of the weights of the iterators that make up that index
         weights = []
         for ind in indexes:
             weights.append(np.prod([self.weights[i][j] for i, j in enumerate(ind)]))
         sum_weights = sum(weights)
-        self.curr_weights = [i/sum_weights for i in weights]
         if 'total' in kwargs:
             self.total = kwargs['total']
+        factor = self.total / sum_weights 
+        self.curr_weights = [i*factor for i in weights]
+
         self.indexes = indexes
         self.len_indexes = len(indexes)
         self.curr_ind = 0 # tracks the current indexes index in indexes
         self.cumm_weight = 0.0
         self.curr_pbar_index = 0
-        self.pbar = tqdm(total=self.total, bar_format='{l_bar}{bar}| {elapsed}<{remaining}')
+        self.pbar = tqdm(total=self.total, bar_format=self.bar_format)
+        
+    def sub_tqdm(self, iterable, weights=None, name='', **kwargs):
+        how_many = determine_length_of_iterable(iterable, weights, **kwargs)
+        self.levels += 1
+        my_level = self.levels
+        if len(name):
+            name += ': '
+        self.names.append(name)
+        self.ind_by_level.append(0)
+        weight_vals, weight_sum = make_weight_list(iterable, how_many, weights=weights)
+        if my_level == 1:
+            weight_factor = self.curr_weights[self.curr_ind]  # multiply with current weight of level 0
+        else:
+            weight_factor = self.weight_by_level[-1][self.ind_by_level[my_level-2]]
+        weight_factor = weight_factor/weight_sum
+        weight_vals = [w*weight_factor for w in weight_vals]
+        self.weight_by_level.append(weight_vals)
+        ind = 0
+        self.pbar.set_description(self.names[-1]+' (' +str(ind) + '/' + str(how_many) + ')')
+        iterator = iter(iterable)
+        yield next(iterator) 
+        for i in range(1, how_many):
+            elem = next(iterator)
+            if my_level == self.levels: # no sub-call -> update pbar
+                self.cumm_weight += self.weight_by_level[-1][ind]
+                ind += 1
+                new_count = round(self.cumm_weight)
+                diff_count = new_count - self.curr_pbar_index
+                self.pbar.set_description(self.names[-1]+' (' +str(ind) + '/' + str(how_many) + ')')
+                self.pbar.update(diff_count)
+                self.current_count = new_count
+                self.curr_pbar_index = new_count
+                destroyed_subcall_last = 0
+            else: # there was a subcall -> destroy it
+                ind += 1
+                self.levels -= 1
+                self.weight_by_level.pop()
+                self.ind_by_level.pop()
+                self.names.pop()
+                destroyed_subcall_last = 1
+            self.ind_by_level[my_level-1] = ind
+            yield elem
+        if not destroyed_subcall_last: # if there was a subcall, the progress bar was already updated
+            self.cumm_weight += self.weight_by_level[-1][ind]
+            new_count = round(self.cumm_weight)
+            diff_count = new_count - self.current_count
+            self.current_count = new_count
+            self.curr_pbar_index = new_count
+            self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
+            self.pbar.update(diff_count)
+        else:
+            self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
+                
     def increment(self):
         # increment 
         curr_weight = self.curr_weights[self.curr_ind]
         self.curr_ind += 1
         #self.pbar.set_description('(' +str(i) + '/' + str(self.len_indexes) + ')')
-        self.cumm_weight += curr_weight * self.total
-        new_index = round(self.cumm_weight)
-        diff = new_index - self.curr_pbar_index
-        self.curr_pbar_index = new_index
-        self.pbar.update(diff)
-        if self.curr_ind == len(indexes): # close pbar
-            self.pbar.close()
+        if self.levels == 0:
+            self.cumm_weight += curr_weight 
+            new_index = round(self.cumm_weight)
+            diff = new_index - self.curr_pbar_index
+            self.curr_pbar_index = new_index
+            self.pbar.update(diff)
+        else: # reset sublevels
+            self.levels = 0
+            self.weight_by_level = []
+            self.ind_by_level = []
+            self.names = []
+            
+    def close(self):
+        self.pbar.close()
+        
+    def all_indexes(self):
+        list_of_indexes = [list(np.arange(0, len(l))) for l in list_of_iterators]
+        return np.array(list(itertools.product(*list_of_indexes)))
+
```

### Comparing `weighted_tqdm-0.5/src/weighted_tqdm.egg-info/PKG-INFO` & `weighted_tqdm-0.6/src/weighted_tqdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: weighted-tqdm
-Version: 0.5
+Version: 0.6
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.5.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.6.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # weighted_tqdm
 
 Install via 
-`pip install weighted_tqdm`
+`pip install weighted-tqdm`
 
 Import via
 `from weighted_tqdm import *`
 
 ## Description
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
 ```
```

### Comparing `weighted_tqdm-0.5/test/test_JIT_kronbinations.py` & `weighted_tqdm-0.6/test/test_JIT_kronbinations.py`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.5/test/test_kronbinations.py` & `weighted_tqdm-0.6/test/test_kronbinations.py`

 * *Files identical despite different names*

