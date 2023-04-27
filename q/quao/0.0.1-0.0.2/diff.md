# Comparing `tmp/quao-0.0.1.tar.gz` & `tmp/quao-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.0.1.tar", last modified: Thu Apr 27 03:41:06 2023, max compression
+gzip compressed data, was "quao-0.0.2.tar", last modified: Thu Apr 27 04:26:30 2023, max compression
```

## Comparing `quao-0.0.1.tar` & `quao-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 03:41:06.385785 quao-0.0.1/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-04-27 03:41:06.384786 quao-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.0.1/README.md
--rw-rw-rw-   0        0        0     1241 2023-04-27 03:32:16.000000 quao-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 03:41:06.386787 quao-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 03:41:06.269287 quao-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 03:41:06.307288 quao-0.0.1/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.0.1/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:41:06.345286 quao-0.0.1/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.0.1/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.0.1/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     2900 2023-04-26 11:10:24.000000 quao-0.0.1/src/quao/backend.py
--rw-rw-rw-   0        0        0      366 2023-04-26 11:27:39.000000 quao-0.0.1/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:41:06.382783 quao-0.0.1/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.0.1/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-04-26 05:03:52.000000 quao-0.0.1/src/quao/sdk/braket.py
--rw-rw-rw-   0        0        0     1640 2023-04-26 05:03:52.000000 quao-0.0.1/src/quao/sdk/cirq.py
--rw-rw-rw-   0        0        0     2110 2023-04-26 10:35:09.000000 quao-0.0.1/src/quao/sdk/qiskit.py
--rw-rw-rw-   0        0        0     1218 2023-04-27 02:50:32.000000 quao-0.0.1/src/quao/sdk/qsharp.py
--rw-rw-rw-   0        0        0     2442 2023-04-26 10:59:14.000000 quao-0.0.1/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:41:06.335287 quao-0.0.1/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-04-27 03:41:06.000000 quao-0.0.1/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-04-27 03:41:06.000000 quao-0.0.1/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 03:41:06.000000 quao-0.0.1/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2023-04-27 03:41:06.000000 quao-0.0.1/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 03:41:06.000000 quao-0.0.1/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 04:26:30.898668 quao-0.0.2/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-04-27 04:26:30.897671 quao-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1241 2023-04-27 04:25:01.000000 quao-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 04:26:30.898668 quao-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 04:26:30.800575 quao-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 04:26:30.826819 quao-0.0.2/src/quao/
+-rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.0.2/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:26:30.866775 quao-0.0.2/src/quao/algorithms/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.0.2/src/quao/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.0.2/src/quao/algorithms/shor.py
+-rw-rw-rw-   0        0        0     2900 2023-04-26 11:10:24.000000 quao-0.0.2/src/quao/backend.py
+-rw-rw-rw-   0        0        0      366 2023-04-26 11:27:39.000000 quao-0.0.2/src/quao/dataUtils.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:26:30.894692 quao-0.0.2/src/quao/sdk/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.0.2/src/quao/sdk/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-04-26 05:03:52.000000 quao-0.0.2/src/quao/sdk/braket.py
+-rw-rw-rw-   0        0        0     1640 2023-04-26 05:03:52.000000 quao-0.0.2/src/quao/sdk/cirq.py
+-rw-rw-rw-   0        0        0     2110 2023-04-26 10:35:09.000000 quao-0.0.2/src/quao/sdk/qiskit.py
+-rw-rw-rw-   0        0        0     1218 2023-04-27 02:50:32.000000 quao-0.0.2/src/quao/sdk/qsharp.py
+-rw-rw-rw-   0        0        0     2442 2023-04-26 10:59:14.000000 quao-0.0.2/src/quao/utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:26:30.854777 quao-0.0.2/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-04-27 04:26:30.000000 quao-0.0.2/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-04-27 04:26:30.000000 quao-0.0.2/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 04:26:30.000000 quao-0.0.2/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-04-27 04:26:30.000000 quao-0.0.2/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 04:26:30.000000 quao-0.0.2/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.0.1/LICENSE` & `quao-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/PKG-INFO` & `quao-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -12,15 +12,15 @@
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://citynow.vn/
 Keywords: quao,quantum
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # quao
```

### Comparing `quao-0.0.1/README.md` & `quao-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/pyproject.toml` & `quao-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.0.1"
+version = "0.0.2"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["quao", "quantum"]
 dependencies = [
-    "qiskit==0.36.1",
-    "cirq==1.0.0",
-    "amazon-braket-sdk==1.19.0",
+    "qiskit==0.41.1",
+    "cirq==1.1.0",
+    "amazon-braket-sdk==1.36.5",
     "numpy>=1.22.3",
-    "strangeworks==0.2.13",
-    "strangeworks-braket==0.1.3"
+    "strangeworks==0.2.16",
+    "strangeworks-braket==1.0.3"
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://citynow.vn/"
 
 [tool.bumpver]
-current_version = "0.2.3"
+current_version = "0.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `quao-0.0.1/src/quao/algorithms/shor.py` & `quao-0.0.2/src/quao/algorithms/shor.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/src/quao/backend.py` & `quao-0.0.2/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/src/quao/sdk/braket.py` & `quao-0.0.2/src/quao/sdk/braket.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/src/quao/sdk/cirq.py` & `quao-0.0.2/src/quao/sdk/cirq.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/src/quao/sdk/qiskit.py` & `quao-0.0.2/src/quao/sdk/qiskit.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/src/quao/sdk/qsharp.py` & `quao-0.0.2/src/quao/sdk/qsharp.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/src/quao/utilities.py` & `quao-0.0.2/src/quao/utilities.py`

 * *Files identical despite different names*

### Comparing `quao-0.0.1/src/quao.egg-info/PKG-INFO` & `quao-0.0.2/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -12,15 +12,15 @@
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://citynow.vn/
 Keywords: quao,quantum
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # quao
```

