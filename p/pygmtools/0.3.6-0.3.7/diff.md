# Comparing `tmp/pygmtools-0.3.6.tar.gz` & `tmp/pygmtools-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.3.6.tar", last modified: Mon Mar 27 09:04:57 2023, max compression
+gzip compressed data, was "pygmtools-0.3.7.tar", last modified: Thu Apr 27 15:32:24 2023, max compression
```

## Comparing `pygmtools-0.3.6.tar` & `pygmtools-0.3.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 09:04:57.493804 pygmtools-0.3.6/
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-03-27 09:04:33.000000 pygmtools-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 09:04:33.000000 pygmtools-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-03-27 09:04:57.493804 pygmtools-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-03-27 09:04:33.000000 pygmtools-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 09:04:57.489804 pygmtools-0.3.6/pygmtools/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26415 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    40750 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    57449 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    57459 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/jittor_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/jittor_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    63643 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    43089 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    69204 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    59271 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/numpy_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    56491 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/paddle_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/paddle_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    57454 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/pytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    23046 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/tensorflow_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    47249 2023-03-27 09:04:34.000000 pygmtools-0.3.6/pygmtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 09:04:57.489804 pygmtools-0.3.6/pygmtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-03-27 09:04:57.000000 pygmtools-0.3.6/pygmtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-27 09:04:57.000000 pygmtools-0.3.6/pygmtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 09:04:57.000000 pygmtools-0.3.6/pygmtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-27 09:04:57.000000 pygmtools-0.3.6/pygmtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 09:04:57.000000 pygmtools-0.3.6/pygmtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 09:04:57.493804 pygmtools-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-27 09:04:34.000000 pygmtools-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 09:04:57.493804 pygmtools-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-03-27 09:04:34.000000 pygmtools-0.3.6/tests/test_classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-03-27 09:04:34.000000 pygmtools-0.3.6/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-03-27 09:04:34.000000 pygmtools-0.3.6/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-03-27 09:04:34.000000 pygmtools-0.3.6/tests/test_multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-03-27 09:04:34.000000 pygmtools-0.3.6/tests/test_neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-27 09:04:34.000000 pygmtools-0.3.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.621053 pygmtools-0.3.7/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-27 15:32:08.000000 pygmtools-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 15:32:08.000000 pygmtools-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-04-27 15:32:24.621053 pygmtools-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-04-27 15:32:08.000000 pygmtools-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.617053 pygmtools-0.3.7/pygmtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26415 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47379 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57869 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57459 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/jittor_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/jittor_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75786 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/mindspore_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43089 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69204 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59271 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/numpy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56491 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/paddle_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/paddle_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57454 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/pytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23046 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/tensorflow_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.617053 pygmtools-0.3.7/pygmtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:32:24.621053 pygmtools-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-27 15:32:08.000000 pygmtools-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.621053 pygmtools-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_utils.py
```

### Comparing `pygmtools-0.3.6/PKG-INFO` & `pygmtools-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.6
+Version: 0.3.7
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
@@ -136,25 +136,25 @@
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/paddle_logo.png" alt="paddle logo" width="200"/>
 
 * [Tensorflow](https://tensorflow.google.cn/) (GPU friendly, deep learning friendly)
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/tensorflow_logo.png" alt="tensorflow logo" width="200"/>
 
-### Development status (0.3.6)
+### Development status (0.3.7)
 
 |                     | Numpy | PyTorch | Jittor | PaddlePaddle | Tensorflow | MindSpore |
 | ------------------- | ----- | ------- | ------ | ------------ | ---------- | --------- |
-| Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | 🧱        |
-| Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | 🧱        |
+| Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
+| Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Multi-Graph Solvers | ✔    | ✔       | ✔      | ✔            | 📆         | 📆        |
 | Neural Solvers      | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
 | Examples Gallery    | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
 
-✔: Supported; 🧱: Work in progress; 📆: Planned for future versions (contributions welcomed!).
+✔: Supported; 📆: Planned for future versions (contributions welcomed!).
 
 For more details, please [read the documentation](https://pygmtools.readthedocs.io/en/latest/guide/get_started.html#install-other-backends).
 
 ## Pretrained Models
 
 The library includes several neural network solvers. The pretrained models shall be automatically downloaded upon 
 needed from Google Drive. If you are experiencing issues accessing Google Drive, please download the pretrained models
```

### Comparing `pygmtools-0.3.6/README.md` & `pygmtools-0.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,25 +116,25 @@
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/paddle_logo.png" alt="paddle logo" width="200"/>
 
 * [Tensorflow](https://tensorflow.google.cn/) (GPU friendly, deep learning friendly)
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/tensorflow_logo.png" alt="tensorflow logo" width="200"/>
 
-### Development status (0.3.6)
+### Development status (0.3.7)
 
 |                     | Numpy | PyTorch | Jittor | PaddlePaddle | Tensorflow | MindSpore |
 | ------------------- | ----- | ------- | ------ | ------------ | ---------- | --------- |
-| Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | 🧱        |
-| Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | 🧱        |
+| Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
+| Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Multi-Graph Solvers | ✔    | ✔       | ✔      | ✔            | 📆         | 📆        |
 | Neural Solvers      | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
 | Examples Gallery    | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
 
-✔: Supported; 🧱: Work in progress; 📆: Planned for future versions (contributions welcomed!).
+✔: Supported; 📆: Planned for future versions (contributions welcomed!).
 
 For more details, please [read the documentation](https://pygmtools.readthedocs.io/en/latest/guide/get_started.html#install-other-backends).
 
 ## Pretrained Models
 
 The library includes several neural network solvers. The pretrained models shall be automatically downloaded upon 
 needed from Google Drive. If you are experiencing issues accessing Google Drive, please download the pretrained models
```

### Comparing `pygmtools-0.3.6/pygmtools/__init__.py` & `pygmtools-0.3.7/pygmtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .benchmark import Benchmark
 from .linear_solvers import sinkhorn, hungarian
 from .classic_solvers import rrwm, sm, ipfp
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm
 import pygmtools.utils as utils
 BACKEND = 'numpy'
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 __author__ = 'ThinkLab at SJTU'
 
 
 def env_report():
     """
     Print environment report
     """
```

### Comparing `pygmtools-0.3.6/pygmtools/benchmark.py` & `pygmtools-0.3.7/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/classic_solvers.py` & `pygmtools-0.3.7/pygmtools/classic_solvers.py`

 * *Files 13% similar despite different names*

```diff
@@ -233,14 +233,74 @@
             >>> optim = nn.SGD(model.parameters(), lr=0.1)
             >>> X = model(K, n1, n2)
             >>> loss = X.sum()
             >>> optim.step(loss)
             >>> len(jt.nonzero(K.opt_grad(optim)))
             2560
 
+    .. dropdown:: mindspore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+            >>> _ = mindspore.set_seed(1)
+            >>> mindspore.set_context(mode=mindspore.PYNATIVE_MODE)
+
+            # Generate a batch of isomorphic graphs
+            >>> batch_size = 10
+            >>> X_gt = mindspore.numpy.zeros((batch_size, 4, 4))
+            >>> X_gt[:, mindspore.numpy.arange(0, 4, dtype=mindspore.int64), mindspore.ops.Randperm(4)(mindspore.Tensor([4], dtype=mindspore.int32))] = 1
+            >>> A1 = mindspore.numpy.rand((batch_size, 4, 4))
+            >>> A2 = mindspore.ops.BatchMatMul()(mindspore.ops.BatchMatMul()(X_gt.swapaxes(1, 2), A1), X_gt)
+            >>> n1 = n2 = mindspore.Tensor([4] * batch_size)
+
+            # Build affinity matrix
+            >>> conn1, edge1, ne1 = pygm.utils.dense_to_sparse(A1)
+            >>> conn2, edge2, ne2 = pygm.utils.dense_to_sparse(A2)
+            >>> import functools
+            >>> gaussian_aff = functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.) # set affinity function
+            >>> K = pygm.utils.build_aff_mat(None, edge1, conn1, None, edge2, conn2, n1, None, n2, None, edge_aff_fn=gaussian_aff)
+
+            # Solve by SM. Note that X is normalized with a squared sum of 1
+            >>> X = pygm.sm(K, n1, n2)
+            >>> (X ** 2).sum(axis=(1, 2))
+            [1.0000002  0.9999998  1.0000002  0.99999964 1.         1.0000001
+            1.         1.         1.         0.99999994]
+
+            # Accuracy
+            >>> (pygm.hungarian(X) * X_gt).sum() / X_gt.sum()
+            1.0
+
+            # This solver supports gradient back-propogation
+            >>> def fn(K, n1, n2):
+            >>>     res = pygm.sm(K, n1, n2).sum()
+            >>>     return res
+
+            >>> g = mindspore.ops.grad(fn)(K, n1, n2)
+            >>> mindspore.ops.count_nonzero(g)
+            
+            # This solver supports gradient back-propogation
+            >>> from jittor import nn
+            >>> class Model(nn.Module):
+            ...     def __init__(self, K):
+            ...         self.K = K
+            ...     def execute(self, K, n1, n2):
+            ...         X = pygm.sm(K, n1, n2)
+            ...         return X
+
+            >>> model = Model(K)
+            >>> optim = nn.SGD(model.parameters(), lr=0.1)
+            >>> X = model(K, n1, n2)
+            >>> loss = X.sum()
+            >>> optim.step(loss)
+            >>> len(jt.nonzero(K.opt_grad(optim)))
+            2560
+
     .. dropdown:: Tensorflow Example
 
         ::
 
             >>> import tensorflow as tf
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'tensorflow'
@@ -262,14 +322,21 @@
             >>> conn2, edge2, ne2 = pygm.utils.dense_to_sparse(A2)
             >>> import functools
             >>> gaussian_aff = functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.) # set affinity function
             >>> K = pygm.utils.build_aff_mat(None, edge1, conn1, None, edge2, conn2, n1, None, n2, None, edge_aff_fn=gaussian_aff)
 
             # Solve by SM. Note that X is normalized with a squared sum of 1
             >>> X = pygm.sm(K, n1, n2)
+            >>> (X ** 2).sum(axis=(1, 2))
+            [1.         0.9999998  0.99999976 1.         0.99999976 1.
+            1.         1.0000001  1.0000001  1.        ]
+
+            # Accuracy
+            >>> (pygm.hungarian(X) * X_gt).sum() / X_gt.sum()
+            1.0
             >>> tf.reduce_sum((X ** 2), axis=[1, 2])
             <tf.Tensor: shape=(10,), dtype=float32, numpy=
             array([1.        , 1.0000001 , 1.        , 0.9999999 , 1.        ,
                    1.        , 1.0000001 , 0.99999994, 1.        , 0.9999998 ],
                   dtype=float32)>
 
             # Accuracy
@@ -542,14 +609,61 @@
             >>> optim = nn.SGD(model.parameters(), lr=0.1)
             >>> X = model(K, n1, n2, beta=100)
             >>> loss = X.sum()
             >>> optim.step(loss)
             >>> len(jt.nonzero(K.opt_grad(optim)))
             1536
 
+    .. dropdown:: mindspore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+            >>> _ = mindspore.set_seed(1)
+            >>> mindspore.set_context(mode=mindspore.PYNATIVE_MODE)
+
+            # Generate a batch of isomorphic graphs
+            >>> batch_size = 10
+            >>> X_gt = mindspore.numpy.zeros((batch_size, 4, 4))
+            >>> X_gt[:, mindspore.numpy.arange(0, 4, dtype=mindspore.int64), mindspore.ops.Randperm(4)(mindspore.Tensor([4], dtype=mindspore.int32))] = 1
+            >>> A1 = mindspore.numpy.rand((batch_size, 4, 4))
+            >>> A2 = mindspore.ops.BatchMatMul()(mindspore.ops.BatchMatMul()(X_gt.swapaxes(1, 2), A1), X_gt)
+            >>> n1 = n2 = mindspore.Tensor([4] * batch_size)
+
+            # Build affinity matrix
+            >>> conn1, edge1, ne1 = pygm.utils.dense_to_sparse(A1)
+            >>> conn2, edge2, ne2 = pygm.utils.dense_to_sparse(A2)
+            >>> import functools
+            >>> gaussian_aff = functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.) # set affinity function
+            >>> K = pygm.utils.build_aff_mat(None, edge1, conn1, None, edge2, conn2, n1, None, n2, None, edge_aff_fn=gaussian_aff)
+
+            # Solve by RRWM. Note that X is normalized with a sum of 1
+            >>> X = pygm.rrwm(K, n1, n2, beta=100)
+            >>> X.sum(axis=(1, 2))
+            [1.         0.99999994 0.99999994 1.         1.0000002  1.
+            1.         1.         1.0000001  1.0000001 ]
+
+            # Accuracy
+            >>> (pygm.hungarian(X) * X_gt).sum() / X_gt.sum()
+            1.0
+
+            # This solver supports gradient back-propogation
+            >>> def fn(K, n1, n2, beta):
+            >>>     X = pygm.rrwm(K, n1, n2, beta=beta)
+            >>>     X_gt = mindspore.numpy.zeros((batch_size, 4, 4))
+            >>>     X_gt[:, mindspore.numpy.arange(0, 4, dtype=mindspore.int64),mindspore.ops.Randperm(4)(mindspore.Tensor([4], dtype=mindspore.int32))] = 1
+            >>>     res = pygm.utils.permutation_loss(X, X_gt)
+            >>>     return res
+
+            >>> g = mindspore.ops.grad(fn)(K, n1, n2, beta=100)
+            >>> mindspore.ops.count_nonzero(g)
+            2560
+
     .. dropdown:: Tensorflow Example
 
         ::
 
             >>> import tensorflow as tf
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'tensorflow'
@@ -819,14 +933,51 @@
                     [0. 0. 0. 1.]
                     [0. 1. 0. 0.]], dtype=float32)
 
             # Accuracy
             >>> (pygm.hungarian(X) * X_gt).sum() / X_gt.sum()
             jt.Var([1.], dtype=float32)
 
+    .. dropdown:: mindspore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+            >>> _ = mindspore.set_seed(1)
+
+            # Generate a batch of isomorphic graphs
+            >>> batch_size = 10
+            >>> X_gt = mindspore.numpy.zeros((batch_size, 4, 4))
+            >>> X_gt[:, mindspore.numpy.arange(0, 4, dtype=mindspore.int64), mindspore.ops.Randperm(4)(mindspore.Tensor([4], dtype=mindspore.int32))] = 1
+            >>> A1 = mindspore.numpy.rand((batch_size, 4, 4))
+            >>> A2 = mindspore.ops.BatchMatMul()(mindspore.ops.BatchMatMul()(X_gt.swapaxes(1, 2), A1), X_gt)
+            >>> n1 = mindspore.Tensor([4] * batch_size)
+            >>> n2 = mindspore.Tensor([4] * batch_size)
+
+            # Build affinity matrix
+            >>> conn1, edge1, ne1 = pygm.utils.dense_to_sparse(A1)
+            >>> conn2, edge2, ne2 = pygm.utils.dense_to_sparse(A2)
+            >>> import functools
+            >>> gaussian_aff = functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.) # set affinity function
+            >>> K = pygm.utils.build_aff_mat(None, edge1, conn1, None, edge2, conn2, n1, None, n2, None, edge_aff_fn=gaussian_aff)
+
+            # Solve by IPFP
+            >>> X = pygm.ipfp(K, n1, n2)
+            >>> X[0]
+            [[1. 0. 0. 0.]
+             [0. 0. 0. 1.]
+             [0. 0. 1. 0.]
+             [0. 1. 0. 0.]]
+
+            # Accuracy
+            >>> (pygm.hungarian(X) * X_gt).sum() / X_gt.sum()
+            1.0
+
     .. dropdown:: Tensorflow Example
 
         ::
 
             >>> import tensorflow as tf
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'tensorflow'
```

### Comparing `pygmtools-0.3.6/pygmtools/dataset.py` & `pygmtools-0.3.7/pygmtools/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,18 @@
 
             file_names = tar.getnames()
             print('Unzipping files...')
             sleep(0.5)
             for file_name in tqdm(file_names):
                 tar.extract(file_name, "data/PascalVOC/")
             tar.close()
-            os.remove(filename)
+            try:
+                os.remove(filename)
+            except PermissionError:
+                pass
 
         if name == "PascalVOC":
             print('Downloading dataset PascalVOC...')
             filename = "data/PascalVOC.tar"
             download(filename=filename, url=url, to_cache=False)
             try:
                 tar = tarfile.open(filename, "r")
@@ -239,15 +242,18 @@
 
             file_names = tar.getnames()
             print('Unzipping files...')
             sleep(0.5)
             for file_name in tqdm(file_names):
                 tar.extract(file_name, "data/PascalVOC/")
             tar.close()
-            os.remove(filename)
+            try:
+                os.remove(filename)
+            except PermissionError:
+                pass
         return filename
 
     def __filter_list(self, a_xml_list):
         """
         Filter out ``'truncated'``, ``'occluded'`` and ``'difficult'`` images following the practice of previous works.
         In addition, this dataset has uncleaned label (in person category). They are omitted as suggested by README.
         """
@@ -533,15 +539,18 @@
             os.remove(filename)
             return self.download(url, retries - 1)
 
         print('Unzipping files...')
         sleep(0.5)
         for file in tqdm(fz.namelist()):
             fz.extract(file, "data/WillowObject/")
-        os.remove(filename)
+        try:
+            os.remove(filename)
+        except PermissionError:
+            pass
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
@@ -812,15 +821,18 @@
 
         file_names = tar.getnames()
         print('Unzipping files...')
         sleep(0.5)
         for file_name in tqdm(file_names):
             tar.extract(file_name, "data/")
         tar.close()
-        os.remove(filename)
+        try:
+            os.remove(filename)
+        except PermissionError:
+            pass
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
@@ -1061,15 +1073,18 @@
 
         file_names = tar.getnames()
         print('Unzipping files...')
         sleep(0.5)
         for file_name in tqdm(file_names):
             tar.extract(file_name, "data/")
         tar.close()
-        os.remove(filename)
+        try:
+            os.remove(filename)
+        except PermissionError:
+            pass
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
@@ -1254,15 +1269,18 @@
 
         file_names = tar.getnames()
         print('Unzipping files...')
         sleep(0.5)
         for file_name in tqdm(file_names):
             tar.extract(file_name, "data/")
         tar.close()
-        os.remove(filename)
+        try:
+            os.remove(filename)
+        except PermissionError:
+            pass
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
```

### Comparing `pygmtools-0.3.6/pygmtools/dataset_config.py` & `pygmtools-0.3.7/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/jittor_backend.py` & `pygmtools-0.3.7/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/jittor_modules.py` & `pygmtools-0.3.7/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/linear_solvers.py` & `pygmtools-0.3.7/pygmtools/linear_solvers.py`

 * *Files 16% similar despite different names*

```diff
@@ -503,14 +503,113 @@
                     [0.03084473 0.01085788 0.12689069 0.02784578 0.32605886]
                     [0.03192548 0.00745005 0.13391027 0.16087341 0.12289305]
                     [0.2982054  0.01659602 0.32997176 0.06988242 0.10573398]
                     [0.29787776 0.0322356  0.08654935 0.22023994 0.06619392]], dtype=float32)
             >>> print('row_sum:', x.sum(1), 'col_sum:', x.sum(0))
             row_sum: jt.Var([0.8776659  0.52249795 0.45705223 0.8203896  0.70309657], dtype=float32) col_sum: jt.Var([0.7831943  0.30627945 0.73395807 0.61827636 0.938994  ], dtype=float32)
 
+    .. dropdown:: MindSpore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+            >>> np.random.seed(0)
+
+            # 2-dimensional (non-batched) input
+            >>> s_2d = mindspore.Tensor(np.random.rand(5, 5))
+            >>> s_2d
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[5.48813504e-001, 7.15189366e-001, 6.02763376e-001, 5.44883183e-001, 4.23654799e-001],
+                 [6.45894113e-001, 4.37587211e-001, 8.91773001e-001, 9.63662761e-001, 3.83441519e-001],
+                 [7.91725038e-001, 5.28894920e-001, 5.68044561e-001, 9.25596638e-001, 7.10360582e-002],
+                 [8.71292997e-002, 2.02183974e-002, 8.32619846e-001, 7.78156751e-001, 8.70012148e-001],
+                 [9.78618342e-001, 7.99158564e-001, 4.61479362e-001, 7.80529176e-001, 1.18274426e-001]])
+            >>> x = pygm.sinkhorn(s_2d)
+            >>> x
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[1.88802237e-001, 2.49909146e-001, 1.92022173e-001, 1.60342782e-001, 2.08923658e-001],
+                 [1.89450662e-001, 1.72404455e-001, 2.33450110e-001, 2.21947620e-001, 1.82747159e-001],
+                 [2.37135825e-001, 2.04348002e-001, 1.82712427e-001, 2.31145830e-001, 1.44657896e-001],
+                 [1.17310392e-001, 1.22969199e-001, 2.38239095e-001, 1.99615882e-001, 3.21865485e-001],
+                 [2.67300884e-001, 2.50369198e-001, 1.53576195e-001, 1.86947886e-001, 1.41805802e-001]])
+            >>> print('row_sum:', x.sum(1), 'col_sum:', x.sum(0))
+            row_sum: [1.         1.00000001 0.99999998 1.00000005 0.99999997] col_sum: [1. 1. 1. 1. 1.]
+
+            # 3-dimensional (batched) input
+            >>> s_3d = mindspore.Tensor(np.random.rand(3, 5, 5))
+            >>> x = pygm.sinkhorn(s_3d)
+            >>> print('row_sum:', x.sum(2))
+            row_sum: [[1.         1.         1.         1.         1.        ]
+                      [0.99999998 1.00000002 0.99999999 1.00000003 0.99999999]
+                      [1.         1.         1.         1.         1.        ]]
+            >>> print('col_sum:', x.sum(1))
+            col_sum: [[1. 1. 1. 1. 1.]
+                      [1. 1. 1. 1. 1.]
+                      [1. 1. 1. 1. 1.]]
+
+            # If the 3-d tensor are with different number of nodes
+            >>> n1 = mindspore.Tensor([3, 4, 5])
+            >>> n2 = mindspore.Tensor([3, 4, 5])
+            >>> x = pygm.sinkhorn(s_3d, n1, n2)
+            >>> x[0] # non-zero size: 3x3
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[3.66659344e-001, 2.14981580e-001, 4.18359055e-001, 0.00000000e+000, 0.00000000e+000],
+                 [2.76036207e-001, 4.42702065e-001, 2.81261746e-001, 0.00000000e+000, 0.00000000e+000],
+                 [3.57304449e-001, 3.42316355e-001, 3.00379198e-001, 0.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000]])
+            >>> x[1] # non-zero size: 4x4
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[2.88478308e-001, 2.05830510e-001, 3.42420911e-001, 1.63270208e-001, 0.00000000e+000],
+                 [2.26567517e-001, 3.01530213e-001, 1.94079686e-001, 2.77822621e-001, 0.00000000e+000],
+                 [2.53463783e-001, 1.96498526e-001, 3.25650495e-001, 2.24387154e-001, 0.00000000e+000],
+                 [2.31490392e-001, 2.96140751e-001, 1.37848909e-001, 3.34520016e-001, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000]])
+            >>> x[2] # non-zero size: 5x5
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[2.01473521e-001, 1.95419860e-001, 2.49427981e-001, 1.73463970e-001, 1.80214669e-001],
+                 [2.10507324e-001, 1.76209477e-001, 1.86454688e-001, 2.03846840e-001, 2.22981672e-001],
+                 [1.83196232e-001, 1.80240070e-001, 1.76198709e-001, 1.66413296e-001, 2.93951694e-001],
+                 [2.07543757e-001, 2.23644304e-001, 1.96581006e-001, 2.05708473e-001, 1.66522460e-001],
+                 [1.97279167e-001, 2.24486289e-001, 1.91337616e-001, 2.50567421e-001, 1.36329506e-001]])
+
+            # non-squared input
+            >>> s_non_square = mindspore.Tensor(np.random.rand(4, 5))
+            >>> x = pygm.sinkhorn(s_non_square, dummy_row=True) # set dummy_row=True for non-squared cases
+            >>> print('row_sum:', x.sum(1), 'col_sum:', x.sum(0))
+            row_sum: [1. 1. 1. 1.] col_sum: [0.78239609 0.80485526 0.80165627 0.80004254 0.81104984]
+
+            # allow matching to void nodes by setting unmatch1 and unmatch2
+            >>> s_2d = mindspore.Tensor(np.random.randn(5, 5))
+            >>> s_2d
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[1.05000207e-002, 1.78587049e+000, 1.26912093e-001, 4.01989363e-001, 1.88315070e+000],
+                 [-1.34775906e+000, -1.27048500e+000, 9.69396708e-001, -1.17312341e+000, 1.94362119e+000],
+                 [-4.13618981e-001, -7.47454811e-001, 1.92294203e+000, 1.48051479e+000, 1.86755896e+000],
+                 [9.06044658e-001, -8.61225685e-001, 1.91006495e+000, -2.68003371e-001, 8.02456396e-001],
+                 [9.47251968e-001, -1.55010093e-001, 6.14079370e-001, 9.22206672e-001, 3.76425531e-001]])
+            >>> unmatch1 = mindspore.Tensor(np.random.randn(5))
+            >>> unmatch1
+            Tensor(shape=[5], dtype=Float64, value= [-1.09940079e+000, 2.98238174e-001, 1.32638590e+000, -6.94567860e-001, -1.49634540e-001])
+            >>> unmatch2 = mindspore.Tensor(np.random.randn(5))
+            >>> unmatch2
+            Tensor(shape=[5], dtype=Float64, value= [-4.35153552e-001, 1.84926373e+000, 6.72294757e-001, 4.07461836e-001, -7.69916074e-001])
+            >>> x = pygm.sinkhorn(s_2d, unmatch1=unmatch1, unmatch2=unmatch2, max_iter=40)
+            >>> x
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[1.24341010e-001, 2.39139910e-001, 5.66359709e-002, 1.39434794e-001, 3.18114246e-001],
+                 [3.08447251e-002, 1.08578709e-002, 1.26890674e-001, 2.78457752e-002, 3.26058897e-001],
+                 [3.19254796e-002, 7.45003720e-003, 1.33910250e-001, 1.60873453e-001, 1.22893042e-001],
+                 [2.98205355e-001, 1.65960124e-002, 3.29971742e-001, 6.98824247e-002, 1.05733960e-001],
+                 [2.97877737e-001, 3.22356021e-002, 8.65493605e-002, 2.20239960e-001, 6.61939270e-002]])
+            >>> print('row_sum:', x.sum(1), 'col_sum:', x.sum(0))
+            row_sum: [0.87766593 0.52249794 0.45705226 0.82038949 0.70309659] col_sum: [0.78319431 0.30627943 0.733958   0.61827641 0.93899407]
+
     .. dropdown:: Tensorflow Example
 
         ::
 
             >>> import tensorflow as tf
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'tensorflow'
@@ -1024,14 +1123,87 @@
             >>> x
             jt.Var([[0. 0. 0. 0. 0.]
                     [0. 0. 0. 0. 1.]
                     [0. 0. 1. 0. 0.]
                     [0. 0. 0. 0. 0.]
                     [0. 0. 0. 0. 0.]], dtype=float32)
 
+    .. dropdown:: MindSpore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+            >>> np.random.seed(0)
+
+            # 2-dimensional (non-batched) input
+            >>> s_2d = mindspore.Tensor(np.random.rand(5, 5))
+            >>> s_2d
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[5.48813504e-001, 7.15189366e-001, 6.02763376e-001, 5.44883183e-001, 4.23654799e-001],
+                 [6.45894113e-001, 4.37587211e-001, 8.91773001e-001, 9.63662761e-001, 3.83441519e-001],
+                 [7.91725038e-001, 5.28894920e-001, 5.68044561e-001, 9.25596638e-001, 7.10360582e-002],
+                 [8.71292997e-002, 2.02183974e-002, 8.32619846e-001, 7.78156751e-001, 8.70012148e-001],
+                 [9.78618342e-001, 7.99158564e-001, 4.61479362e-001, 7.80529176e-001, 1.18274426e-001]])
+            >>> x = pygm.hungarian(s_2d)
+            >>> x
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 1.00000000e+000],
+                 [1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000]])
+
+            # 3-dimensional (batched) input
+            >>> s_3d = mindspore.Tensor(np.random.rand(3, 5, 5))
+            >>> n1 = n2 = mindspore.Tensor([3, 4, 5])
+            >>> x = pygm.hungarian(s_3d, n1, n2)
+            >>> x
+            Tensor(shape=[3, 5, 5], dtype=Float64, value=
+                [[[0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000]],
+                 [[1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000]],
+                 [[0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 1.00000000e+000],
+                  [0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                  [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000]]])
+
+            # allow matching to void nodes by setting unmatch1 and unmatch2
+            >>> s_2d = mindspore.Tensor(np.random.randn(5, 5))
+            >>> s_2d
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[-1.16514984e+000, 9.00826487e-001, 4.65662440e-001, -1.53624369e+000, 1.48825219e+000],
+                 [1.89588918e+000, 1.17877957e+000, -1.79924836e-001, -1.07075262e+000, 1.05445173e+000],
+                 [-4.03176947e-001, 1.22244507e+000, 2.08274978e-001, 9.76639036e-001, 3.56366397e-001],
+                 [7.06573168e-001, 1.05000207e-002, 1.78587049e+000, 1.26912093e-001, 4.01989363e-001],
+                 [1.88315070e+000, -1.34775906e+000, -1.27048500e+000, 9.69396708e-001, -1.17312341e+000]])
+            >>> unmatch1 = mindspore.Tensor(np.random.randn(5))
+            >>> unmatch1
+            Tensor(shape=[5], dtype=Float64, value= [1.94362119e+000, -4.13618981e-001, -7.47454811e-001, 1.92294203e+000, 1.48051479e+000])
+            >>> unmatch2 = mindspore.Tensor(np.random.randn(5))
+            >>> unmatch2
+            Tensor(shape=[5], dtype=Float64, value= [1.86755896e+000, 9.06044658e-001, -8.61225685e-001, 1.91006495e+000, -2.68003371e-001])
+            >>> x = pygm.hungarian(s_2d, unmatch1=unmatch1, unmatch2=unmatch2)
+            >>> x
+            Tensor(shape=[5, 5], dtype=Float64, value=
+                [[0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 1.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 1.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000],
+                 [0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000, 0.00000000e+000]])
+
     .. dropdown:: Tensorflow Example
 
         ::
 
             >>> import tensorflow as tf
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'tensorflow'
```

### Comparing `pygmtools-0.3.6/pygmtools/multi_graph_solvers.py` & `pygmtools-0.3.7/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/neural_solvers.py` & `pygmtools-0.3.7/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/numpy_backend.py` & `pygmtools-0.3.7/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/numpy_modules.py` & `pygmtools-0.3.7/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/paddle_backend.py` & `pygmtools-0.3.7/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/paddle_modules.py` & `pygmtools-0.3.7/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/pytorch_backend.py` & `pygmtools-0.3.7/pygmtools/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/pytorch_modules.py` & `pygmtools-0.3.7/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/tensorflow_backend.py` & `pygmtools-0.3.7/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/pygmtools/utils.py` & `pygmtools-0.3.7/pygmtools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,45 @@
             # Build affinity matrix based on node features
             >>> F1 = paddle.rand((batch_size, 4, 10))
             >>> F2 = paddle.rand((batch_size, 4, 10))
             >>> K3 = pygm.utils.build_aff_mat(F1, edge1, conn1, F2, edge2, conn2, n1, ne1, n2, ne2, edge_aff_fn=gaussian_aff)
 
             # The affinity matrices K, K2, K3 can be further processed by GM solvers
 
+    .. dropdown:: mindspore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+
+            # Generate a batch of graphs
+            >>> batch_size = 10
+            >>> A1 = mindspore.numpy.rand((batch_size, 4, 4))
+            >>> A2 = mindspore.numpy.rand((batch_size, 4, 4))
+            >>> n1 = n2 = mindspore.Tensor([4] * batch_size)
+
+            # Build affinity matrix by the default inner-product function
+            >>> conn1, edge1, ne1 = pygm.utils.dense_to_sparse(A1)
+            >>> conn2, edge2, ne2 = pygm.utils.dense_to_sparse(A2)
+            >>> K = pygm.utils.build_aff_mat(None, edge1, conn1, None, edge2, conn2, n1, ne1, n2, ne2)
+
+            # Build affinity matrix by gaussian kernel
+            >>> import functools
+            >>> gaussian_aff = functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.)
+            >>> K2 = pygm.utils.build_aff_mat(None, edge1, conn1, None, edge2, conn2, n1, ne1, n2, ne2, edge_aff_fn=gaussian_aff)
+
+            # Build affinity matrix based on node features
+            >>> F1 = mindspore.numpy.rand((batch_size, 4, 10))
+            >>> F2 = mindspore.numpy.rand((batch_size, 4, 10))
+            >>> K3 = pygm.utils.build_aff_mat(F1, edge1, conn1, F2, edge2, conn2, n1, ne1, n2, ne2, edge_aff_fn=gaussian_aff)
+
+            # The affinity matrices K, K2, K3 can be further processed by GM solvers
+
     """
     if backend is None:
         backend = pygmtools.BACKEND
     __get_shape = functools.partial(_get_shape, backend=backend)
 
     # check the correctness of input
     batch_size = None
@@ -382,14 +413,41 @@
             >>> F1 = paddle.rand((4, 10))
             >>> F2 = paddle.rand((5, 10))
             >>> F3 = paddle.rand((3, 10))
             >>> batched_F = pygm.utils.build_batch([F1, F2, F3])
             >>> batched_F.shape
             [3, 5, 10]
 
+    .. dropdown:: mindspore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+
+            # batched adjacency matrices
+            >>> A1 = mindspore.numpy.rand((4, 4))
+            >>> A2 = mindspore.numpy.rand((5, 5))
+            >>> A3 = mindspore.numpy.rand((3, 3))
+            >>> batched_A, ori_shape = pygm.utils.build_batch([A1, A2, A3], return_ori_dim=True)
+            >>> batched_A.shape
+            (3, 5, 5)
+            >>> ori_shape
+            (Tensor(shape=[3], dtype=Int64, value= [4, 5, 3]),
+             Tensor(shape=[3], dtype=Int64, value= [4, 5, 3]))
+
+            # batched node features (feature dimension=10)
+            >>> F1 = mindspore.numpy.rand((4, 10))
+            >>> F2 = mindspore.numpy.rand((5, 10))
+            >>> F3 = mindspore.numpy.rand((3, 10))
+            >>> batched_F = pygm.utils.build_batch([F1, F2, F3])
+            >>> batched_F.shape
+            (3, 5, 10)
+
     """
     if backend is None:
         backend = pygmtools.BACKEND
     for item in input:
         _check_data_type(item, backend)
     args = (input, return_ori_dim)
     try:
@@ -488,14 +546,39 @@
             >>> edge.shape # edge feature (batch x num_edge x feature_dim)
             torch.Size([10, 16, 1])
 
             >>> ne
             Tensor(shape=[10], dtype=int64, place=Place(cpu), stop_gradient=True,
                     [16, 16, 16, 16, 16, 16, 16, 16, 16, 16])
 
+    .. dropdown:: mindspore Example
+
+        ::
+
+            >>> import mindspore
+            >>> import pygmtools as pygm
+            >>> pygm.BACKEND = 'mindspore'
+            >>> _ = mindspore.set_seed(0)
+
+            >>> batch_size = 10
+            >>> A = mindspore.numpy.rand((batch_size, 4, 4))
+            >>> mindspore.numpy.diagonal(A, axis1=1, axis2=2)[:] = 0 # remove the diagonal elements
+            >>> A.shape
+            (10, 4, 4)
+
+            >>> conn, edge, ne = pygm.utils.dense_to_sparse(A)
+            >>> conn.shape # connectivity: (batch x num_edge x 2)
+            (10, 16, 2)
+
+            >>> edge.shape # edge feature (batch x num_edge x feature_dim)
+            (10, 16, 1)
+
+            >>> ne
+            [16 16 16 16 16 16 16 16 16 16]
+
     """
     if backend is None:
         backend = pygmtools.BACKEND
     _check_data_type(dense_adj, backend)
     if _check_shape(dense_adj, 2, backend):
         dense_adj = _unsqueeze(dense_adj, 0, backend)
         non_batched_input = True
@@ -788,15 +871,15 @@
         if self.backend != 'numpy':
             raise ValueError('Attempting to convert from non-numpy data.')
         if new_backend is None:
             new_backend = pygmtools.BACKEND
         self.backend = new_backend
         for k, v in self.match_dict.items():
             self.match_dict[k] = from_numpy(v, device, self.backend)
-    
+
     def to_numpy_(self):
         """
         In-place operation for :func:`~pygmtools.utils.MultiMatchingResult.to_numpy`.
         """
         for k, v in self.match_dict.items():
             self.match_dict[k] = to_numpy(v, self.backend)
         self.backend = 'numpy'
```

### Comparing `pygmtools-0.3.6/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.3.7/pygmtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.6
+Version: 0.3.7
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
@@ -136,25 +136,25 @@
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/paddle_logo.png" alt="paddle logo" width="200"/>
 
 * [Tensorflow](https://tensorflow.google.cn/) (GPU friendly, deep learning friendly)
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/tensorflow_logo.png" alt="tensorflow logo" width="200"/>
 
-### Development status (0.3.6)
+### Development status (0.3.7)
 
 |                     | Numpy | PyTorch | Jittor | PaddlePaddle | Tensorflow | MindSpore |
 | ------------------- | ----- | ------- | ------ | ------------ | ---------- | --------- |
-| Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | 🧱        |
-| Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | 🧱        |
+| Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
+| Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Multi-Graph Solvers | ✔    | ✔       | ✔      | ✔            | 📆         | 📆        |
 | Neural Solvers      | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
 | Examples Gallery    | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
 
-✔: Supported; 🧱: Work in progress; 📆: Planned for future versions (contributions welcomed!).
+✔: Supported; 📆: Planned for future versions (contributions welcomed!).
 
 For more details, please [read the documentation](https://pygmtools.readthedocs.io/en/latest/guide/get_started.html#install-other-backends).
 
 ## Pretrained Models
 
 The library includes several neural network solvers. The pretrained models shall be automatically downloaded upon 
 needed from Google Drive. If you are experiencing issues accessing Google Drive, please download the pretrained models
```

### Comparing `pygmtools-0.3.6/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.3.7/pygmtools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pygmtools/benchmark.py
 pygmtools/classic_solvers.py
 pygmtools/dataset.py
 pygmtools/dataset_config.py
 pygmtools/jittor_backend.py
 pygmtools/jittor_modules.py
 pygmtools/linear_solvers.py
+pygmtools/mindspore_backend.py
 pygmtools/multi_graph_solvers.py
 pygmtools/neural_solvers.py
 pygmtools/numpy_backend.py
 pygmtools/numpy_modules.py
 pygmtools/paddle_backend.py
 pygmtools/paddle_modules.py
 pygmtools/pytorch_backend.py
```

### Comparing `pygmtools-0.3.6/setup.py` & `pygmtools-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/tests/test_classic_solvers.py` & `pygmtools-0.3.7/tests/test_classic_solvers.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,26 @@
 import torch
 import functools
 import itertools
 from tqdm import tqdm
 
 from test_utils import *
 
+import platform
+
+os_name = platform.system()
+
+def get_backends(backend):
+    if backend == "all":
+        backends = ['pytorch', 'numpy', 'paddle', 'jittor', 'tensorflow'] if os_name == 'Linux' else ['pytorch', 'numpy',  'paddle', 'tensorflow']
+    else:
+        backends = ["pytorch", backend]
+    return backends
+
+
 # The testing function for quadratic assignment
 def _test_classic_solver_on_isomorphic_graphs(graph_num_nodes, node_feat_dim, solver_func, matrix_params, backends):
     assert 'edge_aff_fn' in matrix_params
     assert 'node_aff_fn' in matrix_params
     if backends[0] != 'pytorch': backends.insert(0, 'pytorch') # force pytorch as the reference backend
 
     batch_size = len(graph_num_nodes)
@@ -185,135 +197,157 @@
                 accuracy = (pygm.utils.to_numpy(pygm.hungarian(_X, _n1, _n2)) * X_gt).sum() / X_gt.sum()
 
             assert accuracy == 1, f"GM is inaccurate for {working_backend}, accuracy={accuracy:.4f}, " \
                                   f"params: {';'.join([k + '=' + str(v) for k, v in prob_param_dict.items()])};" \
                                   f"{';'.join([k + '=' + str(v) for k, v in solver_param_dict.items()])}"
 
             if last_X is not None:
-                assert np.abs(pygm.utils.to_numpy(_X) - last_X).sum() < 5e-4, \
+                assert np.abs(pygm.utils.to_numpy(_X) - last_X).sum() < 1e-3, \
                     f"Incorrect GM solution for {working_backend}\n" \
                     f"params: {';'.join([k + '=' + str(v) for k, v in prob_param_dict.items()])}\n" \
                     f"{';'.join([k + '=' + str(v) for k, v in solver_param_dict.items()])}"
             last_X = pygm.utils.to_numpy(_X)
 
 
-def test_hungarian():
+def test_hungarian(get_backend):
+    backends = get_backends(get_backend)
     _test_classic_solver_on_linear_assignment(list(range(10, 30, 2)), list(range(30, 10, -2)), 10, pygm.hungarian, {
         'nproc': [1, 2, 4],
         'outlier_num': [0, 5, 10]
-    }, ['pytorch', 'numpy', 'paddle' ,'jittor','tensorflow'])
+    }, backends)
 
     # non-batched input
     _test_classic_solver_on_linear_assignment([10], [30], 10, pygm.hungarian, {
         'nproc': [1],
         'outlier_num': [0, 5]
-    }, ['pytorch', 'numpy', 'paddle' ,'jittor','tensorflow'])
+    }, backends)
 
 
-def test_sinkhorn():
+def test_sinkhorn(get_backend):
+    backends = get_backends(get_backend)
     # test non-symmetric matching
     args1 = (list(range(10, 30, 2)), list(range(30, 10, -2)), 10, pygm.sinkhorn, {
-            'tau': [0.1, 0.01],
-            'max_iter': [10, 20, 50],
-            'batched_operation': [True, False],
-            'dummy_row': [True, ],
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+        'tau': [0.1, 0.01],
+        'max_iter': [10, 20, 50],
+        'batched_operation': [True, False],
+        'dummy_row': [True, ],
+    }, backends)
 
     # test symmetric matching
     args2 = (list(range(10, 30, 2)), list(range(10, 30, 2)), 10, pygm.sinkhorn, {
         'tau': [0.1, 0.01],
         'max_iter': [10, 20, 50],
         'batched_operation': [True, False],
         'dummy_row': [True, False],
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
     # test outlier matching (non-symmetric)
     args3 = (list(range(10, 30, 2)), list(range(30, 10, -2)), 10, pygm.sinkhorn, {
         'tau': [0.01, 0.001],
         'max_iter': [500, 1000],
         'batched_operation': [True, False],
         'dummy_row': [True, False],
         'outlier_num': [5, 10]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
     # test outlier matching (symmetric)
     args4 = (list(range(10, 30, 2)), list(range(10, 30, 2)), 10, pygm.sinkhorn, {
         'tau': [0.01, 0.001],
         'max_iter': [500, 1000],
         'batched_operation': [True, False],
         'dummy_row': [True, False],
         'outlier_num': [5, 10]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
     # test non-batched matching
     args5 = ([30], [10], 10, pygm.sinkhorn, {
         'tau': [0.01],
         'max_iter': [500],
         'batched_operation': [True],
         'dummy_row': [True],
         'outlier_num': [0, 5]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
     _test_classic_solver_on_linear_assignment(*args1)
     _test_classic_solver_on_linear_assignment(*args2)
     _test_classic_solver_on_linear_assignment(*args3)
     _test_classic_solver_on_linear_assignment(*args4)
     _test_classic_solver_on_linear_assignment(*args5)
 
 
-def test_rrwm():
-    _test_classic_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 10, pygm.rrwm, {
-        'alpha': [0.1, 0.5, 0.9],
-        'beta': [0.1, 1, 10],
-        'sk_iter': [10, 20],
-        'max_iter': [20, 50],
-        'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
-        'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+def test_rrwm(get_backend):
+    backends = get_backends(get_backend)
+    if "mindspore" in backends:
+        _test_classic_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 10, pygm.rrwm, {
+            'alpha': [0.1, 0.5],
+            'beta': [0.1, 1],
+            'sk_iter': [10, 20],
+            'max_iter': [20],
+            'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
+            'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
+        }, backends)
+    else:
+        _test_classic_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 10, pygm.rrwm, {
+            'alpha': [0.1, 0.5, 0.9],
+            'beta': [0.1, 1, 10],
+            'sk_iter': [10, 20],
+            'max_iter': [20, 50],
+            'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
+            'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
+        }, backends)
 
     # non-batched input
     _test_classic_solver_on_isomorphic_graphs([10], 10, pygm.rrwm, {
         'alpha': [0.1],
         'beta': [0.1],
         'sk_iter': [10],
         'max_iter': [20],
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.)],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1)]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
 
-def test_sm():
-    _test_classic_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 10, pygm.sm, {
-        'max_iter': [10, 50, 100],
-        'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
-        'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+def test_sm(get_backend):
+    backends = get_backends(get_backend)
+    if "mindspore" in backends:
+        _test_classic_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 10, pygm.sm, {
+            'max_iter': [10, 50],
+            'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
+            'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
+        }, backends)
+    else:
+        _test_classic_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 10, pygm.sm, {
+            'max_iter': [10, 50, 100],
+            'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
+            'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
+        }, backends)
 
     # non-batched input
     _test_classic_solver_on_isomorphic_graphs([10], 10, pygm.sm, {
         'max_iter': [10],
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.)],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1)]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
 
-def test_ipfp():
+def test_ipfp(get_backend):
+    backends = get_backends(get_backend)
     _test_classic_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 10, pygm.ipfp, {
         'max_iter': [10, 50, 100],
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
     # non-batched input
     _test_classic_solver_on_isomorphic_graphs([10], 10, pygm.ipfp, {
         'max_iter': [10],
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.)],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1)]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor','tensorflow'])
+    }, backends)
 
 
 if __name__ == '__main__':
-    test_hungarian()
-    test_sinkhorn()
-    test_rrwm()
-    test_sm()
-    test_ipfp()
+    test_hungarian('')
+    test_sinkhorn('')
+    test_rrwm('')
+    test_sm('')
+    test_ipfp('')
```

### Comparing `pygmtools-0.3.6/tests/test_dataset.py` & `pygmtools-0.3.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.6/tests/test_misc.py` & `pygmtools-0.3.7/tests/test_misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 import sys
 sys.path.insert(0, '.')
 import pygmtools as pygm
 import itertools
 import numpy as np
 
+import platform
+os_name = platform.system()
+backends = ['pytorch', 'numpy', 'paddle', 'jittor', 'tensorflow'] if os_name == 'Linux' else ['pytorch', 'numpy', 'paddle', 'tensorflow']
 
 def test_env_report():
     pygm.env_report()
 
 
 def test_generate_isomorphic_graphs():
-    backends = ['pytorch', 'numpy', 'paddle', 'jittor', 'tensorflow']
     for backend in backends:
         pygm.BACKEND = backend
         A, X = pygm.utils.generate_isomorphic_graphs(10)
         A_shape, X_shape = pygm.utils._get_shape(A), pygm.utils._get_shape(X)
         assert A_shape[0] == 2 and A_shape[1] == 10 and A_shape[2] == 10
         assert X_shape[0] == 10 and X_shape[1] == 10
 
@@ -45,16 +47,17 @@
         pygm.utils.generate_isomorphic_graphs(10, backend='null')
     except NotImplementedError:
         pass
 
 
 def test_permutation_loss():
     num_nodes = 10
-    backends = ['pytorch', 'paddle', 'jittor', 'tensorflow']
     for backend in backends:
+        if backend == 'numpy':
+            continue
         pygm.BACKEND = backend
         A, X_gt = pygm.utils.generate_isomorphic_graphs(num_nodes)
         n1 = n2 = num_nodes
         conn1, edge1 = pygm.utils.dense_to_sparse(A[0])
         conn2, edge2 = pygm.utils.dense_to_sparse(A[1])
         K = pygm.utils.build_aff_mat(None, edge1, conn1, None, edge2, conn2)
         S = pygm.rrwm(K, n1, n2)  # solving QAP
@@ -76,15 +79,15 @@
     pygm.BACKEND = 'numpy'
     As, X = pygm.utils.generate_isomorphic_graphs(num_nodes, num_graphs)
     mmX = pygm.utils.MultiMatchingResult()
     for i in range(X.shape[0]):
         for j in range(X.shape[1]):
             mmX[i, j] = X[i, j]
 
-    for backend in ['numpy', 'pytorch', 'paddle', 'jittor']:
+    for backend in backends:
         newX = pygm.utils.from_numpy(mmX, backend=backend)
         newX.__repr__()
         newX.__str__()
 
     try:
         pygm.utils.from_numpy(X, backend='null')
     except NotImplementedError:
```

### Comparing `pygmtools-0.3.6/tests/test_multi_graph_solvers.py` & `pygmtools-0.3.7/tests/test_multi_graph_solvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,34 @@
 
 import random
 
 sys.path.insert(0, '.')
 
 import numpy as np
 import torch
-import jittor as jt
 import functools
 import itertools
 from tqdm import tqdm
 
 from test_utils import *
+import platform
+
+os_name = platform.system()
+backends = ['pytorch', 'numpy', 'paddle', 'jittor'] if os_name == 'Linux' else ['pytorch', 'numpy', 'paddle']
+if os_name == 'Linux':
+    import jittor as jt
+
 
 # The testing function
 def _test_mgm_solver_on_isomorphic_graphs(num_graph, num_node, node_feat_dim, solver_func, mode, matrix_params, backends):
     if mode == 'lawler-qap':
         assert 'edge_aff_fn' in matrix_params
     assert 'node_aff_fn' in matrix_params
     if backends[0] != 'pytorch':
-        backends.insert(0, 'pytorch') # force pytorch as the reference backend
+        backends.insert(0, 'pytorch')  # force pytorch as the reference backend
 
     # Generate isomorphic graphs
     pygm.BACKEND = 'pytorch'
     # As, Fs are for kb-qap algorithms
     torch.manual_seed(1)
     As, X_gt, Fs = pygm.utils.generate_isomorphic_graphs(num_node, num_graph, node_feat_dim)
     # As_1, As_2, Fs_1, Fs_2 are for lawler-qap algorithms
@@ -52,16 +58,16 @@
     As, Fs, As_1, As_2, Fs_1, Fs_2, X_gt = data_to_numpy(As, Fs, As_1, As_2, Fs_1, Fs_2, X_gt)
 
     # call the solver
     total = 1
     for val in matrix_params.values():
         total *= len(val)
     for values in tqdm(itertools.product(*matrix_params.values()), total=total):
-        aff_param_dict = {} # for affinity functions (supported keys: 'node_aff_fn', 'edge_aff_fn')
-        solver_param_dict = {} # for solvers
+        aff_param_dict = {}  # for affinity functions (supported keys: 'node_aff_fn', 'edge_aff_fn')
+        solver_param_dict = {}  # for solvers
         for k, v in zip(matrix_params.keys(), values):
             if k in ['node_aff_fn', 'edge_aff_fn']:
                 aff_param_dict[k] = v
             else:
                 if k == 'x0' and v is not None:
                     # (1-matrix_params['x0']) matchings are correct, the others are randomly permuted
                     x0_prob = v
@@ -88,15 +94,15 @@
             if mode == 'lawler-qap':
                 _As_1, _As_2, _Fs_1, _Fs_2, _X_gt = data_from_numpy(As_1, As_2, Fs_1, Fs_2, X_gt)
                 _conn1, _edge1, _ne1 = pygm.utils.dense_to_sparse(_As_1)
                 _conn2, _edge2, _ne2 = pygm.utils.dense_to_sparse(_As_2)
 
                 _K = pygm.utils.build_aff_mat(_Fs_1, _edge1, _conn1, _Fs_2, _edge2, _conn2, None, _ne1, None, _ne2,
                                               **aff_param_dict)
-                _K = _K.reshape((num_graph, num_graph, num_node**2, num_node**2))
+                _K = _K.reshape((num_graph, num_graph, num_node ** 2, num_node ** 2))
                 if last_K is not None:
                     assert np.abs(pygm.utils.to_numpy(_K) - last_K).sum() < 0.1, \
                         f"Incorrect affinity matrix for {working_backend}, " \
                         f"params: {';'.join([k + '=' + str(v) for k, v in aff_param_dict.items()])};" \
                         f"{';'.join([k + '=' + str(v) for k, v in solver_param_dict.items()])}"
                 last_K = pygm.utils.to_numpy(_K)
                 _X = solver_func(_K, **solver_param_dict)
@@ -113,16 +119,16 @@
                                           f"params: {';'.join([k + '=' + str(v) for k, v in aff_param_dict.items()])};" \
                                           f"{';'.join([k + '=' + str(v) for k, v in solver_param_dict.items()])}"
                 else:
                     assert accuracy >= 1 - x0_prob, f"GM is inaccurate for {working_backend}, accuracy={accuracy}, " \
                                                     f"params: {';'.join([k + '=' + str(v) for k, v in aff_param_dict.items()])};" \
                                                     f"{';'.join([k + '=' + str(v) for k, v in solver_param_dict.items()])}"
             elif mode == 'kb-qap':
-                Fs1 = np.expand_dims(Fs, 1).repeat(num_graph, axis=1).reshape(num_graph**2, num_node, node_feat_dim)
-                Fs2 = np.expand_dims(Fs, 0).repeat(num_graph, axis=0).reshape(num_graph**2, num_node, node_feat_dim)
+                Fs1 = np.expand_dims(Fs, 1).repeat(num_graph, axis=1).reshape(num_graph ** 2, num_node, node_feat_dim)
+                Fs2 = np.expand_dims(Fs, 0).repeat(num_graph, axis=0).reshape(num_graph ** 2, num_node, node_feat_dim)
                 _As, _Fs1, _Fs2, _X_gt = data_from_numpy(As, Fs1, Fs2, X_gt)
                 node_aff_mat = aff_param_dict['node_aff_fn'](_Fs1, _Fs2)
                 node_aff_mat = node_aff_mat.reshape((num_graph, num_graph, num_node, num_node))
                 _X = solver_func(_As, node_aff_mat, **solver_param_dict)
 
                 if last_X is not None:
                     diff = 0
@@ -152,64 +158,65 @@
             else:
                 raise ValueError(f'Unknown mode: {mode}')
             if 'x0' in solver_param_dict and solver_param_dict['x0'] is not None:
                 solver_param_dict['x0'] = pygm.utils.to_numpy(solver_param_dict['x0'])
             if 'ns' in solver_param_dict and solver_param_dict['ns'] is not None:
                 solver_param_dict['ns'] = pygm.utils.to_numpy(solver_param_dict['ns'])
 
+
 def test_cao():
     num_nodes = 5
     num_graphs = 10
     _test_mgm_solver_on_isomorphic_graphs(num_graphs, num_nodes, 10, pygm.cao, 'lawler-qap', {
         'mode': ['time', 'memory'],
         'x0': [None, 0.2, 0.5],
         'lambda_init': [0.1, 0.3],
         'qap_solver': [functools.partial(pygm.ipfp, n1max=num_nodes, n2max=num_nodes), None],
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor'])
+    }, backends)
 
 
 def test_mgm_floyd():
     num_nodes = 5
     num_graphs = 10
     _test_mgm_solver_on_isomorphic_graphs(num_graphs, num_nodes, 10, pygm.mgm_floyd, 'lawler-qap', {
         'mode': ['time', 'memory'],
         'x0': [None, 0.2, 0.5],
         'param_lambda': [0.1, 0.3],
         'qap_solver': [functools.partial(pygm.ipfp, n1max=num_nodes, n2max=num_nodes), None],
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn]
-    }, ['pytorch', 'numpy', 'paddle', 'jittor'])
+    }, backends)
 
 
 def test_gamgm():
     num_nodes = 5
     num_graphs = 10
     # test without outliers
     _test_mgm_solver_on_isomorphic_graphs(num_graphs, num_nodes, 10, pygm.gamgm, 'kb-qap', {
-            'sk_init_tau': [0.5, 0.1],
-            'sk_min_tau': [0.1, 0.05],
-            'param_lambda': [0.1, 0.5],
-            'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn],
-            'verbose': [True]
-        }, ['pytorch', 'numpy', 'paddle', 'jittor'])
+        'sk_init_tau': [0.5, 0.1],
+        'sk_min_tau': [0.1, 0.05],
+        'param_lambda': [0.1, 0.5],
+        'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn],
+        'verbose': [True]
+    }, backends)
 
     # test with outliers
     _test_mgm_solver_on_isomorphic_graphs(num_graphs, num_nodes, 10, pygm.gamgm, 'kb-qap', {
-            'sk_init_tau': [0.5],
-            'sk_gamma': [0.8],
-            'sk_min_tau': [0.1],
-            'param_lambda': [0.],
-            'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1)],
-            'verbose': [True],
-            'n_univ': [10],
-            'outlier_thresh': [0., 0.1],
-            'ns': [np.array([num_nodes] * (num_graphs // 2) + [num_nodes-1] * (num_graphs - num_graphs // 2))],
-        }, ['pytorch', 'numpy', 'paddle', 'jittor'])
+        'sk_init_tau': [0.5],
+        'sk_gamma': [0.8],
+        'sk_min_tau': [0.1],
+        'param_lambda': [0.],
+        'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1)],
+        'verbose': [True],
+        'n_univ': [10],
+        'outlier_thresh': [0., 0.1],
+        'ns': [np.array([num_nodes] * (num_graphs // 2) + [num_nodes - 1] * (num_graphs - num_graphs // 2))],
+    }, backends)
 
 
 def test_gamgm_backward():
     # Pytorch
     pygm.BACKEND = 'pytorch'
     torch.manual_seed(1)
 
@@ -230,47 +237,49 @@
     acc = matched / X_gt.sum()
 
     # Backward pass via black-box trick
     acc.backward()
     assert torch.sum(W.grad != 0) > 0
 
     # Jittor
-    pygm.BACKEND = 'jittor'
-    jt.set_global_seed(2)
-
-    # Generate 10 isomorphic graphs
-    graph_num = 10
-    As, X_gt, Fs = pygm.utils.generate_isomorphic_graphs(node_num=4, graph_num=10, node_feat_dim=20)
-
-    # Compute node-wise similarity by inner-product and Sinkhorn
-    W = jt.matmul(Fs.unsqueeze(1), Fs.transpose(1, 2).unsqueeze(0))
-    W = pygm.sinkhorn(W.reshape(graph_num ** 2, 4, 4)).reshape(graph_num, graph_num, 4, 4)
-
-    # This function is differentiable by the black-box trick
-    class Model(jt.nn.Module):
-        def __init__(self, W):
-            self.W = W
-        def execute (self, As) :
-            X = pygm.gamgm(As, self.W)
-            return X
-
-    W.start_grad()
-    model = Model(W)
-    X = model(As)
-    matched = 0
-    for i, j in itertools.product(range(graph_num), repeat=2):
-        matched += (X[i,j] * X_gt[i,j]).sum()
-    acc = matched / X_gt.sum()
-
-    # Backward pass via black-box trick
-    optim = jt.nn.SGD(model.parameters(), lr=0.1)
-    optim.step(acc)
-    grad = W.opt_grad(optim)
-    print(jt.sum(grad != 0))
-    assert jt.sum(grad != 0) > 0
+    if os_name == 'Linux':
+        pygm.BACKEND = 'jittor'
+        jt.set_global_seed(2)
+
+        # Generate 10 isomorphic graphs
+        graph_num = 10
+        As, X_gt, Fs = pygm.utils.generate_isomorphic_graphs(node_num=4, graph_num=10, node_feat_dim=20)
+
+        # Compute node-wise similarity by inner-product and Sinkhorn
+        W = jt.matmul(Fs.unsqueeze(1), Fs.transpose(1, 2).unsqueeze(0))
+        W = pygm.sinkhorn(W.reshape(graph_num ** 2, 4, 4)).reshape(graph_num, graph_num, 4, 4)
+
+        # This function is differentiable by the black-box trick
+        class Model(jt.nn.Module):
+            def __init__(self, W):
+                self.W = W
+
+            def execute(self, As):
+                X = pygm.gamgm(As, self.W)
+                return X
+
+        W.start_grad()
+        model = Model(W)
+        X = model(As)
+        matched = 0
+        for i, j in itertools.product(range(graph_num), repeat=2):
+            matched += (X[i, j] * X_gt[i, j]).sum()
+        acc = matched / X_gt.sum()
+
+        # Backward pass via black-box trick
+        optim = jt.nn.SGD(model.parameters(), lr=0.1)
+        optim.step(acc)
+        grad = W.opt_grad(optim)
+        print(jt.sum(grad != 0))
+        assert jt.sum(grad != 0) > 0
 
 
 if __name__ == '__main__':
     test_gamgm_backward()
     test_gamgm()
     test_mgm_floyd()
     test_cao()
```

### Comparing `pygmtools-0.3.6/tests/test_neural_solvers.py` & `pygmtools-0.3.7/tests/test_neural_solvers.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 import torch
 import functools
 import itertools
 from tqdm import tqdm
 
 from test_utils import *
 
+import platform
+os_name = platform.system()
+backends = ['pytorch', 'numpy', 'jittor', 'paddle'] if os_name == 'Linux' else ['pytorch', 'numpy', 'paddle']
+
 
 # The testing function for quadratic assignment
 def _test_neural_solver_on_isomorphic_graphs(graph_num_nodes, node_feat_dim, solver_func, mode, matrix_params, backends):
     if mode == 'lawler-qap':
         assert 'edge_aff_fn' in matrix_params
         assert 'node_aff_fn' in matrix_params
     if backends[0] != 'pytorch':
@@ -131,74 +135,74 @@
                                   f"params: {';'.join([k + '=' + str(v) for k, v in aff_param_dict.items()])};" \
                                   f"{';'.join([k + '=' + str(v) for k, v in solver_param_dict.items()])}"
 
 
 def test_pca_gm():
     _test_neural_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 1024, pygm.pca_gm, 'individual-graphs', {
         'pretrain': ['voc', 'willow', 'voc-all'],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
     # non-batched input
     _test_neural_solver_on_isomorphic_graphs([10], 1024, pygm.pca_gm, 'individual-graphs', {
         'pretrain': ['voc'],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
     # test more layers
     _test_neural_solver_on_isomorphic_graphs([10], 1024, pygm.pca_gm, 'individual-graphs', {
         'num_layers': [3],
         'pretrain': [None],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
 
 def test_ipca_gm():
     _test_neural_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 1024, pygm.ipca_gm, 'individual-graphs', {
         'pretrain': ['voc', 'willow'],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
     # non-batched input
     _test_neural_solver_on_isomorphic_graphs([10], 1024, pygm.ipca_gm, 'individual-graphs', {
         'pretrain': ['voc'],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
     # test more layers
     _test_neural_solver_on_isomorphic_graphs([10], 1024, pygm.ipca_gm, 'individual-graphs', {
         'num_layers': [3],
         'pretrain': [None],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
 
 def test_cie():
     _test_neural_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 1024, pygm.cie, 'individual-graphs-edge', {
             'pretrain': ['voc', 'willow'],
-        }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+        }, backends)
 
     # non-batched input
     _test_neural_solver_on_isomorphic_graphs([10], 1024, pygm.cie, 'individual-graphs-edge', {
         'pretrain': ['voc'],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
     # test more layers
     _test_neural_solver_on_isomorphic_graphs([10], 1024, pygm.cie, 'individual-graphs-edge', {
         'num_layers': [3],
         'pretrain': [None],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
 def test_ngm():
     _test_neural_solver_on_isomorphic_graphs(list(range(10, 30, 2)), 1024, pygm.ngm, 'lawler-qap', {
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.), pygm.utils.inner_prod_aff_fn],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1), pygm.utils.inner_prod_aff_fn],
         'pretrain': ['voc', 'willow'],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
     # non-batched input
     _test_neural_solver_on_isomorphic_graphs([10], 1024, pygm.ngm, 'lawler-qap', {
         'edge_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=1.)],
         'node_aff_fn': [functools.partial(pygm.utils.gaussian_aff_fn, sigma=.1)],
         'pretrain': ['voc'],
-    }, ['pytorch', 'numpy', 'jittor', 'paddle'])
+    }, backends)
 
 
 if __name__ == '__main__':
     test_pca_gm()
     test_ipca_gm()
     test_cie()
     test_ngm()
```

### Comparing `pygmtools-0.3.6/tests/test_utils.py` & `pygmtools-0.3.7/tests/test_utils.py`

 * *Files identical despite different names*

