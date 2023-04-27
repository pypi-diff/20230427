# Comparing `tmp/pyqrack-1.6.3.tar.gz` & `tmp/pyqrack-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqrack-1.6.3.tar", last modified: Mon Apr 24 15:23:39 2023, max compression
+gzip compressed data, was "pyqrack-1.6.4.tar", last modified: Thu Apr 27 18:42:30 2023, max compression
```

## Comparing `pyqrack-1.6.3.tar` & `pyqrack-1.6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-24 15:23:39.952937 pyqrack-1.6.3/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.6.3/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-04-24 15:23:39.952937 pyqrack-1.6.3/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-04-24 15:23:34.000000 pyqrack-1.6.3/README.md
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.6.3/pyproject.toml
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-24 15:23:39.952937 pyqrack-1.6.3/pyqrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      401 2022-06-02 15:55:19.000000 pyqrack-1.6.3/pyqrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.6.3/pyqrack/pauli.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-04-04 19:59:28.000000 pyqrack-1.6.3/pyqrack/qrack_simulator.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-24 15:23:39.952937 pyqrack-1.6.3/pyqrack/qrack_system/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.6.3/pyqrack/qrack_system/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    25397 2023-04-24 15:23:34.000000 pyqrack-1.6.3/pyqrack/qrack_system/qrack_system.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-24 15:23:39.952937 pyqrack-1.6.3/pyqrack/util/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.6.3/pyqrack/util/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.6.3/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-24 15:23:39.952937 pyqrack-1.6.3/pyqrack.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-04-24 15:23:39.000000 pyqrack-1.6.3/pyqrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      412 2023-04-24 15:23:39.000000 pyqrack-1.6.3/pyqrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-04-24 15:23:39.000000 pyqrack-1.6.3/pyqrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-04-24 15:23:39.000000 pyqrack-1.6.3/pyqrack.egg-info/not-zip-safe
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-04-24 15:23:39.000000 pyqrack-1.6.3/pyqrack.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-04-24 15:23:39.952937 pyqrack-1.6.3/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-04-24 15:08:54.000000 pyqrack-1.6.3/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-27 18:42:30.607042 pyqrack-1.6.4/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1064 2021-12-27 16:00:58.000000 pyqrack-1.6.4/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-04-27 18:42:30.607042 pyqrack-1.6.4/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2767 2023-04-27 18:42:22.000000 pyqrack-1.6.4/README.md
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      104 2021-12-27 16:00:58.000000 pyqrack-1.6.4/pyproject.toml
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-27 18:42:30.607042 pyqrack-1.6.4/pyqrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      401 2022-06-02 15:55:19.000000 pyqrack-1.6.4/pyqrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      654 2022-06-18 20:18:56.000000 pyqrack-1.6.4/pyqrack/pauli.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    83208 2023-04-04 19:59:28.000000 pyqrack-1.6.4/pyqrack/qrack_simulator.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-27 18:42:30.607042 pyqrack-1.6.4/pyqrack/qrack_system/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      334 2021-12-27 16:00:58.000000 pyqrack-1.6.4/pyqrack/qrack_system/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    25397 2023-04-27 18:42:22.000000 pyqrack-1.6.4/pyqrack/qrack_system/qrack_system.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-27 18:42:30.607042 pyqrack-1.6.4/pyqrack/util/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      333 2022-06-18 20:18:56.000000 pyqrack-1.6.4/pyqrack/util/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2065 2022-06-18 20:18:56.000000 pyqrack-1.6.4/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-04-27 18:42:30.607042 pyqrack-1.6.4/pyqrack.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3744 2023-04-27 18:42:30.000000 pyqrack-1.6.4/pyqrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      412 2023-04-27 18:42:30.000000 pyqrack-1.6.4/pyqrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-04-27 18:42:30.000000 pyqrack-1.6.4/pyqrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-04-27 18:42:30.000000 pyqrack-1.6.4/pyqrack.egg-info/not-zip-safe
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        8 2023-04-27 18:42:30.000000 pyqrack-1.6.4/pyqrack.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-04-27 18:42:30.607042 pyqrack-1.6.4/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1559 2023-04-27 18:32:03.000000 pyqrack-1.6.4/setup.py
```

### Comparing `pyqrack-1.6.3/LICENSE` & `pyqrack-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrack-1.6.3/PKG-INFO` & `pyqrack-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.6.3
+Version: 1.6.4
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.6.3/README.md` & `pyqrack-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pyqrack-1.6.3/pyqrack/pauli.py` & `pyqrack-1.6.4/pyqrack/pauli.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.6.3/pyqrack/qrack_simulator.py` & `pyqrack-1.6.4/pyqrack/qrack_simulator.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.6.3/pyqrack/qrack_system/qrack_system.py` & `pyqrack-1.6.4/pyqrack/qrack_system/qrack_system.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.6.3/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py` & `pyqrack-1.6.4/pyqrack/util/convert_qiskit_circuit_to_qasm_experiment.py`

 * *Files identical despite different names*

### Comparing `pyqrack-1.6.3/pyqrack.egg-info/PKG-INFO` & `pyqrack-1.6.4/pyqrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrack
-Version: 1.6.3
+Version: 1.6.4
 Summary: pyqrack - Pure Python vm6502q/qrack Wrapper
 Home-page: https://github.com/vm6502q/pyqrack
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: MIT
 Keywords: pyqrack qrack simulator quantum gpu
 Classifier: Environment :: Console
```

### Comparing `pyqrack-1.6.3/setup.py` & `pyqrack-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 
 requirements = []
 
-VERSION = "1.6.3"
+VERSION = "1.6.4"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
 
 setup(
```

