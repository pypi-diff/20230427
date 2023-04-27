# Comparing `tmp/kiwigrad-0.20.tar.gz` & `tmp/kiwigrad-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.20.tar", last modified: Wed Apr 19 21:54:29 2023, max compression
+gzip compressed data, was "kiwigrad-0.21.tar", last modified: Thu Apr 27 13:49:51 2023, max compression
```

## Comparing `kiwigrad-0.20.tar` & `kiwigrad-0.21.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-19 21:54:29.006917 kiwigrad-0.20/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.20/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.20/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3068 2023-04-19 21:54:29.006436 kiwigrad-0.20/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1312 2023-04-19 21:51:11.000000 kiwigrad-0.20/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-19 21:54:29.001933 kiwigrad-0.20/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      289 2023-04-19 21:53:41.000000 kiwigrad-0.20/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.20/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.20/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1200 2023-04-19 20:42:21.000000 kiwigrad-0.20/kiwigrad/layers.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3211 2023-04-19 21:53:28.000000 kiwigrad-0.20/kiwigrad/neurons.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1531 2023-04-19 21:16:15.000000 kiwigrad-0.20/kiwigrad/nn.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.20/kiwigrad/skeleton.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-19 21:54:29.004968 kiwigrad-0.20/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3068 2023-04-19 21:54:28.000000 kiwigrad-0.20/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      349 2023-04-19 21:54:28.000000 kiwigrad-0.20/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-19 21:54:28.000000 kiwigrad-0.20/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-19 21:54:28.000000 kiwigrad-0.20/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-19 21:54:28.000000 kiwigrad-0.20/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-19 21:53:46.000000 kiwigrad-0.20/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-19 21:54:29.007085 kiwigrad-0.20/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-19 21:54:29.005493 kiwigrad-0.20/test/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1353 2023-04-19 21:20:17.000000 kiwigrad-0.20/test/test.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.890771 kiwigrad-0.21/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.21/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.21/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3178 2023-04-27 13:49:51.888813 kiwigrad-0.21/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1320 2023-04-20 21:05:52.000000 kiwigrad-0.21/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.878316 kiwigrad-0.21/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      324 2023-04-27 13:43:36.000000 kiwigrad-0.21/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8659 2023-04-27 13:36:32.000000 kiwigrad-0.21/kiwigrad/engine.c
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.21/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.21/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.21/kiwigrad/layers.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.21/kiwigrad/neurons.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.21/kiwigrad/nn.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.21/kiwigrad/skeleton.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.884191 kiwigrad-0.21/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3178 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      376 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-27 13:49:51.000000 kiwigrad-0.21/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-27 13:47:47.000000 kiwigrad-0.21/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-27 13:49:51.891179 kiwigrad-0.21/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      942 2023-04-27 13:39:57.000000 kiwigrad-0.21/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-27 13:49:51.886318 kiwigrad-0.21/test/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1353 2023-04-19 21:20:17.000000 kiwigrad-0.21/test/test.py
```

### Comparing `kiwigrad-0.20/LICENSE` & `kiwigrad-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.20/PKG-INFO` & `kiwigrad-0.21/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.20
+Version: 0.21
 Summary: Mini deep learning framework
+Home-page: https://github.com/marcosalvalaggio/femtograd
+Author: Marco Salvalaggio
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,25 +22,26 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/marcosalvalaggio/femtograd
 Project-URL: Bug Tracker, https://github.com/marcosalvalaggio/femtogradissues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kiwigrad
 
 <h1 align="center">
-<img src="logo.png" width="300">
+<img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![PyPI version fury.io](https://badge.fury.io/py/kiwigrad.svg)](https://pypi.python.org/pypi/kiwigrad/)
 
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
@@ -57,20 +60,21 @@
 * Support for RNN1 feedforward neural networks.
 
 ### Example Implementation
 
 Here's an example implementation of a MLP net using Kiwigrad:
 
 ```python 
-from kiwigrad import * 
+from kiwigrad import MLP, Layer
 
 class PotNet(MLP):
     def __init__(self):
         layers = [
             Layer(nin=2, nout=16, bias=True, activation="relu"),
             Layer(nin=16, nout=16, bias=True, activation="relu"),
             Layer(nin=16, nout=1, bias=True, activation="linear")
         ]
         super().__init__(layers=layers)
 
 model = PotNet()
 ```
+
```

### Comparing `kiwigrad-0.20/README.md` & `kiwigrad-0.21/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Kiwigrad
 
 <h1 align="center">
-<img src="logo.png" width="300">
+<img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![PyPI version fury.io](https://badge.fury.io/py/kiwigrad.svg)](https://pypi.python.org/pypi/kiwigrad/)
 
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
@@ -24,15 +24,15 @@
 * Support for RNN1 feedforward neural networks.
 
 ### Example Implementation
 
 Here's an example implementation of a MLP net using Kiwigrad:
 
 ```python 
-from kiwigrad import * 
+from kiwigrad import MLP, Layer
 
 class PotNet(MLP):
     def __init__(self):
         layers = [
             Layer(nin=2, nout=16, bias=True, activation="relu"),
             Layer(nin=16, nout=16, bias=True, activation="relu"),
             Layer(nin=16, nout=1, bias=True, activation="linear")
```

### Comparing `kiwigrad-0.20/kiwigrad/engine.py` & `kiwigrad-0.21/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.20/kiwigrad/graph.py` & `kiwigrad-0.21/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.20/kiwigrad/layers.py` & `kiwigrad-0.21/kiwigrad/layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .engine import Value
+#from .engine import Value
+from kiwigrad.engine import Value
 from .neurons import Neuron, RNN1Neuron
 from typing import Literal
 from .skeleton import Module
 
 
 class Layer(Module):
```

### Comparing `kiwigrad-0.20/kiwigrad/neurons.py` & `kiwigrad-0.21/kiwigrad/neurons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .engine import Value
+#from .engine import Value
+from kiwigrad.engine import Value
 import random 
 from typing import Literal
 from .skeleton import Module
 
 
 class Neuron(Module):
```

### Comparing `kiwigrad-0.20/kiwigrad/nn.py` & `kiwigrad-0.21/kiwigrad/nn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .engine import Value
+#from .engine import Value
+from kiwigrad.engine import Value
 import pickle
 from typing import Literal
 from .skeleton import Module
 
 
 class MLP(Module):
```

### Comparing `kiwigrad-0.20/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.21/kiwigrad.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.20
+Version: 0.21
 Summary: Mini deep learning framework
+Home-page: https://github.com/marcosalvalaggio/femtograd
+Author: Marco Salvalaggio
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -20,25 +22,26 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/marcosalvalaggio/femtograd
 Project-URL: Bug Tracker, https://github.com/marcosalvalaggio/femtogradissues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kiwigrad
 
 <h1 align="center">
-<img src="logo.png" width="300">
+<img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![PyPI version fury.io](https://badge.fury.io/py/kiwigrad.svg)](https://pypi.python.org/pypi/kiwigrad/)
 
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
@@ -57,20 +60,21 @@
 * Support for RNN1 feedforward neural networks.
 
 ### Example Implementation
 
 Here's an example implementation of a MLP net using Kiwigrad:
 
 ```python 
-from kiwigrad import * 
+from kiwigrad import MLP, Layer
 
 class PotNet(MLP):
     def __init__(self):
         layers = [
             Layer(nin=2, nout=16, bias=True, activation="relu"),
             Layer(nin=16, nout=16, bias=True, activation="relu"),
             Layer(nin=16, nout=1, bias=True, activation="linear")
         ]
         super().__init__(layers=layers)
 
 model = PotNet()
 ```
+
```

### Comparing `kiwigrad-0.20/pyproject.toml` & `kiwigrad-0.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kiwigrad"
-version = "0.20"
+version = "0.21"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Mini deep learning framework"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `kiwigrad-0.20/test/test.py` & `kiwigrad-0.21/test/test.py`

 * *Files identical despite different names*

