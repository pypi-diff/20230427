# Comparing `tmp/weighted_tqdm-0.4.tar.gz` & `tmp/weighted_tqdm-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_tqdm-0.4.tar", last modified: Wed Apr 26 13:47:54 2023, max compression
+gzip compressed data, was "weighted_tqdm-0.5.tar", last modified: Thu Apr 27 15:18:54 2023, max compression
```

## Comparing `weighted_tqdm-0.4.tar` & `weighted_tqdm-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:54.122403 weighted_tqdm-0.4/
--rw-rw-rw-   0        0        0     1096 2023-04-26 13:47:48.000000 weighted_tqdm-0.4/LICENSE
--rw-rw-rw-   0        0        0     1894 2023-04-26 13:47:54.122403 weighted_tqdm-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1373 2023-04-26 13:47:48.000000 weighted_tqdm-0.4/README.md
--rw-rw-rw-   0        0        0      516 2023-04-26 13:47:54.138042 weighted_tqdm-0.4/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-04-26 13:47:48.000000 weighted_tqdm-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:54.106372 weighted_tqdm-0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:54.106372 weighted_tqdm-0.4/src/weighted_tqdm/
--rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.4/src/weighted_tqdm/__init__.py
--rw-rw-rw-   0        0        0     2630 2023-04-26 13:35:01.000000 weighted_tqdm-0.4/src/weighted_tqdm/weighted_tqdm.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:54.122403 weighted_tqdm-0.4/src/weighted_tqdm.egg-info/
--rw-rw-rw-   0        0        0     1894 2023-04-26 13:47:53.000000 weighted_tqdm-0.4/src/weighted_tqdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-04-26 13:47:54.000000 weighted_tqdm-0.4/src/weighted_tqdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 13:47:53.000000 weighted_tqdm-0.4/src/weighted_tqdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 13:47:53.000000 weighted_tqdm-0.4/src/weighted_tqdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 13:47:53.000000 weighted_tqdm-0.4/src/weighted_tqdm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 13:47:54.122403 weighted_tqdm-0.4/test/
--rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 weighted_tqdm-0.4/test/test_JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 weighted_tqdm-0.4/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.725123 weighted_tqdm-0.5/
+-rw-rw-rw-   0        0        0     1096 2023-04-27 15:18:36.000000 weighted_tqdm-0.5/LICENSE
+-rw-rw-rw-   0        0        0     2967 2023-04-27 15:18:54.725123 weighted_tqdm-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-04-27 15:18:36.000000 weighted_tqdm-0.5/README.md
+-rw-rw-rw-   0        0        0      516 2023-04-27 15:18:54.732197 weighted_tqdm-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-04-27 15:18:36.000000 weighted_tqdm-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.621787 weighted_tqdm-0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.640404 weighted_tqdm-0.5/src/weighted_tqdm/
+-rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.5/src/weighted_tqdm/__init__.py
+-rw-rw-rw-   0        0        0    10990 2023-04-27 15:06:20.000000 weighted_tqdm-0.5/src/weighted_tqdm/weighted_tqdm.py
+drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.691858 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/
+-rw-rw-rw-   0        0        0     2967 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-27 15:18:54.000000 weighted_tqdm-0.5/src/weighted_tqdm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 15:18:54.725123 weighted_tqdm-0.5/test/
+-rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 weighted_tqdm-0.5/test/test_JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 weighted_tqdm-0.5/test/test_kronbinations.py
```

### Comparing `weighted_tqdm-0.4/LICENSE` & `weighted_tqdm-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.4/PKG-INFO` & `weighted_tqdm-0.5/src/weighted_tqdm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: weighted_tqdm
-Version: 0.4
+Name: weighted-tqdm
+Version: 0.5
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.4.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.5.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -18,31 +18,42 @@
 `pip install weighted_tqdm`
 
 Import via
 `from weighted_tqdm import *`
 
 ## Description
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
-**qudit_tqdm** is a special variant of tqdm, that predicts the remaining time for calculations in quantum mechanics, with the added arguments `dit` specifying whether its a calculation of qubits (default `dit=2` or `dit=3` for qutrits), and the argument `exp` specifying the scaling of computational time with the dimension of a hilbert space. 
-
-
-
-### Examples:
 ```
-from weighted_tqdm import *
-
 how_many_qubits = [1,2,3,4,5]
 qubits weights = lambda x: (2**x)**3
 for i in weighted_tqdm(how_many_qubits, weights=weights):
     # do something
 ```
-or equivalently 
+
+**qudit_tqdm** is a special variant of tqdm, that predicts the remaining time for calculations in quantum mechanics, with the added arguments `dit` specifying whether its a calculation of qubits (default `dit=2` or `dit=3` for qutrits), and the argument `exp` specifying the scaling of computational time with the dimension of a hilbert space. 
 ```
-from weighted_tqdm import *
-how_many_qubits = [1,2,3,4,5]
 for i in qudit_tqdm(how_many_qubits, dim=2, exp=3):
-    # do something
+    time.sleep((2**i)**3)
 ```
 
+**progress** is a generator of progress bars which allows each iteration within a nested set of loops to update a single progress bar. It allows adding classic `tqdm`, but also `weighted_tqdm` or `qudit_tqdm` to different nested loops.
+```
+p = progress()
+for i in p.weighted_tqdm(range(5), weights=lambda i: (i+1), name='outer'):
+    for j in p.tqdm((1,2,3,4,5), name='inner'):
+        time.sleep(0.1*(i+1))
+```
+
+**weighted_kronbinations_tqdm** is the final progress bar, which allows the use of weighted progress bars for `kronbination` loops. Unlike the other functions, tehe update has to manually be added to every iteration.
+```
+list_of_iterators = [range(3), [1,2,3]]    # list of the iterators
+list_of_weights = [ones(3), lambda x: (2**x)**3]    # weights for each iterator
+indexes = np.array([[0,0], [0,1], [0,2], [1,0], [1,1], [1,2]]])    # specify the indexes which are being executed 
+p = weighted_kronbinations_tqdm(list_of_iterators, list_of_weights)    # initialize the generator
+p.init(indexes)    # prepare a progress bar 
+for i in indexes:
+    p.increment()  # update the progress bar
+    time.sleep((2**list_of_iterators[1][i[1]])**3)    # do something
+```
 
 ## Authors: 
 By Michael Schilling
```

### Comparing `weighted_tqdm-0.4/setup.cfg` & `weighted_tqdm-0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 340d  ..version = 0.4.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 350d  ..version = 0.5.
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
-00000150: 732f 7461 6773 2f76 302e 342e 7461 722e  s/tags/v0.4.tar.
+00000150: 732f 7461 6773 2f76 302e 352e 7461 722e  s/tags/v0.5.tar.
 00000160: 677a 0d0a 5072 6f67 7261 6d6d 696e 6720  gz..Programming 
 00000170: 4c61 6e67 7561 6765 203d 203a 2050 7974  Language = : Pyt
 00000180: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
 00000190: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
 000001a0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
 000001b0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
 000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
```

### Comparing `weighted_tqdm-0.4/setup.py` & `weighted_tqdm-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "weighted_tqdm",
-    version    = "0.4",
+    version     = "0.5",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "weighted_tqdm allows for weighted iterations in tqdm progress bars.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.4.tar.gz",
+    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.5.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `weighted_tqdm-0.4/src/weighted_tqdm.egg-info/PKG-INFO` & `weighted_tqdm-0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: weighted-tqdm
-Version: 0.4
+Name: weighted_tqdm
+Version: 0.5
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.4.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.5.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -18,31 +18,42 @@
 `pip install weighted_tqdm`
 
 Import via
 `from weighted_tqdm import *`
 
 ## Description
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
-**qudit_tqdm** is a special variant of tqdm, that predicts the remaining time for calculations in quantum mechanics, with the added arguments `dit` specifying whether its a calculation of qubits (default `dit=2` or `dit=3` for qutrits), and the argument `exp` specifying the scaling of computational time with the dimension of a hilbert space. 
-
-
-
-### Examples:
 ```
-from weighted_tqdm import *
-
 how_many_qubits = [1,2,3,4,5]
 qubits weights = lambda x: (2**x)**3
 for i in weighted_tqdm(how_many_qubits, weights=weights):
     # do something
 ```
-or equivalently 
+
+**qudit_tqdm** is a special variant of tqdm, that predicts the remaining time for calculations in quantum mechanics, with the added arguments `dit` specifying whether its a calculation of qubits (default `dit=2` or `dit=3` for qutrits), and the argument `exp` specifying the scaling of computational time with the dimension of a hilbert space. 
 ```
-from weighted_tqdm import *
-how_many_qubits = [1,2,3,4,5]
 for i in qudit_tqdm(how_many_qubits, dim=2, exp=3):
-    # do something
+    time.sleep((2**i)**3)
 ```
 
+**progress** is a generator of progress bars which allows each iteration within a nested set of loops to update a single progress bar. It allows adding classic `tqdm`, but also `weighted_tqdm` or `qudit_tqdm` to different nested loops.
+```
+p = progress()
+for i in p.weighted_tqdm(range(5), weights=lambda i: (i+1), name='outer'):
+    for j in p.tqdm((1,2,3,4,5), name='inner'):
+        time.sleep(0.1*(i+1))
+```
+
+**weighted_kronbinations_tqdm** is the final progress bar, which allows the use of weighted progress bars for `kronbination` loops. Unlike the other functions, tehe update has to manually be added to every iteration.
+```
+list_of_iterators = [range(3), [1,2,3]]    # list of the iterators
+list_of_weights = [ones(3), lambda x: (2**x)**3]    # weights for each iterator
+indexes = np.array([[0,0], [0,1], [0,2], [1,0], [1,1], [1,2]]])    # specify the indexes which are being executed 
+p = weighted_kronbinations_tqdm(list_of_iterators, list_of_weights)    # initialize the generator
+p.init(indexes)    # prepare a progress bar 
+for i in indexes:
+    p.increment()  # update the progress bar
+    time.sleep((2**list_of_iterators[1][i[1]])**3)    # do something
+```
 
 ## Authors: 
 By Michael Schilling
```

### Comparing `weighted_tqdm-0.4/test/test_JIT_kronbinations.py` & `weighted_tqdm-0.5/test/test_JIT_kronbinations.py`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.4/test/test_kronbinations.py` & `weighted_tqdm-0.5/test/test_kronbinations.py`

 * *Files identical despite different names*

