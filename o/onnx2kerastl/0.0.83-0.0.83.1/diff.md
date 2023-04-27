# Comparing `tmp/onnx2kerastl-0.0.83.tar.gz` & `tmp/onnx2kerastl-0.0.83.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.83.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.83.1.tar", max compression
```

## Comparing `onnx2kerastl-0.0.83.tar` & `onnx2kerastl-0.0.83.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/LICENSE
--rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.83/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13188 2023-04-24 08:19:57.529136 onnx2kerastl-0.0.83/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11246 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.83/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      499 2023-04-24 08:20:01.601311 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-24 08:32:43.815742 onnx2kerastl-0.0.83/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-24 08:32:43.811742 onnx2kerastl-0.0.83/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3309 2023-04-24 08:20:01.601311 onnx2kerastl-0.0.83/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5328 2023-04-24 06:18:47.644616 onnx2kerastl-0.0.83/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-24 08:32:43.803742 onnx2kerastl-0.0.83/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-24 08:32:43.807742 onnx2kerastl-0.0.83/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    16675 2023-04-24 08:32:43.807742 onnx2kerastl-0.0.83/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5354 2023-04-24 08:32:43.803742 onnx2kerastl-0.0.83/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-04-24 08:32:43.823742 onnx2kerastl-0.0.83/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.83/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/LICENSE
+-rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.83.1/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83.1/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13188 2023-04-27 05:26:04.514498 onnx2kerastl-0.0.83.1/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    13847 2023-04-27 14:37:06.882137 onnx2kerastl-0.0.83.1/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      499 2023-04-27 05:26:04.514498 onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-24 14:18:00.054331 onnx2kerastl-0.0.83.1/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.83.1/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83.1/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3309 2023-04-27 05:26:04.514498 onnx2kerastl-0.0.83.1/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83.1/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5328 2023-04-24 06:18:47.644616 onnx2kerastl-0.0.83.1/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.83.1/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.83.1/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83.1/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    16675 2023-04-27 05:26:04.514498 onnx2kerastl-0.0.83.1/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5354 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.83.1/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83.1/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83.1/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1032 2023-04-27 14:37:11.014160 onnx2kerastl-0.0.83.1/pyproject.toml
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.83.1/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.83/LICENSE` & `onnx2kerastl-0.0.83.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/convolution_layers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 import logging
-
+from typing import List
+import tensorflow as tf
 import keras
+from .utils import ensure_tf_type, ensure_numpy_type, is_numpy
+from functools import partial
+from tensorflow.python.framework.ops import EagerTensor
+
+
+def calculate_permute_values(n_dims: int, to_channel_first: bool) -> List[int]:
+    if to_channel_first:
+        return [n_dims - 1] + list(range(1, n_dims - 1))
+    else:
+        return list(range(2, n_dims)) + [1]
+
 
-from .utils import ensure_tf_type, ensure_numpy_type
+def permute_wrap_conv_if_constant(partial_func, conv_input, is_constant):
+    if is_constant:
+        input_shape = tf.shape(conv_input)
+        permuted = keras.layers.Permute(calculate_permute_values(len(input_shape), to_channel_first=False))(conv_input)
+        conv_res = partial_func(data_format="channels_last")(permuted)
+        result = keras.layers.Permute(calculate_permute_values(len(input_shape), to_channel_first=True))(conv_res)
+    else:
+        result = partial_func()(conv_input)
+    return result
 
 
 def convert_conv(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert convolution layer
     :param node: current operation node
     :param params: operation attributes
@@ -31,14 +51,15 @@
         W = ensure_numpy_type(layers[node.input[1]])
         bias = None
 
     else:
         raise NotImplementedError('Not implemented')
 
     input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
+    is_constant = is_numpy(input_0) or isinstance(input_0, EagerTensor)
     n_groups = params['group'] if 'group' in params else 1
     dilation = params['dilations'][0] if 'dilations' in params else 1
     pads = params['pads'] if 'pads' in params else [0, 0, 0]
     strides = params['strides'] if 'strides' in params else [1, 1, 1]
 
     if len(W.shape) == 5:  # 3D conv
         logger.debug('3D convolution')
@@ -53,27 +74,39 @@
         out_channels, channels_per_group, dimension, height, width = W.shape
         W = W.transpose(2, 3, 4, 1, 0)
 
         if has_bias:
             weights = [W, bias]
         else:
             weights = [W]
-        conv = keras.layers.Conv3D(
-            filters=out_channels,
-            kernel_size=(dimension, height, width),
-            strides=(strides[0], strides[1], strides[2]),
-            padding='valid',
-            weights=weights,
-            use_bias=has_bias,
-            activation=None,
-            dilation_rate=dilation,
-            name=keras_name,
-            groups=n_groups
-        )
-        layers[node_name] = conv(input_0)
+        conv_args = { "filters": out_channels,
+        "kernel_size": (dimension, height, width),
+        "strides": (strides[0], strides[1], strides[2]),
+        "padding": 'valid',
+        "weights": weights,
+        "use_bias": has_bias,
+        "activation": None,
+        "dilation_rate": dilation,
+        "name": keras_name,
+        "groups": n_groups}
+        partial_conv = partial(keras.layers.Conv3D, **conv_args)
+        layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
+        # conv = keras.layers.Conv3D(
+        #     filters=out_channels,
+        #     kernel_size=(dimension, height, width),
+        #     strides=(strides[0], strides[1], strides[2]),
+        #     padding='valid',
+        #     weights=weights,
+        #     use_bias=has_bias,
+        #     activation=None,
+        #     dilation_rate=dilation,
+        #     name=keras_name,
+        #     groups=n_groups
+        # )
+        # layers[node_name] = conv(input_0)
 
     elif len(W.shape) == 4:  # 2D conv
         logger.debug('2D convolution')
 
         padding = None
         if len(pads) == 2 and (pads[0] > 0 or pads[1] > 0):
             padding = (pads[0], pads[1])
@@ -93,72 +126,95 @@
         W = W.transpose(2, 3, 1, 0)
         height, width, channels_per_group, out_channels = W.shape
 
         if has_bias:
             weights = [W, bias]
         else:
             weights = [W]
-
-        conv = keras.layers.Conv2D(
-            filters=out_channels,
-            kernel_size=(height, width),
-            strides=(strides[0], strides[1]),
-            padding='valid',
-            weights=weights,
-            use_bias=has_bias,
-            activation=None,
-            dilation_rate=dilation,
-            groups=n_groups,
-            name=keras_name
-        )
-
-        layers[node_name] = conv(input_0)
+        conv_args = {"filters": out_channels,
+        "kernel_size": (height, width),
+        "strides": (strides[0], strides[1]),
+        "padding": 'valid',
+        "weights": weights,
+        "use_bias": has_bias,
+        "activation": None,
+        "dilation_rate": dilation,
+        "name": keras_name,
+        "groups": n_groups}
+        partial_conv = partial(keras.layers.Conv2D, **conv_args)
+        layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
+        # conv = keras.layers.Conv2D(
+        #     filters=out_channels,
+        #     kernel_size=(height, width),
+        #     strides=(strides[0], strides[1]),
+        #     padding='valid',
+        #     weights=weights,
+        #     use_bias=has_bias,
+        #     activation=None,
+        #     dilation_rate=dilation,
+        #     groups=n_groups,
+        #     name=keras_name
+        # )
+        #
+        # layers[node_name] = conv(input_0)
     else:
         # 1D conv
         W = W.transpose(2, 1, 0)
         width, channels, n_filters = W.shape
         print(width, channels, n_filters, has_bias)
 
         if has_bias:
             weights = [W, bias]
         else:
             weights = [W]
 
         padding = None
         if len(pads) == 2 and (pads[0] > 0 or pads[1] > 0):
             padding = (pads[0], pads[1])
-
+        conv_args = {"filters": n_filters,
+        "kernel_size": (width),
+        "strides": (strides[0]),
+        "weights": weights,
+        "use_bias": has_bias,
+        "activation": None,
+        "dilation_rate": dilation,
+        "name": keras_name,
+        "groups": n_groups}
         if padding:
-            conv = keras.layers.Conv1D(
-                filters=n_filters,
-                kernel_size=width,
-                strides=strides[0],
-                padding='same',
-                weights=weights,
-                use_bias=has_bias,
-                activation=None,
-                dilation_rate=dilation,
-                groups=n_groups,
-                name=keras_name,
-                data_format='channels_first')
+            conv_args['padding'] = 'same'
+            # conv = keras.layers.Conv1D(
+            #     filters=n_filters,
+            #     kernel_size=width,
+            #     strides=strides[0],
+            #     padding='same',
+            #     weights=weights,
+            #     use_bias=has_bias,
+            #     activation=None,
+            #     dilation_rate=dilation,
+            #     groups=n_groups,
+            #     name=keras_name,
+            #     data_format='channels_first')
         else:
-            conv = keras.layers.Conv1D(
-                filters=n_filters,
-                kernel_size=width,
-                strides=strides[0],
-                padding='valid',
-                weights=weights,
-                use_bias=has_bias,
-                activation=None,
-                dilation_rate=dilation,
-                groups=n_groups,
-                name=keras_name,
-                data_format='channels_first')
+            conv_args['padding'] = 'valid'
 
-        layers[node_name] = conv(input_0)
+            # conv = keras.layers.Conv1D(
+            #     filters=n_filters,
+            #     kernel_size=width,
+            #     strides=strides[0],
+            #     padding='valid',
+            #     weights=weights,
+            #     use_bias=has_bias,
+            #     activation=None,
+            #     dilation_rate=dilation,
+            #     groups=n_groups,
+            #     name=keras_name,
+            #     data_format='channels_first')
+        partial_conv = partial(keras.layers.Conv1D, **conv_args)
+        layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
+        # layers[node_name] = conv(input_0)
 
         # padding_name = keras_name + '_pad'
         # padding_layer = keras.layers.ZeroPadding1D(
         #     padding=(pads[0]),
         #     name=padding_name
         # )
         # print(input_0)
```

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.83.1/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.83/pyproject.toml` & `onnx2kerastl-0.0.83.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.83"
+version = "0.0.83.1"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.83/PKG-INFO` & `onnx2kerastl-0.0.83.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.83
+Version: 0.0.83.1
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

