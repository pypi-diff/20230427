# Comparing `tmp/fedml-0.8.3a9.tar.gz` & `tmp/fedml-0.8.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fedml-0.8.3a9.tar", last modified: Thu Apr 13 14:45:37 2023, max compression
+gzip compressed data, was "dist/fedml-0.8.4a1.tar", last modified: Thu Apr 27 10:21:01 2023, max compression
```

## Comparing `fedml-0.8.3a9.tar` & `fedml-0.8.4a1.tar`

### file list

```diff
@@ -1,1118 +1,1164 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/
--rw-r--r--   0 runner     (501) staff       (20)     3806 2023-04-13 14:45:37.000000 fedml-0.8.3a9/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/tests/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/tests/security/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/tests/security/attack/
--rw-r--r--   0 runner     (501) staff       (20)     1218 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/test_label_flipping_attack.py
--rw-r--r--   0 runner     (501) staff       (20)      730 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/test_backdoor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:37.000000 fedml-0.8.3a9/tests/security/attack/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1159 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/test_model_replacement_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5147 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/test_invertgradient.py
--rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/test_byzantine_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5519 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      955 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/test_edge_case_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     1466 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/attack/test_dlg.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:37.000000 fedml-0.8.3a9/tests/security/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/tests/security/defense/
--rw-r--r--   0 runner     (501) staff       (20)      376 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_rfa.py
--rw-r--r--   0 runner     (501) staff       (20)     1942 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_residual_based_reweighting.py
--rw-r--r--   0 runner     (501) staff       (20)     1139 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_wbc.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/defense/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1099 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/defense/test_crfl.py
--rw-r--r--   0 runner     (501) staff       (20)     1871 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_geometric_median.py
--rw-r--r--   0 runner     (501) staff       (20)     2682 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_slsgd_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1327 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_weak_dp.py
--rw-r--r--   0 runner     (501) staff       (20)     1525 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_norm_diff_clipping.py
--rw-r--r--   0 runner     (501) staff       (20)     5913 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1555 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/defense/test_bulyan.py
--rw-r--r--   0 runner     (501) staff       (20)      805 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_robust_learning_rate_defense.py
--rw-r--r--   0 runner     (501) staff       (20)      999 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/defense/test_coordinate_wise_trimmed_mean.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1206 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_krum.py
--rwxr-xr-x   0 runner     (501) staff       (20)      987 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/defense/test_cclip.py
--rw-r--r--   0 runner     (501) staff       (20)      390 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/defense/test_coordinate_median.py
--rw-r--r--   0 runner     (501) staff       (20)      902 2023-04-13 14:43:38.000000 fedml-0.8.3a9/tests/security/defense/test_foolsgold_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2208 2023-04-13 14:43:39.000000 fedml-0.8.3a9/tests/security/defense/test_soteria.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:36.000000 fedml-0.8.3a9/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2326 2023-04-13 14:42:13.000000 fedml-0.8.3a9/README.md
--rw-r--r--   0 runner     (501) staff       (20)     4581 2023-04-13 14:43:36.000000 fedml-0.8.3a9/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_silo/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2026 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       89 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       89 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/main_fedml_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)      196 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/mlops_client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:41.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:41.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:44.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:44.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2003 2023-04-13 14:42:45.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:45.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2024 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)     4403 2023-04-13 14:42:37.000000 fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)     5218 2023-04-13 14:42:37.000000 fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2033 2023-04-13 14:42:37.000000 fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py
--rw-r--r--   0 runner     (501) staff       (20)     2020 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1435 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:40.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      757 2023-04-13 14:42:40.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      757 2023-04-13 14:42:40.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-04-13 14:42:40.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:40.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2119 2023-04-13 14:42:40.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      827 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      965 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)      827 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)     4098 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1739 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py
--rw-r--r--   0 runner     (501) staff       (20)     5323 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1999 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2013 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:39.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:43.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2003 2023-04-13 14:42:43.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:43.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:44.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:44.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:44.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1993 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py
--rw-r--r--   0 runner     (501) staff       (20)     3354 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1387 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)     2007 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py
--rw-r--r--   0 runner     (501) staff       (20)      699 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:10.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:08.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      391 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:40.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-13 14:42:41.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-13 14:42:41.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-13 14:42:41.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:09.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/main_fedml_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:42.000000 fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_device/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/
--rw-r--r--   0 runner     (501) staff       (20)     1214 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      801 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/cross_device/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/
--rw-r--r--   0 runner     (501) staff       (20)     1170 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-13 14:42:36.000000 fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/examples/centralized/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/centralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    20282 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/centralized/main.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_fedopt_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:48.000000 fedml-0.8.3a9/examples/simulation/mpi_fedopt_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:49.000000 fedml-0.8.3a9/examples/simulation/mpi_fedopt_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_vertical_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:43:00.000000 fedml-0.8.3a9/examples/simulation/sp_vertical_mnist_lr_example/torch_vertical_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/examples/simulation/sp_vertical_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_fedopt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:59.000000 fedml-0.8.3a9/examples/simulation/sp_fedopt_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:59.000000 fedml-0.8.3a9/examples/simulation/sp_fedopt_mnist_lr_example/torch_fedopt_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_decentralized_fl_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/simulation/mpi_decentralized_fl_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      222 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/simulation/mpi_decentralized_fl_example/mpi_decentralized_fl_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/sp_decentralized_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:57.000000 fedml-0.8.3a9/examples/simulation/sp_decentralized_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:57.000000 fedml-0.8.3a9/examples/simulation/sp_decentralized_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:54.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/torch_fedgkt_cifar10_resnet56.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:54.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     5590 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     4816 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/reddit_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6461 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/main.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_hierarchicalfl_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:59.000000 fedml-0.8.3a9/examples/simulation/sp_hierarchicalfl_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:59.000000 fedml-0.8.3a9/examples/simulation/sp_hierarchicalfl_mnist_lr_example/torch_hierarchicalfl_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/simulation/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedopt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:55.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedopt_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:55.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedopt_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedgan_mnist_gan_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:54.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedgan_mnist_gan_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:54.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedgan_mnist_gan_example/torch_fedgan_mnist_gan_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_fedavg_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/simulation/mpi_fedavg_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:48.000000 fedml-0.8.3a9/examples/simulation/mpi_fedavg_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_seq/
--rw-r--r--   0 runner     (501) staff       (20)      762 2023-04-13 14:42:54.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_seq/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_fedprox_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:50.000000 fedml-0.8.3a9/examples/simulation/mpi_fedprox_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:51.000000 fedml-0.8.3a9/examples/simulation/mpi_fedprox_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)       69 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      423 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fednas_cifar10_dart_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:55.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fednas_cifar10_dart_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:55.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fednas_cifar10_dart_example/torch_fednas_cifar10_dart_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:43:00.000000 fedml-0.8.3a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:59.000000 fedml-0.8.3a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:59.000000 fedml-0.8.3a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-13 14:42:59.000000 fedml-0.8.3a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:56.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:56.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/torch_splitnn_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_fednova_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fednova_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fednova_mnist_lr_example/torch_fednova_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_base_framework_example/
--rw-r--r--   0 runner     (501) staff       (20)      222 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/simulation/mpi_base_framework_example/mpi_base_framework_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:46.000000 fedml-0.8.3a9/examples/simulation/mpi_base_framework_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_cnn_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_cnn_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_cnn_example/torch_fedavg_mnist_cnn_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:52.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-13 14:42:53.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedprox_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:56.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedprox_mnist_lr_example/torch_fedprox_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:55.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_fedprox_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:12.000000 fedml-0.8.3a9/examples/simulation/sp_turboaggregate_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/examples/simulation/sp_turboaggregate_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:43:00.000000 fedml-0.8.3a9/examples/simulation/sp_turboaggregate_mnist_lr_example/torch_turboaggregate_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_async_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:51.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_async_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1042 2023-04-13 14:42:51.000000 fedml-0.8.3a9/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:11.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-13 14:42:58.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_datasets_and_models_example/torch_fedavg_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:57.000000 fedml-0.8.3a9/examples/simulation/sp_fedavg_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:42:35.000000 fedml-0.8.3a9/examples/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-13 14:45:37.000000 fedml-0.8.3a9/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/
--rw-r--r--   0 runner     (501) staff       (20)     1078 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/launch_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)     4169 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/runner.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/cross_silo/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/cross_silo/lightsecagg/
--rw-r--r--   0 runner     (501) staff       (20)     3009 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_message_define.py
--rw-r--r--   0 runner     (501) staff       (20)    11077 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/lightsecagg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13517 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)    12846 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     3467 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_api.py
--rw-r--r--   0 runner     (501) staff       (20)      157 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/cross_silo/server/
--rw-r--r--   0 runner     (501) staff       (20)     2212 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/cross_silo/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    15366 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/cross_silo/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    11613 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1056 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/cross_silo/server/server_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     1917 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/fedml_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2025 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/fedml_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/cross_silo/client/
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     5161 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2680 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-13 14:43:13.000000 fedml-0.8.3a9/fedml/cross_silo/client/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7549 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/fedml_client_master_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_silo/client/fedml_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     1079 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/launch_cross_silo_horizontal.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/schedule/
--rw-r--r--   0 runner     (501) staff       (20)     5761 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/schedule/runtime_estimate.py
--rw-r--r--   0 runner     (501) staff       (20)     9840 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/schedule/seq_train_scheduler.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/schedule/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/core/alg_frame/
--rw-r--r--   0 runner     (501) staff       (20)      795 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/alg_frame/params.py
--rw-r--r--   0 runner     (501) staff       (20)     1855 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/alg_frame/client_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/alg_frame/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      894 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/alg_frame/context.py
--rw-r--r--   0 runner     (501) staff       (20)     5737 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/alg_frame/server_aggregator.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/core/distributed/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/distributed/topology/
--rw-r--r--   0 runner     (501) staff       (20)     5001 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/topology/asymmetric_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      479 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/topology/base_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     3853 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/topology/symmetric_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/topology/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/crypto/
--rw-r--r--   0 runner     (501) staff       (20)     2167 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/crypto/crypto_api.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/crypto/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/distributed/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8764 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/fedml_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:18.000000 fedml-0.8.3a9/fedml/core/distributed/communication/
--rw-r--r--   0 runner     (501) staff       (20)      153 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/observer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/communication/s3/
--rw-r--r--   0 runner     (501) staff       (20)     1680 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/s3/remote_storage_mnn.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/s3/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    21800 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/s3/remote_storage.py
--rw-r--r--   0 runner     (501) staff       (20)     2792 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/s3/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:18.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mpi/
--rw-r--r--   0 runner     (501) staff       (20)     1648 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mpi/mpi_send_thread.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mpi/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4977 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mpi/com_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1603 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mpi/mpi_receive_thread.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:18.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/
--rw-r--r--   0 runner     (501) staff       (20)     1255 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_server.py
--rw-r--r--   0 runner     (501) staff       (20)     6381 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:18.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/proto/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/proto/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4236 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py
--rw-r--r--   0 runner     (501) staff       (20)      346 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/ip_config_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     6272 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/communication/trpc/
--rw-r--r--   0 runner     (501) staff       (20)     1614 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/trpc/trpc_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/trpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4807 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/trpc/trpc_comm_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/trpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      377 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/distributed/communication/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2612 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/message.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_web3/
--rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_web3/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14594 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_thetastore/
--rwxr-xr-x   0 runner     (501) staff       (20)      109 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_thetastore/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14669 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)      869 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      518 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/distributed/communication/base_com_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:18.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3/
--rwxr-xr-x   0 runner     (501) staff       (20)      123 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    15504 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:18.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13720 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt/mqtt_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:18.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3_mnn/
--rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-04-13 14:43:06.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3_mnn/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    12233 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/web3_storage/
--rw-r--r--   0 runner     (501) staff       (20)     3604 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/web3_storage/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:19.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/theta_storage/
--rw-r--r--   0 runner     (501) staff       (20)     6834 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/theta_storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:07.000000 fedml-0.8.3a9/fedml/core/distributed/distributed_storage/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/distributed/flow/
--rw-r--r--   0 runner     (501) staff       (20)    12684 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/flow/fedml_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/flow/fedml_executor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/flow/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      338 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/flow/fedml_flow_constants.py
--rw-r--r--   0 runner     (501) staff       (20)     3248 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/distributed/flow/test_fedml_flow.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/security/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/core/security/attack/
--rw-r--r--   0 runner     (501) staff       (20)     4005 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/attack/model_replacement_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)      440 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/attack/attack_base.py
--rw-r--r--   0 runner     (501) staff       (20)     3424 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/attack/edge_case_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     3607 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/attack/byzantine_attack.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/attack/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6102 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/attack/lazy_worker.py
--rw-r--r--   0 runner     (501) staff       (20)    27345 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/attack/invert_gradient_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     6066 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/attack/dlg_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     4712 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/attack/revealing_labels_from_gradients_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/attack/label_flipping_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5286 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/attack/backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     3738 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/fedml_attacker.py
--rw-r--r--   0 runner     (501) staff       (20)     1208 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/security/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7568 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/fedml_defender.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/core/security/common/
--rw-r--r--   0 runner     (501) staff       (20)     1973 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/common/bucket.py
--rw-r--r--   0 runner     (501) staff       (20)      734 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/common/net.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1856 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/common/attack_defense_data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     7488 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/common/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/core/security/defense/
--rw-r--r--   0 runner     (501) staff       (20)     8885 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/three_sigma_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2172 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/norm_diff_clipping_defense.py
--rw-r--r--   0 runner     (501) staff       (20)    10320 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/residual_based_reweighting_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     8375 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/three_sigma_krum_defense.py
--rw-r--r--   0 runner     (501) staff       (20)      994 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2849 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/slsgd_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1610 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/coordinate_wise_median_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3640 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/wbc_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2675 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/robust_learning_rate_defense.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1071 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/RFA_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1682 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/defense_base.py
--rw-r--r--   0 runner     (501) staff       (20)     3568 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/foolsgold_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3709 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/soteria_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     5462 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/bulyan_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     4636 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/cross_round_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     6525 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/three_sigma_geomedian_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1988 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/geometric_median_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3054 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/crfl_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1173 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/outlier_detection.py
--rw-r--r--   0 runner     (501) staff       (20)     1008 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/weak_dp_defense.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2650 2023-04-13 14:43:10.000000 fedml-0.8.3a9/fedml/core/security/defense/cclip_defense.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2564 2023-04-13 14:43:11.000000 fedml-0.8.3a9/fedml/core/security/defense/krum_defense.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/mlops/
--rw-r--r--   0 runner     (501) staff       (20)     8983 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/mlops_configs.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/mlops/ssl/
--rw-r--r--   0 runner     (501) staff       (20)     4089 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)     4085 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)     1947 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mlops/ssl/open-root-ca.crt
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/ssl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4093 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)    21213 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/mlops_metrics.py
--rw-r--r--   0 runner     (501) staff       (20)     4891 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/mlops_profiler_event.py
--rw-r--r--   0 runner     (501) staff       (20)     1377 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/mlops_status.py
--rw-r--r--   0 runner     (501) staff       (20)    33177 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11124 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mlops/stats_impl.py
--rw-r--r--   0 runner     (501) staff       (20)     1410 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/mlops_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    17257 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/mlops_runtime_log_daemon.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3906 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mlops/system_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     8060 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/mlops/mlops_runtime_log.py
--rw-r--r--   0 runner     (501) staff       (20)     1117 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/core/common/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      298 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/common/ml_engine_backend.py
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/common/singleton.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/mpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6017 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mpc/lightsecagg.py
--rw-r--r--   0 runner     (501) staff       (20)    12340 2023-04-13 14:43:09.000000 fedml-0.8.3a9/fedml/core/mpc/secagg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/dp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/dp/mechanisms/
--rw-r--r--   0 runner     (501) staff       (20)     1443 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/mechanisms/dp_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)      659 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/mechanisms/laplace.py
--rw-r--r--   0 runner     (501) staff       (20)       83 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/mechanisms/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      177 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/mechanisms/base_dp_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)     1037 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/mechanisms/gaussian.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/dp/test/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/test/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2532 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/test/test_fed_privacy_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)     4178 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/fedml_differential_privacy.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/dp/frames/
--rw-r--r--   0 runner     (501) staff       (20)     3293 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/frames/NbAFL.py
--rw-r--r--   0 runner     (501) staff       (20)     2444 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/frames/dp_clip.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/frames/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1101 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/frames/cdp.py
--rw-r--r--   0 runner     (501) staff       (20)      470 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/frames/ldp.py
--rw-r--r--   0 runner     (501) staff       (20)     2118 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/frames/base_dp_solution.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/dp/budget_accountant/
--rw-r--r--   0 runner     (501) staff       (20)     6747 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/budget_accountant/rdp_analysis.py
--rw-r--r--   0 runner     (501) staff       (20)     1141 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/budget_accountant/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6915 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/budget_accountant/rdp_accountant.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:20.000000 fedml-0.8.3a9/fedml/core/dp/common/
--rw-r--r--   0 runner     (501) staff       (20)       69 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/common/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2411 2023-04-13 14:43:08.000000 fedml-0.8.3a9/fedml/core/dp/common/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/core/contribution/
--rw-r--r--   0 runner     (501) staff       (20)     5603 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/contribution/gtg_shapley_value.py
--rw-r--r--   0 runner     (501) staff       (20)     3197 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/contribution/mr_shapley_value.py
--rw-r--r--   0 runner     (501) staff       (20)     1665 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/contribution/base_contribution_assessor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/contribution/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4930 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/contribution/leave_one_out.py
--rw-r--r--   0 runner     (501) staff       (20)     1922 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/contribution/contribution_assessor_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/core/data/
--rw-r--r--   0 runner     (501) staff       (20)      158 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4937 2023-04-13 14:43:05.000000 fedml-0.8.3a9/fedml/core/data/noniid_partition.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/distributed/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/distributed/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:07.000000 fedml-0.8.3a9/fedml/config/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/config/simulaton_mpi/
--rw-r--r--   0 runner     (501) staff       (20)      964 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/config/simulaton_mpi/fedml_config.yaml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/config/simulation_sp/
--rw-r--r--   0 runner     (501) staff       (20)     1091 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/config/simulation_sp/fedml_config.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)     7490 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/arguments.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:28.000000 fedml-0.8.3a9/fedml/mlops/
--rw-r--r--   0 runner     (501) staff       (20)     2189 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/mlops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2021 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/cross_device/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/cross_device/server_mnn/
--rw-r--r--   0 runner     (501) staff       (20)     2190 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/server_mnn/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/server_mnn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    18567 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/server_mnn/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     2772 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/server_mnn/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7827 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/server_mnn/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1264 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/server_mnn/server_mnn_api.py
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      579 2023-04-13 14:43:12.000000 fedml-0.8.3a9/fedml/cross_device/mnn_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/centralized/
--rw-r--r--   0 runner     (501) staff       (20)     6588 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/centralized/centralized_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/centralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      685 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/launch_simulation.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:30.000000 fedml-0.8.3a9/fedml/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/fedavg/client.py
--rw-r--r--   0 runner     (501) staff       (20)       34 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12457 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/fedavg/fedavg_api.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/fedprox/
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fedprox/client.py
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fedprox/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11535 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fedprox/fedprox_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7850 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/TA_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     7880 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/mpc_function.py
--rw-r--r--   0 runner     (501) staff       (20)      818 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/TA_client.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/feddyn/
--rw-r--r--   0 runner     (501) staff       (20)     1916 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/feddyn/client copy.py
--rw-r--r--   0 runner     (501) staff       (20)     1941 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/feddyn/client.py
--rw-r--r--   0 runner     (501) staff       (20)       42 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/feddyn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    16395 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/feddyn/feddyn_trainer copy.py
--rw-r--r--   0 runner     (501) staff       (20)    15943 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/feddyn/feddyn_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/
--rw-r--r--   0 runner     (501) staff       (20)     1355 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/client.py
--rw-r--r--   0 runner     (501) staff       (20)     3625 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/party_models.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2241 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/vfl.py
--rw-r--r--   0 runner     (501) staff       (20)    10964 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/vfl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     3887 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/fednova/
--rw-r--r--   0 runner     (501) staff       (20)     8207 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fednova/fednova.py
--rw-r--r--   0 runner     (501) staff       (20)    12457 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fednova/fednova_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)    10932 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fednova/fednova_api.py
--rw-r--r--   0 runner     (501) staff       (20)     6496 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fednova/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fednova/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2258 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fednova/comm_helpers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/fedopt/
--rw-r--r--   0 runner     (501) staff       (20)    12255 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fedopt/fedopt_api.py
--rw-r--r--   0 runner     (501) staff       (20)     1456 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fedopt/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fedopt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/fedopt/optrepo.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/
--rw-r--r--   0 runner     (501) staff       (20)     2133 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2391 2023-04-13 14:43:34.000000 fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/group.py
--rw-r--r--   0 runner     (501) staff       (20)     4644 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/mime/
--rw-r--r--   0 runner     (501) staff       (20)     1494 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/mime/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/mime/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3192 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/mime/opt_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    13370 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/mime/mime_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/scaffold/
--rw-r--r--   0 runner     (501) staff       (20)    13084 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/scaffold/scaffold_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     2677 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/scaffold/client.py
--rw-r--r--   0 runner     (501) staff       (20)       46 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/simulation/sp/scaffold/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/sp/decentralized/
--rw-r--r--   0 runner     (501) staff       (20)     4187 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/decentralized/decentralized_fl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     4328 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/decentralized/client_dsgd.py
--rw-r--r--   0 runner     (501) staff       (20)     5514 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/decentralized/client_pushsum.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/decentralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5741 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/sp/decentralized/topology_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:33.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     2689 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6818 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3602 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAvgAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2542 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4462 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAvgServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/
--rw-r--r--   0 runner     (501) staff       (20)     2589 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2338 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/SplitNNAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      591 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     1733 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3996 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     2043 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/split_nn/server_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2438 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2804 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     7365 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4607 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3460 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxAPI.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:34.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/
--rw-r--r--   0 runner     (501) staff       (20)     4494 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGanServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3809 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGanAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3633 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/gan_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)      880 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2218 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGANTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     7774 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGANAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2625 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGanClientManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:34.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/
--rw-r--r--   0 runner     (501) staff       (20)    15801 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     2120 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/FedGKTAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     3165 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4940 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      671 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/message_def.py
--rw-r--r--   0 runner     (501) staff       (20)     2925 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     6492 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/
--rw-r--r--   0 runner     (501) staff       (20)      428 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1858 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1123 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/central_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     1147 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/algorithm_api.py
--rw-r--r--   0 runner     (501) staff       (20)      438 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/client_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/base_framework/central_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     3409 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4903 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3324 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     3531 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2222 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     3863 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     7993 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     4779 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4164 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)     3274 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:33.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/
--rw-r--r--   0 runner     (501) staff       (20)     5488 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3489 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    13844 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3079 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5954 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3284 2023-04-13 14:43:27.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/
--rw-r--r--   0 runner     (501) staff       (20)      386 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1112 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     2374 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      738 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/algorithm_api.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/
--rw-r--r--   0 runner     (501) staff       (20)      504 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     7074 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2198 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1801 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     3470 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     1842 2023-04-13 14:43:26.000000 fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/host_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:25.000000 fedml-0.8.3a9/fedml/simulation/mpi/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:34.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/
--rw-r--r--   0 runner     (501) staff       (20)    11022 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3767 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     2295 2023-04-13 14:43:28.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    10792 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)      693 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:35.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/
--rw-r--r--   0 runner     (501) staff       (20)     3490 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     5687 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4893 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)    10695 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3306 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fednova/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:35.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/
--rw-r--r--   0 runner     (501) staff       (20)     8893 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      578 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2663 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/optrepo.py
--rw-r--r--   0 runner     (501) staff       (20)     3297 2023-04-13 14:43:29.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1307 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4470 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:36.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/
--rw-r--r--   0 runner     (501) staff       (20)     3300 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    12025 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1009 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     4464 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/optrepo.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1307 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5535 2023-04-13 14:43:30.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/
--rw-r--r--   0 runner     (501) staff       (20)     3507 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      716 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     1927 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     6138 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/MyModelTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12406 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)    10700 2023-04-13 14:43:32.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2448 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     4172 2023-04-13 14:43:31.000000 fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)      205 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/simulation/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     9847 2023-04-13 14:43:33.000000 fedml-0.8.3a9/fedml/simulation/simulator.py
--rw-r--r--   0 runner     (501) staff       (20)    13612 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:37.000000 fedml-0.8.3a9/fedml/utils/
--rw-r--r--   0 runner     (501) staff       (20)    10317 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/utils/model_utils.py
--rw-r--r--   0 runner     (501) staff       (20)      735 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/utils/logging.py
--rw-r--r--   0 runner     (501) staff       (20)    10524 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/utils/compression.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-13 14:43:35.000000 fedml-0.8.3a9/fedml/utils/context.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/cli/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)    14236 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/client_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)    11063 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/client_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2195 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/client_daemon.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5658 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/docker_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)    51790 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/client_runner.py
--rw-r--r--   0 runner     (501) staff       (20)    15185 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/client_constants.py
--rw-r--r--   0 runner     (501) staff       (20)    10779 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/client_diagnosis.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1923 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/client_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3126 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/edge_deployment/simulator_daemon.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:16.000000 fedml-0.8.3a9/fedml/cli/model_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)     5025 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_inference.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2265 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_client_daemon.py
--rw-r--r--   0 runner     (501) staff       (20)     7935 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/modelops_configs.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1937 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_server_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)    68065 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_server_runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)    25696 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_cards.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1937 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_client_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5426 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/docker_client_login.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    16417 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_server_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)    16754 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_cache.py
--rwxr-xr-x   0 runner     (501) staff       (20)    31076 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_deployment.py
--rwxr-xr-x   0 runner     (501) staff       (20)      816 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_server_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1766 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_object.py
--rwxr-xr-x   0 runner     (501) staff       (20)    26434 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_db.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6554 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_login_entry.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14992 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_client_data_interface.py
--rw-r--r--   0 runner     (501) staff       (20)    19913 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_server_constants.py
--rwxr-xr-x   0 runner     (501) staff       (20)     8166 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_monitor.py
--rw-r--r--   0 runner     (501) staff       (20)    25461 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_client_constants.py
--rwxr-xr-x   0 runner     (501) staff       (20)    42572 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_client_runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5460 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/docker_server_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2915 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_server_daemon.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6819 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_client_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2759 2023-04-13 14:43:03.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_msg_object.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2995 2023-04-13 14:43:02.000000 fedml-0.8.3a9/fedml/cli/model_deployment/device_model_inference_entry.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/env/
--rw-r--r--   0 runner     (501) staff       (20)     3453 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/env/collect_env.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/env/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    40597 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/cli.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/cli/build-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1253 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      629 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1253 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/torch_client.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      650 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:00.000000 fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:14.000000 fedml-0.8.3a9/fedml/cli/comm_utils/
--rw-r--r--   0 runner     (501) staff       (20)    18132 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/comm_utils/sys_utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/comm_utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      295 2023-04-13 14:43:01.000000 fedml-0.8.3a9/fedml/cli/comm_utils/yaml_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/cli/server_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)      749 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/server_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)    70911 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/server_runner.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2848 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/job_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5692 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/docker_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1925 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/server_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2451 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/server_daemon.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:17.000000 fedml-0.8.3a9/fedml/cli/server_deployment/templates/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/templates/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/templates/fedml-aggregator-data-pv.yaml
--rw-r--r--   0 runner     (501) staff       (20)      279 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/templates/fedml-aggregator-data-pvc.yaml
--rw-r--r--   0 runner     (501) staff       (20)      275 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/templates/fedml-server-svc.yaml
--rw-r--r--   0 runner     (501) staff       (20)     1370 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)    13814 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/server_login.py
--rw-r--r--   0 runner     (501) staff       (20)    13791 2023-04-13 14:43:04.000000 fedml-0.8.3a9/fedml/cli/server_deployment/server_constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:26.000000 fedml-0.8.3a9/fedml/ml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:27.000000 fedml-0.8.3a9/fedml/ml/aggregator/
--rw-r--r--   0 runner     (501) staff       (20)      548 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/aggregator_creator.py
--rw-r--r--   0 runner     (501) staff       (20)     2488 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     4187 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/default_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5621 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2408 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator_classification.py
--rw-r--r--   0 runner     (501) staff       (20)    10546 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/agg_operator.py
--rw-r--r--   0 runner     (501) staff       (20)     3388 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:27.000000 fedml-0.8.3a9/fedml/ml/engine/
--rw-r--r--   0 runner     (501) staff       (20)    11319 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/engine/ml_engine_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/engine/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1345 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/engine/torch_process_group_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:28.000000 fedml-0.8.3a9/fedml/ml/trainer/
--rw-r--r--   0 runner     (501) staff       (20)     3953 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/scaffold_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)      580 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/trainer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)     9496 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/fednova_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/trainer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/local_optimizer.py
--rw-r--r--   0 runner     (501) staff       (20)     5923 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/fedprox_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     3578 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     6857 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/ml/trainer/feddyn_trainer copy.py
--rw-r--r--   0 runner     (501) staff       (20)     5180 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/feddyn_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5063 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     6274 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/mime_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4026 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer_tag_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)     5805 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:28.000000 fedml-0.8.3a9/fedml/model/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:30.000000 fedml-0.8.3a9/fedml/model/linear/
--rw-r--r--   0 runner     (501) staff       (20)      433 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/linear/lr.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/linear/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      544 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/linear/lr_cifar10.py
--rw-r--r--   0 runner     (501) staff       (20)       52 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4549 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/model_hub.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:30.000000 fedml-0.8.3a9/fedml/model/mobile/
--rw-r--r--   0 runner     (501) staff       (20)      988 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/mobile/mnn_lenet.py
--rw-r--r--   0 runner     (501) staff       (20)     3860 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/mobile/mnn_resnet.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/mobile/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      774 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/mobile/torch_lenet.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:30.000000 fedml-0.8.3a9/fedml/model/nlp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/nlp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6272 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/nlp/model_args.py
--rw-r--r--   0 runner     (501) staff       (20)     4687 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/nlp/rnn.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:30.000000 fedml-0.8.3a9/fedml/model/finance/
--rw-r--r--   0 runner     (501) staff       (20)      458 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/finance/vfl_feature_extractor.py
--rw-r--r--   0 runner     (501) staff       (20)     2385 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/finance/vfl_models_standalone.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/finance/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      354 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/finance/vfl_classifier.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:29.000000 fedml-0.8.3a9/fedml/model/cv/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:29.000000 fedml-0.8.3a9/fedml/model/cv/resnet56/
--rw-r--r--   0 runner     (501) staff       (20)     9541 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet56/resnet_pretrained.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet56/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8241 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet56/resnet_server.py
--rw-r--r--   0 runner     (501) staff       (20)     9507 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet56/resnet_client.py
--rw-r--r--   0 runner     (501) staff       (20)     6216 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/vgg.py
--rw-r--r--   0 runner     (501) staff       (20)      455 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/test_cnn.py
--rw-r--r--   0 runner     (501) staff       (20)    16186 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet_torch.py
--rw-r--r--   0 runner     (501) staff       (20)    25891 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/efficientnet_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7751 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet_cifar.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10352 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/mobilenet_v3.py
--rw-r--r--   0 runner     (501) staff       (20)    19954 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/batchnorm_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7629 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/cnn.py
--rw-r--r--   0 runner     (501) staff       (20)     1590 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/mnist_gan.py
--rw-r--r--   0 runner     (501) staff       (20)    17984 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/efficientnet.py
--rw-r--r--   0 runner     (501) staff       (20)    25096 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet_all.py
--rw-r--r--   0 runner     (501) staff       (20)     4593 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/mobilenet.py
--rw-r--r--   0 runner     (501) staff       (20)    74592 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/common.py
--rw-r--r--   0 runner     (501) staff       (20)    10274 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:29.000000 fedml-0.8.3a9/fedml/model/cv/darts/
--rw-r--r--   0 runner     (501) staff       (20)     7088 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/model_search_gdas.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1713 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/visualize.py
--rw-r--r--   0 runner     (501) staff       (20)    18693 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/architect.py
--rw-r--r--   0 runner     (501) staff       (20)     7681 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/model.py
--rw-r--r--   0 runner     (501) staff       (20)     4504 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/operations.py
--rw-r--r--   0 runner     (501) staff       (20)     3268 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/utils.py
--rw-r--r--   0 runner     (501) staff       (20)    12302 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/model_search.py
--rw-r--r--   0 runner     (501) staff       (20)     8673 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/train.py
--rw-r--r--   0 runner     (501) staff       (20)     3486 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/genotypes.py
--rw-r--r--   0 runner     (501) staff       (20)    14555 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/darts/train_search.py
--rw-r--r--   0 runner     (501) staff       (20)     7625 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/resnet_gn.py
--rw-r--r--   0 runner     (501) staff       (20)     5343 2023-04-13 14:43:24.000000 fedml-0.8.3a9/fedml/model/cv/group_normalization.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/device/
--rw-r--r--   0 runner     (501) staff       (20)     2833 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/device/gpu_mapping_cross_silo.py
--rw-r--r--   0 runner     (501) staff       (20)     3632 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/device/gpu_mapping_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)     5611 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/device/device.py
--rw-r--r--   0 runner     (501) staff       (20)      112 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      346 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/device/ip_config_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/fa/
--rw-r--r--   0 runner     (501) staff       (20)     1817 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/runner.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/fa/cross_silo/
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/fa_server.py
--rw-r--r--   0 runner     (501) staff       (20)      645 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/fa_client.py
--rw-r--r--   0 runner     (501) staff       (20)      186 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/fa/cross_silo/server/
--rw-r--r--   0 runner     (501) staff       (20)     2182 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11137 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     5135 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      879 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/cross_silo/server/server_initializer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/
--rw-r--r--   0 runner     (501) staff       (20)     1526 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/message_define.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1853 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/fa_local_analyzer.py
--rw-r--r--   0 runner     (501) staff       (20)     1960 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     5993 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/cross_silo/client/fedml_client_master_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/fa/aggregator/
--rw-r--r--   0 runner     (501) staff       (20)     1903 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/aggregator/frequency_estimation_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1885 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/aggregator/intersection_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1559 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/aggregator/union_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2114 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/aggregator/avg_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3908 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/aggregator/k_percentile_element_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/aggregator/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1163 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/aggregator/global_analyzer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:26.000000 fedml-0.8.3a9/fedml/fa/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:26.000000 fedml-0.8.3a9/fedml/fa/simulation/sp/
--rw-r--r--   0 runner     (501) staff       (20)     1192 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/simulation/sp/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/simulation/sp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3316 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/fa/simulation/sp/simulator.py
--rw-r--r--   0 runner     (501) staff       (20)      119 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/simulation/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      606 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/fa/simulation/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2832 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/fa/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:26.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/
--rw-r--r--   0 runner     (501) staff       (20)     4574 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/heavy_hitter_triehh.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      453 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/frequency_estimation.py
--rw-r--r--   0 runner     (501) staff       (20)     1245 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/client_analyzer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)      392 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/k_percentage_element.py
--rw-r--r--   0 runner     (501) staff       (20)      223 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/intersection.py
--rw-r--r--   0 runner     (501) staff       (20)      217 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/union.py
--rw-r--r--   0 runner     (501) staff       (20)      348 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/local_analyzer/avg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/fa/base_frame/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/base_frame/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      527 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/base_frame/server_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      911 2023-04-13 14:43:21.000000 fedml-0.8.3a9/fedml/fa/base_frame/client_analyzer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:26.000000 fedml-0.8.3a9/fedml/fa/data/
--rw-r--r--   0 runner     (501) staff       (20)     2564 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/data/data_loader.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:26.000000 fedml-0.8.3a9/fedml/fa/data/twitter_Sentiment140/
--rw-r--r--   0 runner     (501) staff       (20)      932 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/data/twitter_Sentiment140/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/data/twitter_Sentiment140/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       75 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      927 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/data/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:26.000000 fedml-0.8.3a9/fedml/fa/data/fake_numeric_data/
--rw-r--r--   0 runner     (501) staff       (20)      526 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/data/fake_numeric_data/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:22.000000 fedml-0.8.3a9/fedml/fa/data/fake_numeric_data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      545 2023-04-13 14:43:23.000000 fedml-0.8.3a9/fedml/launch_cross_device.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/data/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:22.000000 fedml-0.8.3a9/fedml/data/MNIST/
--rw-r--r--   0 runner     (501) staff       (20)     5448 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/MNIST/mnist_mobile_preprocessor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     4826 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/MNIST/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/MNIST/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/MNIST/stats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:24.000000 fedml-0.8.3a9/fedml/data/lending_club_loan/
--rw-r--r--   0 runner     (501) staff       (20)     7729 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/lending_club_loan/lending_club_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/lending_club_loan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2291 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/lending_club_loan/lending_club_feature_group.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/fed_cifar100/
--rw-r--r--   0 runner     (501) staff       (20)     6320 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fed_cifar100/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fed_cifar100/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      517 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fed_cifar100/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     2631 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fed_cifar100/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:21.000000 fedml-0.8.3a9/fedml/data/FederatedEMNIST/
--rw-r--r--   0 runner     (501) staff       (20)     6737 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/FederatedEMNIST/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/FederatedEMNIST/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      426 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/FederatedEMNIST/dataset.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/cifar100/
--rw-r--r--   0 runner     (501) staff       (20)    11837 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar100/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2077 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar100/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar100/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    21968 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)      156 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/file_operation.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:24.000000 fedml-0.8.3a9/fedml/data/shakespeare/
--rwxr-xr-x   0 runner     (501) staff       (20)     3431 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/shakespeare/language_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4135 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/shakespeare/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/shakespeare/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      335 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/shakespeare/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/shakespeare/stats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/data/synthetic_1_1/
--rw-r--r--   0 runner     (501) staff       (20)     4562 2023-04-13 14:43:19.000000 fedml-0.8.3a9/fedml/data/synthetic_1_1/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:19.000000 fedml-0.8.3a9/fedml/data/synthetic_1_1/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3210 2023-04-13 14:43:20.000000 fedml-0.8.3a9/fedml/data/synthetic_1_1/stats.py
--rw-r--r--   0 runner     (501) staff       (20)     2749 2023-04-13 14:43:19.000000 fedml-0.8.3a9/fedml/data/synthetic_1_1/generate_synthetic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:22.000000 fedml-0.8.3a9/fedml/data/Landmarks/
--rw-r--r--   0 runner     (501) staff       (20)      375 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/Landmarks/download_with_tff.py
--rw-r--r--   0 runner     (501) staff       (20)    14871 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/Landmarks/download_without_tff.py
--rw-r--r--   0 runner     (501) staff       (20)    11159 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/Landmarks/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2191 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/Landmarks/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/Landmarks/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    14342 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/Landmarks/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2090 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/Landmarks/check_download.py
--rw-r--r--   0 runner     (501) staff       (20)     7872 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/Landmarks/download_without_tf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/fednlp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fednlp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/fednlp/base/
--rw-r--r--   0 runner     (501) staff       (20)      169 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fednlp/base/globals.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:24.000000 fedml-0.8.3a9/fedml/data/fednlp/base/preprocess/
--rw-r--r--   0 runner     (501) staff       (20)     4794 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/preprocess/base_example.py
--rw-r--r--   0 runner     (501) staff       (20)      363 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/preprocess/base_data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/preprocess/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      224 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/preprocess/base_preprocessor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fednlp/base/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:24.000000 fedml-0.8.3a9/fedml/data/fednlp/base/raw_data/
--rw-r--r--   0 runner     (501) staff       (20)     1428 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/raw_data/partition.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/raw_data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3636 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:24.000000 fedml-0.8.3a9/fedml/data/fednlp/base/data_manager/
--rw-r--r--   0 runner     (501) staff       (20)    16505 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fednlp/base/data_manager/base_data_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fednlp/base/data_manager/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8248 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/fednlp/base/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:22.000000 fedml-0.8.3a9/fedml/data/NUS_WIDE/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/NUS_WIDE/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11281 2023-04-13 14:43:15.000000 fedml-0.8.3a9/fedml/data/NUS_WIDE/nus_wide_dataset.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:24.000000 fedml-0.8.3a9/fedml/data/stackoverflow_lr/
--rw-r--r--   0 runner     (501) staff       (20)     8487 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/stackoverflow_lr/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/stackoverflow_lr/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2841 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/stackoverflow_lr/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     4272 2023-04-13 14:43:18.000000 fedml-0.8.3a9/fedml/data/stackoverflow_lr/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/fed_shakespeare/
--rw-r--r--   0 runner     (501) staff       (20)     6100 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fed_shakespeare/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fed_shakespeare/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3633 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/fed_shakespeare/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:22.000000 fedml-0.8.3a9/fedml/data/ImageNet/
--rw-r--r--   0 runner     (501) staff       (20)    11416 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/ImageNet/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     6718 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/ImageNet/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/ImageNet/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5874 2023-04-13 14:43:14.000000 fedml-0.8.3a9/fedml/data/ImageNet/datasets_hdf5.py
--rw-r--r--   0 runner     (501) staff       (20)     1429 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/data_loader_cross_silo.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/cinic10/
--rw-r--r--   0 runner     (501) staff       (20)    13807 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cinic10/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     3071 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cinic10/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cinic10/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:25.000000 fedml-0.8.3a9/fedml/data/stackoverflow_nwp/
--rw-r--r--   0 runner     (501) staff       (20)     7023 2023-04-13 14:43:19.000000 fedml-0.8.3a9/fedml/data/stackoverflow_nwp/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:19.000000 fedml-0.8.3a9/fedml/data/stackoverflow_nwp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2171 2023-04-13 14:43:19.000000 fedml-0.8.3a9/fedml/data/stackoverflow_nwp/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     2508 2023-04-13 14:43:19.000000 fedml-0.8.3a9/fedml/data/stackoverflow_nwp/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:22.000000 fedml-0.8.3a9/fedml/data/UCI/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/UCI/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6215 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/UCI/data_loader_for_susy_and_ro.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/edge_case_examples/
--rw-r--r--   0 runner     (501) staff       (20)    44697 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/edge_case_examples/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)    20285 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/edge_case_examples/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:17.000000 fedml-0.8.3a9/fedml/data/edge_case_examples/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:23.000000 fedml-0.8.3a9/fedml/data/cifar10/
--rw-r--r--   0 runner     (501) staff       (20)    13825 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar10/efficient_loader.py
--rw-r--r--   0 runner     (501) staff       (20)    11902 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar10/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2378 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar10/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)     3972 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar10/without_reload.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-13 14:43:16.000000 fedml-0.8.3a9/fedml/data/cifar10/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-13 14:45:13.000000 fedml-0.8.3a9/fedml.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3806 2023-04-13 14:45:06.000000 fedml-0.8.3a9/fedml.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    45945 2023-04-13 14:45:06.000000 fedml-0.8.3a9/fedml.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)       45 2023-04-13 14:45:06.000000 fedml-0.8.3a9/fedml.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      595 2023-04-13 14:45:06.000000 fedml-0.8.3a9/fedml.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       21 2023-04-13 14:45:06.000000 fedml-0.8.3a9/fedml.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-13 14:45:06.000000 fedml-0.8.3a9/fedml.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/
+-rw-r--r--   0 runner     (501) staff       (20)     3806 2023-04-27 10:21:01.000000 fedml-0.8.4a1/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/tests/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/tests/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/tests/security/attack/
+-rw-r--r--   0 runner     (501) staff       (20)     1218 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/test_label_flipping_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)      730 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/test_backdoor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/test_model_replacement_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5147 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/test_invertgradient.py
+-rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/test_byzantine_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5519 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      955 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/test_edge_case_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1466 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/attack/test_dlg.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/tests/security/defense/
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_rfa.py
+-rw-r--r--   0 runner     (501) staff       (20)     1942 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_residual_based_reweighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_wbc.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1099 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_crfl.py
+-rw-r--r--   0 runner     (501) staff       (20)     1871 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_geometric_median.py
+-rw-r--r--   0 runner     (501) staff       (20)     2682 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_slsgd_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1327 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_weak_dp.py
+-rw-r--r--   0 runner     (501) staff       (20)     1525 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_norm_diff_clipping.py
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1555 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_bulyan.py
+-rw-r--r--   0 runner     (501) staff       (20)      805 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_robust_learning_rate_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)      999 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_coordinate_wise_trimmed_mean.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1206 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_krum.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      987 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_cclip.py
+-rw-r--r--   0 runner     (501) staff       (20)      390 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_coordinate_median.py
+-rw-r--r--   0 runner     (501) staff       (20)      902 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_foolsgold_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2208 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/security/defense/test_soteria.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2326 2023-04-27 10:20:41.000000 fedml-0.8.4a1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     4574 2023-04-27 10:20:44.000000 fedml-0.8.4a1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2026 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/main_fedml_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)      196 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/mlops_client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2003 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2024 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)     4403 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)     5218 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2033 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2020 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1435 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      757 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      757 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2119 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      827 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      965 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)      827 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)     4098 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1739 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py
+-rw-r--r--   0 runner     (501) staff       (20)     5323 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1999 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2013 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2003 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1993 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     3354 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1387 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)     2007 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py
+-rw-r--r--   0 runner     (501) staff       (20)      699 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      391 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/main_fedml_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_device/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/
+-rw-r--r--   0 runner     (501) staff       (20)     1214 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      801 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_device/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/
+-rw-r--r--   0 runner     (501) staff       (20)     1170 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/centralized/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/centralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    20282 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/centralized/main.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_fedopt_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_fedopt_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_fedopt_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_vertical_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_vertical_mnist_lr_example/torch_vertical_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_vertical_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_fedopt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_fedopt_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_fedopt_mnist_lr_example/torch_fedopt_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_decentralized_fl_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_decentralized_fl_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      222 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_decentralized_fl_example/mpi_decentralized_fl_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_decentralized_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/sp_decentralized_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/sp_decentralized_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/torch_fedgkt_cifar10_resnet56.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     5590 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     4816 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/reddit_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6461 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/main.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_hierarchicalfl_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_hierarchicalfl_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_hierarchicalfl_mnist_lr_example/torch_hierarchicalfl_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedopt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedopt_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedopt_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedgan_mnist_gan_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedgan_mnist_gan_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedgan_mnist_gan_example/torch_fedgan_mnist_gan_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_fedavg_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_fedavg_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_fedavg_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_seq/
+-rw-r--r--   0 runner     (501) staff       (20)      762 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_seq/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_fedprox_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_fedprox_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_fedprox_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      423 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fednas_cifar10_dart_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fednas_cifar10_dart_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fednas_cifar10_dart_example/torch_fednas_cifar10_dart_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/torch_splitnn_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_fednova_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_fednova_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_fednova_mnist_lr_example/torch_fednova_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_base_framework_example/
+-rw-r--r--   0 runner     (501) staff       (20)      222 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_base_framework_example/mpi_base_framework_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_base_framework_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_cnn_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_cnn_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_cnn_example/torch_fedavg_mnist_cnn_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedprox_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedprox_mnist_lr_example/torch_fedprox_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_fedprox_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_turboaggregate_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_turboaggregate_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:44.000000 fedml-0.8.4a1/examples/simulation/sp_turboaggregate_mnist_lr_example/torch_turboaggregate_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_async_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_async_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1042 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_datasets_and_models_example/torch_fedavg_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/simulation/sp_fedavg_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:43.000000 fedml-0.8.4a1/examples/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-27 10:21:01.000000 fedml-0.8.4a1/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/
+-rw-r--r--   0 runner     (501) staff       (20)     1061 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/launch_serving.py
+-rw-r--r--   0 runner     (501) staff       (20)     1078 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/launch_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)     6931 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/runner.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cross_silo/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cross_silo/lightsecagg/
+-rw-r--r--   0 runner     (501) staff       (20)     3009 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)    11077 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/lightsecagg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    13517 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)    12846 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3467 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_api.py
+-rw-r--r--   0 runner     (501) staff       (20)      157 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/cross_silo/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15312 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11613 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1917 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2025 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cross_silo/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7549 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_silo/client/fedml_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1079 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/launch_cross_silo_horizontal.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/serving/
+-rw-r--r--   0 runner     (501) staff       (20)      163 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/serving/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15366 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11613 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1340 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1456 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/serving/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7549 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/serving/client/fedml_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/schedule/
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/schedule/runtime_estimate.py
+-rw-r--r--   0 runner     (501) staff       (20)     9840 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/schedule/seq_train_scheduler.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/schedule/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/alg_frame/
+-rw-r--r--   0 runner     (501) staff       (20)      795 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/alg_frame/params.py
+-rw-r--r--   0 runner     (501) staff       (20)     1855 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/alg_frame/client_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/alg_frame/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      894 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/alg_frame/context.py
+-rw-r--r--   0 runner     (501) staff       (20)     5737 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/alg_frame/server_aggregator.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/topology/
+-rw-r--r--   0 runner     (501) staff       (20)     5001 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/topology/asymmetric_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      479 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/topology/base_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3853 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/topology/symmetric_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/topology/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/crypto/
+-rw-r--r--   0 runner     (501) staff       (20)     2167 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/crypto/crypto_api.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/crypto/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8764 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/fedml_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/
+-rw-r--r--   0 runner     (501) staff       (20)      153 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/observer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/s3/
+-rw-r--r--   0 runner     (501) staff       (20)     1680 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/s3/remote_storage_mnn.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/s3/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    21800 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/s3/remote_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)     2792 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/s3/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mpi/
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mpi/mpi_send_thread.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mpi/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4977 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mpi/com_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1603 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mpi/mpi_receive_thread.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/
+-rw-r--r--   0 runner     (501) staff       (20)     1255 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     6381 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/proto/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/proto/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4236 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py
+-rw-r--r--   0 runner     (501) staff       (20)      346 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/ip_config_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     6272 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/trpc/
+-rw-r--r--   0 runner     (501) staff       (20)     1614 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/trpc/trpc_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/trpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4807 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/trpc/trpc_comm_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/trpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      377 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2612 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/message.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_web3/
+-rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_web3/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14594 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_thetastore/
+-rwxr-xr-x   0 runner     (501) staff       (20)      109 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_thetastore/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14669 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      869 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      518 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/base_com_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3/
+-rwxr-xr-x   0 runner     (501) staff       (20)      123 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    15504 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    13720 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt/mqtt_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3_mnn/
+-rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3_mnn/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    12233 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/web3_storage/
+-rw-r--r--   0 runner     (501) staff       (20)     3604 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/web3_storage/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/theta_storage/
+-rw-r--r--   0 runner     (501) staff       (20)     6834 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/theta_storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/distributed_storage/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/distributed/flow/
+-rw-r--r--   0 runner     (501) staff       (20)    12684 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/flow/fedml_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/flow/fedml_executor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/flow/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      338 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/flow/fedml_flow_constants.py
+-rw-r--r--   0 runner     (501) staff       (20)     3248 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/distributed/flow/test_fedml_flow.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/security/attack/
+-rw-r--r--   0 runner     (501) staff       (20)     4005 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/model_replacement_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)      440 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/attack_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     3424 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/edge_case_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3607 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/byzantine_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6102 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/lazy_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)    27345 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/invert_gradient_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     6066 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/dlg_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     4712 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/revealing_labels_from_gradients_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     2551 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/label_flipping_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5286 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/attack/backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3738 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/fedml_attacker.py
+-rw-r--r--   0 runner     (501) staff       (20)     1208 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7568 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/fedml_defender.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/security/common/
+-rw-r--r--   0 runner     (501) staff       (20)     1973 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/common/bucket.py
+-rw-r--r--   0 runner     (501) staff       (20)      734 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/common/net.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1856 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/common/attack_defense_data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     7488 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/common/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/security/defense/
+-rw-r--r--   0 runner     (501) staff       (20)     8885 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/three_sigma_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2172 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/norm_diff_clipping_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)    10320 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/residual_based_reweighting_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     8375 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/three_sigma_krum_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)      994 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2849 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/slsgd_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1610 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/coordinate_wise_median_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3640 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/wbc_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2675 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/robust_learning_rate_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1071 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/RFA_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1682 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/defense_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     3568 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/foolsgold_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3709 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/soteria_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     5462 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/bulyan_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     4636 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/cross_round_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     6525 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/three_sigma_geomedian_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1988 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/geometric_median_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3054 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/crfl_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/outlier_detection.py
+-rw-r--r--   0 runner     (501) staff       (20)     1008 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/weak_dp_defense.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2650 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/cclip_defense.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2564 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/security/defense/krum_defense.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/mlops/
+-rw-r--r--   0 runner     (501) staff       (20)     8983 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/mlops_configs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/mlops/ssl/
+-rw-r--r--   0 runner     (501) staff       (20)     4089 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)     4085 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)     1947 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/ssl/open-root-ca.crt
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/ssl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4093 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)    21213 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/mlops_metrics.py
+-rw-r--r--   0 runner     (501) staff       (20)     4891 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/mlops_profiler_event.py
+-rw-r--r--   0 runner     (501) staff       (20)     1377 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/mlops_status.py
+-rw-r--r--   0 runner     (501) staff       (20)    33177 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11124 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/stats_impl.py
+-rw-r--r--   0 runner     (501) staff       (20)     1410 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/mlops_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    17257 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/mlops_runtime_log_daemon.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3906 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/system_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     8097 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mlops/mlops_runtime_log.py
+-rw-r--r--   0 runner     (501) staff       (20)     1117 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/common/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      298 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/common/ml_engine_backend.py
+-rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/common/singleton.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/mpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6017 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mpc/lightsecagg.py
+-rw-r--r--   0 runner     (501) staff       (20)    12340 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/mpc/secagg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/dp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/dp/mechanisms/
+-rw-r--r--   0 runner     (501) staff       (20)     1443 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/mechanisms/dp_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)      659 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/mechanisms/laplace.py
+-rw-r--r--   0 runner     (501) staff       (20)       83 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/mechanisms/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      177 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/mechanisms/base_dp_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)     1037 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/mechanisms/gaussian.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/dp/test/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/test/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2532 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/test/test_fed_privacy_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)     4178 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/fedml_differential_privacy.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/dp/frames/
+-rw-r--r--   0 runner     (501) staff       (20)     3293 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/frames/NbAFL.py
+-rw-r--r--   0 runner     (501) staff       (20)     2444 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/frames/dp_clip.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/frames/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1101 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/frames/cdp.py
+-rw-r--r--   0 runner     (501) staff       (20)      470 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/frames/ldp.py
+-rw-r--r--   0 runner     (501) staff       (20)     2118 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/frames/base_dp_solution.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/dp/budget_accountant/
+-rw-r--r--   0 runner     (501) staff       (20)     6747 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/budget_accountant/rdp_analysis.py
+-rw-r--r--   0 runner     (501) staff       (20)     1141 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/budget_accountant/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6915 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/budget_accountant/rdp_accountant.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/dp/common/
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/common/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2411 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/dp/common/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/contribution/
+-rw-r--r--   0 runner     (501) staff       (20)     5603 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/contribution/gtg_shapley_value.py
+-rw-r--r--   0 runner     (501) staff       (20)     3197 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/contribution/mr_shapley_value.py
+-rw-r--r--   0 runner     (501) staff       (20)     1665 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/contribution/base_contribution_assessor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/contribution/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4930 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/contribution/leave_one_out.py
+-rw-r--r--   0 runner     (501) staff       (20)     1922 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/contribution/contribution_assessor_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/core/data/
+-rw-r--r--   0 runner     (501) staff       (20)      158 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4937 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/core/data/noniid_partition.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/distributed/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/distributed/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/config/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/config/simulaton_mpi/
+-rw-r--r--   0 runner     (501) staff       (20)      964 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/config/simulaton_mpi/fedml_config.yaml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/config/simulation_sp/
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/config/simulation_sp/fedml_config.yaml
+-rwxr-xr-x   0 runner     (501) staff       (20)     8038 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/arguments.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/mlops/
+-rw-r--r--   0 runner     (501) staff       (20)     2354 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/mlops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2210 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cross_device/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cross_device/server_mnn/
+-rw-r--r--   0 runner     (501) staff       (20)     2190 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/server_mnn/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/server_mnn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    18567 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/server_mnn/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2772 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/server_mnn/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7827 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/server_mnn/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/server_mnn/server_mnn_api.py
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      579 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cross_device/mnn_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/centralized/
+-rw-r--r--   0 runner     (501) staff       (20)     6588 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/centralized/centralized_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/centralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      685 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/launch_simulation.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedavg/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       34 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12457 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedavg/fedavg_api.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/fedprox/
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedprox/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedprox/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11535 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedprox/fedprox_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7850 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/TA_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/mpc_function.py
+-rw-r--r--   0 runner     (501) staff       (20)      818 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/TA_client.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/feddyn/
+-rw-r--r--   0 runner     (501) staff       (20)     1916 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/feddyn/client copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     1941 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/feddyn/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       42 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/feddyn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    16395 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/feddyn/feddyn_trainer copy.py
+-rw-r--r--   0 runner     (501) staff       (20)    15943 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/feddyn/feddyn_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)     1355 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     3625 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/party_models.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2241 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/vfl.py
+-rw-r--r--   0 runner     (501) staff       (20)    10964 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/vfl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     3887 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/fednova/
+-rw-r--r--   0 runner     (501) staff       (20)     8207 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fednova/fednova.py
+-rw-r--r--   0 runner     (501) staff       (20)    12457 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fednova/fednova_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)    10932 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fednova/fednova_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     6496 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fednova/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fednova/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2258 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fednova/comm_helpers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/fedopt/
+-rw-r--r--   0 runner     (501) staff       (20)    12255 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedopt/fedopt_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     1456 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedopt/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedopt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/fedopt/optrepo.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)     2133 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2391 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/group.py
+-rw-r--r--   0 runner     (501) staff       (20)     4644 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/mime/
+-rw-r--r--   0 runner     (501) staff       (20)     1494 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/mime/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/mime/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3192 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/mime/opt_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    13370 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/mime/mime_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/scaffold/
+-rw-r--r--   0 runner     (501) staff       (20)    13084 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/scaffold/scaffold_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2677 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/scaffold/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       46 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/scaffold/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/sp/decentralized/
+-rw-r--r--   0 runner     (501) staff       (20)     4187 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/decentralized/decentralized_fl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     4328 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/decentralized/client_dsgd.py
+-rw-r--r--   0 runner     (501) staff       (20)     5514 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/decentralized/client_pushsum.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/decentralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5741 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/sp/decentralized/topology_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     2689 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6818 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3602 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAvgAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2542 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4462 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAvgServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/
+-rw-r--r--   0 runner     (501) staff       (20)     2589 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2338 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/SplitNNAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      591 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     1733 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3996 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2043 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/split_nn/server_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2438 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2804 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     7365 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4607 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3460 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxAPI.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/
+-rw-r--r--   0 runner     (501) staff       (20)     4494 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGanServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3809 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGanAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/gan_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      880 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2218 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGANTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     7774 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGANAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2625 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGanClientManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/
+-rw-r--r--   0 runner     (501) staff       (20)    15801 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2120 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/FedGKTAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     3165 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4940 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      671 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/message_def.py
+-rw-r--r--   0 runner     (501) staff       (20)     2925 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     6492 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/
+-rw-r--r--   0 runner     (501) staff       (20)      428 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1858 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1123 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/central_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     1147 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/algorithm_api.py
+-rw-r--r--   0 runner     (501) staff       (20)      438 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/client_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/base_framework/central_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     3409 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4903 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3324 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3531 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2222 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3863 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     7993 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     4779 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4164 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)     3274 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/
+-rw-r--r--   0 runner     (501) staff       (20)     5488 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3489 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    13844 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3079 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5954 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3284 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/
+-rw-r--r--   0 runner     (501) staff       (20)      386 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1112 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     2374 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      738 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/algorithm_api.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)      504 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     7074 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2198 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1801 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     3470 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1842 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/host_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/
+-rw-r--r--   0 runner     (501) staff       (20)    11022 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3767 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2295 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    10792 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      693 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/
+-rw-r--r--   0 runner     (501) staff       (20)     3490 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     5687 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4893 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)    10695 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3306 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fednova/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/
+-rw-r--r--   0 runner     (501) staff       (20)     8893 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      578 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2663 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/optrepo.py
+-rw-r--r--   0 runner     (501) staff       (20)     3297 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1307 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4470 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/
+-rw-r--r--   0 runner     (501) staff       (20)     3300 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    12025 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1009 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     4464 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/optrepo.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1307 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5535 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/
+-rw-r--r--   0 runner     (501) staff       (20)     3507 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      716 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     1927 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     6138 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/MyModelTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12406 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)    10700 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2448 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     4172 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      205 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     9847 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/simulation/simulator.py
+-rw-r--r--   0 runner     (501) staff       (20)    14606 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/utils/
+-rw-r--r--   0 runner     (501) staff       (20)    10317 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/utils/model_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      735 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/utils/logging.py
+-rw-r--r--   0 runner     (501) staff       (20)    10524 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/utils/compression.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/utils/context.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/
+-rwxr-xr-x   0 runner     (501) staff       (20)      313 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/cli_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)    14236 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/client_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    11063 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/client_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2266 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/client_daemon.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5658 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/docker_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    52330 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/client_runner.py
+-rw-r--r--   0 runner     (501) staff       (20)    15185 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/client_constants.py
+-rw-r--r--   0 runner     (501) staff       (20)    10779 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/client_diagnosis.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1969 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/client_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3126 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/edge_deployment/simulator_daemon.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/model_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)     5427 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_inference.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2320 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_client_daemon.py
+-rw-r--r--   0 runner     (501) staff       (20)     7935 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/modelops_configs.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_server_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    73746 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_server_runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    25696 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_cards.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_client_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5426 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/docker_client_login.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    16417 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_server_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    16754 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_cache.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    32464 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_deployment.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      816 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_server_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1766 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_object.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    26434 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_db.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6554 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_login_entry.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14992 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_client_data_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)    19913 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_server_constants.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     8168 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_monitor.py
+-rw-r--r--   0 runner     (501) staff       (20)    25461 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_client_constants.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    46387 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_client_runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5460 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/docker_server_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2986 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_server_daemon.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6819 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_client_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2759 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_msg_object.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2906 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/model_deployment/device_model_inference_entry.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/env/
+-rw-r--r--   0 runner     (501) staff       (20)     3453 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/env/collect_env.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/env/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    45366 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/cli.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      629 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/torch_client.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      650 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/comm_utils/
+-rw-r--r--   0 runner     (501) staff       (20)    24706 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/comm_utils/sys_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/comm_utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      295 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/comm_utils/yaml_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/server_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)      749 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/server_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    71491 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/server_runner.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2848 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/job_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5692 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/docker_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1971 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/server_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    10533 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/app_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2522 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/server_daemon.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cli/server_deployment/templates/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/templates/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/templates/fedml-aggregator-data-pv.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      279 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/templates/fedml-aggregator-data-pvc.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      275 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/templates/fedml-server-svc.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     1370 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml
+-rwxr-xr-x   0 runner     (501) staff       (20)    13814 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/server_login.py
+-rw-r--r--   0 runner     (501) staff       (20)    14281 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cli/server_deployment/server_constants.py
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/launch_cheeath_llm.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/ml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/ml/aggregator/
+-rw-r--r--   0 runner     (501) staff       (20)      548 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/aggregator_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2488 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4187 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/default_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5621 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2408 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)    10546 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/agg_operator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3388 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/ml/engine/
+-rw-r--r--   0 runner     (501) staff       (20)    11319 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/engine/ml_engine_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/engine/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1345 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/engine/torch_process_group_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/ml/trainer/
+-rw-r--r--   0 runner     (501) staff       (20)     3953 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/scaffold_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      580 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/trainer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)     9496 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/fednova_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/local_optimizer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5923 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/fedprox_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3578 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     6857 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/feddyn_trainer copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     5180 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/feddyn_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5063 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     6274 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/mime_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4026 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer_tag_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)     5805 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/linear/
+-rw-r--r--   0 runner     (501) staff       (20)      433 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/linear/lr.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/linear/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      544 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/linear/lr_cifar10.py
+-rw-r--r--   0 runner     (501) staff       (20)       52 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4549 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/model_hub.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/mobile/
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/mobile/mnn_lenet.py
+-rw-r--r--   0 runner     (501) staff       (20)     3860 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/mobile/mnn_resnet.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/mobile/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      774 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/mobile/torch_lenet.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/nlp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/nlp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6272 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/nlp/model_args.py
+-rw-r--r--   0 runner     (501) staff       (20)     4687 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/nlp/rnn.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/finance/
+-rw-r--r--   0 runner     (501) staff       (20)      458 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/finance/vfl_feature_extractor.py
+-rw-r--r--   0 runner     (501) staff       (20)     2385 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/finance/vfl_models_standalone.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/finance/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      354 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/finance/vfl_classifier.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/cv/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/cv/resnet56/
+-rw-r--r--   0 runner     (501) staff       (20)     9541 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet56/resnet_pretrained.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet56/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8241 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet56/resnet_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     9507 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet56/resnet_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     6216 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/vgg.py
+-rw-r--r--   0 runner     (501) staff       (20)      455 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/test_cnn.py
+-rw-r--r--   0 runner     (501) staff       (20)    16186 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet_torch.py
+-rw-r--r--   0 runner     (501) staff       (20)    25891 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/efficientnet_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7751 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10352 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/mobilenet_v3.py
+-rw-r--r--   0 runner     (501) staff       (20)    19954 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/batchnorm_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7629 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/cnn.py
+-rw-r--r--   0 runner     (501) staff       (20)     1590 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/mnist_gan.py
+-rw-r--r--   0 runner     (501) staff       (20)    17984 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/efficientnet.py
+-rw-r--r--   0 runner     (501) staff       (20)    25096 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet_all.py
+-rw-r--r--   0 runner     (501) staff       (20)     4593 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/mobilenet.py
+-rw-r--r--   0 runner     (501) staff       (20)    74592 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/common.py
+-rw-r--r--   0 runner     (501) staff       (20)    10274 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/model/cv/darts/
+-rw-r--r--   0 runner     (501) staff       (20)     7088 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/model_search_gdas.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1713 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/visualize.py
+-rw-r--r--   0 runner     (501) staff       (20)    18693 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/architect.py
+-rw-r--r--   0 runner     (501) staff       (20)     7681 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     4504 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/operations.py
+-rw-r--r--   0 runner     (501) staff       (20)     3268 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    12302 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/model_search.py
+-rw-r--r--   0 runner     (501) staff       (20)     8673 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/train.py
+-rw-r--r--   0 runner     (501) staff       (20)     3486 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/genotypes.py
+-rw-r--r--   0 runner     (501) staff       (20)    14555 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/darts/train_search.py
+-rw-r--r--   0 runner     (501) staff       (20)     7625 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/resnet_gn.py
+-rw-r--r--   0 runner     (501) staff       (20)     5343 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/model/cv/group_normalization.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/device/
+-rw-r--r--   0 runner     (501) staff       (20)     2833 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/device/gpu_mapping_cross_silo.py
+-rw-r--r--   0 runner     (501) staff       (20)     3632 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/device/gpu_mapping_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)     5611 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/device/device.py
+-rw-r--r--   0 runner     (501) staff       (20)      112 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      346 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/device/ip_config_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cheetah_llm/
+-rw-r--r--   0 runner     (501) staff       (20)      159 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cheetah_llm/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15366 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11613 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1942 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2050 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7549 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/cheetah_llm/client/fedml_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/
+-rw-r--r--   0 runner     (501) staff       (20)     1817 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/runner.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/cross_silo/
+-rw-r--r--   0 runner     (501) staff       (20)      674 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/fa_server.py
+-rw-r--r--   0 runner     (501) staff       (20)      645 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/fa_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      186 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/cross_silo/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2182 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11137 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     5135 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      879 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/server/server_initializer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/
+-rw-r--r--   0 runner     (501) staff       (20)     1526 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/message_define.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1853 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/fa_local_analyzer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1960 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     5993 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/cross_silo/client/fedml_client_master_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/aggregator/
+-rw-r--r--   0 runner     (501) staff       (20)     1903 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/aggregator/frequency_estimation_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1885 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/aggregator/intersection_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1559 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/aggregator/union_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2114 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/aggregator/avg_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3908 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/aggregator/k_percentile_element_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/aggregator/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1163 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/aggregator/global_analyzer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)      414 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/simulation/sp/
+-rw-r--r--   0 runner     (501) staff       (20)     1192 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/simulation/sp/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/simulation/sp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3316 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/simulation/sp/simulator.py
+-rw-r--r--   0 runner     (501) staff       (20)      119 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/simulation/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      606 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/simulation/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2832 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/
+-rw-r--r--   0 runner     (501) staff       (20)     4574 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/heavy_hitter_triehh.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      453 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/frequency_estimation.py
+-rw-r--r--   0 runner     (501) staff       (20)     1245 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/client_analyzer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)      392 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/k_percentage_element.py
+-rw-r--r--   0 runner     (501) staff       (20)      223 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/intersection.py
+-rw-r--r--   0 runner     (501) staff       (20)      217 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/union.py
+-rw-r--r--   0 runner     (501) staff       (20)      348 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/local_analyzer/avg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/base_frame/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/base_frame/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      527 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/base_frame/server_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      911 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/base_frame/client_analyzer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/data/
+-rw-r--r--   0 runner     (501) staff       (20)     2564 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/data/data_loader.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/data/twitter_Sentiment140/
+-rw-r--r--   0 runner     (501) staff       (20)      932 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/data/twitter_Sentiment140/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/data/twitter_Sentiment140/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       75 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      927 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/data/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/fa/data/fake_numeric_data/
+-rw-r--r--   0 runner     (501) staff       (20)      526 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/data/fake_numeric_data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/fa/data/fake_numeric_data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      545 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/launch_cross_device.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/MNIST/
+-rw-r--r--   0 runner     (501) staff       (20)     5448 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/MNIST/mnist_mobile_preprocessor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4826 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/MNIST/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/MNIST/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/MNIST/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/lending_club_loan/
+-rw-r--r--   0 runner     (501) staff       (20)     7729 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/lending_club_loan/lending_club_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/lending_club_loan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2291 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/lending_club_loan/lending_club_feature_group.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/fed_cifar100/
+-rw-r--r--   0 runner     (501) staff       (20)     6320 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fed_cifar100/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fed_cifar100/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      517 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fed_cifar100/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2631 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fed_cifar100/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/FederatedEMNIST/
+-rw-r--r--   0 runner     (501) staff       (20)     6737 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/FederatedEMNIST/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/FederatedEMNIST/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      426 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/FederatedEMNIST/dataset.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/cifar100/
+-rw-r--r--   0 runner     (501) staff       (20)    11837 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar100/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2077 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar100/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar100/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    21968 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)      156 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/file_operation.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/shakespeare/
+-rwxr-xr-x   0 runner     (501) staff       (20)     3431 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/shakespeare/language_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4135 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/shakespeare/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/shakespeare/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      335 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/shakespeare/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/shakespeare/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/synthetic_1_1/
+-rw-r--r--   0 runner     (501) staff       (20)     4562 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/synthetic_1_1/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/synthetic_1_1/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3210 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/synthetic_1_1/stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     2749 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/synthetic_1_1/generate_synthetic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/Landmarks/
+-rw-r--r--   0 runner     (501) staff       (20)      375 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/download_with_tff.py
+-rw-r--r--   0 runner     (501) staff       (20)    14871 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/download_without_tff.py
+-rw-r--r--   0 runner     (501) staff       (20)    11159 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2191 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14342 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2090 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/check_download.py
+-rw-r--r--   0 runner     (501) staff       (20)     7872 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/Landmarks/download_without_tf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/fednlp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/fednlp/base/
+-rw-r--r--   0 runner     (501) staff       (20)      169 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/globals.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/fednlp/base/preprocess/
+-rw-r--r--   0 runner     (501) staff       (20)     4794 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/preprocess/base_example.py
+-rw-r--r--   0 runner     (501) staff       (20)      363 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/preprocess/base_data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/preprocess/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      224 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/preprocess/base_preprocessor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/fednlp/base/raw_data/
+-rw-r--r--   0 runner     (501) staff       (20)     1428 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/raw_data/partition.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/raw_data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3636 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/fednlp/base/data_manager/
+-rw-r--r--   0 runner     (501) staff       (20)    16505 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/data_manager/base_data_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/data_manager/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8248 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fednlp/base/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/NUS_WIDE/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/NUS_WIDE/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11281 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/NUS_WIDE/nus_wide_dataset.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/stackoverflow_lr/
+-rw-r--r--   0 runner     (501) staff       (20)     8487 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_lr/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_lr/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2841 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_lr/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     4272 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_lr/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/fed_shakespeare/
+-rw-r--r--   0 runner     (501) staff       (20)     6100 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fed_shakespeare/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fed_shakespeare/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/fed_shakespeare/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/ImageNet/
+-rw-r--r--   0 runner     (501) staff       (20)    11416 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/ImageNet/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     6718 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/ImageNet/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/ImageNet/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5874 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/ImageNet/datasets_hdf5.py
+-rw-r--r--   0 runner     (501) staff       (20)     1429 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/data_loader_cross_silo.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/cinic10/
+-rw-r--r--   0 runner     (501) staff       (20)    13807 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cinic10/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     3071 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cinic10/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cinic10/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/stackoverflow_nwp/
+-rw-r--r--   0 runner     (501) staff       (20)     7023 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_nwp/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_nwp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2171 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_nwp/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2508 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/stackoverflow_nwp/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/UCI/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/UCI/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6215 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/UCI/data_loader_for_susy_and_ro.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/edge_case_examples/
+-rw-r--r--   0 runner     (501) staff       (20)    44697 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/edge_case_examples/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)    20285 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/edge_case_examples/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/edge_case_examples/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:01.000000 fedml-0.8.4a1/fedml/data/cifar10/
+-rw-r--r--   0 runner     (501) staff       (20)    13825 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar10/efficient_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)    11902 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar10/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2378 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar10/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)     3972 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar10/without_reload.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 10:20:44.000000 fedml-0.8.4a1/fedml/data/cifar10/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3806 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    47555 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)       45 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      588 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       21 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-27 10:21:00.000000 fedml-0.8.4a1/fedml.egg-info/dependency_links.txt
```

### Comparing `fedml-0.8.3a9/PKG-INFO` & `fedml-0.8.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml
-Version: 0.8.3a9
+Version: 0.8.4a1
 Summary: A research and production integrated edge-cloud library for federated/distributed machine learning at anywhere at any scale.
 Home-page: https://github.com/FedML-AI/FedML
 Author: FedML Team
 Author-email: ch@fedml.ai
 License: Apache 2.0
 Description: # FedML - The community building and connecting AI anywhere at any scale
```

### Comparing `fedml-0.8.3a9/tests/security/attack/test_label_flipping_attack.py` & `fedml-0.8.4a1/tests/security/attack/test_label_flipping_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/attack/test_backdoor.py` & `fedml-0.8.4a1/tests/security/attack/test_backdoor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/attack/test_model_replacement_backdoor_attack.py` & `fedml-0.8.4a1/tests/security/attack/test_model_replacement_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/attack/test_invertgradient.py` & `fedml-0.8.4a1/tests/security/attack/test_invertgradient.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/attack/test_byzantine_attack.py` & `fedml-0.8.4a1/tests/security/attack/test_byzantine_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/attack/utils.py` & `fedml-0.8.4a1/tests/security/attack/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/attack/test_edge_case_backdoor_attack.py` & `fedml-0.8.4a1/tests/security/attack/test_edge_case_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/attack/test_dlg.py` & `fedml-0.8.4a1/tests/security/attack/test_dlg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_residual_based_reweighting.py` & `fedml-0.8.4a1/tests/security/defense/test_residual_based_reweighting.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_wbc.py` & `fedml-0.8.4a1/tests/security/defense/test_wbc.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_crfl.py` & `fedml-0.8.4a1/tests/security/defense/test_crfl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_geometric_median.py` & `fedml-0.8.4a1/tests/security/defense/test_geometric_median.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_slsgd_defense.py` & `fedml-0.8.4a1/tests/security/defense/test_slsgd_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_weak_dp.py` & `fedml-0.8.4a1/tests/security/defense/test_weak_dp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_norm_diff_clipping.py` & `fedml-0.8.4a1/tests/security/defense/test_norm_diff_clipping.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/utils.py` & `fedml-0.8.4a1/tests/security/defense/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_bulyan.py` & `fedml-0.8.4a1/tests/security/defense/test_bulyan.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_robust_learning_rate_defense.py` & `fedml-0.8.4a1/tests/security/defense/test_robust_learning_rate_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_coordinate_wise_trimmed_mean.py` & `fedml-0.8.4a1/tests/security/defense/test_coordinate_wise_trimmed_mean.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_krum.py` & `fedml-0.8.4a1/tests/security/defense/test_krum.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_cclip.py` & `fedml-0.8.4a1/tests/security/defense/test_cclip.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_foolsgold_defense.py` & `fedml-0.8.4a1/tests/security/defense/test_foolsgold_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/tests/security/defense/test_soteria.py` & `fedml-0.8.4a1/tests/security/defense/test_soteria.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/README.md` & `fedml-0.8.4a1/README.md`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/setup.py` & `fedml-0.8.4a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,27 @@
             self.universal = True
             _bdist_wheel.finalize_options(self)
 
 except ImportError:
     bdist_wheel = None
 
 requirements = [
-    "numpy>=1.21,<=1.23",
+    "numpy>=1.21",
     "PyYAML",
     "h5py",
     "tqdm",
     "wget",
     "paho-mqtt",
     "boto3",
     "pynvml",
     "scikit-learn",
     "networkx",
     "click",
-    "torch==1.13.1",
-    "torchvision==0.14.1",
+    "torch>=1.13.1",
+    "torchvision>=0.14.1",
     "spacy",
     "gensim",
     "multiprocess",
     "smart-open==6.3.0",
     "nvidia-ml-py3",
     "matplotlib",
     "dill",
@@ -85,15 +85,15 @@
 
 
 # if platform.machine() == "x86_64":
 #    requirements.append("MNN==1.1.6")
 
 setup(
     name="fedml",
-    version="0.8.3a9",
+    version="0.8.4a1",
     author="FedML Team",
     author_email="ch@fedml.ai",
     description="A research and production integrated edge-cloud library for "
                 "federated/distributed machine learning at anywhere at any scale.",
     long_description=io.open(os.path.join("README.md"), "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/FedML-AI/FedML",
```

### Comparing `fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.4a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py` & `fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py` & `fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py` & `fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py` & `fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py` & `fedml-0.8.4a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py` & `fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py` & `fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py` & `fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py` & `fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py` & `fedml-0.8.4a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py` & `fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py` & `fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py` & `fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py` & `fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py` & `fedml-0.8.4a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py` & `fedml-0.8.4a1/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py` & `fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py` & `fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py` & `fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py` & `fedml-0.8.4a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/centralized/main.py` & `fedml-0.8.4a1/examples/centralized/main.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/reddit_trainer.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/reddit_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg/main.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg/main.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.4a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.4a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.4a1/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/launch_cross_silo_hi.py` & `fedml-0.8.4a1/fedml/launch_cross_silo_hi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_message_define.py` & `fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py` & `fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py` & `fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py` & `fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/lightsecagg/lsa_fedml_api.py` & `fedml-0.8.4a1/fedml/cross_silo/lightsecagg/lsa_fedml_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/server/message_define.py` & `fedml-0.8.4a1/fedml/cross_silo/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/server/fedml_server_manager.py` & `fedml-0.8.4a1/fedml/serving/server/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/server/fedml_aggregator.py` & `fedml-0.8.4a1/fedml/cross_silo/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/server/server_initializer.py` & `fedml-0.8.4a1/fedml/cross_silo/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/fedml_client.py` & `fedml-0.8.4a1/fedml/cross_silo/fedml_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/fedml_server.py` & `fedml-0.8.4a1/fedml/cross_silo/fedml_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/client_initializer.py` & `fedml-0.8.4a1/fedml/cross_silo/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/client_launcher.py` & `fedml-0.8.4a1/fedml/cross_silo/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/message_define.py` & `fedml-0.8.4a1/fedml/cross_silo/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.4a1/fedml/cross_silo/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/fedml_client_slave_manager.py` & `fedml-0.8.4a1/fedml/cross_silo/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/process_group_manager.py` & `fedml-0.8.4a1/fedml/cross_silo/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/utils.py` & `fedml-0.8.4a1/fedml/cross_silo/client/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/fedml_client_master_manager.py` & `fedml-0.8.4a1/fedml/cross_silo/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_silo/client/fedml_trainer.py` & `fedml-0.8.4a1/fedml/cross_silo/client/fedml_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/launch_cross_silo_horizontal.py` & `fedml-0.8.4a1/fedml/launch_cross_silo_horizontal.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/schedule/runtime_estimate.py` & `fedml-0.8.4a1/fedml/core/schedule/runtime_estimate.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/schedule/seq_train_scheduler.py` & `fedml-0.8.4a1/fedml/core/schedule/seq_train_scheduler.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/alg_frame/params.py` & `fedml-0.8.4a1/fedml/core/alg_frame/params.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/alg_frame/client_trainer.py` & `fedml-0.8.4a1/fedml/core/alg_frame/client_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/alg_frame/context.py` & `fedml-0.8.4a1/fedml/core/alg_frame/context.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/alg_frame/server_aggregator.py` & `fedml-0.8.4a1/fedml/core/alg_frame/server_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/topology/asymmetric_topology_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/topology/asymmetric_topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/topology/symmetric_topology_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/topology/symmetric_topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/crypto/crypto_api.py` & `fedml-0.8.4a1/fedml/core/distributed/crypto/crypto_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/fedml_comm_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/fedml_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/s3/remote_storage_mnn.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/s3/remote_storage_mnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/s3/remote_storage.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/s3/remote_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/s3/utils.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/s3/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mpi/mpi_send_thread.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mpi/mpi_send_thread.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mpi/com_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mpi/com_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mpi/mpi_receive_thread.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mpi/mpi_receive_thread.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_server.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_comm_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/trpc/trpc_server.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/trpc/trpc_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/trpc/trpc_comm_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/trpc/trpc_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/message.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/message.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/utils.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/base_com_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/base_com_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mqtt/mqtt_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mqtt/mqtt_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py` & `fedml-0.8.4a1/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py` & `fedml-0.8.4a1/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py` & `fedml-0.8.4a1/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/flow/fedml_flow.py` & `fedml-0.8.4a1/fedml/core/distributed/flow/fedml_flow.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/flow/fedml_executor.py` & `fedml-0.8.4a1/fedml/core/distributed/flow/fedml_executor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/distributed/flow/test_fedml_flow.py` & `fedml-0.8.4a1/fedml/core/distributed/flow/test_fedml_flow.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/model_replacement_backdoor_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/model_replacement_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/edge_case_backdoor_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/edge_case_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/byzantine_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/byzantine_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/lazy_worker.py` & `fedml-0.8.4a1/fedml/core/security/attack/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/invert_gradient_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/invert_gradient_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/dlg_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/dlg_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/revealing_labels_from_gradients_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/revealing_labels_from_gradients_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/label_flipping_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/label_flipping_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/attack/backdoor_attack.py` & `fedml-0.8.4a1/fedml/core/security/attack/backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/fedml_attacker.py` & `fedml-0.8.4a1/fedml/core/security/fedml_attacker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/constants.py` & `fedml-0.8.4a1/fedml/core/security/constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/fedml_defender.py` & `fedml-0.8.4a1/fedml/core/security/fedml_defender.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/common/bucket.py` & `fedml-0.8.4a1/fedml/core/security/common/bucket.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/common/net.py` & `fedml-0.8.4a1/fedml/core/security/common/net.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/common/attack_defense_data_loader.py` & `fedml-0.8.4a1/fedml/core/security/common/attack_defense_data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/common/utils.py` & `fedml-0.8.4a1/fedml/core/security/common/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/three_sigma_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/three_sigma_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/norm_diff_clipping_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/norm_diff_clipping_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/residual_based_reweighting_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/residual_based_reweighting_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/three_sigma_krum_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/three_sigma_krum_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/slsgd_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/slsgd_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/coordinate_wise_median_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/coordinate_wise_median_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/wbc_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/wbc_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/robust_learning_rate_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/robust_learning_rate_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/RFA_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/RFA_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/defense_base.py` & `fedml-0.8.4a1/fedml/core/security/defense/defense_base.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/foolsgold_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/foolsgold_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/soteria_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/soteria_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/bulyan_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/bulyan_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/cross_round_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/cross_round_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/three_sigma_geomedian_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/three_sigma_geomedian_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/geometric_median_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/geometric_median_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/crfl_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/crfl_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/outlier_detection.py` & `fedml-0.8.4a1/fedml/core/security/defense/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/weak_dp_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/weak_dp_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/cclip_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/cclip_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/security/defense/krum_defense.py` & `fedml-0.8.4a1/fedml/core/security/defense/krum_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/mlops_configs.py` & `fedml-0.8.4a1/fedml/core/mlops/mlops_configs.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt` & `fedml-0.8.4a1/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt` & `fedml-0.8.4a1/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/ssl/open-root-ca.crt` & `fedml-0.8.4a1/fedml/core/mlops/ssl/open-root-ca.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt` & `fedml-0.8.4a1/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/mlops_metrics.py` & `fedml-0.8.4a1/fedml/core/mlops/mlops_metrics.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/mlops_profiler_event.py` & `fedml-0.8.4a1/fedml/core/mlops/mlops_profiler_event.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/mlops_status.py` & `fedml-0.8.4a1/fedml/core/mlops/mlops_status.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/__init__.py` & `fedml-0.8.4a1/fedml/core/mlops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/stats_impl.py` & `fedml-0.8.4a1/fedml/core/mlops/stats_impl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/mlops_utils.py` & `fedml-0.8.4a1/fedml/core/mlops/mlops_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/mlops_runtime_log_daemon.py` & `fedml-0.8.4a1/fedml/core/mlops/mlops_runtime_log_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/system_stats.py` & `fedml-0.8.4a1/fedml/core/mlops/system_stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mlops/mlops_runtime_log.py` & `fedml-0.8.4a1/fedml/core/mlops/mlops_runtime_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         stdout_handle.setFormatter(format_str)
         if show_stdout_log:
             stdout_handle.setLevel(logging.INFO)
             self.logger.setLevel(logging.INFO)
         else:
             stdout_handle.setLevel(logging.CRITICAL)
             self.logger.setLevel(logging.CRITICAL)
+        self.logger.handlers.clear()
         self.logger.addHandler(stdout_handle)
         if hasattr(self, "should_write_log_file") and self.should_write_log_file:
             when = 'D'
             backup_count = 100
             file_handle = handlers.TimedRotatingFileHandler(filename=log_file_path, when=when,
                                                             backupCount=backup_count, encoding='utf-8')
             file_handle.setFormatter(format_str)
```

### Comparing `fedml-0.8.3a9/fedml/core/__init__.py` & `fedml-0.8.4a1/fedml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mpc/lightsecagg.py` & `fedml-0.8.4a1/fedml/core/mpc/lightsecagg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/mpc/secagg.py` & `fedml-0.8.4a1/fedml/core/mpc/secagg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/mechanisms/dp_mechanism.py` & `fedml-0.8.4a1/fedml/core/dp/mechanisms/dp_mechanism.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/mechanisms/laplace.py` & `fedml-0.8.4a1/fedml/core/dp/mechanisms/laplace.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/mechanisms/gaussian.py` & `fedml-0.8.4a1/fedml/core/dp/mechanisms/gaussian.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/test/test_fed_privacy_mechanism.py` & `fedml-0.8.4a1/fedml/core/dp/test/test_fed_privacy_mechanism.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/fedml_differential_privacy.py` & `fedml-0.8.4a1/fedml/core/dp/fedml_differential_privacy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/frames/NbAFL.py` & `fedml-0.8.4a1/fedml/core/dp/frames/NbAFL.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/frames/dp_clip.py` & `fedml-0.8.4a1/fedml/core/dp/frames/dp_clip.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/frames/cdp.py` & `fedml-0.8.4a1/fedml/core/dp/frames/cdp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/frames/base_dp_solution.py` & `fedml-0.8.4a1/fedml/core/dp/frames/base_dp_solution.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/budget_accountant/rdp_analysis.py` & `fedml-0.8.4a1/fedml/core/dp/budget_accountant/rdp_analysis.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/budget_accountant/__init__.py` & `fedml-0.8.4a1/fedml/core/dp/budget_accountant/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/budget_accountant/rdp_accountant.py` & `fedml-0.8.4a1/fedml/core/dp/budget_accountant/rdp_accountant.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/dp/common/utils.py` & `fedml-0.8.4a1/fedml/core/dp/common/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/contribution/gtg_shapley_value.py` & `fedml-0.8.4a1/fedml/core/contribution/gtg_shapley_value.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/contribution/mr_shapley_value.py` & `fedml-0.8.4a1/fedml/core/contribution/mr_shapley_value.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/contribution/base_contribution_assessor.py` & `fedml-0.8.4a1/fedml/core/contribution/base_contribution_assessor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/contribution/leave_one_out.py` & `fedml-0.8.4a1/fedml/core/contribution/leave_one_out.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/contribution/contribution_assessor_manager.py` & `fedml-0.8.4a1/fedml/core/contribution/contribution_assessor_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/core/data/noniid_partition.py` & `fedml-0.8.4a1/fedml/core/data/noniid_partition.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/config/simulaton_mpi/fedml_config.yaml` & `fedml-0.8.4a1/fedml/config/simulaton_mpi/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/config/simulation_sp/fedml_config.yaml` & `fedml-0.8.4a1/fedml/config/simulation_sp/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/arguments.py` & `fedml-0.8.4a1/fedml/arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from .constants import (
     FEDML_TRAINING_PLATFORM_SIMULATION,
     FEDML_SIMULATION_TYPE_MPI,
     FEDML_SIMULATION_TYPE_SP,
     FEDML_TRAINING_PLATFORM_CROSS_SILO,
     FEDML_TRAINING_PLATFORM_CROSS_DEVICE,
     FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL,
+    FEDML_TRAINING_PLATFORM_CHEETAH_LLM,
+    FEDML_TRAINING_PLATFORM_SERVING,
 )
 
 
 def add_args():
     parser = argparse.ArgumentParser(description="FedML")
     parser.add_argument(
         "--yaml_config_file",
@@ -106,14 +108,18 @@
                 print(
                     "training_type == FEDML_TRAINING_PLATFORM_SIMULATION and comm_backend == FEDML_SIMULATION_TYPE_MPI"
                 )
             elif training_type == FEDML_TRAINING_PLATFORM_CROSS_SILO:
                 print("training_type == FEDML_TRAINING_PLATFORM_CROSS_SILO")
             elif training_type == FEDML_TRAINING_PLATFORM_CROSS_DEVICE:
                 print("training_type == FEDML_TRAINING_PLATFORM_CROSS_DEVICE")
+            elif training_type == FEDML_TRAINING_PLATFORM_CHEETAH_LLM:
+                print("training_type == FEDML_TRAINING_PLATFORM_CHEETAH_LLM")
+            elif training_type == FEDML_TRAINING_PLATFORM_SERVING:
+                print("training_type == FEDML_TRAINING_PLATFORM_SERVING")
             else:
                 raise Exception(
                     "no such a platform. training_type = {}, backend = {}".format(
                         training_type, comm_backend
                     )
                 )
 
@@ -139,14 +145,18 @@
                 self.gpu_mapping_file = path.join(
                     path_current_file, "config/simulaton_mpi/gpu_mapping.yaml"
                 )
             elif training_type == FEDML_TRAINING_PLATFORM_CROSS_SILO:
                 pass
             elif training_type == FEDML_TRAINING_PLATFORM_CROSS_DEVICE:
                 pass
+            elif training_type == FEDML_TRAINING_PLATFORM_CHEETAH_LLM:
+                pass
+            elif training_type == FEDML_TRAINING_PLATFORM_SERVING:
+                pass
             else:
                 pass
         
 
         if hasattr(self, "training_type"):
             training_type = self.training_type
```

### Comparing `fedml-0.8.3a9/fedml/mlops/__init__.py` & `fedml-0.8.4a1/fedml/mlops/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import logging
+import traceback
+
 from ..core import mlops
 
 
 def pre_setup(args):
     mlops.pre_setup(args)
 
 
@@ -68,15 +71,18 @@
 
 
 def log_client_model_info(round_index, total_rounds, model_url):
     mlops.log_client_model_info(round_index, total_rounds, model_url)
 
 
 def log_sys_perf(sys_args=None):
-    mlops.log_sys_perf(sys_args)
+    try:
+        mlops.log_sys_perf(sys_args)
+    except Exception as e:
+        logging.info("excpetions when logging sys perf: {}".format(traceback.format_exc()))
 
 
 def log_server_payload(run_id, edge_id, payload):
     mlops.log_server_payload(run_id, edge_id, payload)
 
 
 from ..cli.edge_deployment.client_constants import ClientConstants
```

### Comparing `fedml-0.8.3a9/fedml/constants.py` & `fedml-0.8.4a1/fedml/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # FedML TRAINING PLATFORM
 FEDML_TRAINING_PLATFORM_SIMULATION = "simulation"
 FEDML_TRAINING_PLATFORM_CROSS_SILO = "cross_silo"
 FEDML_TRAINING_PLATFORM_CROSS_DEVICE = "cross_device"
 FEDML_TRAINING_PLATFORM_DISTRIBUTED = "distributed"
+FEDML_TRAINING_PLATFORM_CHEETAH_LLM = "cheetah_llm"
+FEDML_TRAINING_PLATFORM_SERVING = "fedml_serving"
 
 # FedML TRAINING PLATFORM TYPE
 FEDML_TRAINING_PLATFORM_CROSS_SILO_TYPE = 1
 FEDML_TRAINING_PLATFORM_SIMULATION_TYPE = 2
 FEDML_TRAINING_PLATFORM_DISTRIBUTED_TYPE = 3
 FEDML_TRAINING_PLATFORM_CROSS_DEVICE_TYPE = 4
+FEDML_TRAINING_PLATFORM_CHEETAH_LLM_TYPE = 5
+FEDML_TRAINING_PLATFORM_SERVING_TYPE = 6
+
 
 # FedML CROSS-SILO SCENARIO
 FEDML_CROSS_SILO_SCENARIO_HORIZONTAL = "horizontal"
 FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL = "hierarchical"
 
 # FedML SIMULATION TYPE
 FEDML_SIMULATION_TYPE_SP = "sp"
```

### Comparing `fedml-0.8.3a9/fedml/cross_device/server_mnn/message_define.py` & `fedml-0.8.4a1/fedml/cross_device/server_mnn/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_device/server_mnn/fedml_server_manager.py` & `fedml-0.8.4a1/fedml/cross_device/server_mnn/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_device/server_mnn/utils.py` & `fedml-0.8.4a1/fedml/cross_device/server_mnn/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_device/server_mnn/fedml_aggregator.py` & `fedml-0.8.4a1/fedml/cross_device/server_mnn/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_device/server_mnn/server_mnn_api.py` & `fedml-0.8.4a1/fedml/cross_device/server_mnn/server_mnn_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cross_device/mnn_server.py` & `fedml-0.8.4a1/fedml/cross_device/mnn_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/centralized/centralized_trainer.py` & `fedml-0.8.4a1/fedml/centralized/centralized_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/launch_simulation.py` & `fedml-0.8.4a1/fedml/launch_simulation.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fedavg/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/fedavg/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fedavg/fedavg_api.py` & `fedml-0.8.4a1/fedml/simulation/sp/fedavg/fedavg_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fedprox/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/fedprox/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fedprox/fedprox_trainer.py` & `fedml-0.8.4a1/fedml/simulation/sp/fedprox/fedprox_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/TA_trainer.py` & `fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/TA_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/mpc_function.py` & `fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/mpc_function.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/turboaggregate/TA_client.py` & `fedml-0.8.4a1/fedml/simulation/sp/turboaggregate/TA_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/feddyn/client copy.py` & `fedml-0.8.4a1/fedml/simulation/sp/feddyn/client copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/feddyn/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/feddyn/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/feddyn/feddyn_trainer copy.py` & `fedml-0.8.4a1/fedml/simulation/sp/feddyn/feddyn_trainer copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/feddyn/feddyn_trainer.py` & `fedml-0.8.4a1/fedml/simulation/sp/feddyn/feddyn_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/party_models.py` & `fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/party_models.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/vfl.py` & `fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/vfl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/vfl_api.py` & `fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/vfl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py` & `fedml-0.8.4a1/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fednova/fednova.py` & `fedml-0.8.4a1/fedml/simulation/sp/fednova/fednova.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fednova/fednova_trainer.py` & `fedml-0.8.4a1/fedml/simulation/sp/fednova/fednova_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fednova/fednova_api.py` & `fedml-0.8.4a1/fedml/simulation/sp/fednova/fednova_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fednova/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/fednova/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fednova/comm_helpers.py` & `fedml-0.8.4a1/fedml/simulation/sp/fednova/comm_helpers.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fedopt/fedopt_api.py` & `fedml-0.8.4a1/fedml/simulation/sp/fedopt/fedopt_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fedopt/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/fedopt/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/fedopt/optrepo.py` & `fedml-0.8.4a1/fedml/simulation/sp/fedopt/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/group.py` & `fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/group.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/hierarchical_fl/trainer.py` & `fedml-0.8.4a1/fedml/simulation/sp/hierarchical_fl/trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/mime/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/mime/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/mime/opt_utils.py` & `fedml-0.8.4a1/fedml/simulation/sp/mime/opt_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/mime/mime_trainer.py` & `fedml-0.8.4a1/fedml/simulation/sp/mime/mime_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/scaffold/scaffold_trainer.py` & `fedml-0.8.4a1/fedml/simulation/sp/scaffold/scaffold_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/scaffold/client.py` & `fedml-0.8.4a1/fedml/simulation/sp/scaffold/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/decentralized/decentralized_fl_api.py` & `fedml-0.8.4a1/fedml/simulation/sp/decentralized/decentralized_fl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/decentralized/client_dsgd.py` & `fedml-0.8.4a1/fedml/simulation/sp/decentralized/client_dsgd.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/decentralized/client_pushsum.py` & `fedml-0.8.4a1/fedml/simulation/sp/decentralized/client_pushsum.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/sp/decentralized/topology_manager.py` & `fedml-0.8.4a1/fedml/simulation/sp/decentralized/topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAvgClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAVGAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAvgAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAvgAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAVGTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg/FedAvgServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg/FedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/split_nn/server.py` & `fedml-0.8.4a1/fedml/simulation/mpi/split_nn/server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/split_nn/SplitNNAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/split_nn/SplitNNAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/split_nn/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/split_nn/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/split_nn/client.py` & `fedml-0.8.4a1/fedml/simulation/mpi/split_nn/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/split_nn/client_manager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/split_nn/client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/split_nn/server_manager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/split_nn/server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedprox/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedprox/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedprox/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedprox/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedprox/FedProxAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedprox/FedProxAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGanServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGanServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGanAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGanAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/gan_trainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/gan_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGANTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGANTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGANAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGANAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgan/FedGanClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgan/FedGanClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/FedGKTAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/FedGKTAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/message_def.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/message_def.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/base_framework/client_manager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/base_framework/client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/base_framework/central_worker.py` & `fedml-0.8.4a1/fedml/simulation/mpi/base_framework/central_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/base_framework/algorithm_api.py` & `fedml-0.8.4a1/fedml/simulation/mpi/base_framework/algorithm_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/base_framework/central_manager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/base_framework/central_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py` & `fedml-0.8.4a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py` & `fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/decentralized_framework/algorithm_api.py` & `fedml-0.8.4a1/fedml/simulation/mpi/decentralized_framework/algorithm_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py` & `fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/classical_vertical_fl/host_manager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/classical_vertical_fl/host_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednas/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednas/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednas/FedNASServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednas/FedNASServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/FedNovaAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/FedNovaAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fednova/my_model_trainer_classification.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fednova/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/optrepo.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt/FedOptServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt/FedOptServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/optrepo.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegClientManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/message_define.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/MyModelTrainer.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/MyModelTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegAggregator.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/utils.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegAPI.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/mpi/fedseg/FedSegServerManager.py` & `fedml-0.8.4a1/fedml/simulation/mpi/fedseg/FedSegServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/simulation/simulator.py` & `fedml-0.8.4a1/fedml/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/__init__.py` & `fedml-0.8.4a1/fedml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 from .constants import (
     FEDML_TRAINING_PLATFORM_SIMULATION,
     FEDML_SIMULATION_TYPE_SP,
     FEDML_SIMULATION_TYPE_MPI,
     FEDML_SIMULATION_TYPE_NCCL,
     FEDML_TRAINING_PLATFORM_CROSS_SILO,
     FEDML_TRAINING_PLATFORM_CROSS_DEVICE,
+    FEDML_TRAINING_PLATFORM_CHEETAH_LLM,
+    FEDML_TRAINING_PLATFORM_SERVING,
 )
 from .core.common.ml_engine_backend import MLEngineBackend
 
 _global_training_type = None
 _global_comm_backend = None
 
-__version__ = "0.8.3a9"
+__version__ = "0.8.4a1"
 
 
 def init(args=None):
     if args is None:
         args = load_arguments(fedml._global_training_type, fedml._global_comm_backend)
 
     """Initialize FedML Engine."""
@@ -78,14 +80,18 @@
         if args.scenario == "horizontal":
             init_cross_silo_horizontal(args)
         elif args.scenario == "hierarchical":
             args = init_cross_silo_hierarchical(args)
 
     elif args.training_type == FEDML_TRAINING_PLATFORM_CROSS_DEVICE:
         args = init_cross_device(args)
+    elif args.training_type == FEDML_TRAINING_PLATFORM_CHEETAH_LLM:
+        args = init_cheetah_llm(args)
+    elif args.training_type == FEDML_TRAINING_PLATFORM_SERVING:
+        args = init_model_serving(args)
     else:
         raise Exception("no such setting: training_type = {}, backend = {}".format(args.training_type, args.backend))
 
     manage_profiling_args(args)
 
     update_client_id_list(args)
 
@@ -317,14 +323,31 @@
                     args.n_proc_per_node = 1
             else:
                 args.n_proc_per_node = 1
 
     return args
 
 
+def init_cheetah_llm(args):
+    args.n_proc_in_silo = 1
+    args.proc_rank_in_silo = 0
+    manage_mpi_args(args)
+    manage_cuda_rpc_args(args)
+    args.process_id = args.rank
+    return args
+
+
+def init_model_serving(args):
+    args.n_proc_in_silo = 1
+    args.proc_rank_in_silo = 0
+    manage_cuda_rpc_args(args)
+    args.process_id = args.rank
+    return args
+
+
 def update_client_id_list(args):
 
     """
         generate args.client_id_list for CLI mode where args.client_id_list is set to None
         In MLOps mode, args.client_id_list will be set to real-time client id list selected by UI (not starting from 1)
     """
     if not hasattr(args, "using_mlops") or (hasattr(args, "using_mlops") and not args.using_mlops):
@@ -375,14 +398,20 @@
 
 from .launch_cross_silo_horizontal import run_cross_silo_server
 from .launch_cross_silo_horizontal import run_cross_silo_client
 
 from .launch_cross_silo_hi import run_hierarchical_cross_silo_server
 from .launch_cross_silo_hi import run_hierarchical_cross_silo_client
 
+from .launch_cheeath_llm import run_cheetah_llm_server
+from .launch_cheeath_llm import run_cheetah_llm_client
+
+from .launch_serving import run_model_serving_client
+from .launch_serving import run_model_serving_server
+
 from .launch_cross_device import run_mnn_server
 
 from .core.common.ml_engine_backend import MLEngineBackend
 
 from .runner import FedMLRunner
 
 __all__ = [
@@ -393,9 +422,13 @@
     "mlops",
     "FedMLRunner",
     "run_simulation",
     "run_cross_silo_server",
     "run_cross_silo_client",
     "run_hierarchical_cross_silo_server",
     "run_hierarchical_cross_silo_client",
+    "run_cheetah_llm_server",
+    "run_cheetah_llm_client",
+    "run_model_serving_client",
+    "run_model_serving_server",
     "run_mnn_server",
 ]
```

### Comparing `fedml-0.8.3a9/fedml/utils/model_utils.py` & `fedml-0.8.4a1/fedml/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/utils/logging.py` & `fedml-0.8.4a1/fedml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/utils/compression.py` & `fedml-0.8.4a1/fedml/utils/compression.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/utils/context.py` & `fedml-0.8.4a1/fedml/utils/context.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/client_data_interface.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/client_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/client_login.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/client_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/client_daemon.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/client_daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 import argparse
 import os
 import time
+import sys
 
 from fedml.cli.comm_utils.sys_utils import cleanup_all_fedml_client_api_processes, \
-    cleanup_all_fedml_client_learning_processes, cleanup_all_fedml_client_login_processes, get_python_program
+    cleanup_all_fedml_client_learning_processes, cleanup_all_fedml_client_login_processes, get_python_program, \
+    daemon_ota_upgrade
 from fedml.cli.edge_deployment.client_constants import ClientConstants
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--type", "-t", help="Login or logout to MLOps platform")
     parser.add_argument("--user", "-u", type=str,
@@ -28,14 +30,16 @@
             ClientConstants.cleanup_run_process()
             cleanup_all_fedml_client_api_processes()
             cleanup_all_fedml_client_learning_processes()
             cleanup_all_fedml_client_login_processes("client_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
+        daemon_ota_upgrade(args)
+
         login_pid = ClientConstants.exec_console_with_shell_script_list(
             [
                 get_python_program(),
                 "-W",
                 "ignore",
                 login_cmd,
                 "-t",
```

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/docker_login.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/docker_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/client_runner.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/client_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -639,53 +639,68 @@
             if self.client_mqtt_mgr is not None:
                 self.client_mqtt_is_connected = False
                 self.client_mqtt_mgr = None
             self.client_mqtt_lock.release()
         except Exception:
             pass
 
-    def callback_start_train(self, topic, payload):
-        # Get training params
-        request_json = json.loads(payload)
-        is_retain = request_json.get("is_retain", False)
-        if is_retain:
-            return
-        self.start_request_json = payload
-        run_id = request_json["runId"]
-
+    def ota_upgrade(self, payload, request_json):
         no_upgrade = False
         upgrade_version = None
+        run_id = request_json["runId"]
+
         try:
             run_config = request_json.get("run_config", None)
             parameters = run_config.get("parameters", None)
             common_args = parameters.get("common_args", None)
             no_upgrade = common_args.get("no_upgrade", False)
             upgrade_version = common_args.get("upgrade_version", None)
         except Exception as e:
             pass
 
-        if not no_upgrade:
-            job_obj = FedMLClientDataInterface.get_instance().get_job_by_id(run_id)
-            if job_obj is None:
-                FedMLClientDataInterface.get_instance(). \
-                    save_started_job(run_id, self.edge_id, time.time(),
-                                     ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
-                                     ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
-                                     payload)
-                self.mlops_metrics.\
-                    report_client_training_status(self.edge_id,
-                                                  ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
-                                                  in_run_id=run_id)
-                if upgrade_version is None or upgrade_version == "latest":
-                    logging.info("Upgrade to latest version...")
-                    os.system("pip uninstall -y fedml;pip install fedml")
-                else:
-                    logging.info(f"Upgrade to version {upgrade_version} ...")
-                    os.system(f"pip uninstall -y fedml;pip install fedml=={upgrade_version}")
-                raise Exception("Upgrading...")
+        should_upgrade = True
+        if upgrade_version is None or upgrade_version == "latest":
+            try:
+                fedml_is_latest_version, local_ver, remote_ver = sys_utils. \
+                    check_fedml_is_latest_version(self.version)
+            except Exception as e:
+                return
+
+            if fedml_is_latest_version:
+                should_upgrade = False
+            upgrade_version = remote_ver
+
+        if no_upgrade:
+            should_upgrade = False
+
+        if should_upgrade:
+            FedMLClientDataInterface.get_instance(). \
+                save_started_job(run_id, self.edge_id, time.time(),
+                                 ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
+                                 ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
+                                 payload)
+            self.mlops_metrics. \
+                report_client_training_status(self.edge_id,
+                                              ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
+                                              in_run_id=run_id)
+
+            logging.info(f"Upgrade to version {upgrade_version} ...")
+
+            sys_utils.do_upgrade(self.version, upgrade_version)
+
+            raise Exception("Restarting after upgraded...")
+
+    def callback_start_train(self, topic, payload):
+        # Get training params
+        request_json = json.loads(payload)
+        is_retain = request_json.get("is_retain", False)
+        if is_retain:
+            return
+        self.start_request_json = payload
+        run_id = request_json["runId"]
 
         if self.run_process is not None and \
                 sys_utils.get_process_running_count(ClientConstants.CLIENT_LOGIN_PROGRAM) >= 2:
             logging.info("There is a running job {}.".format(
                 self.run_process.pid
             ))
             try:
@@ -703,17 +718,21 @@
         server_agent_id = request_json["cloud_agent_id"]
         ClientConstants.exit_process(self.run_process)
         ClientConstants.cleanup_run_process()
         ClientConstants.save_runner_infos(self.args.device_id + "." + self.args.os_name, self.edge_id, run_id=run_id)
 
         # Start log processor for current run
         self.args.run_id = run_id
+        self.args.edge_id = self.edge_id
+        MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
         logging.info("start the log processor")
         MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(run_id, self.edge_id)
 
+        self.ota_upgrade(payload, request_json)
+
         # Start server with multiprocessing mode
         self.request_json = request_json
         client_runner = FedMLClientRunner(
             self.args, edge_id=self.edge_id, request_json=request_json, agent_config=self.agent_config, run_id=run_id
         )
         client_runner.start_request_json = self.start_request_json
         if self.run_process_event is None:
@@ -982,14 +1001,15 @@
         self.mqtt_mgr.send_message_json(active_topic, json.dumps(active_msg))
 
     def recover_start_train_msg_after_upgrading(self):
         try:
             current_job = FedMLClientDataInterface.get_instance().get_current_job()
             if current_job is not None and \
                     current_job.status == ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING:
+                logging.info("start training after upgrading.")
                 topic_start_train = "flserver_agent/" + str(self.edge_id) + "/start_train"
                 self.callback_start_train(topic_start_train, current_job.running_json)
         except Exception as e:
             logging.info("recover starting train message after upgrading: {}".format(traceback.format_exc()))
 
     def on_agent_mqtt_connected(self, mqtt_client_object):
         # The MQTT message topic format is as follows: <sender>/<receiver>/<action>
@@ -1062,15 +1082,15 @@
         # Init local database
         FedMLClientDataInterface.get_instance().create_job_table()
 
         # Start local API services
         python_program = get_python_program()
         local_api_process = ClientConstants.exec_console_with_script(
             "{} -m uvicorn fedml.cli.edge_deployment.client_api:api --host 0.0.0.0 --port {} "
-            "--reload --log-level critical".format(python_program,
+            "--log-level critical".format(python_program,
                                                    ClientConstants.LOCAL_CLIENT_API_PORT),
             should_capture_stdout=False,
             should_capture_stderr=False
         )
 
         # Setup MQTT connected listener
         self.mqtt_mgr.add_connected_listener(self.on_agent_mqtt_connected)
@@ -1087,15 +1107,18 @@
         self.recover_start_train_msg_after_upgrading()
 
     def start_agent_mqtt_loop(self):
         # Start MQTT message loop
         try:
             self.mqtt_mgr.loop_forever()
         except Exception as e:
-            logging.info("Client tracing: {}".format(traceback.format_exc()))
+            if str(e) == "Restarting after upgraded...":
+                logging.info("Restarting after upgraded...")
+            else:
+                logging.info("Client tracing: {}".format(traceback.format_exc()))
             self.mqtt_mgr.loop_stop()
             self.mqtt_mgr.disconnect()
             self.release_client_mqtt_mgr()
             time.sleep(5)
             sys_utils.cleanup_all_fedml_client_login_processes(
                 ClientConstants.CLIENT_LOGIN_PROGRAM, clean_process_group=False)
             sys.exit(1)
```

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/client_constants.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/client_constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/client_diagnosis.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/client_diagnosis.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/client_api.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/client_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 @api.post('/fedml/api/v2/currentJobStatus')
 async def get_current_job_status(request: Request):
     # Get json data
     input_json = await request.json()
 
     current_job = FedMLClientDataInterface.get_instance().get_current_job()
+    if current_job is None:
+        return {}
     response = {"jobId": current_job.job_id,
                 "edgeId": current_job.edge_id,
                 "startedTime": int(float(current_job.started_time)) if current_job.started_time != "" else 0,
                 "endedTime": int(float(current_job.ended_time)) if current_job.ended_time != "" else 0,
                 "progress": current_job.progress, "ETA": int(current_job.eta),
                 "failedTime": int(float(current_job.failed_time))if current_job.ended_time != "" else 0,
                 "errorCode": current_job.error_code,
```

### Comparing `fedml-0.8.3a9/fedml/cli/edge_deployment/simulator_daemon.py` & `fedml-0.8.4a1/fedml/cli/edge_deployment/simulator_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_inference.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import time
 import traceback
 from urllib.parse import urlparse
+import os
 
 from fastapi import FastAPI, Request
 from fedml.cli.model_deployment.device_model_deployment import run_http_inference_with_curl_request
 from fedml.cli.model_deployment.device_server_constants import ServerConstants
 from fedml.cli.model_deployment.device_model_monitor import FedMLModelMetrics
 from fedml.cli.model_deployment.device_model_cache import FedMLModelCache
 
@@ -70,18 +71,21 @@
             inference_response = send_inference_request(inference_output_url, input_list, output_list)
 
         # Calculate model metrics
         model_metrics.calc_metrics(end_point_id, in_end_point_name,
                                    model_id, model_name, model_version,
                                    inference_output_url)
 
+        logging_inference_request(input_json, inference_response)
+
         return inference_response
 
     else:
         inference_response = {"error": True, "message": "token is not valid."}
+        logging_inference_request(input_json, inference_response)
         return inference_response
 
     return inference_response
 
 
 def found_idle_inference_device(end_point_name, in_model_name, in_model_version):
     idle_device = ""
@@ -126,7 +130,14 @@
     FedMLModelCache.get_instance().set_redis_params(settings.redis_addr, settings.redis_port, settings.redis_password)
     cached_token = FedMLModelCache.get_instance(settings.redis_addr, settings.redis_port). \
         get_end_point_token(end_point_name, model_name)
     if cached_token is not None and cached_token == token:
         return True
 
     return False
+
+
+def logging_inference_request(request, response):
+    inference_log_file = os.path.join(ServerConstants.get_log_file_dir(), "inference.log")
+    with open(inference_log_file, "a") as f:
+        f.writelines([f"request: {request}, response: {response}\n"])
+
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_client_daemon.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_client_daemon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import argparse
 import os
 import time
+import sys
 
 from fedml.cli.comm_utils import sys_utils
 from fedml.cli.model_deployment.device_client_constants import ClientConstants
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
@@ -28,14 +29,16 @@
             ClientConstants.cleanup_run_process()
             sys_utils.cleanup_all_fedml_client_api_processes(is_model_device=True)
             sys_utils.cleanup_all_fedml_client_learning_processes()
             sys_utils.cleanup_all_fedml_client_login_processes("device_client_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
+        sys_utils.daemon_ota_upgrade(args)
+
         login_pid = ClientConstants.exec_console_with_shell_script_list(
             [
                 sys_utils.get_python_program(),
                 "-W",
                 "ignore",
                 login_cmd,
                 "-t",
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/modelops_configs.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/modelops_configs.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_server_api.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_server_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 @api.post('/fedml/api/v2/currentJobStatus')
 async def get_current_job_status(request: Request):
     # Get json data
     input_json = await request.json()
 
     current_job = FedMLServerDataInterface.get_instance().get_current_job()
+    if current_job is None:
+        return {}
     response = {"jobId": current_job.job_id,
                 "edgeId": current_job.edge_id,
                 "startedTime": int(float(current_job.started_time)) if current_job.started_time != "" else 0,
                 "endedTime": int(float(current_job.ended_time)) if current_job.ended_time != "" else 0,
                 "progress": current_job.progress, "ETA": int(current_job.eta),
                 "failedTime": int(float(current_job.failed_time))if current_job.ended_time != "" else 0,
                 "errorCode": current_job.error_code,
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_server_runner.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_server_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 from ...core.mlops.mlops_configs import MLOpsConfigs
 from ...core.mlops.mlops_runtime_log_daemon import MLOpsRuntimeLogDaemon
 from ...core.mlops.mlops_status import MLOpsStatus
 from ..comm_utils.sys_utils import get_sys_runner_info, get_python_program
 from .device_model_cache import FedMLModelCache
 from .device_model_msg_object import FedMLModelMsgObject
-
+from ...inference.fedml_server import FedMLInferenceServer
 
 class RunnerError(BaseException):
     """ Runner failed. """
     pass
 
 
 class FedMLServerRunner:
@@ -219,21 +219,40 @@
         memory_size = "256m"  # TODO: Get Memory size for each instance
         model_version = model_config["model_version"]
 
         return run_id, end_point_name, token, user_id, user_name, device_ids, device_objs, model_config, model_name, \
             model_id, model_storage_url, scale_min, scale_max, inference_engine, model_is_from_open, \
             inference_end_point_id, use_gpu, memory_size, model_version
 
+    def inference_run(self):
+        run_id, end_point_name, token, user_id, user_name, device_ids, device_objs, model_config, model_name, \
+            model_id, model_storage_url, scale_min, scale_max, inference_engine, model_is_from_open, \
+            inference_end_point_id, use_gpu, memory_size, model_version = self.parse_model_run_params(self.request_json)
+
+        inference_server = FedMLInferenceServer(self.args,
+                                                end_point_name,
+                                                model_name,
+                                                model_version,
+                                                inference_request=self.request_json)
+        inference_server.run()
+
     def run_impl(self):
         run_id, end_point_name, token, user_id, user_name, device_ids, device_objs, model_config, model_name, \
             model_id, model_storage_url, scale_min, scale_max, inference_engine, model_is_from_open, \
             inference_end_point_id, use_gpu, memory_size, model_version = self.parse_model_run_params(self.request_json)
 
         logging.info("model deployment request: {}".format(self.request_json))
 
+        # Initiate an FedMLInferenceServer object which the request will be forwarded to
+        # server_runner = FedMLServerRunner(
+        #     self.args, run_id=self.run_id, request_json=self.request_json, agent_config=self.agent_config
+        # )
+        # inference_process = Process(target=server_runner.inference_run)
+        # inference_process.start()
+
         logging.info("send deployment stages...")
 
         self.check_runner_stop_event()
 
         # Send stage: MODEL_DEPLOYMENT_STAGE4 = "ForwardRequest2Slave"
         self.send_deployment_stages(self.run_id, model_name, model_id,
                                     "",
@@ -288,27 +307,29 @@
             logging.info(f"start the model inference gateway, end point {run_id}, model name {model_name}...")
             self.check_runner_stop_event()
             process = ServerConstants.exec_console_with_script(
                 "REDIS_ADDR=\"{}\" REDIS_PORT=\"{}\" REDIS_PASSWORD=\"{}\" "
                 "END_POINT_Name=\"{}\" "
                 "MODEL_NAME=\"{}\" MODEL_VERSION=\"{}\" MODEL_INFER_URL=\"{}\" VERSION=\"{}\" "
                 "{} -m uvicorn fedml.cli.model_deployment.device_model_inference:api --host 0.0.0.0 --port {} "
-                "--reload --log-level critical".format(
+                "--log-level critical".format(
                     self.redis_addr, self.redis_port, self.redis_password,
                     end_point_name,
                     model_name, model_version, "", self.args.version,
                     python_program, str(ServerConstants.MODEL_INFERENCE_DEFAULT_PORT)),
                 should_capture_stdout=False,
                 should_capture_stderr=False
             )
 
-    def start_device_inference_monitor(self, run_id, end_point_name, model_id, model_name, model_version):
+    def start_device_inference_monitor(self, run_id, end_point_name,
+                                       model_id, model_name, model_version, check_stopped_event=True):
         # start inference monitor server
         logging.info(f"start the model inference monitor, end point {run_id}, model name {model_name}...")
-        self.check_runner_stop_event()
+        if check_stopped_event:
+            self.check_runner_stop_event()
         pip_source_dir = os.path.dirname(__file__)
         monitor_file = os.path.join(pip_source_dir, "device_model_monitor.py")
         python_program = get_python_program()
         running_model_name = ServerConstants.get_running_model_name(end_point_name,
                                                                     model_name, model_version, run_id, model_id)
         self.monitor_process = ServerConstants.exec_console_with_shell_script_list(
             [
@@ -335,14 +356,20 @@
                 "-rpw",
                 self.redis_password
             ],
             should_capture_stdout=False,
             should_capture_stderr=False
         )
 
+    def stop_device_inference_monitor(self, run_id, end_point_name, model_id, model_name, model_version):
+        # stop inference monitor server
+        logging.info(f"stop the model inference monitor, end point {run_id}, model name {model_name}...")
+        sys_utils.cleanup_model_monitor_processes(run_id, end_point_name,
+                                                  model_id, model_name, model_version)
+
     def cleanup_run_when_finished(self):
         logging.info("Cleanup run successfully when finished.")
 
         self.mlops_metrics.broadcast_server_training_status(
             self.run_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_FINISHED,
             is_from_model=True
         )
@@ -597,14 +624,57 @@
             if edge_id == self.edge_id:
                 continue
             # send delete deployment request to each model device
             topic_delete_deployment = "model_ops/model_device/delete_deployment/{}".format(str(edge_id))
             logging.info("delete_deployment: send topic " + topic_delete_deployment + " to client...")
             self.client_mqtt_mgr.send_message_json(topic_delete_deployment, payload)
 
+    def ota_upgrade(self, payload, request_json):
+        no_upgrade = False
+        upgrade_version = None
+        run_id = request_json["end_point_id"]
+
+        try:
+            parameters = request_json.get("parameters", None)
+            common_args = parameters.get("common_args", None)
+            no_upgrade = common_args.get("no_upgrade", False)
+            upgrade_version = common_args.get("upgrade_version", None)
+        except Exception as e:
+            pass
+
+        should_upgrade = True
+        if upgrade_version is None or upgrade_version == "latest":
+            try:
+                fedml_is_latest_version, local_ver, remote_ver = sys_utils. \
+                    check_fedml_is_latest_version(self.version)
+            except Exception as e:
+                return
+
+            if fedml_is_latest_version:
+                should_upgrade = False
+            upgrade_version = remote_ver
+
+        if no_upgrade:
+            should_upgrade = False
+
+        if should_upgrade:
+            job_obj = FedMLServerDataInterface.get_instance().get_job_by_id(run_id)
+            if job_obj is None:
+                FedMLServerDataInterface.get_instance(). \
+                    save_started_job(run_id, self.edge_id, time.time(),
+                                     ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING,
+                                     ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING,
+                                     payload)
+
+            logging.info(f"Upgrade to version {upgrade_version} ...")
+
+            sys_utils.do_upgrade(self.version, upgrade_version)
+
+            raise Exception("Restarting after upgraded...")
+
     def callback_start_deployment(self, topic, payload):
         """
         topic: model_ops/model_device/start_deployment/model-agent-device-id
         payload: {"timestamp": 1671440005119, "end_point_id": 4325, "token": "FCpWU", "state": "STARTING","user_id": "105", "user_name": "alex.liang2", "device_ids": [693], "device_objs": [{"device_id": "0xT3630FW2YM@MacOS.Edge.Device", "os_type": "MacOS", "id": 693, "ip": "1.1.1.1", "memory": 1024, "cpu": "1.7", "gpu": "Nvidia", "extra_infos":{}}], "model_config": {"model_name": "image-model", "model_id": 111, "model_version": "v1", 'is_from_open": 0, "model_storage_url": "https://fedml.s3.us-west-1.amazonaws.com/1666239314792client-package.zip", "instance_scale_min": 1, "instance_scale_max": 3, "inference_engine": "onnx"}, "parameters": {"hidden_size": 128, "hidden_act": "gelu", "initializer_range": 0.02, "vocab_size": 30522, "hidden_dropout_prob": 0.1, "num_attention_heads": 2, "type_vocab_size": 2, "max_position_embeddings": 512, "num_hidden_layers": 2, "intermediate_size": 512, "attention_probs_dropout_prob": 0.1}}
         """
         logging.info("callback_start_deployment {}".format(payload))
 
@@ -623,14 +693,24 @@
         model_id = model_config["model_id"]
         model_storage_url = model_config["model_storage_url"]
         scale_min = model_config["instance_scale_min"]
         scale_max = model_config["instance_scale_max"]
         inference_engine = model_config["inference_engine"]
         inference_end_point_id = run_id
 
+        # Start log processor for current run
+        self.args.run_id = run_id
+        self.args.edge_id = self.edge_id
+        MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
+        MLOpsRuntimeLogDaemon.get_instance(self.args).set_log_source(
+            ServerConstants.FEDML_LOG_SOURCE_TYPE_MODEL_END_POINT)
+        MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(run_id, self.edge_id)
+
+        self.ota_upgrade(payload, request_json)
+
         run_id = inference_end_point_id
         self.args.run_id = run_id
         self.run_id = run_id
         request_json["run_id"] = run_id
         self.request_json = request_json
         self.running_request_json[str(run_id)] = request_json
 
@@ -658,20 +738,14 @@
                                     ServerConstants.MODEL_DEPLOYMENT_STAGE2["text"],
                                     ServerConstants.MODEL_DEPLOYMENT_STAGE2["text"])
 
         ServerConstants.save_runner_infos(self.args.device_id + "." + self.args.os_name, self.edge_id, run_id=run_id)
         time.sleep(1)
 
         if self.run_as_edge_server_and_agent:
-            # Start log processor for current run
-            MLOpsRuntimeLogDaemon.get_instance(self.args).set_log_source(
-                ServerConstants.FEDML_LOG_SOURCE_TYPE_MODEL_END_POINT)
-            MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(run_id, self.edge_id)
-            self.args.run_id = run_id
-
             server_runner = FedMLServerRunner(
                 self.args, run_id=run_id, request_json=request_json, agent_config=self.agent_config
             )
             server_runner.run_as_edge_server_and_agent = self.run_as_edge_server_and_agent
             server_runner.edge_id = self.edge_id
             server_runner.infer_host = self.infer_host
             server_runner.redis_addr = self.redis_addr
@@ -723,28 +797,36 @@
 
         # Send deployment status to the ModelOps backend
         if prev_status == ClientConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_DEPLOYED:
             self.send_deployment_status(model_msg_object.inference_end_point_id,
                                         model_msg_object.end_point_name,
                                         model_msg_object.model_name, "", prev_status)
 
+        self.start_device_inference_monitor(model_msg_object.run_id, model_msg_object.end_point_name,
+                                            model_msg_object.model_id, model_msg_object.model_name,
+                                            model_msg_object.model_version, check_stopped_event=False)
+
     def callback_deactivate_deployment(self, topic, payload):
         logging.info("callback_deactivate_deployment: topic = %s, payload = %s" % (topic, payload))
 
         # Parse payload as the model message object.
         model_msg_object = FedMLModelMsgObject(topic, payload)
 
         # Set end point as deactivated status
         FedMLModelCache.get_instance().set_redis_params(self.redis_addr, self.redis_port, self.redis_password)
         FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
             set_end_point_activation(model_msg_object.inference_end_point_id,
                                      model_msg_object.model_name, False)
 
         self.set_runner_stopped_event(model_msg_object.run_id)
 
+        self.stop_device_inference_monitor(model_msg_object.run_id, model_msg_object.end_point_name,
+                                           model_msg_object.model_id, model_msg_object.model_name,
+                                           model_msg_object.model_version)
+
     def set_runner_stopped_event(self, run_id):
         server_runner = self.model_runner_mapping.get(run_id, None)
         if server_runner is not None:
             if server_runner.run_process_event is not None:
                 server_runner.run_process_event.set()
             self.model_runner_mapping.pop(run_id)
 
@@ -760,14 +842,18 @@
             set_end_point_activation(model_msg_object.inference_end_point_id,
                                      model_msg_object.end_point_name, False)
 
         self.send_deployment_delete_request_to_edges(payload, model_msg_object)
 
         self.set_runner_stopped_event(model_msg_object.run_id)
 
+        self.stop_device_inference_monitor(model_msg_object.run_id, model_msg_object.end_point_name,
+                                           model_msg_object.model_id, model_msg_object.model_name,
+                                           model_msg_object.model_version)
+
     def send_deployment_results_with_payload(self, end_point_id, end_point_name, payload):
         self.send_deployment_results(end_point_id, end_point_name,
                                      payload["model_name"], payload["model_url"],
                                      payload["model_version"], payload["port"],
                                      payload["inference_engine"],
                                      payload["model_metadata"],
                                      payload["model_config"],
@@ -1285,20 +1371,40 @@
                     continue
 
                 run_id, end_point_name, token, user_id, user_name, device_ids, device_objs, model_config, model_name, \
                     model_id, model_storage_url, scale_min, scale_max, inference_engine, model_is_from_open, \
                     inference_end_point_id, use_gpu, memory_size, model_version = \
                     self.parse_model_run_params(json.loads(job.running_json))
 
+                is_activated = FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
+                    get_end_point_activation(run_id)
+                if not is_activated:
+                    continue
+
                 self.start_device_inference_gateway(run_id, end_point_name, model_id, model_name, model_version)
 
                 self.start_device_inference_monitor(run_id, end_point_name, model_id, model_name, model_version)
         except Exception as e:
             logging.info("recover inference and monitor: {}".format(traceback.format_exc()))
 
+    def recover_start_deployment_msg_after_upgrading(self):
+        try:
+            current_job = FedMLServerDataInterface.get_instance().get_current_job()
+            if current_job is not None and \
+                    current_job.status == ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING:
+                is_activated = FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
+                    get_end_point_activation(current_job.job_id)
+                if not is_activated:
+                    return
+                logging.info("start deployment after upgrading.")
+                topic_start_deployment = "model_ops/model_device/start_deployment/{}".format(str(self.edge_id))
+                self.callback_start_deployment(topic_start_deployment, current_job.running_json)
+        except Exception as e:
+            logging.info("recover starting deployment message after upgrading: {}".format(traceback.format_exc()))
+
     def setup_agent_mqtt_connection(self, service_config):
         # Setup MQTT connection
         self.mqtt_mgr = MqttManager(
             service_config["mqtt_config"]["BROKER_HOST"],
             service_config["mqtt_config"]["BROKER_PORT"],
             service_config["mqtt_config"]["MQTT_USER"],
             service_config["mqtt_config"]["MQTT_PWD"],
@@ -1311,15 +1417,15 @@
         # Init local database
         FedMLServerDataInterface.get_instance().create_job_table()
 
         # Start local API services
         python_program = get_python_program()
         local_api_process = ServerConstants.exec_console_with_script(
             "{} -m uvicorn fedml.cli.model_deployment.server_api:api --host 0.0.0.0 --port {} "
-            "--reload --log-level critical".format(python_program, ServerConstants.LOCAL_SERVER_API_PORT),
+            "--log-level critical".format(python_program, ServerConstants.LOCAL_SERVER_API_PORT),
             should_capture_stdout=False,
             should_capture_stderr=False
         )
 
         self.recover_inference_and_monitor()
 
         MLOpsRuntimeLogDaemon.get_instance(self.args).stop_all_log_processor()
@@ -1336,20 +1442,25 @@
         MLOpsStatus.get_instance().set_server_agent_status(
             self.edge_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_IDLE
         )
         self.mlops_metrics.set_sys_reporting_status(enable=True, is_client=False)
         setattr(self.args, "mqtt_config_path", service_config["mqtt_config"])
         self.mlops_metrics.report_sys_perf(self.args, is_client=False)
 
+        self.recover_start_deployment_msg_after_upgrading()
+
     def start_agent_mqtt_loop(self):
         # Start MQTT message loop
         try:
             self.mqtt_mgr.loop_forever()
         except Exception as e:
-            logging.info("Server tracing: {}".format(traceback.format_exc()))
+            if str(e) == "Restarting after upgraded...":
+                logging.info("Restarting after upgraded...")
+            else:
+                logging.info("Server tracing: {}".format(traceback.format_exc()))
             self.mqtt_mgr.loop_stop()
             self.mqtt_mgr.disconnect()
             self.release_client_mqtt_mgr()
             time.sleep(5)
             sys_utils.cleanup_all_fedml_server_login_processes(
                 ServerConstants.SERVER_LOGIN_PROGRAM, clean_process_group=False)
             sys.exit(1)
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_cards.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_cards.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_client_api.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_client_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 @api.post('/fedml/api/v2/currentJobStatus')
 async def get_current_job_status(request: Request):
     # Get json data
     input_json = await request.json()
 
     current_job = FedMLClientDataInterface.get_instance().get_current_job()
+    if current_job is None:
+        return {}
     response = {"jobId": current_job.job_id,
                 "edgeId": current_job.edge_id,
                 "startedTime": int(float(current_job.started_time)) if current_job.started_time != "" else 0,
                 "endedTime": int(float(current_job.ended_time)) if current_job.ended_time != "" else 0,
                 "progress": current_job.progress, "ETA": int(current_job.eta),
                 "failedTime": int(float(current_job.failed_time))if current_job.ended_time != "" else 0,
                 "errorCode": current_job.error_code,
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/docker_client_login.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/docker_client_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_server_login.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_server_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_cache.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_cache.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_deployment.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_deployment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-
+import io
 import logging
 import os
 import pickle
 import platform
 import shutil
 import time
+import traceback
+
 import requests
 import torch
 import torch.nn
 import tritonclient.http as http_client
 
 import collections.abc
 
@@ -24,14 +26,38 @@
                      inference_use_gpu, inference_memory_size,
                      inference_convertor_image, inference_server_image,
                      infer_host, model_is_from_open, model_params,
                      model_from_open):
     logging.info("Model deployment is starting...")
 
     use_simulation_test_without_triton = False
+    model_metadata = {'name': inference_model_name,
+                      'versions': ['1'], 'platform': 'onnxruntime_onnx',
+                      'inputs': [{'name': 'input2', 'datatype': 'INT32', 'shape': [1, 24]}, {'name': 'input1', 'datatype': 'FP32', 'shape': [1, 2]}],
+                      'outputs': [{'name': 'output', 'datatype': 'FP32', 'shape': [1]}]}
+    model_config = {
+        "platform": "onnxruntime",
+        "max_batch_size": 1,
+        "input_size": [[1, 24], [1, 2]],
+        "input_types": ["int", "float"],
+        "input": [
+            {
+                "name": "input",
+                "data_type": "TYPE_FP32",
+                "dims": []
+            }
+        ],
+        "output": [
+            {
+                "name": "output",
+                "data_type": "TYPE_FP32",
+                "dims": []
+            }
+        ]
+    }
 
     gpu_attach_cmd = ""
     if inference_use_gpu is not None and inference_use_gpu != "":
         gpu_attach_cmd = "--gpus all"
 
     logging.info("Update docker environments...")
 
@@ -59,15 +85,15 @@
         logging.info("install nvidia docker...")
 
         # Setup nvidia docker related packages.
         if not ClientConstants.is_running_on_k8s():
             if sys_name == "Linux":
                 if not triton_server_is_running:
                     os.system(sudo_prefix + "apt-get update")
-                    os.system(sudo_prefix + "apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin")
+                    os.system(sudo_prefix + "apt-get install -y docker-ce docker-ce-cli containerd.io docker-compose-plugin")
                     os.system("distribution=$(. /etc/os-release;echo $ID$VERSION_ID) \
                   && sudo rm -f /usr/share/keyrings/nvidia-container-toolkit-keyring.gpg;curl -fsSL https://nvidia.github.io/libnvidia-container/gpgkey | sudo gpg --dearmor -o /usr/share/keyrings/nvidia-container-toolkit-keyring.gpg \
                   && curl -s -L https://nvidia.github.io/libnvidia-container/experimental/$distribution/libnvidia-container.list | \
                      sed 's#deb https://#deb [signed-by=/usr/share/keyrings/nvidia-container-toolkit-keyring.gpg] https://#g' | \
                      sudo tee /etc/apt/sources.list.d/nvidia-container-toolkit.list")
                     os.system(sudo_prefix + "apt-get update")
                     os.system(sudo_prefix + "apt-get install -y nvidia-docker2")
@@ -83,15 +109,33 @@
         running_model_name = ClientConstants.get_running_model_name(end_point_name,
                                                                     inference_model_name,
                                                                     model_version, end_point_id, model_id)
         if model_from_open is None:
             return running_model_name, "", model_version, {}, {}
 
         with open(model_bin_file, 'rb') as model_pkl_file:
-            open_model_params = pickle.load(model_pkl_file)
+            if not torch.cuda.is_available():
+                class CPUUnpickler(pickle.Unpickler):
+                    def find_class(self, module, name):
+                        if module == 'torch.storage' and name == '_load_from_bytes':
+                            return lambda b: torch.load(io.BytesIO(b), map_location='cpu')
+                        else:
+                            return super().find_class(module, name)
+
+                try:
+                    open_model_params = pickle.load(model_pkl_file)
+                except Exception as e:
+                    logging.info("load model exceptions, try to use another loading method, details: {}".format(traceback.format_exc()))
+                    try:
+                        open_model_params = CPUUnpickler(model_pkl_file).load()
+                    except Exception as ex:
+                        logging.info("load model exceptions when using CPUUnpickler: {}".format(traceback.format_exc()))
+                        return "", "", model_version, model_metadata, model_config
+            else:
+                open_model_params = pickle.load(model_pkl_file)
             model_from_open.load_state_dict(open_model_params)
             model_from_open.eval()
 
         input_size = model_params["input_size"]
         input_types = model_params["input_types"]
 
         dummy_input_list = []
@@ -218,44 +262,23 @@
                                                                              should_capture_stdout=False,
                                                                              should_capture_stderr=False,
                                                                              no_sys_out_err=True)
             log_deployment_result(end_point_id, model_id, triton_server_container_name,
                                   ClientConstants.CMD_TYPE_RUN_TRITON_SERVER, triton_server_process.pid,
                                   running_model_name, inference_engine, inference_http_port)
 
-        inference_output_url, running_model_version, model_metadata, model_config = \
+        inference_output_url, running_model_version, ret_model_metadata, ret_model_config = \
             get_model_info(running_model_name, inference_engine, inference_http_port, infer_host)
-        logging.info("Deploy model successfully, inference url: {}, model metadata: {}, model config: {}".format(
-            inference_output_url, model_metadata, model_config))
+        if inference_output_url != "":
+            logging.info("Deploy model successfully, inference url: {}, model metadata: {}, model config: {}".format(
+                inference_output_url, model_metadata, model_config))
+            model_metadata = ret_model_metadata
+            model_config = ret_model_config
     else:
         inference_output_url = f"http://localhost:{inference_http_port}/v2/models/{running_model_name}/versions/1/infer"
-        model_metadata = {'name': inference_model_name,
-                          'versions': ['1'], 'platform': 'onnxruntime_onnx',
-                          'inputs': [{'name': 'input2', 'datatype': 'INT32', 'shape': [1, 24]}, {'name': 'input1', 'datatype': 'FP32', 'shape': [1, 2]}],
-                          'outputs': [{'name': 'output', 'datatype': 'FP32', 'shape': [1]}]}
-        model_config = {
-            "platform": "onnxruntime",
-            "max_batch_size": 1,
-            "input_size": [[1, 24], [1, 2]],
-            "input_types": ["int", "float"],
-            "input": [
-                {
-                    "name": "input",
-                    "data_type": "TYPE_FP32",
-                    "dims": []
-                }
-            ],
-            "output": [
-                {
-                    "name": "output",
-                    "data_type": "TYPE_FP32",
-                    "dims": []
-                }
-            ]
-        }
 
     return running_model_name, inference_output_url, model_version, model_metadata, model_config
 
 
 def should_exit_logs(end_point_id, model_id, cmd_type, cmd_process_id, model_name, inference_engine, inference_port):
     sudo_prefix = "sudo "
     sys_name = platform.system()
@@ -299,14 +322,15 @@
     sudo_prefix = "sudo "
     sys_name = platform.system()
     if sys_name == "Darwin":
         sudo_prefix = ""
 
     last_out_logs = ""
     last_err_logs = ""
+    deployment_count = 0
     while True:
         if not ClientConstants.is_running_on_k8s():
             logs_cmd = "{}docker logs {}".format(sudo_prefix, cmd_container_name)
             logs_process = ClientConstants.exec_console_with_script(logs_cmd,
                                                                     should_capture_stdout=True,
                                                                     should_capture_stderr=True)
             ret_code, out, err = ClientConstants.get_console_pipe_out_err_results(logs_process)
@@ -320,14 +344,17 @@
                 err_str = err.decode(encoding="utf-8")
                 added_logs = str(err_str).replace(last_err_logs, "")
                 if len(added_logs) > 0:
                     logging.info("{}".format(added_logs))
                 last_err_logs = err_str
 
         time.sleep(3)
+        deployment_count += 1
+        if deployment_count >= 5:
+            break
 
         if should_exit_logs(end_point_id, model_id, cmd_type, cmd_process_id,
                             inference_model_name, inference_engine, inference_http_port):
             break
 
 
 def get_model_info(model_name, inference_engine, inference_http_port, infer_host=None, is_hg_model=False):
@@ -340,20 +367,24 @@
     model_version = ""
     logging.info("triton infer url: {}.".format(local_infer_url))
     if is_hg_model:
         inference_model_name = "{}_{}_inference".format(model_name, inference_engine)
     else:
         inference_model_name = model_name
     triton_client = http_client.InferenceServerClient(url=local_infer_url, verbose=False)
+    wait_count = 0
     while True:
         if not triton_client.is_model_ready(
                 model_name=inference_model_name, model_version=model_version
         ):
             logging.info(f"model {model_name} not yet ready")
             time.sleep(1)
+            wait_count += 1
+            if wait_count >= 15:
+                return "", model_version, {}, {}
         else:
             break
 
     model_metadata = triton_client.get_model_metadata(model_name=inference_model_name, model_version=model_version)
     model_config = triton_client.get_model_config(model_name=inference_model_name, model_version=model_version)
     version_list = model_metadata.get("versions", None)
     if version_list is not None and len(version_list) > 0:
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_server_data_interface.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_server_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_object.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_object.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_db.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import os
 import time
 
-from fedml.cli.model_deployment.device_client_constants import ClientConstants
+from fedml.cli.model_deployment.device_server_constants import ServerConstants
 from sqlalchemy import Column, String, TEXT, Integer, Float, create_engine, and_
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 
 Base = declarative_base()
 
 
@@ -127,17 +127,17 @@
                         "avg_qps": endpoint_metrics.avg_qps, "timestamp": endpoint_metrics.timestamp}
         return json.dumps(metrics_dict)
 
     def open_job_db(self):
         if self.db_connection is not None:
             return
 
-        if not os.path.exists(ClientConstants.get_database_dir()):
-            os.makedirs(ClientConstants.get_database_dir())
-        job_db_path = os.path.join(ClientConstants.get_database_dir(), FedMLModelDatabase.MODEL_DEPLOYMENT_DB)
+        if not os.path.exists(ServerConstants.get_database_dir()):
+            os.makedirs(ServerConstants.get_database_dir())
+        job_db_path = os.path.join(ServerConstants.get_database_dir(), FedMLModelDatabase.MODEL_DEPLOYMENT_DB)
         self.db_engine = create_engine('sqlite:////{}'.format(job_db_path), echo=False)
 
         db_session_class = sessionmaker(bind=self.db_engine)
         self.db_connection = db_session_class()
 
     def close_job_db(self):
         if self.db_connection is not None:
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_login_entry.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_login_entry.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_client_data_interface.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_client_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_server_constants.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_server_constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_monitor.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                                          "model_id": self.current_model_id,
                                          "model_url": self.current_infer_url,
                                          "end_point_id": self.current_end_point_id,
                                          "latency": float(avg_latency),
                                          "qps": int(avg_qps),
                                          "total_request_num": int(total_request_num),
                                          "timestamp": timestamp}
-        print("send monitor metrics {}".format(json.dumps(deployment_monitoring_payload)))
+        # print("send monitor metrics {}".format(json.dumps(deployment_monitoring_payload)))
 
         self.monitor_mqtt_mgr.send_message_json(deployment_monitoring_topic, json.dumps(deployment_monitoring_payload))
         self.monitor_mqtt_mgr.send_message_json(deployment_monitoring_topic_prefix,
                                                 json.dumps(deployment_monitoring_payload))
         return inc_index
 
     def on_mqtt_connected(self, mqtt_client_object):
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_client_constants.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_client_constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_client_runner.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_client_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 from ...core.mlops.mlops_configs import MLOpsConfigs
 from ...core.mlops.mlops_runtime_log_daemon import MLOpsRuntimeLogDaemon
 from ...core.mlops.mlops_status import MLOpsStatus
 from ..comm_utils.sys_utils import get_sys_runner_info, get_python_program
 from .device_model_deployment import start_deployment
 from .device_client_data_interface import FedMLClientDataInterface
+from ...inference.fedml_client import FedMLInferenceClient
 
 
 class RunnerError(Exception):
     """ Runner failed. """
     pass
 
 
@@ -141,19 +142,19 @@
     def package_download_progress(self, count, blksize, filesize):
         self.check_runner_stop_event()
 
         downloaded = count * blksize
         downloaded = filesize if downloaded > filesize else downloaded
         progress = (downloaded / filesize * 100) if filesize != 0 else 0
         progress_int = int(progress)
-        downloaded_kb = format(downloaded/1024, '.2f')
-        
+        downloaded_kb = format(downloaded / 1024, '.2f')
+
         # since this hook funtion is stateless, we need a state to avoid printing progress repeatly
         if count == 0:
-            self.prev_download_progress = 0 
+            self.prev_download_progress = 0
         if progress_int != self.prev_download_progress and progress_int % 5 == 0:
             self.prev_download_progress = progress_int
             logging.info("package downloaded size {} KB, progress {}%".format(downloaded_kb, progress_int))
 
     def build_dynamic_constrain_variables(self, run_id, run_config):
         pass
 
@@ -216,14 +217,26 @@
             self.release_client_mqtt_mgr()
 
     def check_runner_stop_event(self):
         if self.run_process_event.is_set():
             logging.info("Received stopping event.")
             raise RunnerError("Runner stopped")
 
+    def inference_run(self):
+        run_id, end_point_name, token, user_id, user_name, device_ids, device_objs, model_config, model_name, \
+            model_id, model_storage_url, scale_min, scale_max, inference_engine, model_is_from_open, \
+            inference_end_point_id, use_gpu, memory_size, model_version = self.parse_model_run_params(self.request_json)
+
+        inference_client = FedMLInferenceClient(self.args,
+                                                end_point_name,
+                                                model_name,
+                                                model_version,
+                                                inference_request=self.request_json)
+        inference_client.run()
+
     def run_impl(self):
         run_id = self.request_json["end_point_id"]
         end_point_name = self.request_json["end_point_name"]
         token = self.request_json["token"]
         user_id = self.request_json["user_id"]
         user_name = self.request_json["user_name"]
         device_ids = self.request_json["device_ids"]
@@ -247,14 +260,22 @@
 
         self.check_runner_stop_event()
 
         logging.info("model deployment request: {}".format(self.request_json))
 
         MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
 
+        # Initiate an FedMLInferenceClient object
+        # client_runner = FedMLClientRunner(
+        #     self.args, edge_id=self.edge_id, run_id=self.run_id, request_json=self.request_json,
+        #     agent_config=self.agent_config
+        # )
+        # inference_process = Process(target=client_runner.inference_run)
+        # inference_process.start()
+
         self.mlops_metrics.report_client_training_status(self.edge_id,
                                                          ClientConstants.MSG_MLOPS_CLIENT_STATUS_INITIALIZING,
                                                          is_from_model=True,
                                                          running_json=json.dumps(self.request_json))
 
         self.mlops_metrics.report_client_training_status(self.edge_id,
                                                          ClientConstants.MSG_MLOPS_CLIENT_STATUS_RUNNING,
@@ -298,15 +319,16 @@
                     model_from_open = s3_client.read_model_net(model_key,
                                                                ClientConstants.get_model_cache_dir())
 
                 model_input_size, model_input_type = mlops.get_training_model_input_info(model_net_url, s3_config)
                 if model_input_size is not None and model_input_type is not None:
                     model_config_parameters["input_size"] = model_input_size
                     model_config_parameters["input_types"] = model_input_type
-                    logging.info(f"model input size {model_input_size}, input type {model_input_type} from the open platform.")
+                    logging.info(
+                        f"model input size {model_input_size}, input type {model_input_type} from the open platform.")
 
         logging.info("start the model deployment...")
         self.check_runner_stop_event()
         running_model_name, inference_output_url, inference_model_version, model_metadata, model_config = \
             start_deployment(
                 inference_end_point_id, end_point_name, model_id, model_version,
                 unzip_package_path, model_bin_file, model_name, inference_engine,
@@ -321,15 +343,16 @@
                 model_from_open)
         if inference_output_url == "":
             logging.info("failed to deploy the model...")
             self.send_deployment_status(end_point_name, self.edge_id,
                                         model_id, model_name, model_version,
                                         inference_output_url,
                                         ClientConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_FAILED)
-            self.send_deployment_results(end_point_name, self.edge_id, ClientConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_FAILED,
+            self.send_deployment_results(end_point_name, self.edge_id,
+                                         ClientConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_FAILED,
                                          model_id, model_name, inference_output_url,
                                          inference_model_version, ClientConstants.INFERENCE_HTTP_PORT,
                                          inference_engine, model_metadata, model_config)
             self.mlops_metrics.run_id = self.run_id
             self.mlops_metrics.broadcast_client_training_status(self.edge_id,
                                                                 ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED,
                                                                 is_from_model=True)
@@ -478,14 +501,55 @@
             if self.client_mqtt_mgr is not None:
                 self.client_mqtt_is_connected = False
                 self.client_mqtt_mgr = None
             self.client_mqtt_lock.release()
         except Exception:
             pass
 
+    def ota_upgrade(self, payload, request_json):
+        no_upgrade = False
+        upgrade_version = None
+        run_id = request_json["end_point_id"]
+
+        try:
+            parameters = request_json.get("parameters", None)
+            common_args = parameters.get("common_args", None)
+            no_upgrade = common_args.get("no_upgrade", False)
+            upgrade_version = common_args.get("upgrade_version", None)
+        except Exception as e:
+            pass
+
+        should_upgrade = True
+        if upgrade_version is None or upgrade_version == "latest":
+            try:
+                fedml_is_latest_version, local_ver, remote_ver = sys_utils. \
+                    check_fedml_is_latest_version(self.version)
+            except Exception as e:
+                return
+
+            if fedml_is_latest_version:
+                should_upgrade = False
+            upgrade_version = remote_ver
+
+        if no_upgrade:
+            should_upgrade = False
+
+        if should_upgrade:
+            FedMLClientDataInterface.get_instance(). \
+                save_started_job(run_id, self.edge_id, time.time(),
+                                 ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
+                                 ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING,
+                                 payload)
+
+            logging.info(f"Upgrade to version {upgrade_version} ...")
+
+            sys_utils.do_upgrade(self.version, upgrade_version)
+
+            raise Exception("Restarting after upgraded...")
+
     def callback_start_deployment(self, topic, payload):
         """
         topic: model_ops/model_device/start_deployment/model-agent-device-id
         payload: {"model_name": "image-model", "model_storage_url":"s3-url", "instance_scale_min":1, "instance_scale_max":3, "inference_engine":"onnx (or tensorrt)"}
         """
         # get deployment params
         request_json = json.loads(payload)
@@ -508,19 +572,23 @@
         ClientConstants.exit_process(self.process)
         ClientConstants.cleanup_run_process()
         ClientConstants.save_runner_infos(self.args.device_id + "." + self.args.os_name, self.edge_id, run_id=run_id)
 
         # Start log processor for current run
         run_id = inference_end_point_id
         self.args.run_id = run_id
+        self.args.edge_id = self.edge_id
+        MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
         MLOpsRuntimeLogDaemon.get_instance(self.args).set_log_source(
             ClientConstants.FEDML_LOG_SOURCE_TYPE_MODEL_END_POINT)
         MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(run_id, self.edge_id)
 
-        # Start client with multiprocessing mode
+        self.ota_upgrade(payload, request_json)
+
+    # Start client with multiprocessing mode
         request_json["run_id"] = run_id
         self.request_json = request_json
         client_runner = FedMLClientRunner(
             self.args, edge_id=self.edge_id, request_json=request_json, agent_config=self.agent_config, run_id=run_id
         )
         client_runner.infer_host = self.infer_host
         if self.run_process_event is None:
@@ -714,15 +782,15 @@
                 f.write(device_id)
 
         return device_id
 
     def bind_account_and_device_id(self, url, account_id, device_id, os_name, role="md.on_premise_device"):
         ip = requests.get('https://checkip.amazonaws.com').text.strip()
         fedml_ver, exec_path, os_ver, cpu_info, python_ver, torch_ver, mpi_installed, \
-        cpu_usage, available_mem, total_mem, gpu_info, gpu_available_mem, gpu_total_mem = get_sys_runner_info()
+            cpu_usage, available_mem, total_mem, gpu_info, gpu_available_mem, gpu_total_mem = get_sys_runner_info()
         json_params = {
             "accountid": account_id,
             "deviceid": device_id,
             "type": os_name,
             "processor": cpu_info,
             "core_type": cpu_info,
             "network": "",
@@ -795,14 +863,25 @@
                 return
         else:
             status = ClientConstants.get_device_state_from_run_edge_state(current_job.status)
         active_msg = {"ID": self.edge_id, "status": status}
         MLOpsStatus.get_instance().set_client_agent_status(self.edge_id, status)
         self.mqtt_mgr.send_message_json(active_topic, json.dumps(active_msg))
 
+    def recover_start_deployment_msg_after_upgrading(self):
+        try:
+            current_job = FedMLClientDataInterface.get_instance().get_current_job()
+            if current_job is not None and \
+                    current_job.status == ClientConstants.MSG_MLOPS_CLIENT_STATUS_UPGRADING:
+                logging.info("start deployment after upgrading.")
+                topic_start_deployment = "model_ops/model_device/start_deployment/{}".format(str(self.edge_id))
+                self.callback_start_deployment(topic_start_deployment, current_job.running_json)
+        except Exception as e:
+            logging.info("recover starting deployment message after upgrading: {}".format(traceback.format_exc()))
+
     def on_agent_mqtt_connected(self, mqtt_client_object):
         # The MQTT message topic format is as follows: <sender>/<receiver>/<action>
 
         # Setup MQTT message listener for starting deployment
         topic_start_deployment = "model_ops/model_device/start_deployment/{}".format(str(self.edge_id))
         self.mqtt_mgr.add_message_listener(topic_start_deployment, self.callback_start_deployment)
 
@@ -869,15 +948,15 @@
         # Init local database
         FedMLClientDataInterface.get_instance().create_job_table()
 
         # Start local API services
         python_program = get_python_program()
         local_api_process = ClientConstants.exec_console_with_script(
             "{} -m uvicorn fedml.cli.model_deployment.client_api:api --host 0.0.0.0 --port {} "
-            "--reload --log-level critical".format(python_program,
+            "--log-level critical".format(python_program,
                                                    ClientConstants.LOCAL_CLIENT_API_PORT),
             should_capture_stdout=False,
             should_capture_stderr=False
         )
 
         MLOpsRuntimeLogDaemon.get_instance(self.args).stop_all_log_processor()
 
@@ -891,20 +970,25 @@
                                                          ClientConstants.MSG_MLOPS_CLIENT_STATUS_IDLE,
                                                          is_from_model=True)
         MLOpsStatus.get_instance().set_client_agent_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_IDLE)
         self.mlops_metrics.set_sys_reporting_status(enable=True, is_client=True)
         setattr(self.args, "mqtt_config_path", service_config["mqtt_config"])
         self.mlops_metrics.report_sys_perf(self.args)
 
+        self.recover_start_deployment_msg_after_upgrading()
+
     def start_agent_mqtt_loop(self):
         # Start MQTT message loop
         try:
             self.mqtt_mgr.loop_forever()
         except Exception as e:
-            logging.info("Client tracing: {}".format(traceback.format_exc()))
+            if str(e) == "Restarting after upgraded...":
+                logging.info("Restarting after upgraded...")
+            else:
+                logging.info("Client tracing: {}".format(traceback.format_exc()))
             self.mqtt_mgr.loop_stop()
             self.mqtt_mgr.disconnect()
             self.release_client_mqtt_mgr()
             time.sleep(5)
             sys_utils.cleanup_all_fedml_client_login_processes(
                 ClientConstants.CLIENT_LOGIN_PROGRAM, clean_process_group=False)
             sys.exit(1)
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/docker_server_login.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/docker_server_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_server_daemon.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_server_daemon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 import argparse
 import os
 import time
+import sys
 
 from fedml.cli.comm_utils.sys_utils import cleanup_all_fedml_server_api_processes, \
-    cleanup_all_fedml_server_learning_processes, cleanup_all_fedml_server_login_processes, get_python_program
+    cleanup_all_fedml_server_learning_processes, cleanup_all_fedml_server_login_processes, get_python_program, \
+    daemon_ota_upgrade
 from fedml.cli.model_deployment.device_server_constants import ServerConstants
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--type", "-t", help="Login or logout to ModelOps platform")
     parser.add_argument("--user", "-u", type=str,
@@ -33,14 +35,16 @@
             ServerConstants.cleanup_run_process()
             cleanup_all_fedml_server_api_processes(is_model_device=True)
             cleanup_all_fedml_server_learning_processes()
             cleanup_all_fedml_server_login_processes("device_server_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
+        daemon_ota_upgrade(args)
+
         login_pid = ServerConstants.exec_console_with_shell_script_list(
             [
                 get_python_program(),
                 "-W",
                 "ignore",
                 login_cmd,
                 "-t",
```

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_client_login.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_client_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_msg_object.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_msg_object.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/model_deployment/device_model_inference_entry.py` & `fedml-0.8.4a1/fedml/cli/model_deployment/device_model_inference_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,20 @@
     # start unified inference server
     running_model_name = ClientConstants.get_running_model_name(args.end_point_name,
                                                                 args.model_name, args.model_version,
                                                                 args.end_point_id, args.model_id)
     python_program = get_python_program()
     process = ServerConstants.exec_console_with_script(
         "REDIS_ADDR=\"{}\" REDIS_PORT=\"{}\" REDIS_PASSWORD=\"{}\" "
-        "END_POINT_ID=\"{}\" END_POINT_NAME=\"{}\" MODEL_ID=\"{}\" "
+        "END_POINT_NAME=\"{}\" "
         "MODEL_NAME=\"{}\" MODEL_VERSION=\"{}\" MODEL_INFER_URL=\"{}\" VERSION=\"{}\" "
         "{} -m uvicorn fedml.cli.model_deployment.device_model_inference:api --host 0.0.0.0 --port {} "
-        "--reload --log-level critical".format(
+        "--log-level critical".format(
             args.redis_addr, args.redis_port, args.redis_password,
-            str(args.end_point_id), args.end_point_name, str(args.model_id),
+            args.end_point_name,
             args.model_name, args.model_version, args.infer_url, args.config_version,
             python_program, str(args.infer_port)),
         should_capture_stdout=False,
         should_capture_stderr=False
     )
 
     while True:
```

### Comparing `fedml-0.8.3a9/fedml/cli/env/collect_env.py` & `fedml-0.8.4a1/fedml/cli/env/collect_env.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/cli.py` & `fedml-0.8.4a1/fedml/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from fedml.cli.server_deployment.docker_login import logout_with_server_docker_mode
 from fedml.cli.server_deployment.docker_login import logs_with_server_docker_mode
 from fedml.cli.edge_deployment.client_diagnosis import ClientDiagnosis
 from fedml.cli.comm_utils import sys_utils
 from fedml.cli.model_deployment import device_login_entry
 from fedml.cli.model_deployment.device_model_cards import FedMLModelCards
 from fedml.cli.server_deployment.job_manager import FedMLJobManager
+from fedml.cli.cli_utils import platform_is_valid
+from fedml.cli.server_deployment.app_manager import FedMLAppManager
 
 
 FEDML_MLOPS_BUILD_PRE_IGNORE_LIST = 'dist-packages,client-package.zip,server-package.zip,__pycache__,*.pyc,*.git'
 simulator_process_list = list()
 
 
 @click.group()
@@ -82,28 +84,30 @@
         if is_docker:
             logs_with_server_docker_mode(docker_rank)
             return
         display_server_logs()
 
 
 def display_client_logs():
-    run_id, edge_id = sys_utils.get_running_info(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
+    run_id, edge_id = sys_utils.get_running_info(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME,
+                                                 ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
     home_dir = expanduser("~")
     log_file = "{}/{}/fedml/logs/fedml-run-{}-edge-{}.log".format(
         home_dir, ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME, str(run_id), str(edge_id)
     )
     if os.path.exists(log_file):
         with open(log_file) as file_handle:
             log_lines = file_handle.readlines()
         for log_line in log_lines:
             click.echo(log_line)
 
 
 def display_server_logs():
-    run_id, edge_id = sys_utils.get_running_info(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
+    run_id, edge_id = sys_utils.get_running_info(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME,
+                                                 ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
     home_dir = expanduser("~")
     log_file = "{}/{}/fedml/logs/fedml-run-{}-edge-{}.log".format(
         home_dir, ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME, str(run_id), str(edge_id)
     )
     if os.path.exists(log_file):
         with open(log_file) as file_handle:
             log_lines = file_handle.readlines()
@@ -195,15 +199,16 @@
     if is_client is True:
         if is_docker:
             login_with_docker_mode(account_id, version, docker_rank)
             return
         pip_source_dir = os.path.dirname(__file__)
         login_cmd = os.path.join(pip_source_dir, "edge_deployment", "client_daemon.py")
         client_logout()
-        sys_utils.cleanup_login_process(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
+        sys_utils.cleanup_login_process(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME,
+                                        ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_client_learning_processes()
         sys_utils.cleanup_all_fedml_client_login_processes("client_login.py")
         sys_utils.cleanup_all_fedml_client_api_processes(kill_all=True)
 
         try:
             ClientConstants.login_role_list.index(role)
         except ValueError as e:
@@ -249,15 +254,16 @@
         if is_docker:
             login_with_server_docker_mode(account_id, version, docker_rank)
             return
 
         pip_source_dir = os.path.dirname(__file__)
         login_cmd = os.path.join(pip_source_dir, "server_deployment", "server_daemon.py")
         server_logout()
-        sys_utils.cleanup_login_process(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
+        sys_utils.cleanup_login_process(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME,
+                                        ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_server_learning_processes()
         sys_utils.cleanup_all_fedml_server_login_processes("server_login.py")
         sys_utils.cleanup_all_fedml_server_api_processes(kill_all=True)
         login_pid = subprocess.Popen(
             [
                 sys_utils.get_python_program(),
                 "-W",
@@ -310,35 +316,44 @@
 
     if is_client is True:
         if is_docker:
             logout_with_docker_mode(docker_rank)
             return
         sys_utils.cleanup_all_fedml_client_login_processes("client_daemon.py")
         client_logout()
-        sys_utils.cleanup_login_process(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
+        sys_utils.cleanup_login_process(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME,
+                                        ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_client_learning_processes()
         sys_utils.cleanup_all_fedml_client_login_processes("client_login.py")
         sys_utils.cleanup_all_fedml_client_api_processes(kill_all=True)
         sys_utils.cleanup_all_fedml_client_login_processes("client_daemon.py")
 
     if is_server is True:
         if is_docker:
             logout_with_server_docker_mode(docker_rank)
             return
         sys_utils.cleanup_all_fedml_server_login_processes("server_daemon.py")
         server_logout()
-        sys_utils.cleanup_login_process(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
+        sys_utils.cleanup_login_process(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME,
+                                        ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_server_learning_processes()
         sys_utils.cleanup_all_fedml_server_login_processes("server_login.py")
         sys_utils.cleanup_all_fedml_server_api_processes(kill_all=True)
         sys_utils.cleanup_all_fedml_server_login_processes("server_daemon.py")
 
 
 @cli.command("build", help="Build packages for MLOps platform (open.fedml.ai)")
 @click.option(
+    "--platform",
+    "-pf",
+    type=str,
+    default="octopus",
+    help="The platform name at the MLOps platform (options: octopus, parrot, spider, beehive).",
+)
+@click.option(
     "--type",
     "-t",
     type=str,
     default="client",
     help="client or server? (value: client; server)",
 )
 @click.option(
@@ -364,22 +379,25 @@
 @click.option(
     "--ignore",
     "-ig",
     type=str,
     default="",
     help="the ignore list for copying files, the format is as follows: *.model,__pycache__,*.data*, ",
 )
-def mlops_build(type, source_folder, entry_point, config_folder, dest_folder, ignore):
+def mlops_build(platform, type, source_folder, entry_point, config_folder, dest_folder, ignore):
     click.echo("Argument for type: " + type)
     click.echo("Argument for source folder: " + source_folder)
     click.echo("Argument for entry point: " + entry_point)
     click.echo("Argument for config folder: " + config_folder)
     click.echo("Argument for destination package folder: " + dest_folder)
     click.echo("Argument for ignore lists: " + ignore)
 
+    if not platform_is_valid(platform):
+        return
+
     if type == "client" or type == "server":
         click.echo(
             "Now, you are building the fedml packages which will be used in the MLOps "
             "platform."
         )
         click.echo(
             "The packages will be used for client training and server aggregation."
@@ -538,15 +556,15 @@
             "  log_file_dir: /fedml/fedml-package/fedml/data\n",
             "  log_server_url: ${FEDSYS.LOG_SERVER_URL}\n",
             "  client_id_list: ${FEDSYS.CLIENT_ID_LIST}\n",
             "  client_objects: ${FEDSYS.CLIENT_OBJECT_LIST}\n",
             "  is_using_local_data: ${FEDSYS.IS_USING_LOCAL_DATA}\n",
             "  synthetic_data_url: ${FEDSYS.SYNTHETIC_DATA_URL}\n",
             "  client_num_in_total: ${FEDSYS.CLIENT_NUM}\n",
-            ]
+        ]
     )
     mlops_pkg_conf_file.flush()
     mlops_pkg_conf_file.close()
 
     local_mlops_package = os.path.join(mlops_package_base_dir, mlops_package_file_name)
     if os.path.exists(local_mlops_package):
         os.remove(os.path.join(mlops_package_base_dir, mlops_package_file_name))
@@ -581,26 +599,30 @@
     "--s3", "-s", default=None, is_flag=True, help="check the connection to AWS S3 server.",
 )
 @click.option(
     "--mqtt", "-m", default=None, is_flag=True, help="check the connection to mqtt.fedml.ai (1883).",
 )
 @click.option(
 
-    "--mqtt_daemon", "-d", default=None, is_flag=True, help="check the connection to mqtt.fedml.ai (1883) with loop mode.",
+    "--mqtt_daemon", "-d", default=None, is_flag=True,
+    help="check the connection to mqtt.fedml.ai (1883) with loop mode.",
 )
 @click.option(
-    "--mqtt_s3_backend_server", "-msbs", default=None, is_flag=True, help="check the connection to mqtt.fedml.ai (1883) as mqtt+s3 server.",
+    "--mqtt_s3_backend_server", "-msbs", default=None, is_flag=True,
+    help="check the connection to mqtt.fedml.ai (1883) as mqtt+s3 server.",
 )
 @click.option(
-    "--mqtt_s3_backend_client", "-msbc", default=None, is_flag=True, help="check the connection to mqtt.fedml.ai (1883) as mqtt+s3 client.",
+    "--mqtt_s3_backend_client", "-msbc", default=None, is_flag=True,
+    help="check the connection to mqtt.fedml.ai (1883) as mqtt+s3 client.",
 )
 @click.option(
     "--mqtt_s3_backend_run_id", "-rid", type=str, default="fedml_diag_9988", help="mqtt+s3 run id.",
 )
-def mlops_diagnosis(open, s3, mqtt, mqtt_daemon, mqtt_s3_backend_server, mqtt_s3_backend_client, mqtt_s3_backend_run_id):
+def mlops_diagnosis(open, s3, mqtt, mqtt_daemon, mqtt_s3_backend_server, mqtt_s3_backend_client,
+                    mqtt_s3_backend_run_id):
     check_open = open
     check_s3 = s3
     check_mqtt = mqtt
     check_mqtt_daemon = mqtt_daemon
 
     check_mqtt_s3_backend_server = mqtt_s3_backend_server
     check_mqtt_s3_backend_client = mqtt_s3_backend_client
@@ -667,14 +689,15 @@
             "-t",
             "client",
             "-r",
             run_id
         ]
         ).pid
 
+
 @cli.command(
     "env",
     help="collect the environment information to help debugging, including OS, Hardware Architecture, "
          "Python version, etc.",
 )
 def env():
     collect_env()
@@ -688,14 +711,132 @@
     # for argument in arguments:
     #     click.echo(argument)
 
     from fedml.cross_silo.client.client_launcher import CrossSiloLauncher
     CrossSiloLauncher.launch_dist_trainers(arguments[0], list(arguments[1:]))
 
 
+@cli.group("app")
+def app():
+    """
+    Manage applications on the MLOps platform..
+    """
+    pass
+
+
+@app.command("create", help="Create an application on the MLOps platform (open.fedml.ai).")
+@click.option(
+    "--platform",
+    "-pf",
+    type=str,
+    default="octopus",
+    help="The platform name at the MLOps platform (options: octopus, parrot, spider, beehive).",
+)
+@click.option(
+    "--client_package", "-cp", type=str, help="client package path.",
+)
+@click.option(
+    "--server_package", "-sp", type=str, help="server package path.",
+)
+@click.option(
+    "--user", "-u", type=str, help="user id.",
+)
+@click.option(
+    "--api_key", "-k", type=str, help="user api key.",
+)
+@click.option(
+    "--version",
+    "-v",
+    type=str,
+    default="release",
+    help="interact with which version of ModelOps platform. It should be dev, test or release",
+)
+@click.option(
+    "--local_server",
+    "-ls",
+    type=str,
+    default="127.0.0.1",
+    help="local server address.",
+)
+def create_application(platform, application_name, client_package, server_package,
+                       user, api_key, version, local_server):
+    if user is None or api_key is None:
+        click.echo("You must provide arguments for User Id and Api Key (use -u and -k options).")
+        return
+
+    client_package_file = os.path.basename(client_package)
+    server_package_file = os.path.basename(server_package)
+    client_package_url = client_package_file
+    server_package_url = server_package_file
+    FedMLJobManager.get_instance().set_config_version(version)
+    result = FedMLAppManager.get_instance().create_app(platform, application_name,
+                                                       client_package_url, client_package_file, server_package_url, server_package_file,
+                                                       user, api_key)
+    if result:
+        click.echo("Create application {} successfully.".format(application_name))
+    else:
+        click.echo("Failed to create application, please check your network connection "
+                   "whether could be access the MLOps platform.")
+
+
+@app.command("update", help="Update an application on the MLOps platform (open.fedml.ai).")
+@click.option(
+    "--platform",
+    "-pf",
+    type=str,
+    default="octopus",
+    help="The platform name at the MLOps platform (options: octopus, parrot, spider, beehive).",
+)
+@click.option(
+    "--client_package", "-cp", type=str, help="client package path.",
+)
+@click.option(
+    "--server_package", "-sp", type=str, help="server package path.",
+)
+@click.option(
+    "--user", "-u", type=str, help="user id.",
+)
+@click.option(
+    "--api_key", "-k", type=str, help="user api key.",
+)
+@click.option(
+    "--version",
+    "-v",
+    type=str,
+    default="release",
+    help="interact with which version of ModelOps platform. It should be dev, test or release",
+)
+@click.option(
+    "--local_server",
+    "-ls",
+    type=str,
+    default="127.0.0.1",
+    help="local server address.",
+)
+def update_application(platform, application_name, client_package, server_package,
+                       user, api_key, version, local_server):
+    if user is None or api_key is None:
+        click.echo("You must provide arguments for User Id and Api Key (use -u and -k options).")
+        return
+
+    client_package_file = os.path.basename(client_package)
+    server_package_file = os.path.basename(server_package)
+    client_package_url = client_package_file
+    server_package_url = server_package_file
+    FedMLJobManager.get_instance().set_config_version(version)
+    result = FedMLAppManager.get_instance().update_app(platform, application_name,
+                                                       client_package_url, client_package_file, server_package_url, server_package_file,
+                                                       user, api_key)
+    if result:
+        click.echo("Create application {} successfully.".format(application_name))
+    else:
+        click.echo("Failed to create application, please check your network connection "
+                   "whether could be access the MLOps platform.")
+
+
 @cli.group("jobs")
 def jobs():
     """
     Manage jobs on the MLOps platform.
     """
     pass
```

### Comparing `fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml` & `fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml` & `fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml` & `fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml` & `fedml-0.8.4a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/server_data_interface.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/server_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/server_runner.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/server_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,64 +620,88 @@
         edge_id_list = self.request_json["edgeids"]
         logging.info("Edge ids: " + str(edge_id_list))
         for edge_id in edge_id_list:
             topic_start_train = "flserver_agent/" + str(edge_id) + "/start_train"
             logging.info("start_train: send topic " + topic_start_train + " to client...")
             self.client_mqtt_mgr.send_message(topic_start_train, json.dumps(self.request_json))
 
+    def ota_upgrade(self, payload, request_json):
+        no_upgrade = False
+        upgrade_version = None
+        run_id = request_json["runId"]
+
+        try:
+            run_config = request_json.get("run_config", None)
+            parameters = run_config.get("parameters", None)
+            common_args = parameters.get("common_args", None)
+            no_upgrade = common_args.get("no_upgrade", False)
+            upgrade_version = common_args.get("upgrade_version", None)
+        except Exception as e:
+            pass
+
+        should_upgrade = True
+        if upgrade_version is None or upgrade_version == "latest":
+            try:
+                fedml_is_latest_version, local_ver, remote_ver = sys_utils. \
+                    check_fedml_is_latest_version(self.version)
+            except Exception as e:
+                return
+
+            if fedml_is_latest_version:
+                should_upgrade = False
+            upgrade_version = remote_ver
+
+        if no_upgrade:
+            should_upgrade = False
+
+        if should_upgrade:
+            job_obj = FedMLServerDataInterface.get_instance().get_job_by_id(run_id)
+            if job_obj is None:
+                FedMLServerDataInterface.get_instance(). \
+                    save_started_job(run_id, self.edge_id, time.time(),
+                                     ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING,
+                                     ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING,
+                                     payload)
+                self.mlops_metrics.report_server_training_status(run_id,
+                                                                 ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING)
+            logging.info(f"Upgrade to version {upgrade_version} ...")
+
+            sys_utils.do_upgrade(self.version, upgrade_version)
+
+            raise Exception("Restarting after upgraded...")
+
     def callback_start_train(self, topic=None, payload=None):
         logging.info("callback_start_train payload: {}".format(payload))
 
         # get training params
         if self.run_as_cloud_server:
             message_bytes = payload.encode("ascii")
             base64_bytes = base64.b64decode(message_bytes)
             payload = base64_bytes.decode("ascii")
-            request_json = json.loads(payload)
             logging.info("decoded payload: {}".format(payload))
-        else:
-            request_json = json.loads(payload)
-            run_id = request_json["runId"]
-
-            no_upgrade = False
-            upgrade_version = None
-            try:
-                run_config = request_json.get("run_config", None)
-                parameters = run_config.get("parameters", None)
-                common_args = parameters.get("common_args", None)
-                no_upgrade = common_args.get("no_upgrade", False)
-                upgrade_version = common_args.get("upgrade_version", None)
-            except Exception as e:
-                pass
-
-            if not no_upgrade:
-                job_obj = FedMLServerDataInterface.get_instance().get_job_by_id(run_id)
-                if job_obj is None:
-                    FedMLServerDataInterface.get_instance(). \
-                        save_started_job(run_id, self.edge_id, time.time(),
-                                         ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING,
-                                         ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING,
-                                         payload)
-                    self.mlops_metrics.report_server_training_status(run_id,
-                                                                     ServerConstants.MSG_MLOPS_SERVER_STATUS_UPGRADING)
-                    if upgrade_version is None or upgrade_version == "latest":
-                        logging.info("Upgrade to latest version...")
-                        os.system("pip uninstall -y fedml;pip install fedml")
-                    else:
-                        logging.info(f"Upgrade to version {upgrade_version} ...")
-                        os.system(f"pip uninstall -y fedml;pip install fedml=={upgrade_version}")
-
-                    raise Exception("Upgrading...")
 
+        request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
-        self.start_request_json = payload
+
         run_id = request_json["runId"]
         if self.run_as_edge_server_and_agent:
+            # Start log processor for current run
+            logging.info("start the log processor.")
+            self.args.run_id = run_id
+            self.args.edge_id = self.edge_id
+            MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
+            MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(run_id, self.edge_id)
+
+        if not self.run_as_cloud_agent and not self.run_as_cloud_server:
+            self.ota_upgrade(payload, request_json)
+
+        self.start_request_json = payload
+        if self.run_as_edge_server_and_agent:
             if self.run_process is not None and \
                     sys_utils.get_process_running_count(ServerConstants.SERVER_LOGIN_PROGRAM) >= 2:
                 logging.info("There is a running job {}.".format(
                     self.run_process.pid
                 ))
                 try:
                     if self.run_process_event is not None:
@@ -706,17 +730,14 @@
             topic_client_exit_train_with_exception = "flserver_agent/" + str(run_id) + \
                                                      "/client_exit_train_with_exception"
             self.mqtt_mgr.add_message_listener(topic_client_exit_train_with_exception,
                                                self.callback_client_exit_train_with_exception)
             self.mqtt_mgr.subscribe_msg(topic_client_exit_train_with_exception)
 
         if self.run_as_edge_server_and_agent:
-            # Start log processor for current run
-            logging.info("start the log processor.")
-            MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(run_id, self.edge_id)
             self.args.run_id = run_id
 
             server_runner = FedMLServerRunner(
                 self.args, run_id=run_id, request_json=request_json, agent_config=self.agent_config
             )
             server_runner.run_as_edge_server_and_agent = self.run_as_edge_server_and_agent
             server_runner.edge_id = self.edge_id
@@ -1454,15 +1475,15 @@
         # Init local database
         FedMLServerDataInterface.get_instance().create_job_table()
 
         # Start local API services
         python_program = get_python_program()
         local_api_process = ServerConstants.exec_console_with_script(
             "{} -m uvicorn fedml.cli.server_deployment.server_api:api --host 0.0.0.0 --port {} "
-            "--reload --log-level critical".format(python_program, ServerConstants.LOCAL_SERVER_API_PORT),
+            "--log-level critical".format(python_program, ServerConstants.LOCAL_SERVER_API_PORT),
             should_capture_stdout=False,
             should_capture_stderr=False
         )
 
         # Setup MQTT connected listener
         self.mqtt_mgr.add_connected_listener(self.on_agent_mqtt_connected)
         self.mqtt_mgr.add_disconnected_listener(self.on_agent_mqtt_disconnected)
@@ -1479,15 +1500,18 @@
         self.recover_start_train_msg_after_upgrading()
 
     def start_agent_mqtt_loop(self):
         # Start MQTT message loop
         try:
             self.mqtt_mgr.loop_forever()
         except Exception as e:
-            logging.info("Server tracing: {}".format(traceback.format_exc()))
+            if str(e) == "Restarting after upgraded...":
+                logging.info("Restarting after upgraded...")
+            else:
+                logging.info("Server tracing: {}".format(traceback.format_exc()))
             self.mqtt_mgr.loop_stop()
             self.mqtt_mgr.disconnect()
             self.release_client_mqtt_mgr()
             time.sleep(5)
             sys_utils.cleanup_all_fedml_server_login_processes(
                 ServerConstants.SERVER_LOGIN_PROGRAM, clean_process_group=False)
             sys.exit(1)
```

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/job_manager.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/job_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/docker_login.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/docker_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/server_api.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/server_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 @api.post('/fedml/api/v2/currentJobStatus')
 async def get_current_job_status(request: Request):
     # Get json data
     input_json = await request.json()
 
     current_job = FedMLServerDataInterface.get_instance().get_current_job()
+    if current_job is None:
+        return {}
     response = {"jobId": current_job.job_id,
                 "edgeId": current_job.edge_id,
                 "startedTime": int(float(current_job.started_time)) if current_job.started_time != "" else 0,
                 "endedTime": int(float(current_job.ended_time)) if current_job.ended_time != "" else 0,
                 "progress": current_job.progress, "ETA": int(current_job.eta),
                 "failedTime": int(float(current_job.failed_time))if current_job.ended_time != "" else 0,
                 "errorCode": current_job.error_code,
```

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/server_daemon.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/server_daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 import argparse
 import os
 import time
+import sys
 
 from fedml.cli.comm_utils.sys_utils import cleanup_all_fedml_server_api_processes,\
-    cleanup_all_fedml_server_learning_processes,cleanup_all_fedml_server_login_processes, get_python_program
+    cleanup_all_fedml_server_learning_processes,cleanup_all_fedml_server_login_processes, get_python_program, \
+    daemon_ota_upgrade
 from fedml.cli.server_deployment.server_constants import ServerConstants
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--type", "-t", help="Login or logout to MLOps platform")
     parser.add_argument("--user", "-u", type=str,
@@ -30,14 +32,16 @@
             ServerConstants.cleanup_run_process()
             cleanup_all_fedml_server_api_processes()
             cleanup_all_fedml_server_learning_processes()
             cleanup_all_fedml_server_login_processes("server_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
+        daemon_ota_upgrade(args)
+
         login_pid = ServerConstants.exec_console_with_shell_script_list(
             [
                 get_python_program(),
                 "-W",
                 "ignore",
                 login_cmd,
                 "-t",
```

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml` & `fedml-0.8.4a1/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/server_login.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/server_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/cli/server_deployment/server_constants.py` & `fedml-0.8.4a1/fedml/cli/server_deployment/server_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,26 @@
     @staticmethod
     def get_job_start_url(config_version="release"):
         job_ops_url = "{}/fedmlOpsServer/api/v1/application/runApplicationFromCli".format(
             ServerConstants.get_mlops_url(config_version))
         return job_ops_url
 
     @staticmethod
+    def get_app_create_url(config_version="release"):
+        app_url = "{}/fedmlOpsServer/api/v1/application/createApplicationFromCli".format(
+            ServerConstants.get_mlops_url(config_version))
+        return app_url
+
+    @staticmethod
+    def get_app_update_url(config_version="release"):
+        app_url = "{}/fedmlOpsServer/api/v1/application/updateApplicationFromCli".format(
+            ServerConstants.get_mlops_url(config_version))
+        return app_url
+
+    @staticmethod
     def cleanup_run_process():
         try:
             home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
                                            "runner-sub-process.id")
             process_info = load_yaml_config(process_id_file)
```

### Comparing `fedml-0.8.3a9/fedml/ml/aggregator/aggregator_creator.py` & `fedml-0.8.4a1/fedml/ml/aggregator/aggregator_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator_nwp.py` & `fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/aggregator/default_aggregator.py` & `fedml-0.8.4a1/fedml/ml/aggregator/default_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator.py` & `fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator_classification.py` & `fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/aggregator/agg_operator.py` & `fedml-0.8.4a1/fedml/ml/aggregator/agg_operator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/aggregator/my_server_aggregator_prediction.py` & `fedml-0.8.4a1/fedml/ml/aggregator/my_server_aggregator_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/engine/ml_engine_adapter.py` & `fedml-0.8.4a1/fedml/ml/engine/ml_engine_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/engine/torch_process_group_manager.py` & `fedml-0.8.4a1/fedml/ml/engine/torch_process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/scaffold_trainer.py` & `fedml-0.8.4a1/fedml/ml/trainer/scaffold_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/trainer_creator.py` & `fedml-0.8.4a1/fedml/ml/trainer/trainer_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/fednova_trainer.py` & `fedml-0.8.4a1/fedml/ml/trainer/fednova_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/fedprox_trainer.py` & `fedml-0.8.4a1/fedml/ml/trainer/fedprox_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer_nwp.py` & `fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/feddyn_trainer copy.py` & `fedml-0.8.4a1/fedml/ml/trainer/feddyn_trainer copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/feddyn_trainer.py` & `fedml-0.8.4a1/fedml/ml/trainer/feddyn_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer.py` & `fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/mime_trainer.py` & `fedml-0.8.4a1/fedml/ml/trainer/mime_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer_tag_prediction.py` & `fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer_tag_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/ml/trainer/my_model_trainer_classification.py` & `fedml-0.8.4a1/fedml/ml/trainer/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/linear/lr_cifar10.py` & `fedml-0.8.4a1/fedml/model/linear/lr_cifar10.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/model_hub.py` & `fedml-0.8.4a1/fedml/model/model_hub.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/mobile/mnn_lenet.py` & `fedml-0.8.4a1/fedml/model/mobile/mnn_lenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/mobile/mnn_resnet.py` & `fedml-0.8.4a1/fedml/model/mobile/mnn_resnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/mobile/torch_lenet.py` & `fedml-0.8.4a1/fedml/model/mobile/torch_lenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/nlp/model_args.py` & `fedml-0.8.4a1/fedml/model/nlp/model_args.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/nlp/rnn.py` & `fedml-0.8.4a1/fedml/model/nlp/rnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/finance/vfl_models_standalone.py` & `fedml-0.8.4a1/fedml/model/finance/vfl_models_standalone.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet56/resnet_pretrained.py` & `fedml-0.8.4a1/fedml/model/cv/resnet56/resnet_pretrained.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet56/resnet_server.py` & `fedml-0.8.4a1/fedml/model/cv/resnet56/resnet_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet56/resnet_client.py` & `fedml-0.8.4a1/fedml/model/cv/resnet56/resnet_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/vgg.py` & `fedml-0.8.4a1/fedml/model/cv/vgg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet_torch.py` & `fedml-0.8.4a1/fedml/model/cv/resnet_torch.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/efficientnet_utils.py` & `fedml-0.8.4a1/fedml/model/cv/efficientnet_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet_cifar.py` & `fedml-0.8.4a1/fedml/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/mobilenet_v3.py` & `fedml-0.8.4a1/fedml/model/cv/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/batchnorm_utils.py` & `fedml-0.8.4a1/fedml/model/cv/batchnorm_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/cnn.py` & `fedml-0.8.4a1/fedml/model/cv/cnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/mnist_gan.py` & `fedml-0.8.4a1/fedml/model/cv/mnist_gan.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/efficientnet.py` & `fedml-0.8.4a1/fedml/model/cv/efficientnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet_all.py` & `fedml-0.8.4a1/fedml/model/cv/resnet_all.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/mobilenet.py` & `fedml-0.8.4a1/fedml/model/cv/mobilenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/common.py` & `fedml-0.8.4a1/fedml/model/cv/common.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet.py` & `fedml-0.8.4a1/fedml/model/cv/resnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/model_search_gdas.py` & `fedml-0.8.4a1/fedml/model/cv/darts/model_search_gdas.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/visualize.py` & `fedml-0.8.4a1/fedml/model/cv/darts/visualize.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/architect.py` & `fedml-0.8.4a1/fedml/model/cv/darts/architect.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/model.py` & `fedml-0.8.4a1/fedml/model/cv/darts/model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/operations.py` & `fedml-0.8.4a1/fedml/model/cv/darts/operations.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/utils.py` & `fedml-0.8.4a1/fedml/model/cv/darts/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/model_search.py` & `fedml-0.8.4a1/fedml/model/cv/darts/model_search.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/train.py` & `fedml-0.8.4a1/fedml/model/cv/darts/train.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/genotypes.py` & `fedml-0.8.4a1/fedml/model/cv/darts/genotypes.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/darts/train_search.py` & `fedml-0.8.4a1/fedml/model/cv/darts/train_search.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/resnet_gn.py` & `fedml-0.8.4a1/fedml/model/cv/resnet_gn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/model/cv/group_normalization.py` & `fedml-0.8.4a1/fedml/model/cv/group_normalization.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/device/gpu_mapping_cross_silo.py` & `fedml-0.8.4a1/fedml/device/gpu_mapping_cross_silo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/device/gpu_mapping_mpi.py` & `fedml-0.8.4a1/fedml/device/gpu_mapping_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/device/device.py` & `fedml-0.8.4a1/fedml/device/device.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/runner.py` & `fedml-0.8.4a1/fedml/fa/runner.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/fa_server.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/fa_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/fa_client.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/fa_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/server/message_define.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/server/fedml_server_manager.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/server/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/server/fedml_aggregator.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/server/server_initializer.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/client_initializer.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/client_launcher.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/message_define.py` & `fedml-0.8.4a1/fedml/serving/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/fa_local_analyzer.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/client/fa_local_analyzer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/fedml_client_slave_manager.py` & `fedml-0.8.4a1/fedml/serving/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/process_group_manager.py` & `fedml-0.8.4a1/fedml/serving/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/cross_silo/client/fedml_client_master_manager.py` & `fedml-0.8.4a1/fedml/fa/cross_silo/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/aggregator/frequency_estimation_aggregator.py` & `fedml-0.8.4a1/fedml/fa/aggregator/frequency_estimation_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/aggregator/intersection_aggregator.py` & `fedml-0.8.4a1/fedml/fa/aggregator/intersection_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/aggregator/union_aggregator.py` & `fedml-0.8.4a1/fedml/fa/aggregator/union_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/aggregator/avg_aggregator.py` & `fedml-0.8.4a1/fedml/fa/aggregator/avg_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/aggregator/k_percentile_element_aggregator.py` & `fedml-0.8.4a1/fedml/fa/aggregator/k_percentile_element_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/aggregator/global_analyzer_creator.py` & `fedml-0.8.4a1/fedml/fa/aggregator/global_analyzer_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/simulation/sp/client.py` & `fedml-0.8.4a1/fedml/fa/simulation/sp/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/simulation/sp/simulator.py` & `fedml-0.8.4a1/fedml/fa/simulation/sp/simulator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/simulation/utils.py` & `fedml-0.8.4a1/fedml/fa/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/__init__.py` & `fedml-0.8.4a1/fedml/fa/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/local_analyzer/heavy_hitter_triehh.py` & `fedml-0.8.4a1/fedml/fa/local_analyzer/heavy_hitter_triehh.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/local_analyzer/client_analyzer_creator.py` & `fedml-0.8.4a1/fedml/fa/local_analyzer/client_analyzer_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/base_frame/server_aggregator.py` & `fedml-0.8.4a1/fedml/fa/base_frame/server_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/base_frame/client_analyzer.py` & `fedml-0.8.4a1/fedml/fa/base_frame/client_analyzer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/data/data_loader.py` & `fedml-0.8.4a1/fedml/fa/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/data/twitter_Sentiment140/data_loader.py` & `fedml-0.8.4a1/fedml/fa/data/twitter_Sentiment140/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/data/utils.py` & `fedml-0.8.4a1/fedml/fa/data/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/fa/data/fake_numeric_data/data_loader.py` & `fedml-0.8.4a1/fedml/fa/data/fake_numeric_data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/launch_cross_device.py` & `fedml-0.8.4a1/fedml/launch_cross_device.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/MNIST/mnist_mobile_preprocessor.py` & `fedml-0.8.4a1/fedml/data/MNIST/mnist_mobile_preprocessor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/MNIST/data_loader.py` & `fedml-0.8.4a1/fedml/data/MNIST/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/MNIST/stats.py` & `fedml-0.8.4a1/fedml/data/MNIST/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/lending_club_loan/lending_club_dataset.py` & `fedml-0.8.4a1/fedml/data/lending_club_loan/lending_club_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/lending_club_loan/lending_club_feature_group.py` & `fedml-0.8.4a1/fedml/data/lending_club_loan/lending_club_feature_group.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fed_cifar100/data_loader.py` & `fedml-0.8.4a1/fedml/data/fed_cifar100/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fed_cifar100/dataset.py` & `fedml-0.8.4a1/fedml/data/fed_cifar100/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fed_cifar100/utils.py` & `fedml-0.8.4a1/fedml/data/fed_cifar100/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/FederatedEMNIST/data_loader.py` & `fedml-0.8.4a1/fedml/data/FederatedEMNIST/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cifar100/data_loader.py` & `fedml-0.8.4a1/fedml/data/cifar100/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cifar100/datasets.py` & `fedml-0.8.4a1/fedml/data/cifar100/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/data_loader.py` & `fedml-0.8.4a1/fedml/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/file_operation.py` & `fedml-0.8.4a1/fedml/data/file_operation.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/shakespeare/language_utils.py` & `fedml-0.8.4a1/fedml/data/shakespeare/language_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/shakespeare/data_loader.py` & `fedml-0.8.4a1/fedml/data/shakespeare/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/shakespeare/stats.py` & `fedml-0.8.4a1/fedml/data/shakespeare/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/synthetic_1_1/data_loader.py` & `fedml-0.8.4a1/fedml/data/synthetic_1_1/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/synthetic_1_1/stats.py` & `fedml-0.8.4a1/fedml/data/synthetic_1_1/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/synthetic_1_1/generate_synthetic.py` & `fedml-0.8.4a1/fedml/data/synthetic_1_1/generate_synthetic.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/Landmarks/download_without_tff.py` & `fedml-0.8.4a1/fedml/data/Landmarks/download_without_tff.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/Landmarks/data_loader.py` & `fedml-0.8.4a1/fedml/data/Landmarks/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/Landmarks/datasets.py` & `fedml-0.8.4a1/fedml/data/Landmarks/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/Landmarks/utils.py` & `fedml-0.8.4a1/fedml/data/Landmarks/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/Landmarks/check_download.py` & `fedml-0.8.4a1/fedml/data/Landmarks/check_download.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/Landmarks/download_without_tf.py` & `fedml-0.8.4a1/fedml/data/Landmarks/download_without_tf.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fednlp/base/preprocess/base_example.py` & `fedml-0.8.4a1/fedml/data/fednlp/base/preprocess/base_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fednlp/base/raw_data/partition.py` & `fedml-0.8.4a1/fedml/data/fednlp/base/raw_data/partition.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py` & `fedml-0.8.4a1/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fednlp/base/data_manager/base_data_manager.py` & `fedml-0.8.4a1/fedml/data/fednlp/base/data_manager/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fednlp/base/utils.py` & `fedml-0.8.4a1/fedml/data/fednlp/base/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/NUS_WIDE/nus_wide_dataset.py` & `fedml-0.8.4a1/fedml/data/NUS_WIDE/nus_wide_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/stackoverflow_lr/data_loader.py` & `fedml-0.8.4a1/fedml/data/stackoverflow_lr/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/stackoverflow_lr/dataset.py` & `fedml-0.8.4a1/fedml/data/stackoverflow_lr/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/stackoverflow_lr/utils.py` & `fedml-0.8.4a1/fedml/data/stackoverflow_lr/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fed_shakespeare/data_loader.py` & `fedml-0.8.4a1/fedml/data/fed_shakespeare/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/fed_shakespeare/utils.py` & `fedml-0.8.4a1/fedml/data/fed_shakespeare/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/ImageNet/data_loader.py` & `fedml-0.8.4a1/fedml/data/ImageNet/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/ImageNet/datasets.py` & `fedml-0.8.4a1/fedml/data/ImageNet/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/ImageNet/datasets_hdf5.py` & `fedml-0.8.4a1/fedml/data/ImageNet/datasets_hdf5.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/data_loader_cross_silo.py` & `fedml-0.8.4a1/fedml/data/data_loader_cross_silo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cinic10/data_loader.py` & `fedml-0.8.4a1/fedml/data/cinic10/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cinic10/datasets.py` & `fedml-0.8.4a1/fedml/data/cinic10/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/stackoverflow_nwp/data_loader.py` & `fedml-0.8.4a1/fedml/data/stackoverflow_nwp/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/stackoverflow_nwp/dataset.py` & `fedml-0.8.4a1/fedml/data/stackoverflow_nwp/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/stackoverflow_nwp/utils.py` & `fedml-0.8.4a1/fedml/data/stackoverflow_nwp/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/UCI/data_loader_for_susy_and_ro.py` & `fedml-0.8.4a1/fedml/data/UCI/data_loader_for_susy_and_ro.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/edge_case_examples/data_loader.py` & `fedml-0.8.4a1/fedml/data/edge_case_examples/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/edge_case_examples/datasets.py` & `fedml-0.8.4a1/fedml/data/edge_case_examples/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cifar10/efficient_loader.py` & `fedml-0.8.4a1/fedml/data/cifar10/efficient_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cifar10/data_loader.py` & `fedml-0.8.4a1/fedml/data/cifar10/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cifar10/datasets.py` & `fedml-0.8.4a1/fedml/data/cifar10/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml/data/cifar10/without_reload.py` & `fedml-0.8.4a1/fedml/data/cifar10/without_reload.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.3a9/fedml.egg-info/PKG-INFO` & `fedml-0.8.4a1/fedml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml
-Version: 0.8.3a9
+Version: 0.8.4a1
 Summary: A research and production integrated edge-cloud library for federated/distributed machine learning at anywhere at any scale.
 Home-page: https://github.com/FedML-AI/FedML
 Author: FedML Team
 Author-email: ch@fedml.ai
 License: Apache 2.0
 Description: # FedML - The community building and connecting AI anywhere at any scale
```

### Comparing `fedml-0.8.3a9/fedml.egg-info/SOURCES.txt` & `fedml-0.8.4a1/fedml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -187,29 +187,50 @@
 examples/simulation/sp_turboaggregate_mnist_lr_example/__init__.py
 examples/simulation/sp_turboaggregate_mnist_lr_example/torch_turboaggregate_mnist_lr_step_by_step_example.py
 examples/simulation/sp_vertical_mnist_lr_example/__init__.py
 examples/simulation/sp_vertical_mnist_lr_example/torch_vertical_mnist_lr_step_by_step_example.py
 fedml/__init__.py
 fedml/arguments.py
 fedml/constants.py
+fedml/launch_cheeath_llm.py
 fedml/launch_cross_device.py
 fedml/launch_cross_silo_hi.py
 fedml/launch_cross_silo_horizontal.py
+fedml/launch_serving.py
 fedml/launch_simulation.py
 fedml/runner.py
 fedml.egg-info/PKG-INFO
 fedml.egg-info/SOURCES.txt
 fedml.egg-info/dependency_links.txt
 fedml.egg-info/entry_points.txt
 fedml.egg-info/requires.txt
 fedml.egg-info/top_level.txt
 fedml/centralized/__init__.py
 fedml/centralized/centralized_trainer.py
+fedml/cheetah_llm/__init__.py
+fedml/cheetah_llm/fedml_client.py
+fedml/cheetah_llm/fedml_server.py
+fedml/cheetah_llm/client/__init__.py
+fedml/cheetah_llm/client/client_initializer.py
+fedml/cheetah_llm/client/client_launcher.py
+fedml/cheetah_llm/client/fedml_client_master_manager.py
+fedml/cheetah_llm/client/fedml_client_slave_manager.py
+fedml/cheetah_llm/client/fedml_trainer.py
+fedml/cheetah_llm/client/fedml_trainer_dist_adapter.py
+fedml/cheetah_llm/client/message_define.py
+fedml/cheetah_llm/client/process_group_manager.py
+fedml/cheetah_llm/client/utils.py
+fedml/cheetah_llm/server/__init__.py
+fedml/cheetah_llm/server/fedml_aggregator.py
+fedml/cheetah_llm/server/fedml_server_manager.py
+fedml/cheetah_llm/server/message_define.py
+fedml/cheetah_llm/server/server_initializer.py
 fedml/cli/__init__.py
 fedml/cli/cli.py
+fedml/cli/cli_utils.py
 fedml/cli/build-package/__init__.py
 fedml/cli/build-package/mlops-core/__init__.py
 fedml/cli/build-package/mlops-core/fedml-client/__init__.py
 fedml/cli/build-package/mlops-core/fedml-client/client-package/__init__.py
 fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/__init__.py
 fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml
 fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/__init__.py
@@ -262,14 +283,15 @@
 fedml/cli/model_deployment/device_server_data_interface.py
 fedml/cli/model_deployment/device_server_login.py
 fedml/cli/model_deployment/device_server_runner.py
 fedml/cli/model_deployment/docker_client_login.py
 fedml/cli/model_deployment/docker_server_login.py
 fedml/cli/model_deployment/modelops_configs.py
 fedml/cli/server_deployment/__init__.py
+fedml/cli/server_deployment/app_manager.py
 fedml/cli/server_deployment/docker_login.py
 fedml/cli/server_deployment/job_manager.py
 fedml/cli/server_deployment/server_api.py
 fedml/cli/server_deployment/server_constants.py
 fedml/cli/server_deployment/server_daemon.py
 fedml/cli/server_deployment/server_data_interface.py
 fedml/cli/server_deployment/server_login.py
@@ -675,14 +697,32 @@
 fedml/model/mobile/__init__.py
 fedml/model/mobile/mnn_lenet.py
 fedml/model/mobile/mnn_resnet.py
 fedml/model/mobile/torch_lenet.py
 fedml/model/nlp/__init__.py
 fedml/model/nlp/model_args.py
 fedml/model/nlp/rnn.py
+fedml/serving/__init__.py
+fedml/serving/fedml_client.py
+fedml/serving/fedml_server.py
+fedml/serving/client/__init__.py
+fedml/serving/client/client_initializer.py
+fedml/serving/client/client_launcher.py
+fedml/serving/client/fedml_client_master_manager.py
+fedml/serving/client/fedml_client_slave_manager.py
+fedml/serving/client/fedml_trainer.py
+fedml/serving/client/fedml_trainer_dist_adapter.py
+fedml/serving/client/message_define.py
+fedml/serving/client/process_group_manager.py
+fedml/serving/client/utils.py
+fedml/serving/server/__init__.py
+fedml/serving/server/fedml_aggregator.py
+fedml/serving/server/fedml_server_manager.py
+fedml/serving/server/message_define.py
+fedml/serving/server/server_initializer.py
 fedml/simulation/__init__.py
 fedml/simulation/simulator.py
 fedml/simulation/mpi/__init__.py
 fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py
 fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py
 fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py
 fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py
```

### Comparing `fedml-0.8.3a9/fedml.egg-info/requires.txt` & `fedml-0.8.4a1/fedml.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-numpy<=1.23,>=1.21
+numpy>=1.21
 PyYAML
 h5py
 tqdm
 wget
 paho-mqtt
 boto3
 pynvml
 scikit-learn
 networkx
 click
-torch==1.13.1
-torchvision==0.14.1
+torch>=1.13.1
+torchvision>=0.14.1
 spacy
 gensim
 multiprocess
 smart-open==6.3.0
 nvidia-ml-py3
 matplotlib
 dill
```

