# Comparing `tmp/tensorflow_batchnorm_folding-1.0.7.tar.gz` & `tmp/tensorflow_batchnorm_folding-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow_batchnorm_folding-1.0.7.tar", last modified: Thu Apr 27 11:40:22 2023, max compression
+gzip compressed data, was "tensorflow_batchnorm_folding-1.0.8.tar", last modified: Thu Apr 27 12:12:11 2023, max compression
```

## Comparing `tensorflow_batchnorm_folding-1.0.7.tar` & `tensorflow_batchnorm_folding-1.0.8.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.273687 tensorflow_batchnorm_folding-1.0.7/
--rw-r--r--   0 edouard   (1000) edouard   (1000)     1070 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/LICENSE
--rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-04-27 11:40:22.273687 tensorflow_batchnorm_folding-1.0.7/PKG-INFO
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3431 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/README.md
--rw-r--r--   0 edouard   (1000) edouard   (1000)      609 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/pyproject.toml
--rw-r--r--   0 edouard   (1000) edouard   (1000)      676 2023-04-27 11:40:22.273687 tensorflow_batchnorm_folding-1.0.7/setup.cfg
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/
--rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/__init__.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     7430 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/add_biases.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      975 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/back_forth.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     9106 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/calculus.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     6210 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/concat_handler.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      500 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/deep_copy.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      879 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_modif.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3146 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_path.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     2289 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/lambda_layers.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3212 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/modify_bn_graph.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     5252 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/package.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     3440 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     4429 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     8792 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/update_fold_weights.py
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/
--rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/__init__.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)      838 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/test_a_model.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/__init__.py
--rw-r--r--   0 edouard   (1000) edouard   (1000)     5369 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/folder.py
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/
--rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO
--rw-rw-r--   0 edouard   (1000) edouard   (1000)     1364 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt
--rw-rw-r--   0 edouard   (1000) edouard   (1000)        1 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/dependency_links.txt
--rw-rw-r--   0 edouard   (1000) edouard   (1000)       41 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/requires.txt
--rw-rw-r--   0 edouard   (1000) edouard   (1000)       28 2023-04-27 11:40:22.000000 tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/top_level.txt
-drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 11:40:22.269687 tensorflow_batchnorm_folding-1.0.7/tests/
--rw-r--r--   0 edouard   (1000) edouard   (1000)    26535 2023-04-27 11:39:33.000000 tensorflow_batchnorm_folding-1.0.7/tests/test_calculus.py
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:12:11.480616 tensorflow_batchnorm_folding-1.0.8/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     1070 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/LICENSE
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-04-27 12:12:11.480616 tensorflow_batchnorm_folding-1.0.8/PKG-INFO
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     3431 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/README.md
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      540 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/pyproject.toml
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      676 2023-04-27 12:12:11.480616 tensorflow_batchnorm_folding-1.0.8/setup.cfg
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:12:11.476616 tensorflow_batchnorm_folding-1.0.8/src/
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:12:11.476616 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:12:11.480616 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/__init__.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     7430 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/add_biases.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      975 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/back_forth.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     9106 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/calculus.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     6210 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/concat_handler.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      500 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/deep_copy.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      879 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/graph_modif.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     3146 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/graph_path.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     2289 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/lambda_layers.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     4330 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/modify_bn_graph.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     5252 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/package.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     3440 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     4429 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     8792 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/update_fold_weights.py
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:12:11.480616 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/UnitTest/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/UnitTest/__init__.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)      838 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/UnitTest/test_a_model.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/__init__.py
+-rw-r--r--   0 edouard   (1000) edouard   (1000)     5369 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/folder.py
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:12:11.480616 tensorflow_batchnorm_folding-1.0.8/src/tensorflow_batchnorm_folding.egg-info/
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)     5118 2023-04-27 12:12:11.000000 tensorflow_batchnorm_folding-1.0.8/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)     1309 2023-04-27 12:12:11.000000 tensorflow_batchnorm_folding-1.0.8/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)        1 2023-04-27 12:12:11.000000 tensorflow_batchnorm_folding-1.0.8/src/tensorflow_batchnorm_folding.egg-info/dependency_links.txt
+-rw-rw-r--   0 edouard   (1000) edouard   (1000)       28 2023-04-27 12:12:11.000000 tensorflow_batchnorm_folding-1.0.8/src/tensorflow_batchnorm_folding.egg-info/top_level.txt
+drwxrwxr-x   0 edouard   (1000) edouard   (1000)        0 2023-04-27 12:12:11.480616 tensorflow_batchnorm_folding-1.0.8/tests/
+-rw-r--r--   0 edouard   (1000) edouard   (1000)    26535 2023-04-27 12:11:32.000000 tensorflow_batchnorm_folding-1.0.8/tests/test_calculus.py
```

### Comparing `tensorflow_batchnorm_folding-1.0.7/LICENSE` & `tensorflow_batchnorm_folding-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/PKG-INFO` & `tensorflow_batchnorm_folding-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow_batchnorm_folding
-Version: 1.0.7
+Version: 1.0.8
 Summary: Folds BN layers in tf keras models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Edouard Yvinec
 Author-email: Edouard Yvinec <ey@datakalab.com>
 License: MIT License
         
         Copyright (c) 2022 Edouard Yvinec
```

### Comparing `tensorflow_batchnorm_folding-1.0.7/README.md` & `tensorflow_batchnorm_folding-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/pyproject.toml` & `tensorflow_batchnorm_folding-1.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 [project]
 name = "tensorflow_batchnorm_folding"
-version = "1.0.7"
+version = "1.0.8"
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
-dependencies = [
-  "tensorflow >= 2.9.0", "scikit-network>=0.26.0"
-]
 
 [project.urls]
 documentation = "https://www.ijcai.org/proceedings/2022/0223.pdf"
 
 [build-system]
 requires = ["setuptools>=42", "tensorflow >= 2.9.0", "scikit-network>=0.26.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `tensorflow_batchnorm_folding-1.0.7/setup.cfg` & `tensorflow_batchnorm_folding-1.0.8/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensorflow_batchnorm_folding
-version = 1.0.7
+version = 1.0.8
 author = Edouard Yvinec
 author_email = ey@datakalab.com
 description = automatic batch-normalization layer folding for tf.keras models
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/add_biases.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/add_biases.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/back_forth.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/back_forth.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/calculus.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/calculus.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/concat_handler.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/concat_handler.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_modif.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/graph_modif.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/graph_path.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/graph_path.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/lambda_layers.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/lambda_layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/package.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/package.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/tf_bn_fold.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/TensorFlow/update_fold_weights.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/TensorFlow/update_fold_weights.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/UnitTest/test_a_model.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/UnitTest/test_a_model.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/batch_normalization_folding/folder.py` & `tensorflow_batchnorm_folding-1.0.8/src/batch_normalization_folding/folder.py`

 * *Files identical despite different names*

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO` & `tensorflow_batchnorm_folding-1.0.8/src/tensorflow_batchnorm_folding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-batchnorm-folding
-Version: 1.0.7
+Version: 1.0.8
 Summary: Folds BN layers in tf keras models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Edouard Yvinec
 Author-email: Edouard Yvinec <ey@datakalab.com>
 License: MIT License
         
         Copyright (c) 2022 Edouard Yvinec
```

### Comparing `tensorflow_batchnorm_folding-1.0.7/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt` & `tensorflow_batchnorm_folding-1.0.8/src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,10 +19,9 @@
 src/batch_normalization_folding/TensorFlow/to_fold_or_not_to_fold.py
 src/batch_normalization_folding/TensorFlow/update_fold_weights.py
 src/batch_normalization_folding/UnitTest/__init__.py
 src/batch_normalization_folding/UnitTest/test_a_model.py
 src/tensorflow_batchnorm_folding.egg-info/PKG-INFO
 src/tensorflow_batchnorm_folding.egg-info/SOURCES.txt
 src/tensorflow_batchnorm_folding.egg-info/dependency_links.txt
-src/tensorflow_batchnorm_folding.egg-info/requires.txt
 src/tensorflow_batchnorm_folding.egg-info/top_level.txt
 tests/test_calculus.py
```

### Comparing `tensorflow_batchnorm_folding-1.0.7/tests/test_calculus.py` & `tensorflow_batchnorm_folding-1.0.8/tests/test_calculus.py`

 * *Files identical despite different names*

