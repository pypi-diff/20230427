# Comparing `tmp/pyttb-1.6.0.tar.gz` & `tmp/pyttb-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttb-1.6.0.tar", last modified: Sun Apr 16 15:18:22 2023, max compression
+gzip compressed data, was "pyttb-1.6.1.tar", last modified: Thu Apr 27 15:01:50 2023, max compression
```

## Comparing `pyttb-1.6.0.tar` & `pyttb-1.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.839779 pyttb-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-16 15:18:04.000000 pyttb-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-16 15:18:22.839779 pyttb-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-16 15:18:04.000000 pyttb-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.835779 pyttb-1.6.0/pyttb/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    58614 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    75831 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sptenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    91144 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sptensor3.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sumtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/symktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/symtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    58044 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/tucker_als.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.835779 pyttb-1.6.0/pyttb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:18:22.839779 pyttb-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.839779 pyttb-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_import_export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    43526 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    56534 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.288733 pyttb-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 15:01:19.000000 pyttb-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-27 15:01:50.288733 pyttb-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 15:01:19.000000 pyttb-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.284733 pyttb-1.6.1/pyttb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58614 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80311 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sptenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93748 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sptensor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sumtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/symktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/symtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60229 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.284733 pyttb-1.6.1/pyttb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:01:50.288733 pyttb-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.288733 pyttb-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_import_export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42650 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68449 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57951 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_tucker_als.py
```

### Comparing `pyttb-1.6.0/LICENSE` & `pyttb-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/PKG-INFO` & `pyttb-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python Tensor Toolbox
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyttb-1.6.0/README.md` & `pyttb-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyproject.toml` & `pyttb-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/__init__.py` & `pyttb-1.6.1/pyttb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 import warnings
 
 from pyttb.cp_als import cp_als
 from pyttb.cp_apr import *
 from pyttb.export_data import export_data
 from pyttb.hosvd import hosvd
 from pyttb.import_data import import_data
 from pyttb.khatrirao import khatrirao
 from pyttb.ktensor import ktensor
 from pyttb.pyttb_utils import *
 from pyttb.sptenmat import sptenmat
-from pyttb.sptensor import sptensor
+from pyttb.sptensor import sptendiag, sptenrand, sptensor
 from pyttb.sptensor3 import sptensor3
 from pyttb.sumtensor import sumtensor
 from pyttb.symktensor import symktensor
 from pyttb.symtensor import symtensor
 from pyttb.tenmat import tenmat
-from pyttb.tensor import tensor
+from pyttb.tensor import tendiag, tenones, tenrand, tensor, tenzeros
 from pyttb.ttensor import ttensor
 from pyttb.tucker_als import tucker_als
 
 
 def ignore_warnings(ignore=True):
     if ignore:
         warnings.simplefilter("ignore")
```

### Comparing `pyttb-1.6.0/pyttb/cp_als.py` & `pyttb-1.6.1/pyttb/cp_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/cp_apr.py` & `pyttb-1.6.1/pyttb/cp_apr.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/export_data.py` & `pyttb-1.6.1/pyttb/export_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/hosvd.py` & `pyttb-1.6.1/pyttb/hosvd.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/import_data.py` & `pyttb-1.6.1/pyttb/import_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/khatrirao.py` & `pyttb-1.6.1/pyttb/khatrirao.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/ktensor.py` & `pyttb-1.6.1/pyttb/ktensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,100 +1,114 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 
 """Classes and functions for working with Kruskal tensors."""
 from __future__ import annotations
 
+import logging
 import warnings
 
 import numpy as np
 import scipy.sparse as sparse
 import scipy.sparse.linalg
 
 import pyttb as ttb
 from pyttb.pyttb_utils import *
 
 
 class ktensor(object):
     """
-    Class for Kruskal tensors (decomposed).
+    KTENSOR Class for Kruskal tensors (decomposed).
 
     Contains the following data members:
 
-      * ``weights``: :class:`numpy.ndarray` vector containing the weights of the rank-1 tensors defined by the outer \
-    products of the column vectors of the factor_matrices.
-
-      * ``factor_matrices``: :class:`list` of :class:`numpy.ndarray`. The length of the list is equal to the number \
-    of dimensions of the tensor. The shape of the ith element of the list is (n_i, r), where n_i is the length \
-    dimension i and r is the rank of the tensor (as well as the length of the weights vector).
-
-    Although the constructor, `__init__()`, can be used to create an empty :class:`pyttb.ktensor`, there
-    are several class methods that can be used to create an instance of this class:
+    ``weights``: :class:`numpy.ndarray` vector containing the weights of the
+    rank-1 tensors defined by the outer products of the column vectors of the
+    factor_matrices.
+
+    ``factor_matrices``: :class:`list` of :class:`numpy.ndarray`. The length
+    of the list is equal to the number of dimensions of the tensor. The shape
+    of the ith element of the list is (n_i, r), where n_i is the length
+    dimension i and r is the rank of the tensor (as well as the length of the
+    weights vector).
+
+    Although the constructor `__init__()` can be used to create an empty
+    :class:`pyttb.ktensor`, there are several class methods that can be used
+    to create an instance of this class:
 
       * :meth:`from_data`
       * :meth:`from_tensor_type`
       * :meth:`from_factor_matrices`
       * :meth:`from_function`
       * :meth:`from_vector`
+
+    Examples
+    --------
+    For all examples listed below, the following module imports are assumed:
+
+    >>> import pyttb as ttb
+    >>> import numpy as np
     """
 
     __slots__ = ("weights", "factor_matrices")
 
     def __init__(self):
         """
-        Constructor for :class:`pyttb.ktensor`
+        Construct an empty :class:`pyttb.ktensor`
 
-        The constructor takes no arguments and returns an empty :class:`pyttb.ktensor`.
+        The constructor takes no arguments and returns an empty
+        :class:`pyttb.ktensor`.
         """
         # Empty constructor
-        self.weights = np.array([])  # renamed from lambda to weights
-        self.factor_matrices = (
-            []
-        )  # changed from cell array to list; changed name from 'u' to 'factor_matrices'
+        self.weights = np.array([])
+        self.factor_matrices = []
 
     @classmethod
     def from_data(cls, weights, *factor_matrices):
         """
         Construct a :class:`pyttb.ktensor` from weights and factor matrices.
 
-        The length of the list or the number of arguments specified by `factor_matrices` must equal
-        the length of `weights`
+        The length of the list or the number of arguments specified by
+        `factor_matrices` must equal the length of `weights`. See
+        :class:`pyttb.ktensor` for parameter descriptions.
 
         Parameters
         ----------
-        weights: :class:`numpy.ndarray`
-        factor_matrices: :class:`list` of :class:`numpy.ndarray` or variable number of :class:`numpy.ndarray`
+        weights: :class:`numpy.ndarray`, required
+        factor_matrices: :class:`list` of :class:`numpy.ndarray` or variable number of :class:`numpy.ndarray`, required
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create a `ktensor` from weights and a list of factor matrices:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` from weights and a list of factor
+        matrices:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
-        >>> K_from_list = ttb.ktensor.from_data(weights, [fm0, fm1])
-        >>> print(K_from_list)
+        >>> K = ttb.ktensor.from_data(weights, [fm0, fm1])
+        >>> print(K)
         ktensor of shape 2 x 2
         weights=[1. 2.]
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-        Create a `ktensor` from weights and a factor matrices passed as arguments:
+        Create a :class:`pyttb.ktensor` from weights and factor matrices passed as
+        arguments:
 
-        >>> K_from_args = ttb.ktensor.from_data(weights, fm0, fm1)
-        >>> print(K_from_args)
+        >>> K = ttb.ktensor.from_data(weights, fm0, fm1)
+        >>> print(K)
         ktensor of shape 2 x 2
         weights=[1. 2.]
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
@@ -141,28 +155,29 @@
                 k.factor_matrices[i] = k.factor_matrices[i].astype(float)
 
         return k
 
     @classmethod
     def from_tensor_type(cls, source) -> ktensor:
         """
-        Construct a ktensor from another ktensor. A deep copy of the data from the input ktensor
-        is used for the new ktensor.
+        Construct a :class:`pyttb.ktensor` from another
+        :class:`pyttb.ktensor`. A deep copy of the data from the input
+        :class:`pyttb.ktensor` is used for the new :class:`pyttb.ktensor`.
 
         Parameters
         ----------
-        source: :class:`pyttb.ktensor`
+        source: :class:`pyttb.ktensor`, required
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create an instance of a `ktensor`:
+        Examples
+        --------
+        Create an instance of a :class:`pyttb.ktensor`:
 
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> factor_matrices = [fm0, fm1]
         >>> K_source = ttb.ktensor.from_factor_matrices(factor_matrices)
         >>> print(K_source)
         ktensor of shape 2 x 2
@@ -170,28 +185,29 @@
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-        Create another instance of a `ktensor` from the original one above:
+        Create another instance of a :class:`pyttb.ktensor` from the original
+        one above:
 
-        >>> K_copy = ttb.ktensor.from_tensor_type(K_source)
-        >>> print(K_copy)
+        >>> K = ttb.ktensor.from_tensor_type(K_source)
+        >>> print(K)
         ktensor of shape 2 x 2
         weights=[1. 1.]
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-         See also :func:`~pyttb.ktensor.copy`
+        See also :func:`pyttb.ktensor.copy`
         """
         if isinstance(source, ktensor):
             return cls().from_data(
                 source.weights.copy(), [f.copy() for f in source.factor_matrices]
             )
 
         # TODO impement conversion when symktensor has been implemented
@@ -202,47 +218,51 @@
         #     raise NotImplementedError
 
         assert False, "Cannot convert from {} to ktensor".format(str(source.__class__))
 
     @classmethod
     def from_factor_matrices(cls, *factor_matrices):
         """
-        Construct a ktensor from factor matrices. The weights of the returned ktensor will all be equal to 1.
+        Construct a :class:`pyttb.ktensor` from factor matrices. The weights
+        of the returned :class:`pyttb.ktensor` will all be equal to 1.
 
         Parameters
         ----------
-        factor_matrices: :class:`list` of :class:`numpy.ndarray` or variable number of :class:`numpy.ndarray`
-            The number of columns of each of the factor matrices must be the same.
+        factor_matrices: :class:`list` of :class:`numpy.ndarray` or variable number of :class:`numpy.ndarray`, required
+            The number of columns of each of the factor matrices must be the
+            same.
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create a `ktensor` from a list of factor matrices:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` from a :class:`list` of factor
+        matrices:
 
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> factor_matrices = [fm0, fm1]
-        >>> K_from_list = ttb.ktensor.from_factor_matrices(factor_matrices)
-        >>> print(K_from_list)
+        >>> K = ttb.ktensor.from_factor_matrices(factor_matrices)
+        >>> print(K)
         ktensor of shape 2 x 2
         weights=[1. 1.]
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-        Create a `ktensor` from a sequence of factor matrices passed as arguments:
+        Create a :class:`pyttb.ktensor` from factor matrices passed as
+        arguments:
 
-        >>> K_from_args = ttb.ktensor.from_factor_matrices(fm0, fm1)
-        >>> print(K_from_args)
+        >>> K = ttb.ktensor.from_factor_matrices(fm0, fm1)
+        >>> print(K)
         ktensor of shape 2 x 2
         weights=[1. 1.]
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
@@ -260,35 +280,40 @@
             ), "Input parameter 'factor_matrices' must be a list of numpy.array's."
         nc = _factor_matrices[0].shape[1]
         return cls().from_data(np.ones(nc), _factor_matrices)
 
     @classmethod
     def from_function(cls, fun, shape, num_components):
         """
-        Construct a ktensor whose factor matrix entries are set using a function. The weights of the returned ktensor will all be equal to 1.
+        Construct a :class:`pyttb.ktensor` whose factor matrix entries are
+        set using a function. The weights of the returned
+        :class:`pyttb.ktensor` will all be equal to 1.
 
         Parameters
         ----------
-        fun: function
-          A function that can accept a shape (i.e., :class:`tuple` of dimension sizes) and return a :class:`numpy.ndarray`
-          of that shape. Example functions include `numpy.random.random_sample`, `numpy,zeros`, `numpy.ones`.
-        shape: :class:`tuple`
-        num_components: int
+        fun: function, required
+            A function that can accept a shape (i.e., :class:`tuple` of
+            dimension sizes) and return a :class:`numpy.ndarray` of that shape.
+            Example functions include `numpy.random.random_sample`,
+            `numpy,zeros`, `numpy.ones`.
+        shape: :class:`tuple`, required
+        num_components: int, required
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create a `ktensor` with entries of the factor matrices taken from a uniform random distribution:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` with entries of the factor matrices
+        taken from a uniform random distribution:
 
         >>> np.random.seed(1)
-        >>> K_random = ttb.ktensor.from_function(np.random.random_sample, (2, 3, 4), 2)
-        >>> print(K_random)  # doctest: +ELLIPSIS
+        >>> K = ttb.ktensor.from_function(np.random.random_sample, (2, 3, 4), 2)
+        >>> print(K)  # doctest: +ELLIPSIS
         ktensor of shape 2 x 3 x 4
         weights=[1. 1.]
         factor_matrices[0] =
         [[4.1702...e-01 7.2032...e-01]
          [1.1437...e-04 3.0233...e-01]]
         factor_matrices[1] =
         [[0.1467... 0.0923...]
@@ -296,18 +321,18 @@
          [0.3967... 0.5388...]]
         factor_matrices[2] =
         [[0.4191... 0.6852...]
          [0.2044... 0.8781...]
          [0.0273... 0.6704...]
          [0.4173...  0.5586...]]
 
-        Create a `ktensor` with entries equal to 1:
+        Create a :class:`pyttb.ktensor` with entries equal to 1:
 
-        >>> K_ones = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
-        >>> print(K_ones)
+        >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
+        >>> print(K)
         ktensor of shape 2 x 3 x 4
         weights=[1. 1.]
         factor_matrices[0] =
         [[1. 1.]
          [1. 1.]]
         factor_matrices[1] =
         [[1. 1.]
@@ -315,18 +340,18 @@
          [1. 1.]]
         factor_matrices[2] =
         [[1. 1.]
          [1. 1.]
          [1. 1.]
          [1. 1.]]
 
-        Create a `ktensor` with entries equal to 0:
+        Create a :class:`pyttb.ktensor` with entries equal to 0:
 
-        >>> K_zeros = ttb.ktensor.from_function(np.zeros, (2, 3, 4), 2)
-        >>> print(K_zeros)
+        >>> K = ttb.ktensor.from_function(np.zeros, (2, 3, 4), 2)
+        >>> print(K)
         ktensor of shape 2 x 3 x 4
         weights=[1. 1.]
         factor_matrices[0] =
         [[0. 0.]
          [0. 0.]]
         factor_matrices[1] =
         [[0. 0.]
@@ -350,41 +375,48 @@
         for i in range(nd):
             factor_matrices.append(fun((shape[i], num_components)))
         return cls().from_data(weights, factor_matrices)
 
     @classmethod
     def from_vector(cls, data, shape, contains_weights):
         """
-        Construct a ktensor from a vector. The rank of the `ktensor` is inferred from the shape and size of the vector.
+        Construct a :class:`pyttb.ktensor` from a vector (given as a
+        :class:`numpy.ndarray`) and shape (given as a
+        :class:`numpy.ndarray`). The rank of the :class:`pyttb.ktensor`
+        is inferred from the shape and length of the vector.
 
         Parameters
         ----------
-        data: :class:`numpy.ndarray`
-          Vector containing either elements of the factor matrices (when contains_weights==False) or
-          elements of the weights and factor matrices (when contains_weights==True). When both the
-          elements of the weights and the factor_matrices are present, the weights come first and
-          the columns of the factor matrices come next.
-        shape: :class:`numpy.ndarray`
-          Vector containing the shape of the tensor (i.e., sizes of the dimensions).
-        contains_weights: bool
-          Flag to specify whether or not ``data`` contains weights. If False, all weights are set to 1.
+        data: :class:`numpy.ndarray`, required
+            Vector containing either elements of the factor matrices (when
+            `contains_weights`==False) or elements of the weights and factor
+            matrices (when `contains_weights`==True). When both the elements of
+            the weights and the factor_matrices are present, the weights come
+            first and the columns of the factor matrices come next.
+        shape: :class:`numpy.ndarray`, required
+            Vector containing the shape of the tensor (i.e., lengths of the
+            dimensions).
+        contains_weights: bool, required
+            Flag to specify whether or not `data` contains weights. If False,
+            all weights are set to 1.
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create a `ktensor` from a vector containing only elements of the factor matrices:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` from a vector containing only
+        elements of the factor matrices:
 
         >>> rank = 2
         >>> shape = np.array([2, 3, 4])
         >>> data = np.arange(1, rank*sum(shape)+1).astype(float)
-        >>> K_without_weights = ttb.ktensor.from_vector(data[:], shape, False)
-        >>> print(K_without_weights)
+        >>> K = ttb.ktensor.from_vector(data[:], shape, False)
+        >>> print(K)
         ktensor of shape 2 x 3 x 4
         weights=[1. 1.]
         factor_matrices[0] =
         [[1. 3.]
          [2. 4.]]
         factor_matrices[1] =
         [[ 5.  8.]
@@ -392,20 +424,21 @@
          [ 7. 10.]]
         factor_matrices[2] =
         [[11. 15.]
          [12. 16.]
          [13. 17.]
          [14. 18.]]
 
-        Create a `ktensor` from a vector containing elements of both the weights and the factor matrices:
+        Create a :class:`pyttb.ktensor` from a vector containing elements
+        of both the weights and the factor matrices:
 
         >>> weights = 2 * np.ones(rank).astype(float)
         >>> weights_and_data = np.concatenate((weights, data), axis=0)
-        >>> K_with_weights = ttb.ktensor.from_vector(weights_and_data[:], shape, True)
-        >>> print(K_with_weights)
+        >>> K = ttb.ktensor.from_vector(weights_and_data[:], shape, True)
+        >>> print(K)
         ktensor of shape 2 x 3 x 4
         weights=[2. 2.]
         factor_matrices[0] =
         [[1. 3.]
          [2. 4.]]
         factor_matrices[1] =
         [[ 5.  8.]
@@ -458,29 +491,37 @@
             )
             factor_matrices.append(factor_matrix)
 
         return cls().from_data(weights, factor_matrices)
 
     def arrange(self, weight_factor=None, permutation=None):
         """
-        Arrange the rank-1 components of a `ktensor`. The columns are permuted in place, so you must make a copy
-        before calling this method if you want to store the original.
+        Arrange the rank-1 components of a :class:`pyttb.ktensor`. The
+        columns are permuted in place, so you must make a copy before calling
+        this method if you want to store the original :class:`pyttb.ktensor`.
+        One of the parameters, either `weight_factor` or `permutation`
+        must be passed, and passing both parameters leads to an error.
 
         Parameters
         ----------
-        weight_factor:
-        permutation:
+        weight_factor: int, optional
+            The index of the factor that the weights will be absorbed into
+        permutation: :class:`tuple`, :class:`list`, :class:`numpy.ndarray`, optional
+            The new order of the components of the :class:`pyttb.ktensor`
+            into which to permute. The permutation must be of length equal to
+            the number of components of the :class:`pyttb.ktensor`, N, and
+            must be a permutation of 1 to N.
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create the initial `ktensor`:
+        Examples
+        --------
+        Create the initial :class:`pyttb.ktensor`:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> K = ttb.ktensor.from_data(weights, [fm0, fm1])
         >>> print(K)
         ktensor of shape 2 x 2
@@ -544,23 +585,23 @@
         #     X.u{end} = full(X.u{end} * spdiags(X.lambda,0,r,r));
         #     X.lambda = ones(size(X.lambda));
         # end
         return self
 
     def copy(self):
         """
-        Make a deep copy of a `ktensor`.
+        Make a deep copy of a :class:`pyttb.ktensor`.
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create a random `ktensor` with weights of 1:
+        Examples
+        --------
+        Create a random :class:`pyttb.ktensor` with weights of 1:
 
         >>> np.random.seed(1)
         >>> K = ttb.ktensor.from_function(np.random.random_sample, (2, 3, 4), 2)
         >>> print(K)  # doctest: +ELLIPSIS
         ktensor of shape 2 x 3 x 4
         weights=[1. 1.]
         factor_matrices[0] =
@@ -572,101 +613,122 @@
          [0.3967... 0.5388...]]
         factor_matrices[2] =
         [[0.4191... 0.6852...]
          [0.2044... 0.8781...]
          [0.0273... 0.6704...]
          [0.4173... 0.5586...]]
 
-        Create a copy of the `ktensor` and change the weights:
+        Create a copy of the :class:`pyttb.ktensor` and change the weights:
 
-        >>> K1 = K.copy()
-        >>> K1.weights = np.array([2., 3.])
-        >>> print(K1)  # doctest: +ELLIPSIS
+        >>> K2 = K.copy()
+        >>> K2.weights = np.array([2., 3.])
+        >>> print(K2)  # doctest: +ELLIPSIS
         ktensor of shape 2 x 3 x 4
         weights=[2. 3.]
         factor_matrices[0] =
         [[4.1702...e-01 7.2032...e-01]
          [1.1437...e-04 3.023...e-01]]
         factor_matrices[1] =
         [[0.1467... 0.0923...]
          [0.1862... 0.3455...]
          [0.3967... 0.5388...]]
         factor_matrices[2] =
         [[0.4191... 0.6852...]
          [0.2044... 0.8781...]
          [0.0273... 0.6704...]
          [0.4173... 0.5586...]]
+
+        Show that the original :class:`pyttb.ktensor` is unchanged:
+
+        >>> print(K)  # doctest: +ELLIPSIS
+        ktensor of shape 2 x 3 x 4
+        weights=[1. 1.]
+        factor_matrices[0] =
+        [[4.1702...e-01 7.2032...e-01]
+         [1.1437...e-04 3.0233...e-01]]
+        factor_matrices[1] =
+        [[0.1467... 0.0923...]
+         [0.1862... 0.3455...]
+         [0.3967... 0.5388...]]
+        factor_matrices[2] =
+        [[0.4191... 0.6852...]
+         [0.2044... 0.8781...]
+         [0.0273... 0.6704...]
+         [0.4173... 0.5586...]]
         """
         return ttb.ktensor.from_tensor_type(self)
 
     def double(self):
         """
-        Convert `ktensor` to numpy array.
+        Convert :class:`pyttb.ktensor` to :class:`numpy.ndarray`.
 
         Returns
         -------
         :class:`numpy.ndarray`
 
-        Example
-        -------
+        Examples
+        --------
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> factor_matrices = [fm0, fm1]
         >>> K = ttb.ktensor.from_data(weights, factor_matrices)
         >>> K.double()
         array([[29., 39.],
                [63., 85.]])
+        >>> type(K.double())
+        <class 'numpy.ndarray'>
         """
         return self.full().double()
 
     def end(self, k=None):
         """
-        Last index of indexing expression for `ktensor`.
+        Last index of indexing expression for :class:`pyttb.ktensor`.
 
         Parameters
         ----------
-        k: int
-            dimension for subscripted indexing
-        n: int
-            dimensions to index
+        k: int, optional
+          dimension for subscripted indexing
 
         Returns
         -------
         int: index
 
-        Example
-        -------
+        Examples
+        --------
         >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
         >>> print(K.end(2))
         3
         """
 
         if k is not None:  # Subscripted indexing
             return self.shape[k] - 1
         else:  # For linear indexing
             return np.prod(self.shape) - 1
 
     def extract(self, idx=None):
         """
-        Creates a new `ktensor` with only the specified components.
+        Creates a new :class:`pyttb.ktensor` with only the specified
+        components.
 
         Parameters
         ----------
-        idx: int, tuple, list, :class:`numpy.ndarray`
-            Index set of components to extract. It should be the case that `idx` is a subset of
-            [0,...,self.ncomponents]. If this parameter is None or is empty, a copy of the ktensor is returned.
+        idx: int, :class:`tuple`, :class:`list`, :class:`numpy.ndarray`, optional
+            Index set of components to extract. It should be the case that
+            `idx` is a subset of [0,...,`self.ncomponents`]. If this
+            parameter is None or is empty, a copy of the
+            :class:`pyttb.ktensor` is returned.
 
         Returns
         -------
-        :class:`ktensor`
+        :class:`pyttb.ktensor`
 
-        Example
-        -------
-        Create a `ktensor`:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor`:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> K = ttb.ktensor.from_data(weights, [fm0, fm1])
         >>> print(K)
         ktensor of shape 2 x 2
@@ -674,15 +736,16 @@
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-        Create a new `ktensor`, extracting only the second component from each factor of the original `ktensor`:
+        Create a new :class:`pyttb.ktensor`, extracting only the second
+        component from each factor of the original :class:`pyttb.ktensor`:
 
         >>> K.extract([1])
         ktensor of shape 2 x 2
         weights=[2.]
         factor_matrices[0] =
         [[2.]
          [4.]]
@@ -723,33 +786,37 @@
                     new_factor_matrices.append(self.factor_matrices[i][:, components])
                 return self.from_data(new_weights, new_factor_matrices)
         else:
             assert False, "Input parameter must be an int, tuple, list or numpy.ndarray"
 
     def fixsigns(self, other=None):
         """
-        Change the elements of a `ktensor` in place so that the largest magnitude entries for
-        each column vector in each factor matrix are positive, provided that the
-        sign on pairs of vectors in a rank-1 component can be flipped.
+        Change the elements of a :class:`pyttb.ktensor` in place so that the
+        largest magnitude entries for each column vector in each factor
+        matrix are positive, provided that the sign on pairs of vectors in a
+        rank-1 component can be flipped.
 
         Parameters
         ----------
-        other: :class:`pyttb.ktensor`
-            If not None, returns a version of the `ktensor` where some of the signs of
-            the columns of the factor matrices have been flipped to better align
-            with `other`.
+        other: :class:`pyttb.ktensor`, optional
+            If not None, returns a version of the :class:`pyttb.ktensor`
+            where some of the signs of the columns of the factor matrices have
+            been flipped to better align with `other`. In not None, both
+            :class:`pyttb.ktensor` objects are first normalized (using
+            :func:`~pyttb.ktensor.normalize`).
 
         Returns
         -------
         :class:`pyttb.ktensor`
-            The changes are made in place and a reference to the updated tensor is returned
+            The changes are made in place and a reference to the updated
+            tensor is returned
 
-        Example
-        -------
-        Create a `ktensor` with negative large magnitude entries:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` with negative large magnitude entries:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> K = ttb.ktensor.from_data(weights, [fm0, fm1])
         >>> K.factor_matrices[0][1, 1] = -K.factor_matrices[0][1, 1]
         >>> K.factor_matrices[1][1, 1] = -K.factor_matrices[1][1, 1]
@@ -771,20 +838,20 @@
         factor_matrices[0] =
         [[ 1. -2.]
          [ 3.  4.]]
         factor_matrices[1] =
         [[ 5. -6.]
          [ 7.  8.]]
 
-        Fix the signs using another `ktensor`:
+        Fix the signs using another :class:`pyttb.ktensor`:
 
         >>> K = ttb.ktensor.from_data(weights, [fm0, fm1])
         >>> K2 = K.copy()
-        >>> K2.factor_matrices[0][1, 1] = - K2.factor_matrices[0][1, 1]
-        >>> K2.factor_matrices[1][1, 1] = - K2.factor_matrices[1][1, 1]
+        >>> K2.factor_matrices[0][1, 1] = -K2.factor_matrices[0][1, 1]
+        >>> K2.factor_matrices[1][1, 1] = -K2.factor_matrices[1][1, 1]
         >>> K = K.fixsigns(K2)
         >>> print(K)  # doctest: +ELLIPSIS
         ktensor of shape 2 x 2
         weights=[27.2029... 89.4427...]
         factor_matrices[0] =
         [[ 0.3162... -0.4472...]
          [ 0.9486... -0.8944...]]
@@ -865,90 +932,104 @@
                     )
                     best_sign[sort_idx[i], r] = -1
 
             return self
 
     def full(self):
         """
-        Convert a `ktensor` to a (dense) `tensor`.
+        Convert a :class:`pyttb.ktensor` to a :class:`pyttb.tensor`.
 
         Returns
         -------
         :class:`pyttb.tensor`
 
-        Example
-        -------
+        Examples
+        --------
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> K = ttb.ktensor.from_data(weights, [fm0, fm1])
+        >>> print(K)
+        ktensor of shape 2 x 2
+        weights=[1. 2.]
+        factor_matrices[0] =
+        [[1. 2.]
+         [3. 4.]]
+        factor_matrices[1] =
+        [[5. 6.]
+         [7. 8.]]
         >>> print(K.full()) # doctest: +NORMALIZE_WHITESPACE
         tensor of shape 2 x 2
         data[:, :] =
         [[29. 39.]
          [63. 85.]]
         <BLANKLINE>
         """
         data = self.weights @ ttb.khatrirao(self.factor_matrices, reverse=True).T
         return ttb.tensor.from_data(data, self.shape)
 
     def innerprod(self, other):
         """
-        Efficient inner product with a `ktensor`.
+        Efficient inner product with a :class:`pyttb.ktensor`.
 
-        Efficiently computes the inner product between two tensors, self and other.  If other is a ktensor,
-        the inner product is computed using inner products of the factor matrices. Otherwise, the inner product
-        is computed using ttv with all of the columns of self's factor matrices.
+        Efficiently computes the inner product between two tensors, `self`
+            and `other`.  If other is a :class:`pyttb.ktensor`, the inner
+            product is computed using inner products of the factor matrices.
+            Otherwise, the inner product is computed using the `ttv` (tensor
+            times vector) of `other` with all of the columns of
+            `self.factor_matrices`.
 
         Parameters
         ----------
-        other: compute inner product of ktensor with other
+        other: :class:`pyttb.ktensor`, :class:`pyttb.sptensor`, :class:`pyttb.tensor`, or :class:`pyttb.ttensor`, required
+            Tensor with which to compute the inner product.
 
         Returns
         -------
         :float
 
-        Example
-        -------
+        Examples
+        --------
         >>> K = ttb.ktensor.from_function(np.ones, (2,3,4), 2)
         >>> print(K.innerprod(K))
         96.0
         """
         if not (self.shape == other.shape):
             assert False, "Innerprod can only be computed for tensors of the same size"
 
         if isinstance(other, ktensor):
             M = np.outer(self.weights, other.weights)
             for i in range(self.ndims):
                 M = M * (self.factor_matrices[i].T @ other.factor_matrices[i])
             return np.sum(np.sum(M))
 
-        if isinstance(other, (ttb.tensor, ttb.sptensor, ttb.ttensor)):
+        if isinstance(other, (ttb.sptensor, ttb.tensor, ttb.ttensor)):
             res = 0.0
             for r in range(self.ncomponents):
                 vecs = []
                 for n in range(self.ndims):
                     vecs.append(self.factor_matrices[n][:, r])
                 res = res + self.weights[r] * other.ttv(vecs)
             return res
 
     def isequal(self, other):
         """
-        Equal comparator for `ktensors`.
+        Equal comparator for :class:`pyttb.ktensor` objects.
 
         Parameters
         ----------
-        other: compare equality of ktensor to other
+        other: :class:`pyttb.ktensor`, required
+            :class:`pyttb.ktensor` with which to compare.
 
         Returns
         -------
         :bool
 
-        Example
-        -------
+        Examples
+        --------
         >>> K1 = ttb.ktensor.from_function(np.ones, (2,3,4), 2)
         >>> weights = np.ones((2, 1))
         >>> factor_matrices = [np.ones((2, 2)), np.ones((3, 2)), np.ones((4, 2))]
         >>> K2 = ttb.ktensor.from_data(weights, factor_matrices)
         >>> print(K1.isequal(K2))
         True
         """
@@ -961,42 +1042,46 @@
         for k in range(self.ndims):
             if not (self.factor_matrices[k] == other.factor_matrices[k]).all():
                 return False
         return True
 
     def issymmetric(self, return_diffs=False):
         """
-        Returns true if the `ktensor` is exactly symmetric for every permutation.
+        Returns True if the :class:`pyttb.ktensor` is exactly symmetric for
+        every permutation.
 
         Parameters
         ----------
-        return_diffs: bool
-            If True, returns the matrix of the norm of the differences between the factor matrices
+        return_diffs: bool, optional
+            If True, returns the matrix of the norm of the differences between
+            the factor matrices.
 
         Returns
         -------
         :bool
-        :class:`numpy.ndarray`
-            Matrix of the norm of the differences between the factor matrices (optional)
+        :class:`numpy.ndarray`, optional
+            Matrix of the norm of the differences between the factor matrices
 
-        Example
-        -------
-        Create a 'ktensor` that is symmetric and test if it is symmetric:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` that is symmetric and test if it is
+        symmetric:
 
         >>> K = ttb.ktensor.from_function(np.ones, (3, 3, 3), 2)
         >>> print(K.issymmetric())
         True
 
-        Create a `ktensor` that is not symmetric and return the differences:
+        Create a :class:`pyttb.ktensor` that is not symmetric and return the
+        differences:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
-        >>> K1 = ttb.ktensor.from_data(weights, [fm0, fm1])
-        >>> issym, diffs = K1.issymmetric(return_diffs=True)
+        >>> K2 = ttb.ktensor.from_data(weights, [fm0, fm1])
+        >>> issym, diffs = K2.issymmetric(return_diffs=True)
         >>> print(diffs)
         [[0. 8.]
          [0. 0.]]
         """
         diffs = np.zeros((self.ndims, self.ndims))
         for i in range(self.ndims):
             for j in range(i + 1, self.ndims):
@@ -1013,34 +1098,39 @@
         if return_diffs:
             return issym, diffs
         else:
             return issym
 
     def mask(self, W):
         """
-        Extract `ktensor` values as specified by a mask `tensor`
+        Extract :class:`pyttb.ktensor` values as specified by `W`, a
+        :class:`pyttb.tensor` or :class:`pyttb.sptensor` containing
+        only values of zeros (0) and ones (1). The values in the
+        :class:`pyttb.ktensor` corresponding to the indices for the
+        ones (1) in `W` will be returned as a column vector.
 
         Parameters
         ----------
-        W: :class:`pyttb.sptensor`
+        W: :class:`pyttb.tensor` or :class:`pyttb.sptensor`, required
 
         Returns
         -------
-        :class:`Numpy.ndarray`
+        :class:`numpy.ndarray`
 
-        Example
-        -------
-        Create a `ktensor`:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor`:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> K = ttb.ktensor.from_data(weights, [fm0, fm1])
 
-        Create a mask `tensor` and extract the elements of the `ktensor` using the mask:
+        Create a mask :class:`pyttb.tensor` and extract the elements of the
+        :class:`pyttb.ktensor` using the mask:
 
         >>> W = ttb.tensor.from_data(np.array([[0, 1], [1, 0]]))
         >>> print(K.mask(W))
         [[63.]
          [39.]]
         """
         # Error check
@@ -1061,23 +1151,25 @@
                 akvals = self.factor_matrices[k][wsubs[:, [k]], j]
                 tmpvals = tmpvals * akvals
             vals = vals + tmpvals
         return vals
 
     def mttkrp(self, U, n):
         """
-        Matricized `tensor` times Khatri-Rao product for `ktensor`.
+        Matricized tensor times Khatri-Rao product for :class:`pyttb.ktensor`.
 
-        Efficiently calculates the matrix product of the n-mode matricization of the `ktensor` with the
-        Khatri-Rao product of all entries in U, a list of matrices, except the nth.
+        Efficiently calculates the matrix product of the n-mode matricization
+        of the `ktensor` with the Khatri-Rao product of all entries in U,
+        a :class:`list` of factor matrices, except the nth.
 
         Parameters
         ----------
-        U: list of factor matrices
-        n: multiplies by all modes except n
+        U: :class:`list` of factor matrices, required
+        n: int, required
+            Multiply by all modes except n.
 
         Returns
         -------
         :class:`numpy.ndarray`
 
         Examples
         --------
@@ -1106,75 +1198,95 @@
                 W = W * (self.factor_matrices[i].T @ U[i])
 
         # Find each column of answer by multiplying columns of X.u{n} with weights
         return self.factor_matrices[n] @ W
 
     @property
     def ncomponents(self):
-        """Number of components (i.e., number of columns in each factor matrix) of the `ktensor`.
+        """
+        Number of components in the :class:`pyttb.ktensor` (i.e., number of
+        columns in each factor matrix) of the :class:`pyttb.ktensor`.
 
         Returns
         -------
         :int
+
+        Examples
+        --------
+        >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
+        >>> print(K.ncomponents)
+        2
         """
         return len(self.weights)
 
     @property
     def ndims(self):
-        """Number of dimensions (i.e., number of factor_matrices) of the `ktensor`.
+        """
+        Number of dimensions (i.e., number of factor matrices) of the
+        :class:`pyttb.ktensor`.
 
         Returns
         -------
         :int
+
+        Examples
+        --------
+        >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
+        >>> print(K.ndims)
+        3
         """
         return len(self.factor_matrices)
 
     def norm(self):
         """
-        Compute the norm (i.e., square root of the sum of squares of entries) of a `ktensor`.
+        Compute the norm (i.e., square root of the sum of squares of entries)
+        of a :class:`pyttb.ktensor`.
 
         Returns
         --------
         :int
 
-        Example
-        -------
+        Examples
+        --------
         >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
         >>> K.norm()
         9.797958971132712
         """
         # Compute the matrix of correlation coefficients
         coefMatrix = self.weights[:, None] @ self.weights[None, :]
         for f in self.factor_matrices:
             coefMatrix = coefMatrix * (f.T @ f)
         return np.sqrt(np.abs(np.sum(coefMatrix)))
 
     def normalize(self, weight_factor=None, sort=False, normtype=2, mode=None):
         """
-        Normalize the columns of the factor matrices.
+        Normalize the columns of the factor matrices of a
+        :class:`pyttb.ktensor`.
 
         Parameters
         ----------
         weight_factor: {"all", int}, optional
-            Absorb the weights into one or more factors:
-               * "all": absorb weight equally across all factors
-               * int: absorb weight into a single dimension (int must be in range(self.ndims)
-        sort: bool
-            Sort the columns in descending order of the weights
-        normtype: {non-zero int, inf, -inf, 'fro', 'nuc'}, optional
-            Order of the norm (see :func:`numpy.linalg.norm` for possible values)
-        mode: {int, None}
-            Index of factor matrix to normalize. A value of `None` means normalize all factor matrices.
+            Absorb the weights into one or more factors. If "all", absorb
+            weight equally across all factors. If `int`, absorb weight into a
+            single dimension (value must be in range(self.ndims)).
+        sort: bool, optional
+            Sort the columns in descending order of the weights.
+        normtype: {non-negative int, -1, -2, np.inf, -np.inf}, optional
+            Order of the norm (see :func:`numpy.linalg.norm` for possible
+            values).
+        mode: {int, None}, optional
+            Index of factor matrix to normalize. A value of `None` means
+            normalize all factor matrices.
 
         Returns
-        --------
+        -------
         :class:`pyttb.ktensor`
 
-        Example
-        -------
+        Examples
+        --------
         >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
         >>> print(K.normalize())  # doctest: +ELLIPSIS
         ktensor of shape 2 x 3 x 4
         weights=[4.898... 4.898...]
         factor_matrices[0] =
         [[0.7071... 0.7071...]
          [0.7071... 0.7071...]]
@@ -1239,39 +1351,39 @@
                 p = np.argsort(self.weights)[::-1]
                 self = self.arrange(permutation=p)
 
         return self
 
     def nvecs(self, n, r, flipsign=True):
         """
-        Compute the leading mode-n vectors for a `ktensor`.
+        Compute the leading mode-n vectors for a :class:`pyttb.ktensor`.
 
-        Computes the `r` leading eigenvectors of Xn*Xn'
-        (where Xn is the mode-N matricization/unfolding of self), which provides
-        information about the mode-N fibers. In two-dimensions, the `r`
-        leading mode-1 vectors are the same as the 'r' left singular vectors
-        and the `r` leading mode-2 vectors are the same as the `r` right
-        singular vectors. By default, this method computes the top `r`
-        eigenvectors of the matrix Xn*Xn'.
+        Computes the `r` leading eigenvectors of Xn*Xn.T (where Xn is the
+        mode-`n` matricization/unfolding of self), which provides information
+        about the mode-N fibers. In two-dimensions, the `r` leading mode-1
+        vectors are the same as the `r` left singular vectors and the `r`
+        leading mode-2 vectors are the same as the `r` right singular
+        vectors. By default, this method computes the top `r` eigenvectors
+        of Xn*Xn.T.
 
         Parameters
         ----------
-        n: int
-            Mode for tensor matricization
-        r: int
-            Number of eigenvectors to compute and use
-        flipsign: bool
-            Make each column's largest element positive if `True`
+        n: int, required
+            Mode for tensor matricization.
+        r: int, required
+            Number of eigenvectors to compute and use.
+        flipsign: bool, optional
+            If True, make each column's largest element positive.
 
         Returns
         -------
-        :class:`Numpy.ndarray`
+        :class:`numpy.ndarray`
 
-        Example
-        -------
+        Examples
+        --------
         Compute single eigenvector for dimension 0:
 
         >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
         >>> nvecs1 = K.nvecs(0, 1)
         >>> print(nvecs1) # doctest: +ELLIPSIS
         [[0.70710678...]
          [0.70710678...]]
@@ -1291,15 +1403,15 @@
         y = self.factor_matrices[n] @ M @ self.factor_matrices[n].T
 
         if r < y.shape[0] - 1:
             w, v = scipy.sparse.linalg.eigsh(y, r)
             v = v[:, (-np.abs(w)).argsort()]
             v = v[:, :r]
         else:
-            warnings.warn(
+            logging.debug(
                 "Greater than or equal to ktensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
             )
             w, v = scipy.linalg.eigh(y)
             v = v[:, (-np.abs(w)).argsort()]
             v = v[:, :r]
 
         if flipsign:
@@ -1307,33 +1419,32 @@
             for i in range(v.shape[1]):
                 if v[idx[i], i] < 0:
                     v[:, i] *= -1
         return v
 
     def permute(self, order):
         """
-        Permute `ktensor` dimensions.
+        Permute :class:`pyttb.ktensor` dimensions.
 
-        Rearranges the dimensions of A so that they are in the order specified by the
-        vector `order`. The output is a `ktensor` with components rearranged as specified
-        by `order`. The corresponding tensor has the same components as `self` but the order
-        of the subscripts needed to access any particular element is rearranged as
-        specified by `order`.
+        Rearranges the dimensions of a :class:`pyttb.ktensor` so that they are
+        in the order specified by `order`. The corresponding tensor has the
+        same components as `self` but the order of the subscripts needed to
+        access any particular element is rearranged as specified by `order`.
 
         Parameters
         ----------
-        order: :class:`Numpy.ndarray`
+        order: :class:`numpy.ndarray`
+            Permutation of [0,...,self.ndimensions].
 
         Returns
         -------
         :class:`pyttb.ktensor`
-            shapeNew == shapePrevious[order]
 
-        Example
-        -------
+        Examples
+        --------
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> factor_matrices = [fm0, fm1]
         >>> K = ttb.ktensor.from_data(weights, factor_matrices)
         >>> print(K)
         ktensor of shape 2 x 2
@@ -1362,23 +1473,25 @@
         if tuple(range(self.ndims)) != tuple(sorted(order.tolist())):
             assert False, "Invalid permutation"
 
         return ktensor.from_data(self.weights, [self.factor_matrices[i] for i in order])
 
     def redistribute(self, mode):
         """
-        Distribute weights of a `ktensor` to a specified mode
+        Distribute weights of a :class:`pyttb.ktensor` to the specified mode.
+        The redistribution is performed in place.
 
         Parameters
         ----------
         mode: int
+            Must be value in [0,...self.ndims].
 
         Example
         -------
-        Create a `ktensor`:
+        Create a :class:`pyttb.ktensor`:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> factor_matrices = [fm0, fm1]
         >>> K = ttb.ktensor.from_data(weights, factor_matrices)
         >>> print(K)
@@ -1387,15 +1500,15 @@
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-        Distribute weights of that `ktensor` to mode 0:
+        Distribute weights of that :class:`pyttb.ktensor` to mode 0:
 
         >>> K.redistribute(0)
         >>> print(K)
         ktensor of shape 2 x 2
         weights=[1. 1.]
         factor_matrices[0] =
         [[1. 4.]
@@ -1408,84 +1521,89 @@
             self.factor_matrices[mode][:, [r]] = (
                 self.factor_matrices[mode][:, [r]] * self.weights[r]
             )
             self.weights[r] = 1
 
     @property
     def shape(self):
-        """Shape of a `ktensor`.
+        """Shape of a :class:`pyttb.ktensor`.
 
-        Returns the sizes of all dimensions.
+        Returns the lengths of all dimensions of the :class:`pyttb.ktensor`.
 
         Returns
         -------
         :class:`tuple`
         """
         return tuple([f.shape[0] for f in self.factor_matrices])
 
     def score(self, other, weight_penalty=True, threshold=0.99, greedy=True):
         """
-        Checks if two ktensor instances match except for permutation.
+        Checks if two :class:`pyttb.ktensor` instances with the same shapes
+        but potentially different number of components match except for
+        permutation.
+
+        Matching is defined as follows. If `self` and `other` are single-
+        component :class:`pyttb.ktensor` instances that have been normalized
+        so that their weights are `self.weights` and `other.weights`, and their
+        factor matrices are single column vectors containing [a1,a2,...,an] and
+        [b1,b2,...bn], rescpetively, then the score is defined as
 
-        We define matching as follows. If A (self) and B (other) are single component
-        ktensors that have been normalized so that their weights are weights_a and
-        weights_b, then the score is defined as
-
-            score = penalty * (a1.T*b1) * (a2.T*b2) * ... * (aR.T*bR),
+            score = penalty * (a1.T*b1) * (a2.T*b2) * ... * (an.T*bn),
 
         where the penalty is defined by the weights such that
 
-            penalty = 1 - abs(weights_a - weights_b) / max(weights_a, weights_b).
+            penalty = 1 - abs(self.weights - other.weights) / max(self.weights, other.weights).
 
-        The score of multi-component ktensors is a normalized sum of the
-        scores across the best permutation of the components of A. A can have
-        more components than B --- any extra components are ignored in terms of
-        the matching score.
+        The score of multi-component :class:`pyttb.ktensor` instances is a
+        normalized sum of the scores across the best permutation of the
+        components of `self`. `self` can have more components than `other`;
+        any extra components are ignored in terms of the matching score.
 
         Parameters
         ----------
-        other: :class:`pyttb.ktensor`
-            `ktensor` to match against
-        weight_penalty: bool
-            Flag indicating whether or not to consider the weights in the calculations.
-            Default: true
-        threshold: float
+        other: :class:`pyttb.ktensor`, required
+            :class:`pyttb.ktensor` with which to match.
+        weight_penalty: bool, optional
+            Flag indicating whether or not to consider the weights in the
+            calculations.
+        threshold: float, optional
             Threshold specified in the formula above for determining a match.
-            Default: 0.99
-        greedy: bool
+        greedy: bool, optional
             Flag indicating whether or not to consider all possible matchings
-            (exponentially expensive) or just do a greedy matching. Default: true
+            (exponentially expensive) or just do a greedy matching.
 
         Returns
         -------
         int
-            Score (between 0 and 1)
+            Score (between 0 and 1).
         :class:`pyttb.ktensor`
-            Copy of `self`, which has been normalized and permuted to best match `other`
+            Copy of `self`, which has been normalized and permuted to best match
+            `other`.
         bool
-            Flag indicating a match according to a user-specified threshold
-        :class:`Numpy.ndarray`
-            Permutation (i.e. array of indices of the modes of self) of the components
-            of self that was used to best match other
+            Flag indicating a match according to a user-specified threshold.
+        :class:`numpy.ndarray`
+            Permutation (i.e. array of indices of the modes of self) of the
+            components of `self` that was used to best match `other`.
 
-        Example
-        -------
-        Create two `ktensor` instances:
+        Examples
+        --------
+        Create two :class:`pyttb.ktensor` instances and compute the score
+        between them:
 
-        >>> A = ttb.ktensor.from_data(np.array([2., 1., 3.]), np.ones((3,3)), np.ones((4,3)), np.ones((5,3)))
-        >>> B = ttb.ktensor.from_data(np.array([2., 4.]), np.ones((3,2)), np.ones((4,2)), np.ones((5,2)))
-        >>> score,Aperm,flag,perm = A.score(B)  #  Compute `score` using `ktensor.weights`
+        >>> K = ttb.ktensor.from_data(np.array([2., 1., 3.]), np.ones((3,3)), np.ones((4,3)), np.ones((5,3)))
+        >>> K2 = ttb.ktensor.from_data(np.array([2., 4.]), np.ones((3,2)), np.ones((4,2)), np.ones((5,2)))
+        >>> score,Kperm,flag,perm = K.score(K2)
         >>> print(score)
         0.875
         >>> print(perm)
         [0 2 1]
 
-        Compute `score` not using `ktensor.weights`:
+        Compute score without using weights:
 
-        >>> score,Aperm,flag,perm = A.score(B,weight_penalty=False)
+        >>> score,Kperm,flag,perm = K.score(K2,weight_penalty=False)
         >>> print(score)
         1.0
         >>> print(perm)
         [0 1 2]
         """
 
         if not greedy:
@@ -1518,16 +1636,16 @@
         Cbig = ttb.tensor.from_function(np.zeros, (RA, RB, N))
         for n in range(N):
             Cbig[:, :, n] = np.abs(A.factor_matrices[n].T @ B.factor_matrices[n])
 
         # Collapse across all modes using the product
         C = Cbig.collapse(np.array([2]), np.prod).double()
 
-        # Calculate penalty based on differences in the Lambda's
-        # Note that we are assuming the the lambda value are positive because the
+        # Calculate penalty based on differences in the weights
+        # Note that we are assuming the the weights are positive because the
         # ktensor's were previously normalized.
         if weight_penalty:
             P = np.zeros((RA, RB))
             for ra in range(RA):
                 la = A.weights[ra]
                 for rb in range(RB):
                     lb = B.weights[rb]
@@ -1559,26 +1677,28 @@
             tf = np.in1d(foo, best_perm)
             best_perm[RB : RA + 1] = foo[~tf]
             A.arrange(permutation=best_perm)
             return best_score, A, flag, best_perm
 
     def symmetrize(self):
         """
-        Symmetrize a `ktensor` in all modes.
+        Symmetrize a :class:`pyttb.ktensor` in all modes.
 
-        Symmetrize a `ktensor` with respect to all modes so that the resulting `ktensor` is symmetric with respect
-        to any permutation of indices.
+        Symmetrize a :class:`pyttb.ktensor` with respect to all modes so that
+        the resulting :class:`pyttb.ktensor` is symmetric with respect to any
+        permutation of indices.
 
         Returns
         -------
         :class:`pyttb.ktensor`
-            A new `ktensor` whose factor matrices are symmetric
 
-        Example
-        -------
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor`:
+
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> factor_matrices = [fm0, fm1]
         >>> K = ttb.ktensor.from_data(weights, factor_matrices)
         >>> print(K)
         ktensor of shape 2 x 2
@@ -1586,15 +1706,16 @@
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-        Make the factor matrices of the `ktensor` symmetric:
+        Make the factor matrices of the :class:`pyttb.ktensor` symmetric with
+        respect to any permutation of the factor matrices:
 
         >>> K1 = K.symmetrize()
         >>> print(K1) # doctest: +ELLIPSIS
         ktensor of shape 2 x 2
         weights=[1. 1.]
         factor_matrices[0] =
         [[2.3404... 4.9519...]
@@ -1633,29 +1754,30 @@
                     weights[j] = -weights[j]
                     V[:, [j]] = -V[:, [j]]
 
         return self.from_data(weights, [V.copy() for i in range(K.ndims)])
 
     def tolist(self, mode=None):
         """
-        Converts `ktensor` to a list of factor matrices, evenly distributing the weights across factors.
+        Convert :class:`pyttb.ktensor` to a list of factor matrices, evenly
+        distributing the weights across factors. Optionally absorb the
+        weights into a single mode.
 
         Parameters
         ----------
-        mode: int
-            Index of factor matrix to absorb all of the weight.
+        mode: int, optional
+            Index of factor matrix to absorb all of the weights.
 
         Returns
         -------
-        :list of :class:`numpy.ndarray`
-            List of factor matrices
+        :class:`list` of :class:`numpy.ndarray`
 
-        Example
-        -------
-        Create a `ktensor` of all ones:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` of all ones:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
         >>> fm1 = np.array([[5., 6.], [7., 8.]])
         >>> factor_matrices = [fm0, fm1]
         >>> K = ttb.ktensor.from_data(weights, factor_matrices)
         >>> print(K)
@@ -1664,24 +1786,26 @@
         factor_matrices[0] =
         [[1. 2.]
          [3. 4.]]
         factor_matrices[1] =
         [[5. 6.]
          [7. 8.]]
 
-        Spread weights equally to all factors and return list of factor matrices:
+        Spread weights equally to all factors and return list of factor
+        matrices:
 
         >>> fm_list = K.tolist()
         >>> for fm in fm_list: print(fm) # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
         [[1. 2.8284...]
          [3. 5.6568...]]
         [[ 5. 8.4852...]
          [ 7. 11.313...]]
 
-        Shift weight to single factor matrix and return list of factor matrices:
+        Shift weight to single factor matrix and return list of factor
+        matrices:
 
         >>> fm_list = K.tolist(0)
         >>> for fm in fm_list: print(fm)  # doctest: +ELLIPSIS, +NORMALIZE_WHITESPACE
         [[ 8.6023... 40. ]
          [25.8069... 80. ]]
         [[0.5812... 0.6...]
          [0.8137... 0.8...]]
@@ -1703,38 +1827,41 @@
         factor_matrices[0] = factor_matrices[0] @ np.diag(lsgn)
         for n in range(self.ndims):
             factor_matrices[n] = factor_matrices[n] @ D
         return factor_matrices
 
     def tovec(self, include_weights=True):
         """
-        Convert `ktensor` to column vector.
+        Convert :class:`pyttb.ktensor` to column vector. Optionally include
+        or exclude the weights.
 
         Parameters
         ----------
-        include_weights: bool
-          Flag to specify whether or not to include weights in output (default is True).
+        include_weights: bool, optional
+            Flag to specify whether or not to include weights in output.
 
         Returns
         -------
         :class:`numpy.ndarray`
-          The length of the column vector is (sum(K.shape)+1)*K.ncomponents. The vector contains the ktensor
-          weights (if requested) stacked on top of each of the columns of the factor_matrices in order.
+            The length of the column vector is
+            (sum(self.shape)+1)*self.ncomponents. The vector contains the
+            weights (if requested) stacked on top of each of the columns of
+            the factor_matrices in order.
 
-        Example
-        -------
-        Create a `ktensor` from a vector:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` from a vector:
 
         >>> rank = 2
         >>> shape = np.array([2, 3, 4])
         >>> data = np.arange(1, rank*sum(shape)+1)
         >>> weights = 2 * np.ones(rank)
         >>> weights_and_data = np.concatenate((weights, data), axis=0)
-        >>> K_from_vector = ttb.ktensor.from_vector(weights_and_data[:], shape, True)
-        >>> print(K_from_vector)
+        >>> K = ttb.ktensor.from_vector(weights_and_data[:], shape, True)
+        >>> print(K)
         ktensor of shape 2 x 3 x 4
         weights=[2. 2.]
         factor_matrices[0] =
         [[1. 3.]
          [2. 4.]]
         factor_matrices[1] =
         [[ 5.  8.]
@@ -1742,18 +1869,19 @@
          [ 7. 10.]]
         factor_matrices[2] =
         [[11. 15.]
          [12. 16.]
          [13. 17.]
          [14. 18.]]
 
-        Create a ktensor from a vector of data extracted from another `ktensor`:
+        Create a :class:`pyttb.ktensor` from a vector of data extracted from
+        another :class:`pyttb.ktensor`:
 
-        >>> K_from_tovec = ttb.ktensor.from_vector(K_from_vector.tovec(), shape, True)
-        >>> print(K_from_tovec)
+        >>> K2 = ttb.ktensor.from_vector(K.tovec(), shape, True)
+        >>> print(K2)
         ktensor of shape 2 x 3 x 4
         weights=[2. 2.]
         factor_matrices[0] =
         [[1. 3.]
          [2. 4.]]
         factor_matrices[1] =
         [[ 5.  8.]
@@ -1774,62 +1902,60 @@
             offset = 0
 
         for f in self.factor_matrices:
             for r in range(self.ncomponents):
                 x[offset : offset + f.shape[0]] = f[:, r].reshape(f.shape[0])
                 offset += f.shape[0]
 
-        # if include_weights:
-        #     x = np.zeros((self.ncomponents * int(sum(self.shape)+1), 1))
-        #     x[0:self.ncomponents] = self.weights.reshape((len(self.weights), 1))
-        #     offset = self.ncomponents
-        # else:
-        #     x = np.zeros((self.ncomponents * int(sum(self.shape)), 1))
-        #     offset = 0
-        #
-        # for f in self.factor_matrices:
-        #     for r in range(self.ncomponents):
-        #         x[offset:offset+f.shape[0]] = f[:, r].reshape((f.shape[0], 1))
-        #         offset += f.shape[0]
         return x
 
     def ttv(self, vector, dims=None, exclude_dims=None):
         """
-        `Tensor` times vector for `ktensors`.
+        Tensor times vector for a :class:`pyttb.ktensor`.
 
-        Computes the product of a `ktensor` with a vector.  If `dims` is an integer, it specifies
-        the dimension in the `ktensor` along which the vector is multiplied.  If the shape of the vector
-        is = (I,1), then the size of dimension `dims` of the `ktensor` must have size I.  Note that
-        number of dimensions of the returned `tensor` is 1 less than the dimension of the `ktensor` used
-        in the multiplication because dimension `dims` is removed.
-
-        ttv(np.array([v1,v2,...,vN])) computes the product of the `ktensor` with a sequence of vectors in the
-        array.  The products are computed sequentially along all dimensions (or modes) of the `ktensor`. The array
-        contains N=self.ndims vectors.
-
-        ttv(np.array([v1,v2,...,vk]), dims=np.array([I1,I2,...,Ik) computes the sequence of `ktensor`-by-vector
-        products along the dimensions specified by `dims`. In this case, the number of products, k, can be less
-        than N=self.ndims and the order of the sequence does not need to match the order of the dimensions in the
-        `ktensor`. Note that the number of vectors must match the number of dimensions provides, and the length of
-        each vector must match the size of each dimension of the `ktensor` specified in `dims`.
+        Computes the product of a :class:`pyttb.ktensor` with a vector (i.e.,
+        np.array).  If `dims` is an integer, it specifies the dimension in the
+        :class:`pyttb.ktensor` along which the vector is multiplied.
+        If the shape of the vector is = (I,1), then the length of dimension
+        `dims` of the :class:`pyttb.ktensor` must be  I.  Note that the number
+        of dimensions of the returned :class:`pyttb.ktensor` is 1 less than
+        the dimension of the :class:`pyttb.ktensor` used in the
+        multiplication because dimension `dims` is removed.
+
+        If `vector` is a :class:`list` of np.array instances, the
+        :class:`pyttb.ktensor` is multiplied with each vector in the list. The
+        products are computed sequentially along all dimensions (or modes) of
+        the :class:`pyttb.ktensor`, and thus the list must contain `self.ndims`
+        vectors.
+
+        When `dims` is not None, compute the products along the dimensions
+        specified by `dims`. In this case, the number of products can be less
+        than `self.ndims` and the order of the sequence does not need to match
+        the order of the dimensions in the :class:`pyttb.ktensor`. Note that
+        the number of vectors must match the number of dimensions provided,
+        and the length of each vector must match the size of each dimension
+        of the :class:`pyttb.ktensor` specified in `dims`.
 
         Parameters
         ----------
-        vector: :class:`Numpy.ndarray`, list[:class:`Numpy.ndarray`]
-        dims: int, :class:`Numpy.ndarray`
+        vector: :class:`numpy.ndarray` or list[:class:`numpy.ndarray`], required
+        dims: int, :class:`numpy.ndarray`, optional
+        exclude_dims:
 
         Returns
         -------
         float or :class:`pyttb.ktensor`
-            The number of dimensions of the returned `ktensor` is N-k, where N=self.ndims and k = number of
-            vectors provided as input. If k == N, a scalar is returned
+            The number of dimensions of the returned :class:`pyttb.ktensor` is
+            n-k, where n = self.ndims and k = number of vectors provided as
+            input. If k == n, a scalar is returned.
 
-        Example
+        Examples
         -------
-        Compute the product of a `ktensor` and a single vector (results in a `ktensor`):
+        Compute the product of a :class:`pyttb.ktensor` and a single vector
+        (results in a :class:`pyttb.ktensor`):
 
         >>> rank = 2
         >>> shape = np.array([2, 3, 4])
         >>> data = np.arange(1, rank*sum(shape)+1)
         >>> weights = 2 * np.ones(rank)
         >>> weights_and_data = np.concatenate((weights, data), axis=0)
         >>> K = ttb.ktensor.from_vector(weights_and_data[:], shape, True)
@@ -1842,24 +1968,26 @@
          [2. 4.]]
         factor_matrices[1] =
         [[11. 15.]
          [12. 16.]
          [13. 17.]
          [14. 18.]]
 
-        Compute the product of a `ktensor` and a vector for each dimension (results in a `float`):
+        Compute the product of a :class:`pyttb.ktensor` and a vector for each
+        dimension (results in a `float`):
 
         >>> vec2 = np.array([1, 1])
         >>> vec3 = np.array([1, 1, 1])
         >>> vec4 = np.array([1, 1, 1, 1])
         >>> K1 = K.ttv([vec2, vec3, vec4])
         >>> print(K1)
         30348.0
 
-        Compute the product of a `ktensor` and multiple vectors out of order (results in a `ktensor`):
+        Compute the product of a :class:`pyttb.ktensor` and multiple vectors
+        out of order (results in a :class:`pyttb.ktensor`):
 
         >>> K2 = K.ttv([vec4, vec3],np.array([2, 1]))
         >>> print(K2)
         ktensor of shape 2
         weights=[1800. 3564.]
         factor_matrices[0] =
         [[1. 3.]
@@ -1903,39 +2031,42 @@
             factor_matrices = []
             for i in remdims:
                 factor_matrices.append(self.factor_matrices[i])
             return ktensor.from_data(new_weights, factor_matrices)
 
     def update(self, modes, data):
         """
-        Updates a `ktensor` in the specific dimensions, `modes`, with the values in `data`
-        (in vector or matrix form). The value of `mode` must be an integer between 1
-        and self.ndims. Further, the number of elements in `data` must equal self.shape[mode] * self.ncomponents.
+        Updates a :class:`pyttb.ktensor` in the specific dimensions with the
+        values in `data` (in vector or matrix form). The value of `modes` must
+        be a value in [-1,...,self.ndoms]. If the Further, the number of elements in
+        `data` must equal self.shape[modes] * self.ncomponents. The update is
+        performed in place.
 
         Parameters
         ----------
-        modes: list
-            List of dimensions to update; values must be in ascending order. Can include one or more of the following values:
-              * -1: update the weights
-              * `int`: value must be sorted and in `{range(self.ndims)}`
-        data: :class:numpy.ndarray
-            Vector of data values to use in the update
+        modes: int or :class:`list` of int, required
+            List of dimensions to update; values must be in ascending order. If
+            the first element of the list is -1, then update the weights. All
+            other integer values values must be sorted and in
+            [0,...,self.ndims].
+        data: :class:`numpy.ndarray`, required
+            Data values to use in the update.
 
         Results
         -------
         :class:`pyttb.ktensor`
-            The update is performed in place and a reference to self is returned
 
-        Example
-        -------
-        Create a `ktensor` of all ones:
+        Examples
+        --------
+        Create a :class:`pyttb.ktensor` of all ones:
 
         >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
 
-        Create vectors for updating various factor matrices of the `ktensor`:
+        Create vectors for updating various factor matrices of the
+        :class:`pyttb.ktensor`:
 
         >>> vec0 = 2 * np.ones(K.shape[0] * K.ncomponents)
         >>> vec1 = 3 * np.ones(K.shape[1] * K.ncomponents)
         >>> vec2 = 4 * np.ones(K.shape[2] * K.ncomponents)
 
         Update a single factor matrix:
 
@@ -1974,15 +2105,15 @@
          [3. 3.]]
         factor_matrices[2] =
         [[4. 4.]
          [4. 4.]
          [4. 4.]
          [4. 4.]]
 
-        Update some but not all factor matrices
+        Update some but not all factor matrices:
 
         >>> K3 = K.copy()
         >>> vec_some = np.concatenate((vec0, vec2))
         >>> K3 = K3.update([0, 2], vec_some)
         >>> print(K3)
         ktensor of shape 2 x 3 x 4
         weights=[1. 1.]
@@ -2030,19 +2161,20 @@
         if not (loc == len(data)):
             warnings.warn("Failed to consume all of the input data")
 
         return self
 
     def __add__(self, other):
         """
-        Binary addition for `ktensors`.
+        Binary addition for :class:`pyttb.ktensor`.
 
         Parameters
         ----------
-        other: :class:`pyttb.ktensor`
+        other: :class:`pyttb.ktensor`, required
+            :class:`pyttb.ktensor` to add to `self`.
 
         Returns
         -------
         :class:`pyttb.ktensor`
         """
         # TODO include test of other as sumtensor and call sumtensor.__add__
         if not isinstance(other, ktensor):
@@ -2059,44 +2191,45 @@
                     (self.factor_matrices[k], other.factor_matrices[k]), axis=1
                 )
             )
         return ktensor.from_data(weights, factor_matrices)
 
     def __getitem__(self, item):
         """
-        Subscripted reference for a `ktensor`.
+        Subscripted reference for a :class:`pyttb.ktensor`.
 
-        Subscripted reference is used to query the components of a `ktensor`.
+        Subscripted reference is used to query the components of a
+        :class:`pyttb.ktensor`.
 
         Parameters
         ----------
-        item: {tuple(int), int}
+        item: tuple(int) or int, required
 
-        Example
-        -------
+        Examples
+        --------
         >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
-        >>> K.weights #<--returns the weights array (np.array([1., 1.]))
+        >>> K.weights
         array([1., 1.])
-        >>> K.factor_matrices #<--returns a list of 3 np.ndarrays
+        >>> K.factor_matrices
         [array([[1., 1.],
                [1., 1.]]), array([[1., 1.],
                [1., 1.],
                [1., 1.]]), array([[1., 1.],
                [1., 1.],
                [1., 1.],
                [1., 1.]])]
-        >>> K.factor_matrices[0] #<--returns the factor matrix corresponding to the first mode
+        >>> K.factor_matrices[0]
         array([[1., 1.],
                [1., 1.]])
-        >>> K[0] #<-returns the factor matrix corresponding to the first mode
+        >>> K[0]
         array([[1., 1.],
                [1., 1.]])
-        >>> K[1, 2, 0] #<--calculates and returns a specific single element of K
+        >>> K[1, 2, 0]
         2.0
-        >>> K[0][:, [0]] # returns the first column of the factor matrix corresponding to the first mode
+        >>> K[0][:, [0]]
         array([[1.],
                [1.]])
         """
         if isinstance(item, tuple):
             if len(item) == self.ndims:
                 # Extract single element
                 a = 0
@@ -2118,63 +2251,72 @@
         else:
             assert (
                 False
             ), "ktensor.__getitem__() can only extract single elements (tuple of indices) or factor matrices (single index)"
 
     def __neg__(self):
         """
-        Unary minus (negative) for ktensors.
-
-        Parameters
-        ----------
-        other: :class:`pyttb.ktensor`
+        Unary minus (negative) for :class:`pyttb.ktensor` instances.
 
         Returns
         -------
         :class:`pyttb.ktensor`
         """
         return ktensor.from_data(-self.weights, self.factor_matrices)
 
     def __pos__(self):
         """
-        Unary minus (positive) for `ktensors`.
-
-        Parameters
-        ----------
-        other: :class:`pyttb.ktensor`
+        Unary plus (positive) for :class:`pyttb.ktensor` instances.
 
         Returns
         -------
         :class:`pyttb.ktensor`
         """
         return ktensor.from_tensor_type(self)
 
     def __setitem__(self, key, value):
         """
-        Subscripted assignment for `ktensors`.
+        Subscripted assignment for :class:`pyttb.ktensor`.
 
-        Subscripted assignment cannot be used to update individual elements of a `ktensor`. However, you
-        can update the weights vector or the factor matrices of a `ktensor`. The entire factor matrix or weight
+        Subscripted assignment cannot be used to update individual elements of
+        a :class:`pyttb.ktensor`. You can update the weights vector or the
+        factor matrices of a :class:`pyttb.ktensor`.
 
         Example
         -------
-        >>> K = ktensor.from_data(np.ones((4,1)), [np.random.random((2,4)), np.random.random((3,4)), np.random.random((4,4))])
+        >>> K = ttb.ktensor.from_data(np.ones((4,1)), [np.random.random((2,4)), np.random.random((3,4)), np.random.random((4,4))])
         >>> K.weights = 2 * np.ones((4,1))
         >>> K.factor_matrices[0] = np.zeros((2, 4))
         >>> K.factor_matrices = [np.zeros((2, 4)), np.zeros((3, 4)), np.zeros((4, 4))]
+        >>> print(K)
+        ktensor of shape 2 x 3 x 4
+        weights=[[2.]
+         [2.]
+         [2.]
+         [2.]]
+        factor_matrices[0] =
+        [[0. 0. 0. 0.]
+         [0. 0. 0. 0.]]
+        factor_matrices[1] =
+        [[0. 0. 0. 0.]
+         [0. 0. 0. 0.]
+         [0. 0. 0. 0.]]
+        factor_matrices[2] =
+        [[0. 0. 0. 0.]
+         [0. 0. 0. 0.]
+         [0. 0. 0. 0.]
+         [0. 0. 0. 0.]]
         """
         assert (
             False
-        ), "Subscripted assignment cannot be used to update individual elements of a ktensor. However, \
-        you can update the weights vector or the factor matrices of a ktensor. The entire factor matrix or weight \
-        vector must be provided."
+        ), "Subscripted assignment cannot be used to update individual elements of a ktensor. However, you can update the weights vector or the factor matrices of a ktensor. The entire factor matrix or weight vector must be provided."
 
     def __sub__(self, other):
         """
-        Binary subtraction for ktensors.
+        Binary subtraction for :class:`pyttb.ktensor`.
 
         Parameters
         ----------
         other: :class:`pyttb.ktensor`
 
         Returns
         -------
@@ -2194,15 +2336,16 @@
                     (self.factor_matrices[k], other.factor_matrices[k]), axis=1
                 )
             )
         return ktensor.from_data(weights, factor_matrices)
 
     def __mul__(self, other):
         """
-        Elementwise (including scalar) multiplication for ktensors.
+        Elementwise (including scalar) multiplication for
+        :class:`pyttb.ktensor` instances.
 
         Parameters
         ----------
         other: :class:`pyttb.tensor`, :class:`pyttb.sptensor`, float, int
 
         Returns
         -------
@@ -2216,34 +2359,34 @@
 
         assert (
             False
         ), "Multiplication by ktensors only allowed for scalars, tensors, or sptensors"
 
     def __rmul__(self, other):
         """
-        Elementwise (including scalar) multiplication for ktensors.
+        Elementwise (including scalar) multiplication for
+        :class:`pyttb.ktensor` instances.
 
         Parameters
         ----------
         other: :class:`pyttb.tensor`, :class:`pyttb.sptensor`, float, int
 
         Returns
         -------
         :class:`pyttb.ktensor`
         """
         return self.__mul__(other)
 
     def __repr__(self):
         """
-        String representation of a ktensor.
+        String representation of a :class:`pyttb.ktensor`.
 
         Returns
         -------
         str:
-          Contains the shape, weights and factor_matrices as strings on different lines.
         """
         s = ""
         s += "ktensor of shape "
         s += (" x ").join([str(int(d)) for d in self.shape])
         s += "\n"
         s += "weights="
         s += str(self.weights)
```

### Comparing `pyttb-1.6.0/pyttb/pyttb_utils.py` & `pyttb-1.6.1/pyttb/pyttb_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -696,15 +696,15 @@
     """
     if subs.size == 0:
         ok = True
     elif (
         len(subs.shape) == 2
         and (np.isfinite(subs)).all()
         and issubclass(subs.dtype.type, np.integer)
-        and (subs > 0).all()
+        and (subs >= 0).all()
     ):
         ok = True
     else:
         ok = False
 
     if not ok and not nargout:
         assert False, "Subscripts must be a matrix of real positive integers"
```

### Comparing `pyttb-1.6.0/pyttb/sptensor.py` & `pyttb-1.6.1/pyttb/sptensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 """Sparse Tensor Implementation"""
 from __future__ import annotations
 
+import logging
 import warnings
 from collections.abc import Sequence
 from typing import Any, Callable, List, Optional, Tuple, Union, cast, overload
 
 import numpy as np
 import scipy.sparse.linalg
 from numpy_groupies import aggregate as accumarray
@@ -191,15 +192,15 @@
         # TODO what is an MDA?
 
         assert False, "Invalid Tensor Type To initialize Sptensor"
 
     @classmethod
     def from_function(
         cls,
-        function_handle: Callable[[Tuple[float, float]], np.ndarray],
+        function_handle: Callable[[Tuple[int, ...]], np.ndarray],
         shape: Tuple[int, ...],
         nonzeros: float,
     ) -> sptensor:
         """
         Creates a sparse tensor of the specified shape with NZ nonzeros created from
         the specified function handle
 
@@ -293,15 +294,15 @@
 
         # Check for wrong input
         if subs.size > 0 and subs.shape[1] > len(shape):
             assert False, "More subscripts than specified by shape"
 
         # Check for subscripts out of range
         for j, dim in enumerate(shape):
-            if subs.size > 0 and np.max(subs[:, j]) > dim:
+            if subs.size > 0 and np.max(subs[:, j]) >= dim:
                 assert False, "Subscript exceeds sptensor shape"
 
         if subs.size == 0:
             newsubs = np.array([])
             newvals = np.array([])
         else:
             # Identify only the unique indices
@@ -930,15 +931,15 @@
                 "Cannot call nvecs on sptensor with only singleton dimensions"
             )
         tnt = mutatable_sptensor.spmatrix().transpose()
         y = tnt.transpose().dot(tnt)
         if r < y.shape[0] - 1:
             _, v = scipy.sparse.linalg.eigs(y, r)
         else:
-            warnings.warn(
+            logging.debug(
                 "Greater than or equal to sptensor.shape[n] - 1 eigenvectors requires"
                 " cast to dense to solve"
             )
             w, v = scipy.linalg.eig(y.toarray())
             v = v[(-np.abs(w)).argsort()]
             v = v[:, :r]
 
@@ -1044,24 +1045,24 @@
         """
         if isinstance(dims, (float, int)):
             dims = np.array([dims])
         dims, _ = ttb.tt_dimscheck(self.ndims, dims=dims)
 
         if isinstance(factor, ttb.tensor):
             shapeArray = np.array(self.shape)
-            if np.any(factor.shape != shapeArray[dims]):
+            if not np.array_equal(factor.shape, shapeArray[dims]):
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
                 self.subs,
                 self.vals * factor[self.subs[:, dims], "extract"][:, None],
                 self.shape,
             )
         if isinstance(factor, ttb.sptensor):
             shapeArray = np.array(self.shape)
-            if np.any(factor.shape != shapeArray[dims]):
+            if not np.array_equal(factor.shape, shapeArray[dims]):
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
                 self.subs, self.vals * factor.extract(self.subs[:, dims]), self.shape
             )
         if isinstance(factor, np.ndarray):
             shapeArray = np.array(self.shape)
             if factor.shape[0] != shapeArray[dims]:
@@ -2578,7 +2579,92 @@
         Ynt = tt_from_sparse_matrix(Z, siz, final_dim, idx)
 
         if not isinstance(Z, np.ndarray) and Z.nnz <= 0.5 * np.prod(siz):
             return Ynt
         # TODO evaluate performance loss by casting into sptensor then tensor.
         #  I assume minimal since we are already using spare matrix representation
         return ttb.tensor.from_tensor_type(Ynt)
+
+
+def sptenrand(
+    shape: Tuple[int, ...],
+    density: Optional[float] = None,
+    nonzeros: Optional[float] = None,
+) -> sptensor:
+    """
+    Create sptensor with entries drawn from a uniform distribution on the unit interval
+
+    Parameters
+    ----------
+    shape: Shape of resulting tensor
+    density: Density of resulting sparse tensor
+    nonzeros: Number of nonzero entries in resulting sparse tensor
+
+    Returns
+    -------
+    Constructed tensor
+
+    Example
+    -------
+    >>> X = ttb.sptenrand((2,2), nonzeros=1)
+    >>> Y = ttb.sptenrand((2,2), density=0.25)
+    """
+    if density is None and nonzeros is None:
+        raise ValueError("Must set either density or nonzeros")
+
+    if density is not None and nonzeros is not None:
+        raise ValueError("Must set either density or nonzeros but not both")
+
+    if density is not None and not 0 < density <= 1:
+        raise ValueError(f"Density must be a fraction (0, 1] but received {density}")
+
+    if isinstance(density, float):
+        valid_nonzeros = float(np.prod(shape) * density)
+    elif isinstance(nonzeros, (int, float)):
+        valid_nonzeros = nonzeros
+    else:  # pragma: no cover
+        raise ValueError(
+            f"Incorrect types for density:{density} and nonzeros:{nonzeros}"
+        )
+
+    # Typing doesn't play nice with partial
+    # mypy issue: 1484
+    def unit_uniform(pass_through_shape: Tuple[int, ...]) -> np.ndarray:
+        return np.random.uniform(low=0, high=1, size=pass_through_shape)
+
+    return ttb.sptensor.from_function(unit_uniform, shape, valid_nonzeros)
+
+
+def sptendiag(
+    elements: np.ndarray, shape: Optional[Tuple[int, ...]] = None
+) -> sptensor:
+    """
+    Creates a sparse tensor with elements along super diagonal
+    If provided shape is too small the tensor will be enlarged to accomodate
+
+    Parameters
+    ----------
+    elements: Elements to set along the diagonal
+    shape: Shape of resulting tensor
+
+    Returns
+    -------
+    Constructed tensor
+
+    Example
+    -------
+    >>> shape = (2,)
+    >>> values = np.ones(shape)
+    >>> X = ttb.sptendiag(values)
+    >>> Y = ttb.sptendiag(values, (2, 2))
+    >>> X.isequal(Y)
+    True
+    """
+    # Flatten provided elements
+    elements = np.ravel(elements)
+    N = len(elements)
+    if shape is None:
+        constructed_shape = (N,) * N
+    else:
+        constructed_shape = tuple(max(N, dim) for dim in shape)
+    subs = np.tile(np.arange(0, N).transpose(), (len(constructed_shape), 1)).transpose()
+    return sptensor.from_aggregator(subs, elements.reshape((N, 1)), constructed_shape)
```

### Comparing `pyttb-1.6.0/pyttb/sumtensor.py` & `pyttb-1.6.1/pyttb/sumtensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/tenmat.py` & `pyttb-1.6.1/pyttb/tenmat.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb/tensor.py` & `pyttb-1.6.1/pyttb/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 """Dense Tensor Implementation"""
 from __future__ import annotations
 
-import warnings
+import logging
 from itertools import permutations
 from math import factorial
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy.sparse.linalg
 from numpy_groupies import aggregate as accumarray
@@ -786,15 +786,15 @@
         y = Xn @ Xn.T
 
         if r < y.shape[0] - 1:
             w, v = scipy.sparse.linalg.eigsh(y, r)
             v = v[:, (-np.abs(w)).argsort()]
             v = v[:, :r]
         else:
-            warnings.warn(
+            logging.debug(
                 "Greater than or equal to tensor.shape[n] - 1 eigenvectors"
                 " requires cast to dense to solve"
             )
             w, v = scipy.linalg.eigh(y)
             v = v[:, (-np.abs(w)).argsort()]
             v = v[:, :r]
 
@@ -1831,11 +1831,110 @@
                 s += "\n"
         # s += '\n'
         return s
 
     __str__ = __repr__
 
 
+def tenones(shape: Tuple[int, ...]) -> tensor:
+    """
+    Creates a tensor of all ones
+
+    Parameters
+    ----------
+    shape: Shape of resulting tensor
+
+    Returns
+    -------
+    Constructed tensor
+
+    Example
+    -------
+    >>> X = ttb.tenones((2,2))
+    """
+    return tensor.from_function(np.ones, shape)
+
+
+def tenzeros(shape: Tuple[int, ...]) -> tensor:
+    """
+    Creates a tensor of all zeros
+
+    Parameters
+    ----------
+    shape: Shape of resulting tensor
+
+    Returns
+    -------
+    Constructed tensor
+
+    Example
+    -------
+    >>> X = ttb.tenzeros((2,2))
+    """
+    return tensor.from_function(np.zeros, shape)
+
+
+def tenrand(shape: Tuple[int, ...]) -> tensor:
+    """
+    Creates a tensor with entries drawn from a uniform distribution on the unit interval
+
+    Parameters
+    ----------
+    shape: Shape of resulting tensor
+
+    Returns
+    -------
+    Constructed tensor
+
+    Example
+    -------
+    >>> X = ttb.tenrand((2,2))
+    """
+
+    # Typing doesn't play nice with partial
+    # mypy issue: 1484
+    def unit_uniform(pass_through_shape: Tuple[int, ...]) -> np.ndarray:
+        return np.random.uniform(low=0, high=1, size=pass_through_shape)
+
+    return tensor.from_function(unit_uniform, shape)
+
+
+def tendiag(elements: np.ndarray, shape: Optional[Tuple[int, ...]] = None) -> tensor:
+    """
+    Creates a tensor with elements along super diagonal
+    If provided shape is too small the tensor will be enlarged to accomodate
+
+    Parameters
+    ----------
+    elements: Elements to set along the diagonal
+    shape: Shape of resulting tensor
+
+    Returns
+    -------
+    Constructed tensor
+
+    Example
+    -------
+    >>> shape = (2,)
+    >>> values = np.ones(shape)
+    >>> X = ttb.tendiag(values)
+    >>> Y = ttb.tendiag(values, (2, 2))
+    >>> X.isequal(Y)
+    True
+    """
+    # Flatten provided elements
+    elements = np.ravel(elements)
+    N = len(elements)
+    if shape is None:
+        constructed_shape = (N,) * N
+    else:
+        constructed_shape = tuple(max(N, dim) for dim in shape)
+    X = tenzeros(constructed_shape)
+    subs = np.tile(np.arange(0, N).transpose(), (len(constructed_shape), 1))
+    X[subs] = elements
+    return X
+
+
 if __name__ == "__main__":
     import doctest  # pragma: no cover
 
     doctest.testmod()  # pragma: no cover
```

### Comparing `pyttb-1.6.0/pyttb/ttensor.py` & `pyttb-1.6.1/pyttb/ttensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 
+import logging
 import textwrap
-import warnings
 
 import numpy as np
 import scipy
 
 from pyttb import ktensor
 from pyttb import pyttb_utils as ttb_utils
 from pyttb import sptenmat, sptensor, tenmat, tensor
@@ -570,15 +570,15 @@
 
         # TODO: Lifted from tensor, consider common location
         if r < Y.shape[0] - 1:
             w, v = scipy.sparse.linalg.eigsh(Y, r)
             v = v[:, (-np.abs(w)).argsort()]
             v = v[:, :r]
         else:
-            warnings.warn(
+            logging.debug(
                 "Greater than or equal to tensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
             )
             w, v = scipy.linalg.eigh(Y)
             v = v[:, (-np.abs(w)).argsort()]
             v = v[:, :r]
 
         if flipsign:
```

### Comparing `pyttb-1.6.0/pyttb/tucker_als.py` & `pyttb-1.6.1/pyttb/tucker_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/pyttb.egg-info/PKG-INFO` & `pyttb-1.6.1/pyttb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python Tensor Toolbox
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyttb-1.6.0/pyttb.egg-info/SOURCES.txt` & `pyttb-1.6.1/pyttb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_cp_als.py` & `pyttb-1.6.1/tests/test_cp_als.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,20 +34,15 @@
     capsys.readouterr()
     assert pytest.approx(output["fit"], 1) == 0
 
 
 @pytest.mark.indevelopment
 def test_cp_als_tensor_nvecs_init(capsys, sample_tensor):
     (data, T) = sample_tensor
-    with pytest.warns(Warning) as record:
-        (M, Minit, output) = ttb.cp_als(T, 1, init="nvecs")
-    assert (
-        "Greater than or equal to tensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
-    )
+    (M, Minit, output) = ttb.cp_als(T, 1, init="nvecs")
     capsys.readouterr()
     assert pytest.approx(output["fit"], 1) == 0
 
 
 @pytest.mark.indevelopment
 def test_cp_als_tensor_ktensor_init(capsys, sample_tensor):
     (data, T) = sample_tensor
@@ -83,20 +78,15 @@
     capsys.readouterr()
     assert pytest.approx(output["fit"], 1) == 0
 
 
 @pytest.mark.indevelopment
 def test_cp_als_sptensor_nvecs_init(capsys, sample_sptensor):
     (data, T) = sample_sptensor
-    with pytest.warns(Warning) as record:
-        (M, Minit, output) = ttb.cp_als(T, 1, init="nvecs")
-    assert (
-        "Greater than or equal to sptensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
-    )
+    (M, Minit, output) = ttb.cp_als(T, 1, init="nvecs")
     capsys.readouterr()
     assert pytest.approx(output["fit"], 1) == 0
 
 
 @pytest.mark.indevelopment
 def test_cp_als_sptensor_ktensor_init(capsys, sample_sptensor):
     (data, T) = sample_sptensor
```

### Comparing `pyttb-1.6.0/tests/test_cp_apr.py` & `pyttb-1.6.1/tests/test_cp_apr.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_hosvd.py` & `pyttb-1.6.1/tests/test_hosvd.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_import_export_data.py` & `pyttb-1.6.1/tests/test_import_export_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_khatrirao.py` & `pyttb-1.6.1/tests/test_khatrirao.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_ktensor.py` & `pyttb-1.6.1/tests/test_ktensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -706,55 +706,40 @@
     assert np.allclose(K5.factor_matrices[1], fm1)
 
 
 @pytest.mark.indevelopment
 def test_ktensor_nvecs(sample_ktensor_3way):
     (data, K) = sample_ktensor_3way
 
-    with pytest.warns(Warning) as record:
-        assert np.allclose(
-            K.nvecs(0, 1), np.array([[0.5731077440321353], [0.8194800264377384]])
-        )
-    assert (
-        "Greater than or equal to ktensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
-    )
-    with pytest.warns(Warning) as record:
-        assert np.allclose(
-            K.nvecs(0, 2),
-            np.array(
-                [
-                    [0.5731077440321353, 0.8194800264377384],
-                    [0.8194800264377384, -0.5731077440321353],
-                ]
-            ),
-        )
-    assert (
-        "Greater than or equal to ktensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
+    assert np.allclose(
+        K.nvecs(0, 1), np.array([[0.5731077440321353], [0.8194800264377384]])
+    )
+    assert np.allclose(
+        K.nvecs(0, 2),
+        np.array(
+            [
+                [0.5731077440321353, 0.8194800264377384],
+                [0.8194800264377384, -0.5731077440321353],
+            ]
+        ),
     )
 
     assert np.allclose(
         K.nvecs(1, 1),
         np.array([[0.5048631426517823], [0.5745404391632514], [0.6442177356747206]]),
     )
-    with pytest.warns(Warning) as record:
-        assert np.allclose(
-            K.nvecs(1, 2),
-            np.array(
-                [
-                    [0.5048631426517821, 0.7605567306550753],
-                    [0.5745404391632517, 0.0568912743440822],
-                    [0.6442177356747206, -0.6467741818894517],
-                ]
-            ),
-        )
-    assert (
-        "Greater than or equal to ktensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
+    assert np.allclose(
+        K.nvecs(1, 2),
+        np.array(
+            [
+                [0.5048631426517821, 0.7605567306550753],
+                [0.5745404391632517, 0.0568912743440822],
+                [0.6442177356747206, -0.6467741818894517],
+            ]
+        ),
     )
 
     assert np.allclose(
         K.nvecs(2, 1),
         np.array(
             [
                 [0.4507198734531968],
@@ -773,20 +758,15 @@
                 [0.5147179546368857, -0.1872576491687805],
                 [0.5467169952287302, -0.6333249775151949],
             ]
         ),
     )
 
     # Test for r >= N-1, requires cast to dense
-    with pytest.warns(Warning) as record:
-        K.nvecs(1, 3)
-    assert (
-        "Greater than or equal to ktensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
-    )
+    K.nvecs(1, 3)
 
 
 @pytest.mark.indevelopment
 def test_ktensor_permute(sample_ktensor_3way):
     (data, K) = sample_ktensor_3way
     order = np.array([2, 0, 1])
     fm = [data["factor_matrices"][i] for i in order]
```

### Comparing `pyttb-1.6.0/tests/test_package.py` & `pyttb-1.6.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_pyttb_utils.py` & `pyttb-1.6.1/tests/test_pyttb_utils.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_sptensor.py` & `pyttb-1.6.1/tests/test_sptensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1621,24 +1621,19 @@
     assert np.allclose((sptensorInstance.nvecs(1, 1)), np.array([0, 0, 0, 1])[:, None])
     assert np.allclose(
         (sptensorInstance.nvecs(1, 2)),
         np.array([[0, 0, 0, 1], [0, 0, 1, 0]]).transpose(),
     )
 
     # Test for r >= N-1, requires cast to dense
-    with pytest.warns(Warning) as record:
-        ans = np.zeros((4, 3))
-        ans[3, 0] = 1
-        ans[2, 1] = 1
-        ans[1, 2] = 1
-        assert np.allclose((sptensorInstance.nvecs(1, 3)), ans)
-    assert (
-        "Greater than or equal to sptensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
-    )
+    ans = np.zeros((4, 3))
+    ans[3, 0] = 1
+    ans[2, 1] = 1
+    ans[1, 2] = 1
+    assert np.allclose((sptensorInstance.nvecs(1, 3)), ans)
 
     # Negative test, check for only singleton dims
     with pytest.raises(ValueError):
         single_val_sptensor = ttb.sptensor.from_data(
             np.array([[0, 0]]), np.array([1]), shape=(1, 1)
         )
         single_val_sptensor.nvecs(0, 0)
@@ -1754,7 +1749,78 @@
         assert sptensorCopy.isequal(Ynt)
 
     for mode in range(sptensorInstance.ndims):
         sptensorCopy = ttb.sptensor.from_tensor_type(sptensorInstance)
         Xnt = tt_to_sparse_matrix(sptensorCopy, mode, False)
         Ynt = tt_from_sparse_matrix(Xnt, sptensorCopy.shape, mode, 1)
         assert sptensorCopy.isequal(Ynt)
+
+
+def test_sptendiag():
+    N = 4
+    elements = np.arange(0, N)
+    exact_shape = [N] * N
+
+    # Inferred shape
+    X = ttb.sptendiag(elements)
+    for i in range(N):
+        diag_index = (i,) * N
+        assert (
+            X[diag_index] == i
+        ), f"Idx: {diag_index} expected: {i} got: {X[diag_index]}"
+
+    # Exact shape
+    X = ttb.sptendiag(elements, tuple(exact_shape))
+    for i in range(N):
+        diag_index = (i,) * N
+        assert X[diag_index] == i
+
+    # Larger shape
+    larger_shape = exact_shape.copy()
+    larger_shape[0] += 1
+    X = ttb.sptendiag(elements, tuple(larger_shape))
+    for i in range(N):
+        diag_index = (i,) * N
+        assert X[diag_index] == i
+
+    # Smaller Shape
+    smaller_shape = exact_shape.copy()
+    smaller_shape[0] -= 1
+    X = ttb.sptendiag(elements, tuple(smaller_shape))
+    for i in range(N):
+        diag_index = (i,) * N
+        assert X[diag_index] == i
+
+
+def test_sptenrand():
+    arbitrary_shape = (3, 3, 3)
+    rand_tensor = ttb.sptenrand(arbitrary_shape, nonzeros=1)
+    in_unit_interval = np.all(0 <= rand_tensor.vals <= 1)
+    assert (
+        in_unit_interval
+        and rand_tensor.shape == arbitrary_shape
+        and rand_tensor.nnz == 1
+    )
+
+    rand_tensor = ttb.sptenrand(arbitrary_shape, density=1 / np.prod(arbitrary_shape))
+    in_unit_interval = np.all(0 <= rand_tensor.vals <= 1)
+    assert (
+        in_unit_interval
+        and rand_tensor.shape == arbitrary_shape
+        and rand_tensor.nnz == 1
+    )
+
+    # Negative tests
+    # Bad density
+    with pytest.raises(ValueError):
+        ttb.sptenrand(arbitrary_shape, density=-1)
+        ttb.sptenrand(arbitrary_shape, density=2)
+
+    # Missing args
+    # Bad density
+    with pytest.raises(ValueError):
+        ttb.sptenrand(arbitrary_shape)
+
+    # Redundant/contradicting args
+    # Bad density
+    with pytest.raises(ValueError):
+        ttb.sptenrand(arbitrary_shape, density=0.5, nonzeros=2)
```

### Comparing `pyttb-1.6.0/tests/test_tenmat.py` & `pyttb-1.6.1/tests/test_tenmat.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.0/tests/test_tensor.py` & `pyttb-1.6.1/tests/test_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1622,13 +1622,65 @@
         ]
     ).T
 
     # Test for one eigenvector
     assert np.allclose((tensorInstance.nvecs(1, 1)), nv1)
 
     # Test for r >= N-1, requires cast to dense
-    with pytest.warns(Warning) as record:
-        assert np.allclose((tensorInstance.nvecs(1, 2)), nv2)
-    assert (
-        "Greater than or equal to tensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
+    assert np.allclose((tensorInstance.nvecs(1, 2)), nv2)
+
+
+def test_tenones():
+    arbitrary_shape = (3, 3, 3)
+    ones_tensor = ttb.tenones(arbitrary_shape)
+    data_tensor = ttb.tensor.from_data(np.ones(arbitrary_shape))
+    assert np.equal(ones_tensor, data_tensor), "Tenones should match all ones tensor"
+
+
+def test_tenzeros():
+    arbitrary_shape = (3, 3, 3)
+    zeros_tensor = ttb.tenzeros(arbitrary_shape)
+    data_tensor = ttb.tensor.from_data(np.zeros(arbitrary_shape))
+    assert np.equal(zeros_tensor, data_tensor), "Tenzeros should match all zeros tensor"
+
+
+def test_tenrand():
+    arbitrary_shape = (3, 3, 3)
+    rand_tensor = ttb.tenrand(arbitrary_shape)
+    in_unit_interval = np.all((rand_tensor >= 0).data) and np.all(
+        (rand_tensor <= 1).data
     )
+    assert in_unit_interval and rand_tensor.shape == arbitrary_shape
+
+
+def test_tendiag():
+    N = 4
+    elements = np.arange(0, N)
+    exact_shape = [N] * N
+
+    # Inferred shape
+    X = ttb.tendiag(elements)
+    for i in range(N):
+        diag_index = (i,) * N
+        assert X[diag_index] == i
+
+    # Exact shape
+    X = ttb.tendiag(elements, tuple(exact_shape))
+    for i in range(N):
+        diag_index = (i,) * N
+        assert X[diag_index] == i
+
+    # Larger shape
+    larger_shape = exact_shape.copy()
+    larger_shape[0] += 1
+    X = ttb.tendiag(elements, tuple(larger_shape))
+    for i in range(N):
+        diag_index = (i,) * N
+        assert X[diag_index] == i
+
+    # Smaller Shape
+    smaller_shape = exact_shape.copy()
+    smaller_shape[0] -= 1
+    X = ttb.tendiag(elements, tuple(smaller_shape))
+    for i in range(N):
+        diag_index = (i,) * N
+        assert X[diag_index] == i
```

### Comparing `pyttb-1.6.0/tests/test_ttensor.py` & `pyttb-1.6.1/tests/test_ttensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,20 +363,15 @@
     full_eigvals = ttensorInstance.full().nvecs(n, r)
     assert np.allclose(ttensor_eigvals, full_eigvals)
 
     # Test for eig vals larger than shape-1
     n = 1
     r = 2
     full_eigvals = ttensorInstance.full().nvecs(n, r)
-    with pytest.warns(Warning) as record:
-        ttensor_eigvals = ttensorInstance.nvecs(n, r)
-    assert (
-        "Greater than or equal to tensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
-        in str(record[0].message)
-    )
+    ttensor_eigvals = ttensorInstance.nvecs(n, r)
     assert np.allclose(ttensor_eigvals, full_eigvals)
 
     # Negative Tests
     sparse_core = ttb.sptensor()
     sparse_core.shape = ttensorInstance.core.shape
     ttensorInstance.core = sparse_core
```

### Comparing `pyttb-1.6.0/tests/test_tucker_als.py` & `pyttb-1.6.1/tests/test_tucker_als.py`

 * *Files identical despite different names*

