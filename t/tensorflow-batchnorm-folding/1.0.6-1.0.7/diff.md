# Comparing `tmp/tensorflow_batchnorm_folding-1.0.6.tar.gz` & `tmp/tensorflow_batchnorm_folding-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow_batchnorm_folding-1.0.6.tar", last modified: Thu Feb  9 16:48:38 2023, max compression
+gzip compressed data, was "tensorflow_batchnorm_folding-1.0.7.tar", last modified: Thu Apr 27 11:40:22 2023, max compression
```

## Comparing `tensorflow_batchnorm_folding-1.0.6.tar` & `tensorflow_batchnorm_folding-1.0.7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:48:38.700390 tensorflow_batchnorm_folding-1.0.6/
--rw-r--r--   0 edouard   (1000) edouard   (1000)     1070 2023-02-09 16:45:04.000000 tensorflow_batchnorm_folding-1.0.6/LICENSE
--rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-02-09 16:48:38.700390 tensorflow_batchnorm_folding-1.0.6/PKG-INFO
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3431 2023-02-09 16:45:04.000000 tensorflow_batchnorm_folding-1.0.6/README.md
--rw-r--r--   0 edouard   (1000) edouard   (1000)      540 2023-02-09 16:45:04.000000 tensorflow_batchnorm_folding-1.0.6/pyproject.toml
--rw-r--r--   0 edouard   (1000) edouard   (1000)      676 2023-02-09 16:48:38.700390 tensorflow_batchnorm_folding-1.0.6/setup.cfg
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:48:38.696390 tensorflow_batchnorm_folding-1.0.6/src/
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:48:38.696390 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:48:38.700390 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/
--rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/__init__.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     7430 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/add_biases.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      975 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/back_forth.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     9106 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/calculus.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     6210 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/concat_handler.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      500 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/deep_copy.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      879 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/graph_modif.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3146 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/graph_path.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     2289 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/lambda_layers.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3260 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/modify_bn_graph.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     5230 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/package.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3440 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     4429 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     8792 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/update_fold_weights.py
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:48:38.700390 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/UnitTest/
--rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/UnitTest/__init__.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      838 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/UnitTest/test_a_model.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/__init__.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     5369 2023-02-09 16:45:05.000000 tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/folder.py
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:48:38.700390 tensorflow_batchnorm_folding-1.0.6/src/tensorflow_batchnorm_folding.egg-info/
--rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-02-09 16:48:38.000000 tensorflow_batchnorm_folding-1.0.6/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO
--rw-rw-r--   0 edouard   (1000) edouard   (1000)     1309 2023-02-09 16:48:38.000000 tensorflow_batchnorm_folding-1.0.6/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt
--rw-rw-r--   0 edouard   (1000) edouard   (1000)        1 2023-02-09 16:48:38.000000 tensorflow_batchnorm_folding-1.0.6/src/tensorflow_batchnorm_folding.egg-info/dependency_links.txt
--rw-rw-r--   0 edouard   (1000) edouard   (1000)       28 2023-02-09 16:48:38.000000 tensorflow_batchnorm_folding-1.0.6/src/tensorflow_batchnorm_folding.egg-info/top_level.txt
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-02-09 16:48:38.700390 tensorflow_batchnorm_folding-1.0.6/tests/
--rw-r--r--   0 edouard   (1000) edouard   (1000)    26535 2023-02-09 16:45:04.000000 tensorflow_batchnorm_folding-1.0.6/tests/test_calculus.py
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.273687 tensorflow_batchnorm_folding-1.0.7/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     1070 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/LICENSE
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-04-27 11:40:22.273687 tensorflow_batchnorm_folding-1.0.7/PKG-INFO
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     3431 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/README.md
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      609 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/pyproject.toml
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      676 2023-04-27 11:40:22.273687 tensorflow_batchnorm_folding-1.0.7/setup.cfg
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/__init__.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     7430 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/add_biases.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      975 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/back_forth.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     9106 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/calculus.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     6210 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/concat_handler.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      500 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/deep_copy.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      879 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_modif.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     3146 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_path.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     2289 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/lambda_layers.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     3212 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/modify_bn_graph.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     5252 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/package.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     3440 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     4429 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     8792 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/update_fold_weights.py
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/__init__.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      838 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/test_a_model.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/__init__.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     5369 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/folder.py
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)     1364 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)        1 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/dependency_links.txt
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)       41 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/requires.txt
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)       28 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/top_level.txt
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/tests/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)    26535 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/tests/test_calculus.py
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/LICENSE` & `tensorflow_batchnorm_folding-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/PKG-INFO` & `tensorflow_batchnorm_folding-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow_batchnorm_folding
-Version: 1.0.6
+Version: 1.0.7
 Summary: Folds BN layers in tf keras models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Edouard Yvinec
 Author-email: Edouard Yvinec <ey@datakalab.com>
 License: MIT License
         
         Copyright (c) 2022 Edouard Yvinec
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/README.md` & `tensorflow_batchnorm_folding-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/pyproject.toml` & `tensorflow_batchnorm_folding-1.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "tensorflow_batchnorm_folding"
-version = "1.0.6"
+version = "1.0.7"
 description = "Folds BN layers in tf keras models."
 authors = [
     {name = "Edouard Yvinec", email="ey@datakalab.com"}
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
+dependencies = [
+  "tensorflow >= 2.9.0", "scikit-network>=0.26.0"
+]
 
 [project.urls]
 documentation = "https://www.ijcai.org/proceedings/2022/0223.pdf"
 
 [build-system]
-requires = ["setuptools>=42", "tensorflow >= 2.8.0", "scikit-network>=0.26.0"]
+requires = ["setuptools>=42", "tensorflow >= 2.9.0", "scikit-network>=0.26.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/setup.cfg` & `tensorflow_batchnorm_folding-1.0.7/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensorflow_batchnorm_folding
-version = 1.0.6
+version = 1.0.7
 author = Edouard Yvinec
 author_email = ey@datakalab.com
 description = automatic batch-normalization layer folding for tf.keras models
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls = 
@@ -14,15 +14,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/add_biases.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/add_biases.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/back_forth.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/back_forth.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/calculus.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/calculus.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/concat_handler.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/concat_handler.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/graph_modif.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_modif.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/graph_path.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_path.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/lambda_layers.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/lambda_layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/modify_bn_graph.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/modify_bn_graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,49 +27,48 @@
             intermediate_outputs[layer.name] = x
         else:
             if (
                 len(network_dict["input_layers_of"][layer.name]) == 1
                 or isinstance(layer, tf.keras.layers.Lambda)
                 or "tfoplambda" in type(layer).__name__.lower()
             ):
+                copied_layer = type(layer).from_config(layer.get_config())
+                if "weights" in dir(copied_layer):
+                    copied_layer.set_weights(layer.get_weights())
                 x = call_lambda_layer(
-                    layer_input=layer_input, model=model, layer=layer, layer_cpt=cpt + 1
+                    layer_input=layer_input,
+                    model=model,
+                    layer=copied_layer,
+                    layer_cpt=cpt + 1,
                 )
                 intermediate_outputs[layer.name] = x
             else:
                 if (
                     isinstance(layer, tf.keras.layers.Add)
                     or isinstance(layer, tf.keras.layers.Multiply)
                     or isinstance(layer, (tf.keras.layers.Concatenate))
                 ):
-                    x = layer(
+                    copied_layer = type(layer).from_config(layer.get_config())
+                    x = copied_layer(
                         [
                             intermediate_outputs[elem]
                             for elem in network_dict["input_layers_of"][layer.name]
                         ]
                     )
                 else:
-                    x = layer(
+                    x = copied_layer(
                         intermediate_outputs[
                             network_dict["input_layers_of"][layer.name][0]
                         ],
                         intermediate_outputs[
                             network_dict["input_layers_of"][layer.name][1]
                         ],
                     )
                 intermediate_outputs[layer.name] = x
         network_dict["new_output_tensor_of"].update({layer.name: x})
         if layer.name in model.output_names:
             model_outputs.append(x)
-    if len(model_outputs)==0:
-        model_outputs=model_outputs[0]
+    if len(model_outputs) == 0:
+        model_outputs = model_outputs[0]
     output_model = tf.keras.Model(inputs=model.inputs, outputs=model_outputs)
-    for layer in output_model.layers:
-        for node in layer._outbound_nodes:
-            layer_name = node.outbound_layer.name
-            if layer_name in fold_dict:
-                layer._outbound_nodes.remove(node)
-                if "_outbound_nodes_value" in dir(layer):
-                    if node in layer._outbound_nodes_value:
-                        layer._outbound_nodes_value.remove(node)
     output_model._name = model.name
     return output_model
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/package.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/package.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,16 @@
                 return True
     return False
 
 
 def check_packages(verbose: bool = False):
     global PACKAGES_HAVE_BEEN_CHECKED
     if not PACKAGES_HAVE_BEEN_CHECKED:
-        print()
+        if verbose:
+            print()
 
         check_python(verbose=verbose)
         module_v_int = []
         module_v_str = []
         pip_commands = [
             "pip install --upgrade tensorflow",
             "pip install scikit-network",
@@ -88,15 +89,15 @@
                 module_v_int.append([int(e) for e in module_version.split(".")])
 
         pip_commands_to_run = []
         column_0 = ["package"]
         column_1 = ["current version"]
         column_2 = ["recommended version"]
         column_3 = ["checks"]
-        for (version, v_str, reco_version, pip_command, name) in zip(
+        for version, v_str, reco_version, pip_command, name in zip(
             module_v_int,
             module_v_str,
             recommended_version,
             pip_commands,
             packages_to_check,
         ):
             if compare_versions(version, reco_version):
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/TensorFlow/update_fold_weights.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/update_fold_weights.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/UnitTest/test_a_model.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/test_a_model.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/batch_normalization_folding/folder.py` & `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/folder.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO` & `tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-batchnorm-folding
-Version: 1.0.6
+Version: 1.0.7
 Summary: Folds BN layers in tf keras models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Edouard Yvinec
 Author-email: Edouard Yvinec <ey@datakalab.com>
 License: MIT License
         
         Copyright (c) 2022 Edouard Yvinec
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt` & `tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,9 +19,10 @@
 src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py
 src/batch_normalization_folding/TensorFlow/update_fold_weights.py
 src/batch_normalization_folding/UnitTest/__init__.py
 src/batch_normalization_folding/UnitTest/test_a_model.py
 src/tensorflow_batchnorm_folding.egg-info/PKG-INFO
 src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt
 src/tensorflow_batchnorm_folding.egg-info/dependency_links.txt
+src/tensorflow_batchnorm_folding.egg-info/requires.txt
 src/tensorflow_batchnorm_folding.egg-info/top_level.txt
 tests/test_calculus.py
```

### Comparing `tensorflow_batchnorm_folding-1.0.6/tests/test_calculus.py` & `tensorflow_batchnorm_folding-1.0.7/tests/test_calculus.py`

 * *Files identical despite different names*

