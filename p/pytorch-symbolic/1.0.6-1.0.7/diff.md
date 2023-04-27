# Comparing `tmp/pytorch-symbolic-1.0.6.tar.gz` & `tmp/pytorch-symbolic-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-symbolic-1.0.6.tar", last modified: Wed Apr 12 21:54:20 2023, max compression
+gzip compressed data, was "pytorch-symbolic-1.0.7.tar", last modified: Thu Apr 27 12:18:57 2023, max compression
```

## Comparing `pytorch-symbolic-1.0.6.tar` & `pytorch-symbolic-1.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1052 2022-10-01 23:42:11.000000 pytorch-symbolic-1.0.6/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1001)     4240 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/README.md
--rw-r--r--   0 gaha      (1000) gaha      (1001)      188 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pyproject.toml
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/pytorch_symbolic/
--rw-r--r--   0 gaha      (1000) gaha      (1001)      580 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     4936 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/code_generator.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)      623 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/config.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     3784 2023-04-12 21:11:23.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/functions_utility.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)    12693 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/graph_algorithms.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1610 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/model_tools.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     2146 2023-04-12 21:33:14.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_api_2.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)    19582 2023-04-12 21:31:41.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_data.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)    14316 2023-04-12 21:34:01.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_model.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     3900 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/useful_layers.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1001)      993 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)        1 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)       48 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)       17 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)      105 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1261 2023-04-12 21:43:05.000000 pytorch-symbolic-1.0.6/setup.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/tests/
--rw-r--r--   0 gaha      (1000) gaha      (1001)     4239 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_add_to_graph.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     8117 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_basic_ops.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     2230 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_examples.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     2269 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_examples_detached.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1751 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_extreme.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     5305 2023-04-12 21:46:38.000000 pytorch-symbolic-1.0.6/tests/test_creating_models.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     3255 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_multi_in_out.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1759 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_docs_automated.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     2887 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_docs_manual.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1365 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_iterating_and_slicing.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1499 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_nontorch_graphs.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1016 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_raising_assertions.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     2428 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_reusing_nodes.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-27 12:18:57.086366 pytorch-symbolic-1.0.7/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1052 2022-10-01 23:42:11.000000 pytorch-symbolic-1.0.7/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2023-04-27 12:18:57.086366 pytorch-symbolic-1.0.7/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     4240 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/README.md
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      188 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/pyproject.toml
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-27 12:18:57.086366 pytorch-symbolic-1.0.7/pytorch_symbolic/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      580 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     4936 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/code_generator.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      623 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/config.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     3784 2023-04-12 21:11:23.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/functions_utility.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)    12693 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/graph_algorithms.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1610 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/model_tools.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2146 2023-04-12 21:33:14.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/symbolic_api_2.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)    19582 2023-04-12 21:31:41.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/symbolic_data.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)    14745 2023-04-27 12:04:39.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/symbolic_model.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     3900 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/pytorch_symbolic/useful_layers.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-27 12:18:57.086366 pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2023-04-27 12:18:57.000000 pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      993 2023-04-27 12:18:57.000000 pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)        1 2023-04-27 12:18:57.000000 pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)       48 2023-04-27 12:18:57.000000 pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)       17 2023-04-27 12:18:57.000000 pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      105 2023-04-27 12:18:57.086366 pytorch-symbolic-1.0.7/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1261 2023-04-27 10:55:14.000000 pytorch-symbolic-1.0.7/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-27 12:18:57.086366 pytorch-symbolic-1.0.7/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     4239 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_add_to_graph.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     8117 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_basic_ops.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2230 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_creating_examples.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2269 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_creating_examples_detached.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1751 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_creating_extreme.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5305 2023-04-12 21:46:38.000000 pytorch-symbolic-1.0.7/tests/test_creating_models.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     3255 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_creating_multi_in_out.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1759 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2887 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_docs_manual.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1365 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_iterating_and_slicing.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1499 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_nontorch_graphs.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1016 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_raising_assertions.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2428 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.7/tests/test_reusing_nodes.py
```

### Comparing `pytorch-symbolic-1.0.6/LICENSE.txt` & `pytorch-symbolic-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/PKG-INFO` & `pytorch-symbolic-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-symbolic
-Version: 1.0.6
+Version: 1.0.7
 Summary: Provides symbolic API for model creation in PyTorch.
 Home-page: https://github.com/gahaalt/pytorch-symbolic.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Project-URL: Documentation, https://pytorch-symbolic.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytorch-symbolic-1.0.6/README.md` & `pytorch-symbolic-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/__init__.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/code_generator.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/code_generator.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/config.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/config.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/functions_utility.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/functions_utility.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/graph_algorithms.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/graph_algorithms.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/model_tools.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/model_tools.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_api_2.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/symbolic_api_2.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_data.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/symbolic_data.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_model.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/symbolic_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -323,21 +323,30 @@
         execution_order_nodes = self._remove_repeated_execution(execution_order_nodes)
 
         self._execution_order_nodes = execution_order_nodes
         self._execution_order_layers = [node.layer for node in self._execution_order_nodes]
 
         for idx, node in enumerate(self._execution_order_nodes):
             if node._custom_provided_name is not None:
+                # Use layer name provided by the user
                 layer_name = node._custom_provided_name
             else:
+                # Extract the default name of the layer provided by pytorch
                 layer_name = node.layer._get_name()
 
+            # Check how many layers with this name already exist
             self._layer_type_counts.setdefault(layer_name, 0)
             self._layer_type_counts[layer_name] += 1
-            full_layer_name = f"{layer_name}_{self._layer_type_counts[layer_name]}"
+
+            if node._custom_provided_name is None or self._layer_type_counts[layer_name] > 1:
+                full_layer_name = f"{layer_name}_{self._layer_type_counts[layer_name]}"
+            else:
+                # Skip first index only if it was provided by the user
+                full_layer_name = layer_name
+
             self._node_to_layer_name[node] = full_layer_name
             self.add_module(name=full_layer_name, module=node.layer)
 
     def __deepcopy__(self, memo):
         """This copies a working Module, but the underlying graph structure is not copied!"""
         obj = self.detach_from_graph()
         memo[id(self)] = obj
```

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic/useful_layers.py` & `pytorch-symbolic-1.0.7/pytorch_symbolic/useful_layers.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/PKG-INFO` & `pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-symbolic
-Version: 1.0.6
+Version: 1.0.7
 Summary: Provides symbolic API for model creation in PyTorch.
 Home-page: https://github.com/gahaalt/pytorch-symbolic.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Project-URL: Documentation, https://pytorch-symbolic.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/SOURCES.txt` & `pytorch-symbolic-1.0.7/pytorch_symbolic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/setup.py` & `pytorch-symbolic-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="UTF-8")
 
 setup(
     name="pytorch-symbolic",
-    version="1.0.6",
+    version="1.0.7",
     url="https://github.com/gahaalt/pytorch-symbolic.git",
     project_urls={
         "Documentation": "https://pytorch-symbolic.readthedocs.io/",
     },
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
```

### Comparing `pytorch-symbolic-1.0.6/tests/test_add_to_graph.py` & `pytorch-symbolic-1.0.7/tests/test_add_to_graph.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_basic_ops.py` & `pytorch-symbolic-1.0.7/tests/test_basic_ops.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_creating_examples.py` & `pytorch-symbolic-1.0.7/tests/test_creating_examples.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_creating_examples_detached.py` & `pytorch-symbolic-1.0.7/tests/test_creating_examples_detached.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_creating_extreme.py` & `pytorch-symbolic-1.0.7/tests/test_creating_extreme.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_creating_models.py` & `pytorch-symbolic-1.0.7/tests/test_creating_models.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_creating_multi_in_out.py` & `pytorch-symbolic-1.0.7/tests/test_creating_multi_in_out.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_docs_automated.py` & `pytorch-symbolic-1.0.7/tests/test_docs_automated.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_docs_manual.py` & `pytorch-symbolic-1.0.7/tests/test_docs_manual.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_iterating_and_slicing.py` & `pytorch-symbolic-1.0.7/tests/test_iterating_and_slicing.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_nontorch_graphs.py` & `pytorch-symbolic-1.0.7/tests/test_nontorch_graphs.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_raising_assertions.py` & `pytorch-symbolic-1.0.7/tests/test_raising_assertions.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.6/tests/test_reusing_nodes.py` & `pytorch-symbolic-1.0.7/tests/test_reusing_nodes.py`

 * *Files identical despite different names*

