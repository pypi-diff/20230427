# Comparing `tmp/inventronet-0.0.2a0.tar.gz` & `tmp/inventronet-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventronet-0.0.2a0.tar", last modified: Mon Apr 24 15:31:13 2023, max compression
+gzip compressed data, was "inventronet-0.0.3a0.tar", last modified: Thu Apr 27 04:00:56 2023, max compression
```

## Comparing `inventronet-0.0.2a0.tar` & `inventronet-0.0.3a0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.560985 inventronet-0.0.2a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 15:31:13.556985 inventronet-0.0.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.548985 inventronet-0.0.2a0/inventronet/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.552985 inventronet-0.0.2a0/inventronet/activations/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/activations/tanh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.552985 inventronet-0.0.2a0/inventronet/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/layers/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/layers/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/layers/shape_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.556985 inventronet-0.0.2a0/inventronet/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/losses/binary_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/losses/categorical_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/losses/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/losses/mean_squared_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.556985 inventronet-0.0.2a0/inventronet/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/metrics/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.556985 inventronet-0.0.2a0/inventronet/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/models/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.556985 inventronet-0.0.2a0/inventronet/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/inventronet/optimizers/stochastic_gradient_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.552985 inventronet-0.0.2a0/inventronet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 15:31:13.000000 inventronet-0.0.2a0/inventronet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-24 15:31:13.000000 inventronet-0.0.2a0/inventronet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:31:13.000000 inventronet-0.0.2a0/inventronet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 15:31:13.000000 inventronet-0.0.2a0/inventronet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 15:31:13.000000 inventronet-0.0.2a0/inventronet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:31:13.560985 inventronet-0.0.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:13.556985 inventronet-0.0.2a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    24097 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-24 15:30:55.000000 inventronet-0.0.2a0/tests/test_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.996132 inventronet-0.0.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-27 04:00:55.996132 inventronet-0.0.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.980132 inventronet-0.0.3a0/inventronet/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.988132 inventronet-0.0.3a0/inventronet/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/activations/tanh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.988132 inventronet-0.0.3a0/inventronet/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/layers/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/layers/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/layers/shape_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.992132 inventronet-0.0.3a0/inventronet/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/losses/binary_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/losses/categorical_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/losses/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/losses/mean_squared_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.992132 inventronet-0.0.3a0/inventronet/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/metrics/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.996132 inventronet-0.0.3a0/inventronet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/models/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.996132 inventronet-0.0.3a0/inventronet/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/inventronet/optimizers/stochastic_gradient_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.984132 inventronet-0.0.3a0/inventronet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-27 04:00:55.000000 inventronet-0.0.3a0/inventronet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-27 04:00:55.000000 inventronet-0.0.3a0/inventronet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 04:00:55.000000 inventronet-0.0.3a0/inventronet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-27 04:00:55.000000 inventronet-0.0.3a0/inventronet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 04:00:55.000000 inventronet-0.0.3a0/inventronet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 04:00:55.996132 inventronet-0.0.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:55.996132 inventronet-0.0.3a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24181 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-27 04:00:41.000000 inventronet-0.0.3a0/tests/test_optimizers.py
```

### Comparing `inventronet-0.0.2a0/LICENSE` & `inventronet-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/PKG-INFO` & `inventronet-0.0.3a0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: inventronet
-Version: 0.0.2a0
-Summary: A package for building and testing neural networks
-Home-page: https://github.com/inventrohyder/inventronet
-Author: inventrohyder
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: lint
-License-File: LICENSE
-
 # inventronet
 
 inventronet is a package for building and testing neural networks in Python. 
 It provides a simple and intuitive API for creating, training, 
 and evaluating various types of neural network models. 
 It also includes some common loss functions, activation functions, 
 and metrics for neural network problems.
@@ -35,52 +19,80 @@
 neural network object. You can then add layers, loss functions, activation 
 functions, and metrics to the network. You can also specify the learning rate, 
 batch size, and number of epochs for training. 
 Here is an example of creating a simple feed forward neural network for a 
 binary classification problem:
 
 ```python
-# Define the number of epochs and the learning rate
+from typing import Tuple
+
+import matplotlib.pyplot as plt
 import numpy as np
-from inventronet.activations import Sigmoid
+
+from inventronet.activations import Sigmoid, ReLU
 from inventronet.layers import Dense
-from inventronet.losses import MSE
+from inventronet.losses import BinaryCrossEntropy as BCE
 from inventronet.metrics import Accuracy, Precision
 from inventronet.models import Sequential
 from inventronet.optimizers import StochasticGradientDescent
 
 
+def plot_history(history):
+    fig, axs = plt.subplots(1, len(history), figsize=(12, 4), sharex=True)
+
+    for idx, (label, values) in enumerate(history.items()):
+        axs[idx].plot(range(1, len(values) + 1), values)
+        axs[idx].set_title(label)
+        axs[idx].set_xlabel("Epoch")
+        axs[idx].set_ylabel(label)
+        axs[idx].grid(True)
+
+    plt.tight_layout()
+    plt.show()
+
 
 epochs = 10000
-learning_rate = 0.1
+
+
+def glorot_uniform(size: Tuple[int, int]) -> np.ndarray:
+    input_dim, output_dim = size
+    limit = np.sqrt(6 / (input_dim + output_dim))
+    return np.random.uniform(low=-limit, high=limit, size=size)
+
 
 # Define the input and output data
 input_data = np.array([[0, 0, 1], [0, 1, 1], [1, 0, 1], [1, 1, 1]])
 output_data = np.array([[0], [1], [1], [0]])
 
 # Define the neural network with two dense layers
 model = Sequential()
-model.add(Dense(input_dim=3, output_dim=4, activation=Sigmoid()))
-model.add(Dense(input_dim=4, output_dim=1, activation=Sigmoid()))
+model.add(Dense(input_dim=3, output_dim=4, activation=ReLU(), weight_initializer=glorot_uniform))
+model.add(Dense(input_dim=4, output_dim=1, activation=Sigmoid(), weight_initializer=glorot_uniform))
 
 # Define the loss function and the metric
-loss = MSE()
-metric = Precision()
+loss = BCE()
+optimizer = StochasticGradientDescent(learning_rate=0.1)
 
-# Compile the model with the loss function, optimizer and the metric
-model.compile(loss, StochasticGradientDescent(), metric)
+# Compile the model with the loss function, optimizer and the metrics
+model.compile(loss, optimizer, metrics=[Precision(), Accuracy()])
+
+# Set early stopping parameters
+model.set_early_stopping(patience=500, min_delta=1e-4)
 
 # Fit the model on the training data
-model.fit(input_data, output_data, epochs, learning_rate)
+model.fit(input_data, output_data, epochs)
 
 # Evaluate the model on the test data
 loss_value, metric_value = model.evaluate(input_data, output_data)
-print(f"Test Loss: {loss_value:.4f}, Test Precision: {metric_value:.4f}")
+print(f"Test Loss: {loss_value:.4f}, Test metrics: {metric_value}")
+
+# Plot the training history
+plot_history(model.history)
 ```
 
 ## Documentation
 
-You can find the full documentation of inventronet at https://inventronet.readthedocs.io/
+You can find the full documentation of inventronet at https://github.com/inventrohyder/inventronet.
 
 ## License
 
-inventronet is licensed under the MIT License. See the LICENSE file for more details.
+inventronet is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `inventronet-0.0.2a0/inventronet/activations/activation.py` & `inventronet-0.0.3a0/inventronet/activations/activation.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/activations/leaky_relu.py` & `inventronet-0.0.3a0/inventronet/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/activations/linear.py` & `inventronet-0.0.3a0/inventronet/activations/linear.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/activations/relu.py` & `inventronet-0.0.3a0/inventronet/activations/relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/activations/sigmoid.py` & `inventronet-0.0.3a0/inventronet/activations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/activations/softmax.py` & `inventronet-0.0.3a0/inventronet/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/activations/tanh.py` & `inventronet-0.0.3a0/inventronet/activations/tanh.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/layers/batch_normalization.py` & `inventronet-0.0.3a0/inventronet/layers/batch_normalization.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,17 @@
             output_dim: The dimension of the output features.
             momentum: The momentum for the moving average of the running
             statistics. Defaults to 0.9.
             epsilon: The small constant for numerical stability.
               Defaults to 1e-5.
         """
         super().__init__(input_dim, output_dim, None)
+        self.normalized_input = None
+        self.batch_var = None
+        self.batch_mean = None
         self.gamma = np.ones((output_dim,))
         self.beta = np.zeros((output_dim,))
         self.running_mean = np.zeros((output_dim,))
         self.running_var = np.ones((output_dim,))
         self.momentum = momentum
         self.epsilon = epsilon
         self.parameters = {"gamma": self.gamma, "beta": self.beta}
@@ -65,35 +68,34 @@
         self.normalized_input = normalized_input
         output = self.gamma * normalized_input + self.beta
         return output
 
     def backward(
         self,
         error: np.ndarray,
-        learning_rate: float,
         prev_output: np.ndarray = None,
-        **kwargs,
+        training: bool = False,
     ) -> np.ndarray:
         """Perform the backward propagation on the layer.
 
         Args:
+            training: A boolean indicating whether the layer is in training
             error: The error array of shape (batch_size, output_dim).
-            learning_rate: The learning rate for the parameter update.
             prev_output: The previous layer output, not used in this layer.
 
         Returns:
             The gradient array of shape (batch_size, input_dim).
         """
         batch_size = error.shape[0]
         grad_gamma = np.sum(error * self.normalized_input, axis=0)
         grad_beta = np.sum(error, axis=0)
-        self.gamma -= learning_rate * grad_gamma
-        self.beta -= learning_rate * grad_beta
+
         self.gradients["gamma"] = grad_gamma
         self.gradients["beta"] = grad_beta
+
         grad_normalized_input = error * self.gamma
         grad_input = (
             batch_size * grad_normalized_input
             - np.sum(grad_normalized_input, axis=0)
             - self.normalized_input
             * np.sum(grad_normalized_input * self.normalized_input, axis=0)
         ) / (batch_size * np.sqrt(self.batch_var + self.epsilon))
```

### Comparing `inventronet-0.0.2a0/inventronet/layers/dropout.py` & `inventronet-0.0.3a0/inventronet/layers/dropout.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         self.dropout_rate: float = dropout_rate
         self.mask: np.ndarray = None
 
     def forward(self, inputs: np.ndarray, training: bool = False) -> np.ndarray:
         """Perform the layer operation on the inputs.
 
         Args:
+            training: A boolean indicating whether the layer is in training
             inputs: The input array of any shape.
 
         Returns:
             The output array of the same shape as the input.
         """
         self.previous_layer_output: np.ndarray = inputs
 
@@ -37,23 +38,23 @@
             return output
         else:
             return inputs
 
     def backward(
         self,
         error: np.ndarray,
-        learning_rate: float,
         prev_output: np.ndarray = None,
         training: bool = False,
     ) -> np.ndarray:
         """Perform the backpropagation on the error.
 
         Args:
+            training:
+            prev_output:
             error: The error array of the same shape as the output.
-            learning_rate: The learning rate for the weight update.
 
         Returns:
             The output error of the same shape as the input.
         """
         if not isinstance(error, np.ndarray):
             raise ValueError("The error must be a numpy array.")
```

### Comparing `inventronet-0.0.2a0/inventronet/layers/layer.py` & `inventronet-0.0.3a0/inventronet/layers/layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 from abc import ABC, abstractmethod
+from typing import Tuple, Type
 
-from typing import Tuple
 import numpy as np
 
 from ..activations.activation import Activation
 
 
 class Layer(ABC):
+
     @abstractmethod
     def __init__(
-        self, input_dim: int, output_dim: int, activation: Activation, **kwargs
+            self,
+            input_dim: int,
+            output_dim: int,
+            activation: Type[Activation],
     ) -> None:
         """Initialize the layer with the given arguments.
 
         Args:
             input_dim: The dimension of the input features.
             output_dim: The dimension of the output features.
             activation: The activation function for the layer.
-            **kwargs: The keyword arguments for the layer.
         """
         self.input_dim: int = input_dim
         self.output_dim: int = output_dim
-        self.activation: Activation = activation
-        self.kwargs = kwargs
+        self.activation: Type[Activation] = activation
         self.parameters = None
         self.gradients = None
 
         self.previous_layer_output = None
 
     @abstractmethod
-    def forward(self, inputs: np.ndarray, **kwargs) -> np.ndarray:
+    def forward(self, inputs: np.ndarray, training: bool = False) -> np.ndarray:
         """Perform the layer operation on the inputs.
 
         Args:
+            training: A boolean indicating whether the layer is in training
             inputs: The input array of shape (batch_size, input_dim).
 
         Returns:
             The output array of shape (batch_size, output_dim).
         """
         raise NotImplementedError("Layer.forward is not implemented.")
 
     @abstractmethod
     def backward(
-        self,
-        grad: np.ndarray,
-        learning_rate: float,
-        prev_output: np.ndarray = None,
-        **kwargs,
+            self,
+            grad: np.ndarray,
+            prev_output: np.ndarray = None,
+            training: bool = False,
     ) -> np.ndarray:
         """Perform the backward propagation on the layer.
 
         Args:
-            error: The error array of shape (batch_size, output_dim).
-            learning_rate: The learning rate for the gradient update.
+            training: A boolean indicating whether the layer is in training
+            grad: The gradient array of shape (batch_size, output_dim).
             prev_output: The previous output array of
                 shape (batch_size, input_dim).
 
         Returns:
             The propagated error array of shape (batch_size, input_dim).
         """
         raise NotImplementedError("Layer.backward is not implemented.")
```

### Comparing `inventronet-0.0.2a0/inventronet/losses/binary_cross_entropy.py` & `inventronet-0.0.3a0/inventronet/losses/binary_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/losses/categorical_cross_entropy.py` & `inventronet-0.0.3a0/inventronet/losses/categorical_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/losses/loss.py` & `inventronet-0.0.3a0/inventronet/losses/loss.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/losses/mean_absolute_error.py` & `inventronet-0.0.3a0/inventronet/losses/mean_absolute_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,9 +51,9 @@
             The derivative of the loss, scaled by the number of samples.
             Shape: (n_samples,)
         """
         # Compute the sign of the error
         sign = np.sign(y_true - y_pred)
         # Compute the derivative of the mean absolute error
         derivative = -sign / y_true.size
-        print("Gradient: {derivative}")
+        print(f"Gradient: {derivative}")
         return derivative
```

### Comparing `inventronet-0.0.2a0/inventronet/losses/mean_squared_error.py` & `inventronet-0.0.3a0/inventronet/losses/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/inventronet/models/model.py` & `inventronet-0.0.3a0/inventronet/models/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Tuple, Type
 
 import numpy as np
 
 from ..layers.layer import Layer
 from ..losses.loss import Loss
 from ..metrics.metric import Metric
+from ..optimizers.optimizer import Optimizer
 
 
 # Define an abstract base class for a model
 class Model(ABC):
     # Define the initialization method
     def __init__(self) -> None:
         """Initialize an empty list of layers."""
@@ -25,40 +26,40 @@
             layer (Layer): The layer to be added.
         """
         raise NotImplementedError("The add method must be implemented.")
 
     # Define an abstract method for compiling the model with a loss
     # function and a metric
     @abstractmethod
-    def compile(self, loss: Loss, metric: Metric) -> None:
+    def compile(
+            self, loss: Loss, optimizer: Optimizer, metrics: List[Type[Metric]]
+    ) -> None:
         """Compile the model with a loss function and a metric.
 
         Args:
             loss (Loss): The loss function to be used.
-            metric (Metric): The metric to be used.
+            optimizer (Optimizer): The optimizer to be used.
+            metrics (Metric): The metrics to be used.
         """
         raise NotImplementedError("The compile method must be implemented.")
 
     # Define an abstract method for fitting the model on training data
     @abstractmethod
     def fit(
-        self,
-        x_train: np.ndarray,
-        y_train: np.ndarray,
-        epochs: int,
-        learning_rate: float,
+            self,
+            x_train: np.ndarray,
+            y_train: np.ndarray,
+            epochs: int,
     ) -> None:
         """Fit the model on training data.
 
         Args:
             x_train (np.ndarray): The input data for training.
             y_train (np.ndarray): The output data for training.
             epochs (int): The number of epochs to train the model.
-            learning_rate (float): The learning rate for updating the
-            weights and biases.
         """
         raise NotImplementedError("The fit method must be implemented.")
 
     # Define an abstract method for predicting the output for new data
     @abstractmethod
     def predict(self, x_test: np.ndarray) -> np.ndarray:
         """Predict the output for new data.
```

### Comparing `inventronet-0.0.2a0/inventronet/models/sequential.py` & `inventronet-0.0.3a0/inventronet/models/sequential.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,47 @@
 # Define a class for a sequential model
 from typing import List, Tuple, Type
+
 import numpy as np
+from tqdm import tqdm
 
-from ..optimizers.optimizer import Optimizer
+from .model import Model
+from ..layers.layer import Layer
 from ..losses.loss import Loss
 from ..metrics.metric import Metric
-from ..layers.layer import Layer
-from .model import Model
+from ..optimizers.optimizer import Optimizer
 
 
 class Sequential(Model):
     # Define the initialization method
     def __init__(self) -> None:
         """Call the superclass constructor."""
         # Call the superclass constructor
         super().__init__()
+        self.metrics: List[Type[Metric]] = None
+        self.optimizer: Type[Optimizer] = None
+        self.loss: Type[Loss] = None
+        # Attributes for early stopping
+        self.patience: int = None
+        self.min_delta: float = None
+        self.wait: int = 0
+        self.best_loss: float = np.inf
+
+        # Attribute for history
+        self.history = {
+            "loss": [],
+        }
+
+    # Add a method to set early stopping parameters
+    def set_early_stopping(self, patience: int, min_delta: float) -> None:
+        self.patience = patience
+        self.min_delta = min_delta
 
     # Define a method for adding a layer to the model
-    def add(self, layer: Layer) -> None:
+    def add(self, layer: Type[Layer]) -> None:
         """Add a layer to the model.
 
         Args:
             layer (Layer): The layer to be added.
 
         Raises:
             AssertionError: If the layer input dimension is not None and
@@ -34,92 +54,116 @@
             # previous layer output dimension
             if layer.input_dim is None:
                 layer.input_dim = previous_layer.output_dim
             # Otherwise, check if the layer input dimension matches the
             # previous layer output dimension
             else:
                 assert (
-                    layer.input_dim == previous_layer.output_dim
+                        layer.input_dim == previous_layer.output_dim
                 ), "Layer input dimension does not match previous layer output dimension"
         # Append the layer to the list of layers
         self.layers.append(layer)
 
     def compile(
-        self, loss: Loss, optimizer: Optimizer, metrics: List[Type[Metric]]
+            self, loss: Type[Loss], optimizer: Type[Optimizer], metrics: List[Type[Metric]]
     ) -> None:
         """Compile the model with a loss function, an optimizer, and metrics.
 
         Args:
             loss (Loss): The loss function to be used.
             optimizer (Optimizer): The optimizer to be used.
             metrics (List[Metric]): The metrics to be used.
         """
         self.loss = loss
         self.optimizer = optimizer
         self.metrics = metrics
+        # Initialize metric history
+        for metric in metrics:
+            self.history[f"{metric.__class__.__name__}"] = []
 
     def fit(
-        self,
-        x_train: np.ndarray,
-        y_train: np.ndarray,
-        epochs: int,
+            self,
+            x_train: np.ndarray,
+            y_train: np.ndarray,
+            epochs: int,
     ) -> None:
         """Fit the model on training data.
 
         Args:
             x_train (np.ndarray): The input data for training.
             y_train (np.ndarray): The output data for training.
             epochs (int): The number of epochs to train the model.
         """
-        for epoch in range(epochs):
+        progress_bar = tqdm(range(epochs), desc="Training progress")
+        for epoch in progress_bar:
             # Forward pass the input data through the network
             layer_output = x_train
             for layer in self.layers:
                 layer_output = layer.forward(layer_output, training=True)
 
             # Calculate the loss and the metrics
             loss_value = self.loss.function(y_train, layer_output)
             metric_values = [
                 metric.call(y_train, layer_output) for metric in self.metrics
             ]
+            # Update the history
+            self.history["loss"].append(loss_value)
+            for metric, m_value in zip(self.metrics, metric_values):
+                self.history[f"{metric.__class__.__name__}"].append(m_value)
 
-            # Print the loss and the metrics
+            # Update the progress bar description with the loss and metrics
             metrics_str = ", ".join(
                 [
                     f"{metric.__class__.__name__}: {m:.4f}"
                     for metric, m in zip(self.metrics, metric_values)
                 ]
             )
-            print(f"Epoch {epoch + 1}, Loss: {loss_value:.4f}, {metrics_str}")
+            progress_bar.set_description(f"Epoch {epoch + 1}, Loss: {loss_value:.4f}, {metrics_str}")
 
             # Backward pass the error through the network
             layer_error = self.loss.gradient(y_train, layer_output)
-            for layer in reversed(self.layers):
+            for layer_index, layer in enumerate(reversed(self.layers)):
                 layer_input = (
                     layer.previous_layer_output
                     if layer.previous_layer_output is not None
                     else x_train
                 )
-                layer_error = layer.backward(
-                    layer_error, self.optimizer.learning_rate, prev_output=layer_input
-                )
-                self.optimizer.update(layer.parameters, layer.gradients)
+                layer_error = layer.backward(layer_error, prev_output=layer_input)
+
+                # Check shapes before updating the optimizer
+                for key in layer.parameters.keys():
+                    assert layer.parameters[key].shape == layer.gradients[
+                        key].shape, f"Parameter shape {layer.parameters[key].shape} does not match gradient shape {layer.gradients[key].shape}"
+
+                self.optimizer.update(len(self.layers) - 1 - layer_index, layer.parameters, layer.gradients)
+
+            # Check for early stopping
+            if self.patience is not None and self.min_delta is not None:
+                if loss_value < self.best_loss - self.min_delta:
+                    self.best_loss = loss_value
+                    self.wait = 0
+                else:
+                    self.wait += 1
+
+                if self.wait >= self.patience:
+                    progress_bar.close()
+                    print(f"Early stopping on epoch {epoch + 1}")
+                    break
 
-    # Define a method for predicting the output for new data
     def predict(self, x_test: np.ndarray) -> np.ndarray:
         # Forward pass the input data through the network
         layer_output = x_test
         for layer in self.layers:
             layer_output = layer.forward(layer_output)
         # Return the final output
         return layer_output
 
     # Define a method for evaluating the model on test data
     def evaluate(
-        self, x_test: np.ndarray, y_test: np.ndarray
+            self, x_test: np.ndarray, y_test: np.ndarray
     ) -> Tuple[float, List[float]]:
         # Predict the output for the test data
         y_pred = self.predict(x_test)
         # Calculate the loss and the metrics
         loss_value = self.loss.function(y_test, y_pred)
         metric_values = [metric.call(y_test, y_pred) for metric in self.metrics]
         # Return the loss and the metrics
```

### Comparing `inventronet-0.0.2a0/inventronet/optimizers/adam.py` & `inventronet-0.0.3a0/inventronet/optimizers/adam.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,28 +10,26 @@
         beta2: float = 0.999,
         epsilon: float = 1e-8,
     ):
         self.learning_rate = learning_rate
         self.beta1 = beta1
         self.beta2 = beta2
         self.epsilon = epsilon
-        self.m = {}
-        self.v = {}
+        self.m = {}  # Initialize m as an empty dictionary
+        self.v = {}  # Initialize v as an empty dictionary
         self.t = 0
 
-    def update(self, params: dict, gradients: dict):
-        if not self.m:
-            self.m = {key: np.zeros_like(value) for key, value in params.items()}
-            self.v = {key: np.zeros_like(value) for key, value in params.items()}
+    def update(self, layer_id: int, params: dict, gradients: dict):
+        if layer_id not in self.m:
+            self.m[layer_id] = {key: np.zeros_like(value) for key, value in params.items()}
+            self.v[layer_id] = {key: np.zeros_like(value) for key, value in params.items()}
 
         self.t += 1
 
         for key in params.keys():
-            self.m[key] = self.beta1 * self.m[key] + (1 - self.beta1) * gradients[key]
-            self.v[key] = self.beta2 * self.v[key] + (1 - self.beta2) * np.square(
-                gradients[key]
-            )
+            self.m[layer_id][key] = self.beta1 * self.m[layer_id][key] + (1 - self.beta1) * gradients[key]
+            self.v[layer_id][key] = self.beta2 * self.v[layer_id][key] + (1 - self.beta2) * np.square(gradients[key])
 
-            m_hat = self.m[key] / (1 - self.beta1**self.t)
-            v_hat = self.v[key] / (1 - self.beta2**self.t)
+            m_hat = self.m[layer_id][key] / (1 - self.beta1 ** self.t)
+            v_hat = self.v[layer_id][key] / (1 - self.beta2 ** self.t)
 
             params[key] -= self.learning_rate * m_hat / (np.sqrt(v_hat) + self.epsilon)
```

### Comparing `inventronet-0.0.2a0/inventronet.egg-info/PKG-INFO` & `inventronet-0.0.3a0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventronet
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: A package for building and testing neural networks
 Home-page: https://github.com/inventrohyder/inventronet
 Author: inventrohyder
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -35,52 +35,80 @@
 neural network object. You can then add layers, loss functions, activation 
 functions, and metrics to the network. You can also specify the learning rate, 
 batch size, and number of epochs for training. 
 Here is an example of creating a simple feed forward neural network for a 
 binary classification problem:
 
 ```python
-# Define the number of epochs and the learning rate
+from typing import Tuple
+
+import matplotlib.pyplot as plt
 import numpy as np
-from inventronet.activations import Sigmoid
+
+from inventronet.activations import Sigmoid, ReLU
 from inventronet.layers import Dense
-from inventronet.losses import MSE
+from inventronet.losses import BinaryCrossEntropy as BCE
 from inventronet.metrics import Accuracy, Precision
 from inventronet.models import Sequential
 from inventronet.optimizers import StochasticGradientDescent
 
 
+def plot_history(history):
+    fig, axs = plt.subplots(1, len(history), figsize=(12, 4), sharex=True)
+
+    for idx, (label, values) in enumerate(history.items()):
+        axs[idx].plot(range(1, len(values) + 1), values)
+        axs[idx].set_title(label)
+        axs[idx].set_xlabel("Epoch")
+        axs[idx].set_ylabel(label)
+        axs[idx].grid(True)
+
+    plt.tight_layout()
+    plt.show()
+
 
 epochs = 10000
-learning_rate = 0.1
+
+
+def glorot_uniform(size: Tuple[int, int]) -> np.ndarray:
+    input_dim, output_dim = size
+    limit = np.sqrt(6 / (input_dim + output_dim))
+    return np.random.uniform(low=-limit, high=limit, size=size)
+
 
 # Define the input and output data
 input_data = np.array([[0, 0, 1], [0, 1, 1], [1, 0, 1], [1, 1, 1]])
 output_data = np.array([[0], [1], [1], [0]])
 
 # Define the neural network with two dense layers
 model = Sequential()
-model.add(Dense(input_dim=3, output_dim=4, activation=Sigmoid()))
-model.add(Dense(input_dim=4, output_dim=1, activation=Sigmoid()))
+model.add(Dense(input_dim=3, output_dim=4, activation=ReLU(), weight_initializer=glorot_uniform))
+model.add(Dense(input_dim=4, output_dim=1, activation=Sigmoid(), weight_initializer=glorot_uniform))
 
 # Define the loss function and the metric
-loss = MSE()
-metric = Precision()
+loss = BCE()
+optimizer = StochasticGradientDescent(learning_rate=0.1)
 
-# Compile the model with the loss function, optimizer and the metric
-model.compile(loss, StochasticGradientDescent(), metric)
+# Compile the model with the loss function, optimizer and the metrics
+model.compile(loss, optimizer, metrics=[Precision(), Accuracy()])
+
+# Set early stopping parameters
+model.set_early_stopping(patience=500, min_delta=1e-4)
 
 # Fit the model on the training data
-model.fit(input_data, output_data, epochs, learning_rate)
+model.fit(input_data, output_data, epochs)
 
 # Evaluate the model on the test data
 loss_value, metric_value = model.evaluate(input_data, output_data)
-print(f"Test Loss: {loss_value:.4f}, Test Precision: {metric_value:.4f}")
+print(f"Test Loss: {loss_value:.4f}, Test metrics: {metric_value}")
+
+# Plot the training history
+plot_history(model.history)
 ```
 
 ## Documentation
 
-You can find the full documentation of inventronet at https://inventronet.readthedocs.io/
+You can find the full documentation of inventronet at https://github.com/inventrohyder/inventronet.
 
 ## License
 
 inventronet is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `inventronet-0.0.2a0/inventronet.egg-info/SOURCES.txt` & `inventronet-0.0.3a0/inventronet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/setup.py` & `inventronet-0.0.3a0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 package_name = "inventronet"
-package_version = "0.0.2-alpha"
+package_version = "0.0.3-alpha"
 package_description = "A package for building and testing neural networks"
 
 # Read the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     package_long_description = f.read()
 
 package_url = "https://github.com/inventrohyder/inventronet"
```

### Comparing `inventronet-0.0.2a0/tests/test_activations.py` & `inventronet-0.0.3a0/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.2a0/tests/test_layers.py` & `inventronet-0.0.3a0/tests/test_layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from typing import Any
+import inspect
+from typing import Any, Type
 import pytest
 
 
 import numpy as np
 from _pytest.capture import CaptureResult
+from _pytest.fixtures import SubRequest
 
 from inventronet.activations import Sigmoid
+from inventronet.activations.activation import Activation
 
 from inventronet.layers import Dense, Dropout, BatchNormalization
 from inventronet.layers.shape_error import ShapeError
 from hypothesis import given, settings, strategies as st
 
+from inventronet.optimizers.optimizer import Optimizer
+import inventronet.optimizers as optimizers_module
+
 
 def generate_random_array(shape):
     return np.random.randn(*shape)
 
 
 @pytest.fixture
 def random_input() -> np.ndarray:
@@ -32,28 +38,44 @@
 
 
 @pytest.fixture
 def random_biases(random_error: np.ndarray) -> np.ndarray:
     yield generate_random_array((random_error.shape[1],)) * 2
 
 
+all_optimizers = [
+    optimizer
+    for _, optimizer in inspect.getmembers(optimizers_module, inspect.isclass)
+    if issubclass(optimizer, Optimizer) and optimizer != Optimizer
+]
+
+
+@pytest.fixture(params=all_optimizers)
+def optimizer(request: SubRequest) -> Type[Optimizer]:
+    opt: Type[Optimizer] = request.param()
+    # Increase the learning rate
+    opt.learning_rate = 0.1
+    yield opt
+
+
+
 @pytest.fixture
-def sigmoid() -> Sigmoid:
+def activation() -> Type[Activation]:
     yield Sigmoid()
 
 
 class TestDense:
     @pytest.fixture
     def dense(
-        self, sigmoid: Sigmoid, input_dim: int, random_error: np.ndarray
+        self, activation: Type[Activation], input_dim: int, random_error: np.ndarray
     ) -> Dense:
         yield Dense(
             input_dim,
             random_error.shape[1],
-            activation=sigmoid,
+            activation=activation,
             use_bias=False,
         )
 
     @pytest.fixture
     def dense_with_bias(self, dense: Dense, random_biases: np.ndarray) -> Dense:
         dense.use_bias = True
         dense.biases = random_biases
@@ -94,43 +116,41 @@
     ):
         """
         Test the differentiability property of the Dense layer. Ensures
         that forward and backward passes can be performed without errors.
         """
         dense.forward(random_input)
         try:
-            dense.backward(random_error, 0.01)
+            dense.backward(random_error)
         except Exception as e:
             pytest.fail(f"Differentiability test failed with exception: {e}")
 
-    def test_weight_updates(
+    def test_weight_gradients(
         self, dense: Dense, random_input: np.ndarray, random_error: np.ndarray
     ):
         """
-        Test the weight update process after a backward pass. Ensures
-        that the Dense layer's weights are updated after backward propagation.
+        Test the weight gradient computation after a backward pass. Ensures
+        that the Dense layer's weight gradients are computed after backward propagation.
         """
-        learning_rate = 0.01
-        original_weights = dense.weights.copy()
         dense.forward(random_input)
-        dense.backward(random_error, learning_rate)
-        assert not np.allclose(dense.weights, original_weights, atol=1e-6)
+        dense.backward(random_error)
+        assert "weights" in dense.gradients
+        assert dense.gradients["weights"].shape == dense.weights.shape
 
-    def test_bias_updates(
+    def test_bias_gradients(
         self, dense_with_bias: Dense, random_input: np.ndarray, random_error: np.ndarray
     ):
         """
-        Test the bias update process after a backward pass. Ensures
-        that the Dense layer's biases are updated after backward propagation.
+        Test the bias gradient computation after a backward pass. Ensures
+        that the Dense layer's bias gradients are computed after backward propagation.
         """
-        learning_rate = 0.01
-        original_biases = dense_with_bias.biases.copy()
         dense_with_bias.forward(random_input)
-        dense_with_bias.backward(random_error, learning_rate)
-        assert not np.allclose(dense_with_bias.biases, original_biases, atol=1e-6)
+        dense_with_bias.backward(random_error)
+        assert "biases" in dense_with_bias.gradients
+        assert dense_with_bias.gradients["biases"].shape == dense_with_bias.biases.shape
 
     class TestDenseInit:
         def test_name(self, dense: Dense):
             assert dense.name == "Dense"
 
         def test_input_shape(self, dense: Dense):
             assert dense.input_shape == (5,)
@@ -153,88 +173,78 @@
         dense_with_bias: Dense,
     ) -> np.ndarray:
         yield dense_with_bias.forward(random_input)
 
     def test_forward(
         self,
         random_input: np.ndarray[Any, np.float64],
-        sigmoid: Sigmoid,
+        activation: Sigmoid,
         forward_output_train: np.ndarray,
         dense: Dense,
     ):
-        expected_output = sigmoid(np.dot(random_input, dense.weights))
+        expected_output = activation(np.dot(random_input, dense.weights))
         assert np.allclose(forward_output_train, expected_output)
 
     def test_forward_invalid_input(
         self, random_input: np.ndarray[Any, np.float64], dense: Dense
     ):
         invalid_input = random_input[:, :4]
         with pytest.raises(ValueError):
             dense.forward(invalid_input)
 
     class TestBackward:
         def test_backward_output(
             self,
             random_error: np.ndarray,
-            sigmoid: Sigmoid,
+            activation: Sigmoid,
             dense: Dense,
             forward_output_train: np.ndarray,
         ):
             expected_output: np.ndarray = np.dot(
-                random_error * sigmoid.derivative(forward_output_train),
+                random_error * activation.derivative(forward_output_train),
                 dense.weights.T,
             )
             # Assert that the output of the backward method is close to the
             # expected output
-            assert np.allclose(
-                dense.backward(random_error, 0.01), expected_output, atol=1e-3
-            )
-
-        def test_backward_update_weights(
-            self,
-            random_input: np.ndarray,
-            random_error: np.ndarray,
-            sigmoid: Sigmoid,
-            dense: Dense,
-            forward_output_train: np.ndarray,
-        ):
-            expected_weights: np.ndarray = dense.weights - 0.01 * np.dot(
-                random_input.T,
-                random_error * sigmoid.derivative(forward_output_train),
-            )
-            assert np.allclose(dense.weights, expected_weights, atol=0.1)
+            assert np.allclose(dense.backward(random_error), expected_output, atol=1e-3)
 
     class TestBackwardUpdateWeightAndBiases:
         def test_updated_weights(
             self,
             random_input: np.ndarray,
             random_error: np.ndarray,
-            sigmoid: Sigmoid,
+            activation: Sigmoid,
             dense_with_bias: Dense,
             forward_output_with_bias: np.ndarray,
+            optimizer: Type[Optimizer],
         ):
             original_weights = dense_with_bias.weights.copy()
-            dense_with_bias.backward(random_error, 0.01)
-            expected_weights: np.ndarray = original_weights - 0.01 * np.dot(
+            dense_with_bias.backward(random_error)
+            optimizer.update(0, dense_with_bias.parameters, dense_with_bias.gradients)
+            learning_rate = optimizer.learning_rate
+            expected_weights: np.ndarray = original_weights - learning_rate * np.dot(
                 random_input.T,
-                random_error * sigmoid.derivative(forward_output_with_bias),
+                random_error * activation.derivative(forward_output_with_bias),
             )
-            assert np.allclose(dense_with_bias.weights, expected_weights, atol=1e-2)
+
+            assert np.allclose(dense_with_bias.weights, expected_weights, atol=1e-1)
 
         def test_updated_biases(
             self,
             random_error: np.ndarray,
-            sigmoid: Sigmoid,
+            activation: Sigmoid,
             dense_with_bias: Dense,
             forward_output_with_bias: np.ndarray,
+            optimizer: Type[Optimizer],
         ):
             original_bias = dense_with_bias.biases.copy()
-            dense_with_bias.backward(random_error, 0.01)
+            dense_with_bias.backward(random_error)
+            optimizer.update(0, dense_with_bias.parameters, dense_with_bias.gradients)
             expected_bias: np.ndarray = original_bias - 0.01 * np.sum(
-                random_error * sigmoid.derivative(forward_output_with_bias), axis=0
+                random_error * activation.derivative(forward_output_with_bias), axis=0
             )
             assert np.allclose(dense_with_bias.biases, expected_bias, atol=1e-2)
 
     @pytest.mark.usefixtures("forward_output_train")
     def test_backward_invalid_error(
         self, random_error: np.ndarray[Any, np.dtype[np.floating[Any]]], dense: Dense
     ):
@@ -294,15 +304,15 @@
     def test_backward(self, dropout_rate: float, input_dim: int, training: bool):
         input_shape = (10, input_dim)
         random_input = generate_random_array(input_shape)
 
         dropout = Dropout(dropout_rate=dropout_rate, input_dim=input_dim)
         output_array = dropout.forward(random_input, training=training)
         error = generate_random_array(output_array.shape)
-        gradient_array = dropout.backward(error, learning_rate=0.01, training=training)
+        gradient_array = dropout.backward(error, training=training)
 
         assert gradient_array.shape == random_input.shape
 
         if training and dropout_rate < 1:
             assert np.allclose(
                 gradient_array, error * dropout.mask / (1 - dropout_rate)
             )
@@ -339,15 +349,15 @@
         random_input = generate_random_array((5, input_dim))
 
         dropout = Dropout(dropout_rate=dropout_rate, input_dim=input_dim)
         dropout.forward(random_input, training=True)
 
         with pytest.raises(ShapeError):
             invalid_error = generate_random_array((2, 3, 4))
-            dropout.backward(invalid_error, learning_rate=0.01, training=training)
+            dropout.backward(invalid_error, training=training)
 
     class TestDroputInit:
         def test_droput_rate(self, dropout: Dropout, dropout_rate: float):
             assert dropout.dropout_rate == dropout_rate
 
         def test_droput_mask(self, dropout: Dropout):
             assert dropout.mask is None
@@ -380,31 +390,27 @@
 
     class TestBackward:
         def test_gradient_shape(
             self, dropout: Dropout, random_input: np.ndarray, training: bool
         ):
             output_array = dropout.forward(random_input, training=training)
             error = np.random.randn(*output_array.shape)
-            gradient_array = dropout.backward(
-                error, learning_rate=0.01, training=training
-            )
+            gradient_array = dropout.backward(error, training=training)
             assert gradient_array.shape == random_input.shape
 
         def test_gradient_value(
             self,
             dropout: Dropout,
             dropout_rate: float,
             random_input: np.ndarray,
             training: bool,
         ):
             output_array = dropout.forward(random_input, training=training)
             error = np.random.randn(*output_array.shape)
-            gradient_array = dropout.backward(
-                error, learning_rate=0.01, training=training
-            )
+            gradient_array = dropout.backward(error, training=training)
             assert np.allclose(
                 gradient_array, error * dropout.mask / (1 - dropout_rate)
             )
 
     @pytest.mark.parametrize("dropout_rate", [0])
     @pytest.mark.parametrize("training", [True])
     def test_dropout_rate_zero_training_true(
@@ -527,20 +533,26 @@
             pytest.fail(f"Differentiability test failed with exception: {e}")
 
     def test_parameter_updates(
         self,
         batch_normalization: BatchNormalization,
         random_input: np.ndarray,
         random_error: np.ndarray,
+        optimizer: Type[Optimizer],
     ):
-        learning_rate = 0.01
         original_gamma = batch_normalization.gamma.copy()
         original_beta = batch_normalization.beta.copy()
+
         batch_normalization.forward(random_input, training=True)
-        batch_normalization.backward(random_error, learning_rate)
+        batch_normalization.backward(random_error)
+
+        optimizer.update(
+            0, batch_normalization.parameters, batch_normalization.gradients
+        )
+
         assert not np.allclose(batch_normalization.gamma, original_gamma, atol=1e-6)
         assert not np.allclose(batch_normalization.beta, original_beta, atol=1e-6)
 
     def test_output_dimension(
         self, batch_normalization: BatchNormalization, random_input: np.ndarray
     ):
         output = batch_normalization.forward(random_input, training=True)
@@ -582,52 +594,43 @@
         def batch_size(self, random_input: np.ndarray) -> int:
             yield random_input.shape[0]
 
         @pytest.fixture
         def gradients(self, random_input: np.ndarray) -> np.ndarray:
             yield np.random.randn(*random_input.shape)
 
-        @pytest.fixture
-        def learning_rate(
-            self,
-        ) -> float:
-            yield 0.01
-
         def test_backward_pass(
             self,
             batch_normalization: BatchNormalization,
             gradients: np.ndarray,
-            learning_rate: float,
             random_input: np.ndarray,
             epsilon: float,
         ) -> None:
             batch_mean = np.mean(random_input, axis=0)
             batch_var = np.var(random_input, axis=0)
             normalized_input = (random_input - batch_mean) / np.sqrt(
                 batch_var + batch_normalization.epsilon
             )
             expected_output = (
                 gradients
                 - np.mean(gradients, axis=0)
                 - normalized_input * np.mean(gradients * normalized_input, axis=0)
             ) / np.sqrt(batch_var + epsilon)
             batch_normalization.forward(random_input, training=True)
-            output = batch_normalization.backward(
-                gradients, learning_rate=learning_rate
-            )
+            output = batch_normalization.backward(gradients)
             assert np.allclose(output, expected_output, rtol=0.1)
 
         def test_backward_gamma_without_activation(
             self,
             batch_normalization: BatchNormalization,
             random_input: np.ndarray,
             gradients: np.ndarray,
         ):
             batch_normalization.forward(random_input, training=True)
-            batch_normalization.backward(gradients, learning_rate=0.01)
+            batch_normalization.backward(gradients)
 
             batch_mean = np.mean(random_input, axis=0)
             batch_var = np.var(random_input, axis=0)
             normalized_input = (random_input - batch_mean) / np.sqrt(
                 batch_var + batch_normalization.epsilon
             )
             expected_gradient_gamma = np.sum(gradients * normalized_input, axis=0)
@@ -638,13 +641,13 @@
         def test_backward_beta_without_activation(
             self,
             batch_normalization: BatchNormalization,
             random_input: np.ndarray,
             gradients: np.ndarray,
         ):
             batch_normalization.forward(random_input, training=True)
-            batch_normalization.backward(gradients, learning_rate=0.01)
+            batch_normalization.backward(gradients)
 
             expected_gradient_beta = np.sum(gradients, axis=0)
             assert np.allclose(
                 batch_normalization.gradients["beta"], expected_gradient_beta
             )
```

### Comparing `inventronet-0.0.2a0/tests/test_loss.py` & `inventronet-0.0.3a0/tests/test_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import pytest
 import numpy as np
+import pytest
+
 from inventronet.losses import (
     BinaryCrossEntropy,
     CategoricalCrossEntropy,
     MeanAbsoluteError,
     MeanSquaredError,
 )
 
@@ -19,17 +20,17 @@
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (np.array([1, 2, 3]), np.array([1, 2, 3]), 0.0),  # exact match
             # one unit difference
             (np.array([1, 2, 3]), np.array([2, 3, 4]), 1.0),
             (
-                np.array([1, 2, 3]),
-                np.array([0, 0, 0]),
-                2,
+                    np.array([1, 2, 3]),
+                    np.array([0, 0, 0]),
+                    2,
             ),  # large difference
         ],
     )
     def test_mae_function(self, y_true, y_pred, expected, mae: MeanAbsoluteError):
         # Compare the expected and actual outputs with a precision of 7
         # decimal places
         np.testing.assert_almost_equal(
@@ -38,27 +39,27 @@
 
     # Test the derivative method of the MAE loss function with different
     # inputs and outputs
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (
-                np.array([1, 2, 3]),
-                np.array([1, 2, 3]),
-                np.array([0, 0, 0]),
+                    np.array([1, 2, 3]),
+                    np.array([1, 2, 3]),
+                    np.array([0, 0, 0]),
             ),  # exact match
             (
-                np.array([1, 2, 3]),
-                np.array([2, 3, 4]),
-                np.array([0.33333333, 0.33333333, 0.33333333]),
+                    np.array([1, 2, 3]),
+                    np.array([2, 3, 4]),
+                    np.array([0.33333333, 0.33333333, 0.33333333]),
             ),  # one unit difference
             (
-                np.array([1, 2, 3]),
-                np.array([0, 0, 0]),
-                np.array([-0.33333333, -0.33333333, -0.33333333]),
+                    np.array([1, 2, 3]),
+                    np.array([0, 0, 0]),
+                    np.array([-0.33333333, -0.33333333, -0.33333333]),
             ),  # large difference
         ],
     )
     def test_mae_derivative(self, y_true, y_pred, expected, mae: MeanAbsoluteError):
         # Compare the expected and actual outputs with a precision of 7
         # decimal places
         np.testing.assert_almost_equal(
@@ -77,17 +78,17 @@
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (np.array([1, 2, 3]), np.array([1, 2, 3]), 0.0),  # exact match
             # one unit difference
             (np.array([1, 2, 3]), np.array([2, 3, 4]), 1.0),
             (
-                np.array([1, 2, 3]),
-                np.array([0, 0, 0]),
-                4.666666666666667,
+                    np.array([1, 2, 3]),
+                    np.array([0, 0, 0]),
+                    4.666666666666667,
             ),  # large difference
         ],
     )
     def test_mse_function(self, y_true, y_pred, expected, mse: MeanSquaredError):
         # Compare the expected and actual outputs with a precision
         # of 7 decimal places
         np.testing.assert_almost_equal(
@@ -96,27 +97,27 @@
 
     # Test the derivative method of the MSE loss function with different
     # inputs and outputs
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (
-                np.array([1, 2, 3]),
-                np.array([1, 2, 3]),
-                np.array([0, 0, 0]),
+                    np.array([1, 2, 3]),
+                    np.array([1, 2, 3]),
+                    np.array([0, 0, 0]),
             ),  # exact match
             (
-                np.array([1, 2, 3]),
-                np.array([2, 3, 4]),
-                np.array([0.66666667, 0.66666667, 0.66666667]),
+                    np.array([1, 2, 3]),
+                    np.array([2, 3, 4]),
+                    np.array([0.66666667, 0.66666667, 0.66666667]),
             ),  # one unit difference
             (
-                np.array([1, 2, 3]),
-                np.array([0, 0, 0]),
-                np.array([-0.66666667, -1.33333333, -2.0]),
+                    np.array([1, 2, 3]),
+                    np.array([0, 0, 0]),
+                    np.array([-0.66666667, -1.33333333, -2.0]),
             ),  # large difference
         ],
     )
     def test_mse_derivative(self, y_true, y_pred, expected, mse: MeanSquaredError):
         # Compare the expected and actual outputs with a precision of
         # 7 decimal places
         np.testing.assert_almost_equal(
@@ -132,27 +133,27 @@
 
     # Test the function method of the BCE loss function with different
     # inputs and outputs
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (
-                np.array([1, 0, 1]),
-                np.array([0.9, 0.1, 0.9]),
-                0.10536052,
+                    np.array([1, 0, 1]),
+                    np.array([0.9, 0.1, 0.9]),
+                    0.10536052,
             ),  # high confidence
             (
-                np.array([1, 0, 1]),
-                np.array([0.6, 0.4, 0.6]),
-                0.51082562,
+                    np.array([1, 0, 1]),
+                    np.array([0.6, 0.4, 0.6]),
+                    0.51082562,
             ),  # medium confidence
             (
-                np.array([1, 0, 1]),
-                np.array([0.5, 0.5, 0.5]),
-                0.69314718,
+                    np.array([1, 0, 1]),
+                    np.array([0.5, 0.5, 0.5]),
+                    0.69314718,
             ),  # low confidence
         ],
     )
     def test_bce_function(self, y_true, y_pred, expected, bce: BinaryCrossEntropy):
         # Compare the expected and actual outputs with a precision o
         # f 7 decimal places
         np.testing.assert_almost_equal(
@@ -161,27 +162,27 @@
 
     # Test the derivative method of the BCE loss function with different
     # inputs and outputs
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (
-                np.array([1, 0, 1]),
-                np.array([0.9, 0.1, 0.9]),
-                np.array([-0.37037037, 0.3703704, -0.37037037]),
+                    np.array([1, 0, 1]),
+                    np.array([0.9, 0.1, 0.9]),
+                    np.array([-0.37037037, 0.3703704, -0.37037037]),
             ),  # high confidence
             (
-                np.array([1, 0, 1]),
-                np.array([0.6, 0.4, 0.6]),
-                np.array([-0.55555556, 0.55555556, -0.55555556]),
+                    np.array([1, 0, 1]),
+                    np.array([0.6, 0.4, 0.6]),
+                    np.array([-0.55555556, 0.55555556, -0.55555556]),
             ),  # medium confidence
             (
-                np.array([1, 0, 1]),
-                np.array([0.5, 0.5, 0.5]),
-                np.array([-0.66666667, 0.66666667, -0.66666667]),
+                    np.array([1, 0, 1]),
+                    np.array([0.5, 0.5, 0.5]),
+                    np.array([-0.66666667, 0.66666667, -0.66666667]),
             ),  # low confidence
         ],
     )
     def test_bce_derivative(self, y_true, y_pred, expected, bce: BinaryCrossEntropy):
         # Compare the expected and actual outputs with a precision of 7
         # decimal places
         np.testing.assert_almost_equal(
@@ -194,61 +195,61 @@
     def cce(self) -> CategoricalCrossEntropy:
         yield CategoricalCrossEntropy()
 
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (
-                np.array([[1, 0], [0, 1], [1, 0]]),
-                np.array([[0.9, 0.1], [0.1, 0.9], [0.9, 0.1]]),
-                0.10536052,
+                    np.array([[1, 0], [0, 1], [1, 0]]),
+                    np.array([[0.9, 0.1], [0.1, 0.9], [0.9, 0.1]]),
+                    0.10536052,
             ),  # high confidence
             (
-                np.array([[1, 0], [0, 1], [1, 0]]),
-                np.array([[0.6, 0.4], [0.4, 0.6], [0.6, 0.4]]),
-                0.51082562,
+                    np.array([[1, 0], [0, 1], [1, 0]]),
+                    np.array([[0.6, 0.4], [0.4, 0.6], [0.6, 0.4]]),
+                    0.51082562,
             ),  # medium confidence
             (
-                np.array([[1, 0], [0, 1], [1, 0]]),
-                np.array([[0.5, 0.5], [0.5, 0.5], [0.5, 0.5]]),
-                0.69314718,
+                    np.array([[1, 0], [0, 1], [1, 0]]),
+                    np.array([[0.5, 0.5], [0.5, 0.5], [0.5, 0.5]]),
+                    0.69314718,
             ),  # low confidence
         ],
     )
     def test_cce_function(self, y_true, y_pred, expected, cce: CategoricalCrossEntropy):
         # Compare the expected and actual outputs with a precision of
         # 7 decimal places
         np.testing.assert_almost_equal(
             cce.function(y_true, y_pred), expected, decimal=7
         )
 
     @pytest.mark.parametrize(
         "y_true, y_pred, expected",
         [
             (
-                np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]]),
-                np.array([[0.9, 0.05, 0.05], [0.05, 0.9, 0.05], [0.05, 0.05, 0.9]]),
-                np.array([[-0.1, 0.05, 0.05], [0.05, -0.1, 0.05], [0.05, 0.05, -0.1]]),
+                    np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]]),
+                    np.array([[0.9, 0.05, 0.05], [0.05, 0.9, 0.05], [0.05, 0.05, 0.9]]),
+                    np.array([[-0.1, 0.05, 0.05], [0.05, -0.1, 0.05], [0.05, 0.05, -0.1]]),
             ),  # high confidence
             (
-                np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]]),
-                np.array([[0.6, 0.2, 0.2], [0.2, 0.6, 0.2], [0.2, 0.2, 0.6]]),
-                np.array([[-0.4, 0.2, 0.2], [0.2, -0.4, 0.2], [0.2, 0.2, -0.4]]),
+                    np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]]),
+                    np.array([[0.6, 0.2, 0.2], [0.2, 0.6, 0.2], [0.2, 0.2, 0.6]]),
+                    np.array([[-0.4, 0.2, 0.2], [0.2, -0.4, 0.2], [0.2, 0.2, -0.4]]),
             ),  # medium confidence
             (
-                np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]]),
-                np.array([[0.33, 0.33, 0.33], [0.33, 0.33, 0.33], [0.33, 0.33, 0.33]]),
-                np.array(
-                    [[-0.67, 0.33, 0.33], [0.33, -0.67, 0.33], [0.33, 0.33, -0.67]]
-                ),
+                    np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]]),
+                    np.array([[0.33, 0.33, 0.33], [0.33, 0.33, 0.33], [0.33, 0.33, 0.33]]),
+                    np.array(
+                        [[-0.67, 0.33, 0.33], [0.33, -0.67, 0.33], [0.33, 0.33, -0.67]]
+                    ),
             ),  # low confidence
         ],
     )
     def test_cce_derivative(
-        self, y_true, y_pred, expected, cce: CategoricalCrossEntropy
+            self, y_true, y_pred, expected, cce: CategoricalCrossEntropy
     ):
         # Compare the expected and actual outputs with a precision of 7
         # decimal places
         np.testing.assert_almost_equal(
             cce.gradient(y_true, y_pred), expected, decimal=7
         )
```

### Comparing `inventronet-0.0.2a0/tests/test_metrics.py` & `inventronet-0.0.3a0/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Import the pytest module and the metric classes
 import numpy as np
 import pytest
 from inventronet.metrics import Accuracy, Precision
 
 
 # Create a fixture to instantiate the metric classes
 @pytest.fixture
```

### Comparing `inventronet-0.0.2a0/tests/test_model.py` & `inventronet-0.0.3a0/tests/test_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,60 @@
+import inspect
 from typing import Type
-import pytest
-import numpy as np
-from inventronet.optimizers import StochasticGradientDescent
-
-from inventronet.optimizers.optimizer import Optimizer
 
+import numpy as np
+import pytest
+from _pytest.fixtures import SubRequest
 
-from inventronet.models import Sequential
+import inventronet.losses as losses_module
+import inventronet.metrics as metrics_module
+import inventronet.optimizers as optimizers_module
 from inventronet.layers import Dense
-from inventronet.losses import MeanSquaredError
 from inventronet.losses.loss import Loss
-from inventronet.metrics import Accuracy
 from inventronet.metrics.metric import Metric
+from inventronet.models import Sequential
+from inventronet.optimizers.optimizer import Optimizer
 
-
-@pytest.fixture
-def loss() -> Type[Loss]:
-    yield MeanSquaredError()
-
-
-@pytest.fixture
-def metric() -> Type[Metric]:
-    yield Accuracy()
-
-
-@pytest.fixture
-def optimizer() -> Type[Optimizer]:
-    yield StochasticGradientDescent()
+# Get all classes in the metrics module that are subclasses of Metric
+all_metrics = [
+    metric
+    for _, metric in inspect.getmembers(metrics_module, inspect.isclass)
+    if issubclass(metric, Metric) and metric != Metric
+]
+
+# Get all classes in the losses module that are subclasses of Loss
+all_losses = [
+    loss
+    for _, loss in inspect.getmembers(losses_module, inspect.isclass)
+    if issubclass(loss, Loss) and loss != Loss
+]
+
+all_optimizers = [
+    optimizer
+    for _, optimizer in inspect.getmembers(optimizers_module, inspect.isclass)
+    if issubclass(optimizer, Optimizer) and optimizer != Optimizer
+]
+
+
+@pytest.fixture(params=all_metrics)
+def metric(request: SubRequest) -> Type[Metric]:
+    yield request.param()
+
+
+@pytest.fixture(params=all_losses)
+def loss(request: SubRequest) -> Type[Loss]:
+    yield request.param()
+
+
+@pytest.fixture(params=all_optimizers)
+def optimizer(request: SubRequest) -> Type[Optimizer]:
+    opt: Type[Optimizer] = request.param()
+    # Increase the learning rate
+    opt.learning_rate = 0.1
+    yield opt
 
 
 @pytest.fixture
 def dummy_sequential_model() -> Sequential:
     """Create a dummy sequential model with two layers"""
     # Create a sequential model
     model = Sequential()
@@ -40,193 +64,221 @@
     model.add(Dense(2, 1))
     # Return the model
     return model
 
 
 @pytest.fixture
 def dummy_compiled_sequential_model(
-    dummy_sequential_model: Sequential,
-    loss: Type[Loss],
-    optimizer: Type[Optimizer],
-    metric: Type[Metric],
+        dummy_sequential_model: Sequential,
+        loss: Type[Loss],
+        optimizer: Type[Optimizer],
+        metric: Type[Metric],
 ) -> Sequential:
     """Compile the sequential model with a loss function, and a metric."""
     dummy_sequential_model.compile(loss, optimizer, [metric])
     # Return the model
     return dummy_sequential_model
 
 
 @pytest.fixture
 def x() -> np.ndarray:
     # Create some dummy input data
-    yield np.array([[0, 0, 1], [0, 1, 1], [1, 0, 1], [1, 1, 1]])
+    yield np.array([[0, 0, 1], [0, 1, 0], [1, 0, 0], [1, 1, 0]])
 
 
 @pytest.fixture
 def y() -> np.ndarray:
     # Create some dummy output data
-    yield np.array([[0], [1], [1], [0]])
+    yield np.array([[0], [0.5], [0.5], [1]])
 
 
 def test_add(dummy_sequential_model: Sequential):
     """Test the add method of the sequential model."""
     # Try to add a layer with input dimension 4 and output dimension 2
     with pytest.raises(AssertionError):
         dummy_sequential_model.add(Dense(4, 2))
     # Check that the model still has two layers
     assert len(dummy_sequential_model.layers) == 2
 
 
 class TestCompile:
-    def test_model_loss_before(self, dummy_sequential_model: Sequential):
-        with pytest.raises(AttributeError):
-            dummy_sequential_model.loss
 
     def test_model_loss(
-        self,
-        dummy_sequential_model: Sequential,
-        loss: Type[Loss],
-        optimizer: Type[Optimizer],
-        metric: Type[Metric],
+            self,
+            dummy_sequential_model: Sequential,
+            loss: Type[Loss],
+            optimizer: Type[Optimizer],
+            metric: Type[Metric],
     ):
         # Compile the model with a loss function and a metric
         dummy_sequential_model.compile(loss, optimizer, [metric])
         # Check that the model has the loss function
         assert dummy_sequential_model.loss == loss
 
     def test_model_metric_before(self, dummy_sequential_model: Sequential):
         with pytest.raises(AttributeError):
             dummy_sequential_model.metric
 
     def test_model_metric(
-        self,
-        dummy_sequential_model: Sequential,
-        loss: Type[Loss],
-        optimizer: Type[Optimizer],
-        metric: Type[Metric],
+            self,
+            dummy_sequential_model: Sequential,
+            loss: Type[Loss],
+            optimizer: Type[Optimizer],
+            metric: Type[Metric],
     ):
         # Compile the model with a loss function and a metric
         dummy_sequential_model.compile(loss, optimizer, [metric])
         # Check that the model has the metrics
         assert dummy_sequential_model.metrics == [metric]
 
 
 class TestFit:
-    class TestFitUpdatesWeightsAndBiases:
-        def test_layer_1_weights(
+    def test_fit_history_is_dict(
+            self,
+            dummy_compiled_sequential_model: Sequential,
+            x: np.ndarray,
+            y: np.ndarray,
+    ):
+        dummy_compiled_sequential_model.fit(x, y, 5)
+        history = dummy_compiled_sequential_model.history
+        assert isinstance(history, dict)
+
+    def test_fit_history_has_loss_and_metric(
+            self,
+            dummy_compiled_sequential_model: Sequential,
+            x: np.ndarray,
+            y: np.ndarray,
+    ):
+        dummy_compiled_sequential_model.fit(x, y, 5)
+        history = dummy_compiled_sequential_model.history
+        metric_class_name = dummy_compiled_sequential_model.metrics[0].__class__.__name__
+        assert "loss" in history and metric_class_name in history.keys()
+
+    def test_fit_history_correct_length(
             self,
             dummy_compiled_sequential_model: Sequential,
             x: np.ndarray,
             y: np.ndarray,
+    ):
+        dummy_compiled_sequential_model.fit(x, y, 5)
+        history = dummy_compiled_sequential_model.history
+        assert len(history["loss"]) == 5 and all(len(history[key]) == 5 for key in history.keys() if "metric" in key)
+
+    def test_fit_history_values_are_floats(
+            self,
+            dummy_compiled_sequential_model: Sequential,
+            x: np.ndarray,
+            y: np.ndarray,
+    ):
+        dummy_compiled_sequential_model.fit(x, y, 5)
+        history = dummy_compiled_sequential_model.history
+        assert all(isinstance(value, float) for value in history["loss"]) and all(
+            all(isinstance(value, float) for value in history[key]) for key in history.keys() if "metric" in key)
+
+    def test_fit_history_metric_increases(
+            self,
+            dummy_compiled_sequential_model: Sequential,
+            x: np.ndarray,
+            y: np.ndarray,
+    ):
+        dummy_compiled_sequential_model.fit(x, y, 5)
+        history = dummy_compiled_sequential_model.history
+        for key in history.keys():
+            if "metric" in key:
+                assert all(
+                    history[key][i] <= history[key][i + 1] for i in range(len(history[key]) - 1)
+                )
+
+    class TestFitUpdatesWeightsAndBiases:
+        def test_layer_1_weights(
+                self,
+                dummy_compiled_sequential_model: Sequential,
+                x: np.ndarray,
+                y: np.ndarray,
         ):
             # Get the initial weights and biases of the layers
             w1, _ = dummy_compiled_sequential_model.layers[0].get_parameters()
+            print("Initial weights:", w1)
+
             # Fit the model for one epoch
             dummy_compiled_sequential_model.fit(x, y, 1)
+
             # Get the updated weights and biases of the layers
             w1_new, _ = dummy_compiled_sequential_model.layers[0].get_parameters()
+            print("Updated weights:", w1_new)
+
             # Check that the weights have changed
             assert not np.array_equal(w1, w1_new)
 
         def test_layer_1_biases(
-            self,
-            dummy_compiled_sequential_model: Sequential,
-            x: np.ndarray,
-            y: np.ndarray,
+                self,
+                dummy_compiled_sequential_model: Sequential,
+                x: np.ndarray,
+                y: np.ndarray,
         ):
             # Get the initial weights and biases of the layers
             _, b1 = dummy_compiled_sequential_model.layers[0].get_parameters()
             # Fit the model for one epoch
             dummy_compiled_sequential_model.fit(x, y, 1)
             # Get the updated weights and biases of the layers
             _, b1_new = dummy_compiled_sequential_model.layers[0].get_parameters()
             # Check that the biases have changed
             assert not np.array_equal(b1, b1_new)
 
         def test_layer_2_weights(
-            self,
-            dummy_compiled_sequential_model: Sequential,
-            x: np.ndarray,
-            y: np.ndarray,
+                self,
+                dummy_compiled_sequential_model: Sequential,
+                x: np.ndarray,
+                y: np.ndarray,
         ):
             # Get the initial weights and biases of the layers
             w2, _ = dummy_compiled_sequential_model.layers[1].get_parameters()
             # Fit the model for one epoch
             dummy_compiled_sequential_model.fit(x, y, 1)
             # Get the updated weights and biases of the layers
             w2_new, _ = dummy_compiled_sequential_model.layers[1].get_parameters()
             # Check that the weights have changed
             assert not np.array_equal(w2, w2_new)
 
         def test_layer_2_biases(
-            self,
-            dummy_compiled_sequential_model: Sequential,
-            x: np.ndarray,
-            y: np.ndarray,
+                self,
+                dummy_compiled_sequential_model: Sequential,
+                x: np.ndarray,
+                y: np.ndarray,
         ):
             # Get the initial weights and biases of the layers
             _, b2 = dummy_compiled_sequential_model.layers[1].get_parameters()
             # Fit the model for one epoch
             dummy_compiled_sequential_model.fit(x, y, 1)
             # Get the updated weights and biases of the layers
             _, b2_new = dummy_compiled_sequential_model.layers[1].get_parameters()
             # Check that the biases have changed
             assert not np.array_equal(b2, b2_new)
 
-    def test_fit_prints_loss(
-        self,
-        dummy_compiled_sequential_model: Sequential,
-        capsys: pytest.CaptureFixture,
-        x: np.ndarray,
-        y: np.ndarray,
-    ):
-        # Fit the model for one epoch
-        dummy_compiled_sequential_model.fit(x, y, 1)
-        # Capture the standard output
-        captured = capsys.readouterr()
-        # Check that the loss value is printed
-        assert "Loss" in captured.out
-
-    def test_fit_prints_metric(
-        self,
-        dummy_compiled_sequential_model: Sequential,
-        capsys: pytest.CaptureFixture,
-        x: np.ndarray,
-        y: np.ndarray,
-        metric: Type[Metric],
-    ):
-        """Test the fit method prints the metric value."""
-        # Fit the model for one epoch
-        dummy_compiled_sequential_model.fit(x, y, 1)
-        # Capture the standard output
-        captured = capsys.readouterr()
-        # Check that the metric value is printed
-        assert f"{metric.__class__.__name__}" in captured.out
-
 
 class TestSequentialModelProperties:
     def test_layers_property(self, dummy_sequential_model: Sequential):
         assert hasattr(dummy_sequential_model, "layers")
         assert len(dummy_sequential_model.layers) == 2
         assert all(isinstance(layer, Dense) for layer in dummy_sequential_model.layers)
 
     def test_loss_property(
-        self, dummy_compiled_sequential_model: Sequential, loss: Type[Loss]
+            self, dummy_compiled_sequential_model: Sequential, loss: Type[Loss]
     ):
         assert hasattr(dummy_compiled_sequential_model, "loss")
         assert dummy_compiled_sequential_model.loss == loss
 
     def test_optimizer_property(
-        self, dummy_compiled_sequential_model: Sequential, optimizer: Type[Optimizer]
+            self, dummy_compiled_sequential_model: Sequential, optimizer: Type[Optimizer]
     ):
         assert hasattr(dummy_compiled_sequential_model, "optimizer")
         assert dummy_compiled_sequential_model.optimizer == optimizer
 
     def test_metrics_property(
-        self, dummy_compiled_sequential_model: Sequential, metric: Type[Metric]
+            self, dummy_compiled_sequential_model: Sequential, metric: Type[Metric]
     ):
         assert hasattr(dummy_compiled_sequential_model, "metrics")
         assert len(dummy_compiled_sequential_model.metrics) == 1
         assert dummy_compiled_sequential_model.metrics == [metric]
 
 
 def test_layer_compatibility(dummy_sequential_model: Sequential):
@@ -242,50 +294,39 @@
     assert isinstance(first_layer, Dense)
     assert isinstance(second_layer, Dense)
 
     assert first_layer.output_dim == 2
     assert second_layer.input_dim == 2
 
 
-def test_model_compilation(dummy_sequential_model: Sequential):
-    with pytest.raises(AttributeError):
-        dummy_sequential_model.loss
-
-    with pytest.raises(AttributeError):
-        dummy_sequential_model.optimizer
-
-    with pytest.raises(AttributeError):
-        dummy_sequential_model.metrics
-
-
 class TestPredict:
     def test_predict_output_shape(
-        self, dummy_compiled_sequential_model: Sequential, x: np.ndarray
+            self, dummy_compiled_sequential_model: Sequential, x: np.ndarray
     ):
         predictions = dummy_compiled_sequential_model.predict(x)
         assert predictions.shape == (x.shape[0], 1)
 
     def test_predict_output_values(
-        self, dummy_compiled_sequential_model: Sequential, x: np.ndarray
+            self, dummy_compiled_sequential_model: Sequential, x: np.ndarray
     ):
         predictions = dummy_compiled_sequential_model.predict(x)
         assert np.all((predictions >= 0) & (predictions <= 1))
 
 
 class TestEvaluate:
     def test_evaluate_loss(
-        self,
-        dummy_compiled_sequential_model: Sequential,
-        x: np.ndarray,
-        y: np.ndarray,
+            self,
+            dummy_compiled_sequential_model: Sequential,
+            x: np.ndarray,
+            y: np.ndarray,
     ):
         loss_value, _ = dummy_compiled_sequential_model.evaluate(x, y)
         assert isinstance(loss_value, float)
 
     def test_evaluate_metric(
-        self,
-        dummy_compiled_sequential_model: Sequential,
-        x: np.ndarray,
-        y: np.ndarray,
+            self,
+            dummy_compiled_sequential_model: Sequential,
+            x: np.ndarray,
+            y: np.ndarray,
     ):
         _, metric_value = dummy_compiled_sequential_model.evaluate(x, y)
         assert isinstance(metric_value, list)
```

