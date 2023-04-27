# Comparing `tmp/types-tensorflow-2.12.0.0.tar.gz` & `tmp/types-tensorflow-2.12.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.12.0.0.tar", last modified: Thu Mar 23 01:16:02 2023, max compression
+gzip compressed data, was "types-tensorflow-2.12.0.1.tar", last modified: Thu Apr 27 01:16:02 2023, max compression
```

## Comparing `types-tensorflow-2.12.0.0.tar` & `types-tensorflow-2.12.0.1.tar`

### file list

```diff
@@ -1,121 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.820334 types-tensorflow-2.12.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-03-23 01:16:01.000000 types-tensorflow-2.12.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 01:16:01.000000 types-tensorflow-2.12.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-23 01:16:02.820334 types-tensorflow-2.12.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 01:16:02.820334 types-tensorflow-2.12.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-23 01:16:01.000000 types-tensorflow-2.12.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.800334 types-tensorflow-2.12.0.0/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-23 01:16:01.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/_aliases.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.796334 types-tensorflow-2.12.0.0/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.800334 types-tensorflow-2.12.0.0/tensorflow-stubs/compiler/xla/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.800334 types-tensorflow-2.12.0.0/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.800334 types-tensorflow-2.12.0.0/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.804334 types-tensorflow-2.12.0.0/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.808334 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.812334 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.816334 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.816334 types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/test_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/dtypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.816334 types-tensorflow-2.12.0.0/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/keras/initializers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/keras/layers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/math.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.816334 types-tensorflow-2.12.0.0/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.816334 types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.816334 types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/sparse.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.800334 types-tensorflow-2.12.0.0/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.816334 types-tensorflow-2.12.0.0/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-23 01:15:44.000000 types-tensorflow-2.12.0.0/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:16:02.820334 types-tensorflow-2.12.0.0/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-23 01:16:02.000000 types-tensorflow-2.12.0.0/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-23 01:16:02.000000 types-tensorflow-2.12.0.0/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 01:16:02.000000 types-tensorflow-2.12.0.0/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 01:16:02.000000 types-tensorflow-2.12.0.0/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 01:16:02.000000 types-tensorflow-2.12.0.0/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.568947 types-tensorflow-2.12.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-27 01:16:01.000000 types-tensorflow-2.12.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 01:16:01.000000 types-tensorflow-2.12.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 01:16:02.568947 types-tensorflow-2.12.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-27 01:16:01.000000 types-tensorflow-2.12.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.552947 types-tensorflow-2.12.0.1/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 01:16:01.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/_aliases.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.548946 types-tensorflow-2.12.0.1/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.552947 types-tensorflow-2.12.0.1/tensorflow-stubs/compiler/xla/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.552947 types-tensorflow-2.12.0.1/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.548946 types-tensorflow-2.12.0.1/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.552947 types-tensorflow-2.12.0.1/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.556947 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.560947 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.560947 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.560947 types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/test_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/dtypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/initializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/layers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/math.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/sparse.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.548946 types-tensorflow-2.12.0.1/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-27 01:15:35.000000 types-tensorflow-2.12.0.1/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:16:02.564947 types-tensorflow-2.12.0.1/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-27 01:16:02.000000 types-tensorflow-2.12.0.1/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-27 01:16:02.000000 types-tensorflow-2.12.0.1/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:16:02.000000 types-tensorflow-2.12.0.1/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 01:16:02.000000 types-tensorflow-2.12.0.1/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 01:16:02.000000 types-tensorflow-2.12.0.1/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.12.0.0/CHANGELOG.md` & `types-tensorflow-2.12.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.12.0.1 (2023-04-27)
+
+tensorflow: Add legacy optimizers (#9997)
+
 ## 2.12.0.0 (2023-03-23)
 
 [stubsabot] Bump tensorflow to 2.12.* (#9926)
 
 Release: https://pypi.org/pypi/tensorflow/2.12.0
 Homepage: https://www.tensorflow.org/
```

### Comparing `types-tensorflow-2.12.0.0/PKG-INFO` & `types-tensorflow-2.12.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.0
+Version: 2.12.0.1
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `66146b56b9b1bc30b973386520ccb9e43c70acb8`.
+This package was generated from typeshed commit `6cb8bc0ac429d16ddd7aecd44df61ef96795775e`.
```

### Comparing `types-tensorflow-2.12.0.0/setup.py` & `types-tensorflow-2.12.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `66146b56b9b1bc30b973386520ccb9e43c70acb8`.
+This package was generated from typeshed commit `6cb8bc0ac429d16ddd7aecd44df61ef96795775e`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.12.0.0",
+      version="2.12.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-protobuf', 'numpy>=1.20'],
       packages=['tensorflow-stubs'],
-      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/coordination_config_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/distributed_runtime_payloads_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'dtypes.pyi', 'initializers.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers.pyi', 'keras/regularizers.pyi', 'math.pyi', 'python/__init__.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'sparse.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'METADATA.toml']},
+      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/coordination_config_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/distributed_runtime_payloads_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'dtypes.pyi', 'initializers.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'math.pyi', 'python/__init__.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'sparse.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from _typeshed import Incomplete, Unused
 from abc import ABCMeta
 from builtins import bool as _bool
-from collections.abc import Callable, Iterable, Iterator, Sequence
+from collections.abc import Callable, Generator, Iterable, Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from enum import Enum
 from types import TracebackType
 from typing import Any, NoReturn, TypeVar, overload
 from typing_extensions import ParamSpec, Self, TypeAlias
 
 import numpy
 from tensorflow import initializers as initializers, keras as keras, math as math
+from tensorflow._aliases import ContainerGradients, ContainerTensors, ContainerTensorsLike, Gradients, TensorLike
 
 # Explicit import of DType is covered by the wildcard, but
 # is necessary to avoid a crash in pytype.
 from tensorflow.dtypes import *
 from tensorflow.dtypes import DType as DType
 
 # Most tf.math functions are exported as tf, but sadly not all are.
@@ -49,15 +50,16 @@
     sin as sin,
     sinh as sinh,
     sqrt as sqrt,
     square as square,
     subtract as subtract,
     tanh as tanh,
 )
-from tensorflow.sparse import SparseTensor
+from tensorflow.python.trackable.autotrackable import AutoTrackable
+from tensorflow.sparse import SparseTensor as SparseTensor
 
 # Tensors ideally should be a generic type, but properly typing data type/shape
 # will be a lot of work. Until we have good non-generic tensorflow stubs,
 # we will skip making Tensor generic. Also good type hints for shapes will
 # run quickly into many places where type system is not strong enough today.
 # So shape typing is probably not worth doing anytime soon.
 _Slice: TypeAlias = int | slice | None
@@ -259,15 +261,15 @@
     def __init__(self, name: str) -> None: ...
     def __enter__(self) -> str: ...
     def __exit__(self, typ: type[BaseException] | None, value: BaseException | None, traceback: TracebackType | None) -> None: ...
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
-class Module:
+class Module(AutoTrackable):
     def __init__(self, name: str | None = None) -> None: ...
     @property
     def name(self) -> str: ...
     @property
     def name_scope(self) -> name_scope: ...
     # Documentation only specifies these as returning Sequence. Actual
     # implementation does tuple.
@@ -278,8 +280,56 @@
     @property
     def non_trainable_variables(self) -> Sequence[Variable]: ...
     @property
     def submodules(self) -> Sequence[Module]: ...
     @classmethod
     def with_name_scope(cls, method: Callable[_P, _R]) -> Callable[_P, _R]: ...
 
+class UnconnectedGradients(Enum):
+    NONE = "none"
+    ZERO = "zero"
+
+class GradientTape:
+    def __init__(self, persistent: _bool = False, watch_accessed_variables: _bool = True) -> None: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, typ: type[BaseException] | None, value: BaseException | None, traceback: TracebackType | None) -> None: ...
+    # Higher kinded types would be nice here and these overloads are a way to simulate some of them.
+    @overload
+    def gradient(
+        self,
+        target: ContainerTensors,
+        sources: TensorLike,
+        output_gradients: list[Tensor] | None = None,
+        unconnected_gradients: UnconnectedGradients = ...,
+    ) -> Gradients: ...
+    @overload
+    def gradient(
+        self,
+        target: ContainerTensors,
+        sources: Sequence[Tensor],
+        output_gradients: list[Tensor] | None = None,
+        unconnected_gradients: UnconnectedGradients = ...,
+    ) -> list[Gradients]: ...
+    @overload
+    def gradient(
+        self,
+        target: ContainerTensors,
+        sources: Mapping[str, Tensor],
+        output_gradients: list[Tensor] | None = None,
+        unconnected_gradients: UnconnectedGradients = ...,
+    ) -> dict[str, Gradients]: ...
+    @overload
+    def gradient(
+        self,
+        target: ContainerTensors,
+        sources: ContainerTensors,
+        output_gradients: list[Tensor] | None = None,
+        unconnected_gradients: UnconnectedGradients = ...,
+    ) -> ContainerGradients: ...
+    @contextmanager
+    def stop_recording(self) -> Generator[None, None, None]: ...
+    def reset(self) -> None: ...
+    def watch(self, tensor: ContainerTensorsLike) -> None: ...
+    def watched_variables(self) -> tuple[Variable, ...]: ...
+    def __getattr__(self, name: str) -> Incomplete: ...
+
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/keras/layers.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/keras/layers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/math.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.12.0.1/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.0/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.12.0.1/types_tensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.0
+Version: 2.12.0.1
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `66146b56b9b1bc30b973386520ccb9e43c70acb8`.
+This package was generated from typeshed commit `6cb8bc0ac429d16ddd7aecd44df61ef96795775e`.
```

### Comparing `types-tensorflow-2.12.0.0/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.12.0.1/types_tensorflow.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -83,19 +83,25 @@
 tensorflow-stubs/core/util/test_log_pb2.pyi
 tensorflow-stubs/keras/__init__.pyi
 tensorflow-stubs/keras/activations.pyi
 tensorflow-stubs/keras/constraints.pyi
 tensorflow-stubs/keras/initializers.pyi
 tensorflow-stubs/keras/layers.pyi
 tensorflow-stubs/keras/regularizers.pyi
+tensorflow-stubs/keras/optimizers/__init__.pyi
+tensorflow-stubs/keras/optimizers/schedules.pyi
+tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
 tensorflow-stubs/python/__init__.pyi
 tensorflow-stubs/python/keras/__init__.pyi
 tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
 tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
 tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+tensorflow-stubs/python/trackable/__init__.pyi
+tensorflow-stubs/python/trackable/autotrackable.pyi
+tensorflow-stubs/python/trackable/base.pyi
 tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
 tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
 types_tensorflow.egg-info/PKG-INFO
 types_tensorflow.egg-info/SOURCES.txt
 types_tensorflow.egg-info/dependency_links.txt
 types_tensorflow.egg-info/requires.txt
 types_tensorflow.egg-info/top_level.txt
```

