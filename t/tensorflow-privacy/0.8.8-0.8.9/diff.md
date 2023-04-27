# Comparing `tmp/tensorflow_privacy-0.8.8.tar.gz` & `tmp/tensorflow_privacy-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow_privacy-0.8.8.tar", last modified: Fri Mar 10 19:02:10 2023, max compression
+gzip compressed data, was "tensorflow_privacy-0.8.9.tar", last modified: Thu Apr 27 17:00:05 2023, max compression
```

## Comparing `tensorflow_privacy-0.8.8.tar` & `tensorflow_privacy-0.8.9.tar`

### file list

```diff
@@ -1,174 +1,176 @@
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.515553 tensorflow_privacy-0.8.8/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12551 2021-06-07 08:11:32.000000 tensorflow_privacy-0.8.8/LICENSE
--rw-r-----   0 galenandrew (404454) primarygroup (89939)      153 2023-03-10 19:02:10.515553 tensorflow_privacy-0.8.8/PKG-INFO
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5369 2023-02-28 15:45:04.000000 tensorflow_privacy-0.8.8/README.md
--rw-r-----   0 galenandrew (404454) primarygroup (89939)       38 2023-03-10 19:02:10.515553 tensorflow_privacy-0.8.8/setup.cfg
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1579 2022-12-20 19:48:44.000000 tensorflow_privacy-0.8.8/setup.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.495553 tensorflow_privacy-0.8.8/tensorflow_privacy/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5599 2023-03-03 23:12:17.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/__init__.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.495553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2019-10-14 22:29:21.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/__init__.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.499553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2119 2022-01-27 18:36:54.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11158 2023-03-09 21:55:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy_lib.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5825 2023-03-08 20:44:03.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2176 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_noise_from_budget.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2259 2022-08-10 22:19:16.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_lib.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1607 2022-01-31 20:16:32.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2492 2022-01-27 18:32:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/gdp_accountant.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4790 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tensor_buffer.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2737 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tensor_buffer_eager_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2573 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tensor_buffer_graph_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    15945 2022-02-04 15:31:35.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     7801 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.499553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1555 2022-01-28 20:09:38.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9961 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/losses.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    14409 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/losses_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11402 2022-01-28 21:43:44.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/models.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    16102 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/models_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    14094 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/optimizers.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    18768 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/optimizers_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.503553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3531 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6000 2021-08-08 10:43:01.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5552 2021-07-28 00:17:53.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8316 2021-07-28 00:17:53.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4599 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6913 2022-02-02 17:17:00.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6694 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_skellam_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6117 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_skellam_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12074 2022-10-17 16:11:02.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/dp_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1145 2022-10-11 23:01:19.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/dp_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3662 2022-12-20 19:48:44.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/gaussian_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3990 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/gaussian_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5671 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/nested_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6788 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/nested_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3395 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/no_privacy_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2288 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/no_privacy_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3674 2022-02-02 17:17:00.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/normalized_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1370 2022-08-19 22:07:53.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/normalized_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6680 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11268 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8802 2023-03-03 23:12:17.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    19161 2023-03-03 23:12:17.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11008 2022-02-02 17:17:00.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_estimator_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12518 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_estimator_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     7040 2022-10-12 22:46:33.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/restart_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     7710 2022-10-12 22:46:33.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/restart_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1864 2022-01-27 18:36:54.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/test_utils.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    21374 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    22221 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    20223 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation_query_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    18269 2021-08-31 23:05:57.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11449 2022-10-12 19:10:34.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_range_query.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8091 2022-10-12 19:10:34.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_range_query_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.503553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6128 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/binary_class_head.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2896 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/binary_class_head_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2208 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/dnn.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2388 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/dnn_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2567 2022-01-27 18:36:54.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/head_utils.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6001 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_class_head.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3069 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_class_head_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6316 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_label_head.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3157 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_label_head_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3541 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/test_utils.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.503553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2475 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/dnn.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2453 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/dnn_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    20099 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/head.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3357 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/head_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.507553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2023-02-25 05:31:39.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10209 2023-03-07 18:34:20.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    17697 2023-03-07 18:34:20.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8734 2023-03-07 18:34:20.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/gradient_clipping_utils.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    13708 2023-03-07 18:34:20.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/layer_registry.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.507553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/keras_models/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/keras_models/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10725 2023-03-03 20:03:15.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/keras_models/dp_keras_model.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10438 2023-03-03 20:03:15.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/keras_models/dp_keras_model_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.507553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      589 2022-07-27 19:04:31.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5255 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/datasets.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3539 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/datasets_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10002 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3772 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2578 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1538 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.507553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      927 2021-06-07 08:11:32.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      783 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/data_structures.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      783 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/dataset_slicing.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      784 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/keras_evaluation.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      795 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/membership_inference_attack.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      774 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/models.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      776 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/plotting.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      776 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/privacy_report.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      779 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/seq2seq_mia.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      791 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/tf_estimator_evaluation.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.511553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9945 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9739 2022-10-18 23:20:56.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    15920 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4769 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_eager_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    26534 2022-10-17 16:11:02.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    16384 2022-10-21 20:15:21.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    19626 2022-10-21 20:15:21.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    44275 2022-10-17 16:11:02.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10360 2022-09-13 22:19:44.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_vectorized.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    15553 2022-12-22 18:32:11.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8689 2022-07-14 19:14:23.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8962 2022-08-19 00:37:31.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.511553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    14660 2022-10-26 18:15:08.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11300 2022-10-26 18:15:08.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.515553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      589 2021-06-07 08:11:32.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11535 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9837 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_example.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11625 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    46606 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    35235 2023-02-16 07:36:52.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10852 2022-11-08 19:04:53.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    17717 2022-11-08 19:04:53.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6541 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4319 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_example.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3081 2023-02-13 18:52:50.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    21105 2023-02-16 19:23:38.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    17337 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11497 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5743 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2916 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/plotting.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5896 2022-01-28 19:50:07.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9974 2022-07-16 23:30:17.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11489 2022-02-07 17:45:36.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10185 2022-02-07 17:45:36.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10959 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6620 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_example.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6871 2023-02-13 18:52:50.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2990 2023-03-10 17:32:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/utils_tensorboard.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.515553 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4184 2022-08-15 22:06:18.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2844 2022-01-31 21:26:57.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5979 2022-02-21 21:53:43.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3779 2022-02-21 21:53:43.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets_test.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11149 2022-10-26 18:32:41.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/utils.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    13321 2022-10-26 18:32:41.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/utils_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.515553 tensorflow_privacy-0.8.8/tensorflow_privacy/v1/
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2367 2022-01-27 18:36:54.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/v1/__init__.py
--rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      654 2023-03-09 23:21:22.000000 tensorflow_privacy-0.8.8/tensorflow_privacy/version.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-03-10 19:02:10.495553 tensorflow_privacy-0.8.8/tensorflow_privacy.egg-info/
--rw-r-----   0 galenandrew (404454) primarygroup (89939)      153 2023-03-10 19:02:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy.egg-info/PKG-INFO
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     9917 2023-03-10 19:02:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy.egg-info/SOURCES.txt
--rw-r-----   0 galenandrew (404454) primarygroup (89939)        1 2023-03-10 19:02:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy.egg-info/dependency_links.txt
--rw-r-----   0 galenandrew (404454) primarygroup (89939)      312 2023-03-10 19:02:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy.egg-info/requires.txt
--rw-r-----   0 galenandrew (404454) primarygroup (89939)       19 2023-03-10 19:02:10.000000 tensorflow_privacy-0.8.8/tensorflow_privacy.egg-info/top_level.txt
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.916161 tensorflow_privacy-0.8.9/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12551 2021-06-07 08:11:32.000000 tensorflow_privacy-0.8.9/LICENSE
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)      153 2023-04-27 17:00:05.916161 tensorflow_privacy-0.8.9/PKG-INFO
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5369 2023-02-28 15:45:04.000000 tensorflow_privacy-0.8.9/README.md
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)       38 2023-04-27 17:00:05.916161 tensorflow_privacy-0.8.9/setup.cfg
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1581 2023-04-26 21:34:56.000000 tensorflow_privacy-0.8.9/setup.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.896161 tensorflow_privacy-0.8.9/tensorflow_privacy/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5709 2023-03-28 19:42:31.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/__init__.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.896161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2019-10-14 22:29:21.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/__init__.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.896161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2786 2023-04-07 22:07:10.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    17380 2023-04-25 05:16:51.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy_lib.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10241 2023-04-25 05:16:51.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2176 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_noise_from_budget.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2259 2022-08-10 22:19:16.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_lib.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1607 2022-01-31 20:16:32.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2492 2022-01-27 18:32:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/gdp_accountant.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4790 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tensor_buffer.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2737 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tensor_buffer_eager_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2573 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tensor_buffer_graph_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    15945 2022-02-04 15:31:35.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     7801 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.896161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1555 2022-01-28 20:09:38.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9961 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/losses.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    14409 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/losses_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11402 2022-01-28 21:43:44.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/models.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    16102 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/models_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    14094 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/optimizers.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    18768 2022-01-28 20:30:35.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/optimizers_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.904161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3531 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6000 2021-08-08 10:43:01.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5552 2021-07-28 00:17:53.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8316 2021-07-28 00:17:53.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4599 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6913 2022-02-02 17:17:00.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6694 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_skellam_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6117 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_skellam_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12074 2022-10-17 16:11:02.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/dp_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1145 2022-10-11 23:01:19.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/dp_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3662 2022-12-20 19:48:44.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/gaussian_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3990 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/gaussian_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5671 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/nested_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6788 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/nested_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3395 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/no_privacy_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2288 2022-08-19 19:40:10.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/no_privacy_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3674 2022-02-02 17:17:00.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/normalized_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1370 2022-08-19 22:07:53.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/normalized_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6680 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11268 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8802 2023-03-03 23:12:17.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    19161 2023-03-03 23:12:17.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11008 2022-02-02 17:17:00.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_estimator_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12518 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_estimator_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     7040 2022-10-12 22:46:33.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/restart_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     7710 2022-10-12 22:46:33.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/restart_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1864 2022-01-27 18:36:54.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/test_utils.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    21291 2023-04-19 20:17:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    22587 2023-04-19 20:17:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    20223 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation_query_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    18269 2021-08-31 23:05:57.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11421 2023-04-19 20:17:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_range_query.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8091 2022-10-12 19:10:34.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_range_query_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.904161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6128 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/binary_class_head.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2896 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/binary_class_head_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2208 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/dnn.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2388 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/dnn_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2567 2022-01-27 18:36:54.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/head_utils.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6001 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_class_head.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3069 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_class_head_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6316 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_label_head.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3157 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_label_head_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3541 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/test_utils.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.904161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2475 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/dnn.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2453 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/dnn_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    20099 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/head.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3357 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/head_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.904161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2023-02-25 05:31:39.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12309 2023-03-24 21:57:14.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    19524 2023-03-24 21:57:14.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9642 2023-03-31 14:40:37.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/gradient_clipping_utils.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6029 2023-03-31 14:40:37.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/gradient_clipping_utils_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    13708 2023-03-07 18:34:20.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/layer_registry.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.904161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/keras_models/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/keras_models/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    12570 2023-04-06 18:54:16.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/keras_models/dp_keras_model.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    13201 2023-03-16 14:14:36.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/keras_models/dp_keras_model_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.908161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      589 2022-07-27 19:04:31.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5255 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/datasets.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3539 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/datasets_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10002 2022-07-01 17:33:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3772 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2578 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     1538 2022-06-30 18:00:33.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.908161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      927 2021-06-07 08:11:32.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      783 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/data_structures.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      783 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/dataset_slicing.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      784 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/keras_evaluation.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      795 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/membership_inference_attack.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      774 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/models.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      776 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/plotting.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      776 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/privacy_report.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      779 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/seq2seq_mia.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      791 2022-01-26 19:45:47.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/tf_estimator_evaluation.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.912161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9945 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9739 2022-10-18 23:20:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    15920 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4769 2022-02-08 00:05:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_eager_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    26534 2022-10-17 16:11:02.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    18193 2023-03-16 19:35:19.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5438 2023-03-16 19:35:19.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse_distributed_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    20171 2023-03-16 19:35:19.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    44275 2022-10-17 16:11:02.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10360 2022-09-13 22:19:44.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_vectorized.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    15553 2022-12-22 18:32:11.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8689 2022-07-14 19:14:23.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     8962 2022-08-19 00:37:31.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.912161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    14660 2022-10-26 18:15:08.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11300 2022-10-26 18:15:08.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.916161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      589 2021-06-07 08:11:32.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11535 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9837 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_example.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11625 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    47028 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    35235 2023-02-16 07:36:52.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11177 2023-04-13 00:13:44.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    18036 2023-04-13 00:13:44.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6541 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4319 2022-01-28 19:56:55.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_example.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3081 2023-02-13 18:52:50.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    21665 2023-03-28 00:59:45.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    18218 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11529 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5743 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2916 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/plotting.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5896 2022-01-28 19:50:07.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     9974 2022-07-16 23:30:17.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11489 2022-02-07 17:45:36.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10185 2022-02-07 17:45:36.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    10959 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6620 2022-10-03 17:32:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_example.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     6871 2023-02-13 18:52:50.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2990 2023-04-27 16:59:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/utils_tensorboard.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.916161 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      597 2022-01-27 20:39:46.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     4184 2022-08-15 22:06:18.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2844 2022-01-31 21:26:57.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     5979 2022-02-21 21:53:43.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     3779 2022-02-21 21:53:43.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets_test.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    11149 2022-10-26 18:32:41.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/utils.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)    13321 2022-10-26 18:32:41.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/utils_test.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.916161 tensorflow_privacy-0.8.9/tensorflow_privacy/v1/
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)     2367 2022-01-27 18:36:54.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/v1/__init__.py
+-rw-rw-r--   0 galenandrew (404454) primarygroup (89939)      654 2023-04-26 21:34:56.000000 tensorflow_privacy-0.8.9/tensorflow_privacy/version.py
+drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-27 17:00:05.896161 tensorflow_privacy-0.8.9/tensorflow_privacy.egg-info/
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)      153 2023-04-27 17:00:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy.egg-info/PKG-INFO
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)    10083 2023-04-27 17:00:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy.egg-info/SOURCES.txt
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)        1 2023-04-27 17:00:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy.egg-info/dependency_links.txt
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)      312 2023-04-27 17:00:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy.egg-info/requires.txt
+-rw-r-----   0 galenandrew (404454) primarygroup (89939)       19 2023-04-27 17:00:05.000000 tensorflow_privacy-0.8.9/tensorflow_privacy.egg-info/top_level.txt
```

### Comparing `tensorflow_privacy-0.8.8/LICENSE` & `tensorflow_privacy-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/README.md` & `tensorflow_privacy-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/setup.py` & `tensorflow_privacy-0.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,25 @@
     name='tensorflow_privacy',
     version=VERSION,
     url='https://github.com/tensorflow/privacy',
     license='Apache-2.0',
     install_requires=[
         'absl-py>=1.0,==1.*',
         'attrs~=21.4',
-        'dm-tree==0.1.7',
-        'dp-accounting==0.3.0',
+        'dm-tree==0.1.8',
+        'dp-accounting==0.4.1',
         'immutabledict~=2.2',
         'matplotlib~=3.3',
         'numpy~=1.21',
         'packaging~=22.0',
         'pandas~=1.4',
         'parameterized~=0.8',
         'scikit-learn>=1.0,==1.*',
         'scipy~=1.7',
         'statsmodels~=0.13',
         'tensorflow-datasets~=4.5',
         'tensorflow-estimator~=2.4',
         'tensorflow-probability==0.15.0',
         'tensorflow~=2.4',
     ],
-    packages=find_packages())
+    packages=find_packages(),
+)
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   pass
 else:
   # TensorFlow v1 imports
   from tensorflow_privacy import v1
 
   # Analysis
   from tensorflow_privacy.privacy.analysis.compute_dp_sgd_privacy_lib import compute_dp_sgd_privacy
+  from tensorflow_privacy.privacy.analysis.compute_dp_sgd_privacy_lib import compute_dp_sgd_privacy_statement
   from tensorflow_privacy.privacy.analysis.tree_aggregation_accountant import compute_rdp_tree_restart
   from tensorflow_privacy.privacy.analysis.tree_aggregation_accountant import compute_rdp_single_tree
   from tensorflow_privacy.privacy.analysis.tree_aggregation_accountant import compute_zcdp_single_tree
 
   # DPQuery classes
   from tensorflow_privacy.privacy.dp_query.dp_query import DPQuery
   from tensorflow_privacy.privacy.dp_query.dp_query import SumAggregationDPQuery
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy_lib.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_dp_sgd_privacy_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,270 +8,254 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Library for computing privacy values for DP-SGD."""
 
 import math
-from typing import Optional
 
-from absl import app
-from absl import logging
-import dp_accounting
-from scipy import optimize
-
-
-class UserLevelDPComputationError(Exception):
-  """Error raised if user-level epsilon computation fails."""
-
-
-def _compute_dp_sgd_user_privacy(
-    num_epochs: float,
-    noise_multiplier: float,
-    user_delta: float,
-    max_examples_per_user: int,
-    used_microbatching: bool = True,
-    poisson_subsampling_probability: Optional[float] = None,
-) -> float:
-  """Computes add-or-remove-one-user DP epsilon using group privacy.
-
-  This privacy guarantee uses add-or-remove-one-user adjacency, and protects
-  release of all model checkpoints in addition to the final model.
-
-  Uses Vadhan (2017) "The complexity of differential privacy" Lemma 2.2.
-
-  # TODO(b/271330804): Consider using RDP to compute group privacy.
-
-  We use a line search to identify an example-level delta which, when the lemma
-  is applied, yields the requested user-level delta, then use it to compute the
-  user-level epsilon.
-
-  Args:
-    num_epochs: The number of passes over the data. May be fractional.
-    noise_multiplier: The ratio of the noise to the l2 sensitivity.
-    user_delta: The target user-level delta.
-    max_examples_per_user: Upper bound on the number of examples per user.
-    used_microbatching: If true, increases sensitivity by a factor of two.
-    poisson_subsampling_probability: If not None, gives the probability that
-      each record is chosen in a batch. If None, assumes no subsampling.
-
-  Returns:
-    The add-or-remove-one-user DP epsilon value using group privacy.
-
-  Raises:
-    UserLevelDPComputationError: If line search for example-level delta fails.
-  """
-  if num_epochs <= 0:
-    raise ValueError(f'num_epochs must be positive. Found {num_epochs}.')
-  if noise_multiplier < 0:
-    raise ValueError(
-        f'noise_multiplier must be non-negative. Found {noise_multiplier}.'
-    )
-  if not 0 <= user_delta <= 1:
-    raise ValueError(f'user_delta must be between 0 and 1. Found {user_delta}.')
-  if max_examples_per_user <= 0:
-    raise ValueError(
-        'max_examples_per_user must be a positive integer. Found '
-        f'{max_examples_per_user}.'
-    )
+from absl.testing import absltest
+from absl.testing import parameterized
 
-  if max_examples_per_user == 1:
-    # Don't unnecessarily inflate epsilon if one example per user.
-    return _compute_dp_sgd_example_privacy(
-        num_epochs,
-        noise_multiplier,
-        user_delta,
-        used_microbatching,
-        poisson_subsampling_probability,
-    )
+from tensorflow_privacy.privacy.analysis import compute_dp_sgd_privacy_lib
+
+
+_example_privacy = compute_dp_sgd_privacy_lib._compute_dp_sgd_example_privacy
+_user_privacy = compute_dp_sgd_privacy_lib._compute_dp_sgd_user_privacy
+
+
+DP_SGD_STATEMENT_KWARGS = dict(
+    number_of_examples=10000,
+    batch_size=64,
+    num_epochs=5.0,
+    noise_multiplier=2.0,
+    delta=1e-6,
+)
 
-  # The computation below to estimate user_eps works as follows.
-  # We have _compute_dp_sgd_example_privacy which maps
-  #   F(example_delta) -> example_eps
-  # Vadhan (2017) "The complexity of differential privacy" Lemma 2.2 gives us
-  #   G(example_eps, example_delta) -> user_delta
-  #   H(example_eps) -> user_eps.
-  # We first identify an example_delta such that
-  #   G(F(example_delta), example_delta) = user_delta
-  # Specifically, we use a line search in log space to solve for
-  #   log(G(F(example_delta), example_delta)) - log(user_delta) = 0
-  # Then we can return user_eps = H(F(example_delta)).
 
-  log_k = math.log(max_examples_per_user)
-  target_user_log_delta = math.log(user_delta)
+class ComputeDpSgdPrivacyTest(parameterized.TestCase):
 
-  def user_log_delta_gap(example_log_delta):
-    example_eps = _compute_dp_sgd_example_privacy(
+  @parameterized.named_parameters(
+      ('Test0', 60000, 150, 1.3, 15, 1e-5, 0.7242234026109595, 19.0),
+      ('Test1', 100000, 100, 1.0, 30, 1e-7, 1.4154988495444845, 13.0),
+      ('Test2', 100000000, 1024, 0.1, 10, 1e-7, 5907982.31138195, 1.25),
+  )
+  def test_compute_dp_sgd_privacy(self, n, batch_size, noise_multiplier, epochs,
+                                  delta, expected_eps, expected_order):
+    eps, order = compute_dp_sgd_privacy_lib.compute_dp_sgd_privacy(
+        n, batch_size, noise_multiplier, epochs, delta)
+    self.assertAlmostEqual(eps, expected_eps)
+    self.assertEqual(order, expected_order)
+
+    # We perform an additional sanity check on the hard-coded test values.
+    # We do a back-of-the-envelope calculation to obtain a lower bound.
+    # Specifically, we make the approximation that subsampling a q-fraction is
+    # equivalent to multiplying noise scale by 1/q.
+    # This is only an approximation, but can be justified by the central limit
+    # theorem in the Gaussian Differential Privacy framework; see
+    # https://arxiv.org/1911.11607
+    # The approximation error is one-sided and provides a lower bound, which is
+    # the basis of this sanity check. This is confirmed in the above paper.
+    q = batch_size / n
+    steps = epochs * n / batch_size
+    sigma = noise_multiplier * math.sqrt(steps) / q
+    # We compute the optimal guarantee for Gaussian
+    # using https://arxiv.org/abs/1805.06530 Theorem 8 (in v2).
+    low_delta = .5 * math.erfc((eps * sigma - .5 / sigma) / math.sqrt(2))
+    if eps < 100:  # Skip this if it causes overflow; error is minor.
+      low_delta -= math.exp(eps) * .5 * math.erfc(
+          (eps * sigma + .5 / sigma) / math.sqrt(2))
+    self.assertLessEqual(low_delta, delta)
+
+  @parameterized.named_parameters(
+      ('num_epochs_negative', dict(num_epochs=-1.0)),
+      ('noise_multiplier_negative', dict(noise_multiplier=-1.0)),
+      ('example_delta_negative', dict(example_delta=-0.5)),
+      ('example_delta_excessive', dict(example_delta=1.5)),
+  )
+  def test_compute_dp_sgd_example_privacy_bad_args(self, override_args):
+    args = dict(num_epochs=1.0, noise_multiplier=1.0, example_delta=1.0)
+    args.update(override_args)
+    with self.assertRaises(ValueError):
+      _example_privacy(**args)
+
+  @parameterized.named_parameters(
+      ('no_microbatching_no_subsampling', False, None, 10.8602036),
+      ('microbatching_no_subsampling', True, None, 26.2880374),
+      ('no_microbatching_with_subsampling', False, 1e-2, 3.2391922),
+      ('microbatching_with_subsampling', True, 1e-2, 22.5970358),
+  )
+  def test_compute_dp_sgd_example_privacy(
+      self, used_microbatching, poisson_subsampling_probability, expected_eps
+  ):
+    num_epochs = 1.2
+    noise_multiplier = 0.7
+    example_delta = 1e-5
+    eps = _example_privacy(
         num_epochs,
         noise_multiplier,
-        math.exp(example_log_delta),
+        example_delta,
         used_microbatching,
         poisson_subsampling_probability,
     )
+    self.assertAlmostEqual(eps, expected_eps)
 
-    # Estimate user_eps, user_log_delta using Vadhan Lemma 2.2.
-    user_eps = max_examples_per_user * example_eps
-    user_log_delta = log_k + user_eps + example_log_delta
-    return user_log_delta - target_user_log_delta
-
-  # We need bounds on the example-level delta. The supplied user-level delta
-  # is an upper bound. Search exponentially toward zero for lower bound.
-  example_log_delta_max = target_user_log_delta
-  example_log_delta_min = example_log_delta_max - math.log(10)
-  user_log_delta_gap_min = user_log_delta_gap(example_log_delta_min)
-  while user_log_delta_gap_min > 0:
-    # Assuming that _compute_dp_sgd_example_privacy is decreasing in
-    # example_delta, it is not difficult to show that if user_delta_min
-    # corresponding to example_delta_min is too large, then we must reduce
-    # example_delta by at least a factor of (user_delta / user_delta_min).
-    # In other words, if example_log_delta_min is an upper bound, then so is
-    # example_log_delta_min - user_log_delta_gap_min.
-    example_log_delta_max = example_log_delta_min - user_log_delta_gap_min
-    example_log_delta_min = example_log_delta_max - math.log(10)
-    user_log_delta_gap_min = user_log_delta_gap(example_log_delta_min)
-    if not math.isfinite(user_log_delta_gap_min):
-      # User-level (epsilon, delta) DP is not achievable. This can happen
-      # because as example_delta decreases, example_eps increases. So it is
-      # possible for user_delta (which increases in both example_delta and
-      # example_eps) to diverge to infinity as example_delta goes to zero.
-      logging.warn(
-          (
-              'No upper bound on user-level DP epsilon can be computed with %s '
-              'examples per user.'
-          ),
-          max_examples_per_user,
-      )
-      return math.inf
-
-  # By the same logic, we can improve on the lower bound we just found, before
-  # even starting the line search. We actually could do a custom line search
-  # that makes use of this at each step, but brentq should be fast enough.
-  example_log_delta_min -= user_log_delta_gap_min
-
-  example_log_delta, result = optimize.brentq(
-      user_log_delta_gap,
-      example_log_delta_min,
-      example_log_delta_max,
-      full_output=True,
+  @parameterized.named_parameters(
+      ('num_epochs_negative', dict(num_epochs=-1.0)),
+      ('noise_multiplier_negative', dict(noise_multiplier=-1.0)),
+      ('example_delta_negative', dict(user_delta=-0.5)),
+      ('example_delta_excessive', dict(user_delta=1.5)),
+      ('max_examples_per_user_negative', dict(max_examples_per_user=-1)),
   )
+  def test_compute_dp_sgd_user_privacy_bad_args(self, override_args):
+    args = dict(
+        num_epochs=1.0,
+        noise_multiplier=1.0,
+        user_delta=1.0,
+        max_examples_per_user=3,
+    )
+    args.update(override_args)
+    with self.assertRaises(ValueError):
+      _user_privacy(**args)
+
+  def test_user_privacy_one_example_per_user(self):
+    num_epochs = 1.2
+    noise_multiplier = 0.7
+    delta = 1e-5
 
-  if not result.converged:
-    raise UserLevelDPComputationError(
-        'Optimization failed trying to compute user-level DP epsilon.'
+    example_eps = _example_privacy(num_epochs, noise_multiplier, delta)
+    user_eps = _user_privacy(
+        num_epochs,
+        noise_multiplier,
+        delta,
+        max_examples_per_user=1,
     )
+    self.assertEqual(user_eps, example_eps)
 
-  # Vadhan (2017) "The complexity of differential privacy" Lemma 2.2.
-  # user_delta = k * exp(k * example_eps) * example_delta
-  # Given example_delta, we can solve for (k * example_eps) = user_eps.
-  return max(0, target_user_log_delta - log_k - example_log_delta)
-
-
-def _compute_dp_sgd_example_privacy(
-    num_epochs: float,
-    noise_multiplier: float,
-    example_delta: float,
-    used_microbatching: bool = True,
-    poisson_subsampling_probability: Optional[float] = None,
-) -> float:
-  """Computes add-or-remove-one-example DP epsilon.
-
-  This privacy guarantee uses add-or-remove-one-example adjacency, and protects
-  release of all model checkpoints in addition to the final model.
-
-  Args:
-    num_epochs: The number of passes over the data.
-    noise_multiplier: The ratio of the noise to the l2 sensitivity.
-    example_delta: The target delta.
-    used_microbatching: If true, increases sensitivity by a factor of two.
-    poisson_subsampling_probability: If not None, gives the probability that
-      each record is chosen in a batch. If None, assumes no subsampling.
-
-  Returns:
-    The epsilon value.
-  """
-  if num_epochs <= 0:
-    raise ValueError(f'num_epochs must be positive. Found {num_epochs}.')
-  if noise_multiplier < 0:
-    raise ValueError(
-        f'noise_multiplier must be non-negative. Found {noise_multiplier}.'
+  @parameterized.parameters((0.9, 2), (1.1, 3), (2.3, 13))
+  def test_user_privacy_epsilon_delta_consistency(
+      self, noise_multiplier, max_examples_per_user
+  ):
+    """Tests example/user epsilons consistent with Vadhan (2017) Lemma 2.2."""
+    num_epochs = 5
+    example_delta = 1e-8
+    q = 2e-4
+    example_eps = _example_privacy(
+        num_epochs,
+        noise_multiplier=noise_multiplier,
+        example_delta=example_delta,
+        poisson_subsampling_probability=q,
     )
-  if not 0 <= example_delta <= 1:
-    raise ValueError(f'delta must be between 0 and 1. Found {example_delta}.')
 
-  if used_microbatching:
-    # TODO(b/271462792)
-    noise_multiplier /= 2
-
-  event_ = dp_accounting.GaussianDpEvent(noise_multiplier)
-  if poisson_subsampling_probability is not None:
-    event_ = dp_accounting.PoissonSampledDpEvent(
-        sampling_probability=poisson_subsampling_probability, event=event_
+    user_delta = math.exp(
+        math.log(example_delta)
+        + compute_dp_sgd_privacy_lib._logexpm1(
+            max_examples_per_user * example_eps
+        )
+        - compute_dp_sgd_privacy_lib._logexpm1(example_eps)
     )
-    count = int(math.ceil(num_epochs / poisson_subsampling_probability))
-  else:
-    count = int(math.ceil(num_epochs))
-  event_ = dp_accounting.SelfComposedDpEvent(count=count, event=event_)
-
-  rdp_orders = (
-      [1 + x / 10.0 for x in range(1, 100)]
-      + list(range(11, 64))
-      + [128, 256, 512, 1024]
-  )
-  accountant = dp_accounting.rdp.RdpAccountant(rdp_orders)  # TODO(b/271341062)
-  accountant.compose(event_)
-  return accountant.get_epsilon(example_delta)
-
-
-def compute_dp_sgd_privacy(n, batch_size, noise_multiplier, epochs, delta):
-  """Compute epsilon based on the given hyperparameters.
-
-  This function is deprecated. It does not account for doubling of sensitivity
-  with microbatching, and assumes Poisson subsampling, which is rarely used in
-  practice. (See "How to DP-fy ML: A Practical Guide to Machine Learning with
-  Differential Privacy", https://arxiv.org/abs/2303.00654, Sec 5.6.) Most users
-  should call `compute_dp_sgd_privacy_statement` (which will be added shortly),
-  which provides appropriate context for the guarantee (see the reporting
-  recommendations in "How to DP-fy ML", Sec 5.3). If you need a numeric epsilon
-  value under specific assumptions, it is recommended to use the `dp_accounting`
-  libraries directly to compute epsilon, with the precise and correct
-  assumptions of your application.
-
-  Args:
-    n: Number of examples in the training data.
-    batch_size: Batch size used in training.
-    noise_multiplier: Noise multiplier used in training.
-    epochs: Number of epochs in training.
-    delta: Value of delta for which to compute epsilon.
-
-  Returns:
-    A 2-tuple containing the value of epsilon and the optimal RDP order.
-  """
-  # TODO(b/265168958): Update this text for `compute_dp_sgd_privacy_statement`.
-  logging.warn(
-      '`compute_dp_sgd_privacy` is deprecated. It does not account '
-      'for doubling of sensitivity with microbatching, and assumes Poisson '
-      'subsampling, which is rarely used in practice. Please use the '
-      '`dp_accounting` libraries directly to compute epsilon, using the '
-      'precise and correct assumptions of your application.'
-  )
+    user_eps = _user_privacy(
+        num_epochs,
+        noise_multiplier=noise_multiplier,
+        user_delta=user_delta,
+        max_examples_per_user=max_examples_per_user,
+        poisson_subsampling_probability=q,
+    )
+    self.assertAlmostEqual(user_eps, example_eps * max_examples_per_user)
+
+  def test_dp_sgd_privacy_statement_no_user_dp(self):
+    statement = compute_dp_sgd_privacy_lib.compute_dp_sgd_privacy_statement(
+        **DP_SGD_STATEMENT_KWARGS,
+    )
+    expected_statement = """\
+DP-SGD performed over 10000 examples with 64 examples per iteration, noise
+multiplier 2.0 for 5.0 epochs with microbatching, and no bound on number of
+examples per user.
+
+This privacy guarantee protects the release of all model checkpoints in addition
+to the final model.
+
+Example-level DP with add-or-remove-one adjacency at delta = 1e-06 computed with
+RDP accounting:
+    Epsilon with each example occurring once per epoch:        13.376
+    Epsilon assuming Poisson sampling (*):                      1.616
+
+No user-level privacy guarantee is possible without a bound on the number of
+examples per user.
+
+(*) Poisson sampling is not usually done in training pipelines, but assuming
+that the data was randomly shuffled, it is believed the actual epsilon should be
+closer to this value than the conservative assumption of an arbitrary data
+order.
+"""
+    self.assertEqual(statement, expected_statement)
+
+  def test_dp_sgd_privacy_statement_user_dp(self):
+    statement = compute_dp_sgd_privacy_lib.compute_dp_sgd_privacy_statement(
+        **DP_SGD_STATEMENT_KWARGS,
+        max_examples_per_user=3,
+    )
+    expected_statement = """\
+DP-SGD performed over 10000 examples with 64 examples per iteration, noise
+multiplier 2.0 for 5.0 epochs with microbatching, and at most 3 examples per
+user.
+
+This privacy guarantee protects the release of all model checkpoints in addition
+to the final model.
+
+Example-level DP with add-or-remove-one adjacency at delta = 1e-06 computed with
+RDP accounting:
+    Epsilon with each example occurring once per epoch:        13.376
+    Epsilon assuming Poisson sampling (*):                      1.616
+
+User-level DP with add-or-remove-one adjacency at delta = 1e-06 computed using
+RDP accounting and group privacy:
+    Epsilon with each example occurring once per epoch:        85.940
+    Epsilon assuming Poisson sampling (*):                      6.425
+
+(*) Poisson sampling is not usually done in training pipelines, but assuming
+that the data was randomly shuffled, it is believed the actual epsilon should be
+closer to this value than the conservative assumption of an arbitrary data
+order.
+"""
+    self.assertEqual(statement, expected_statement)
+
+  def test_dp_sgd_privacy_statement_user_dp_infinite(self):
+    statement = compute_dp_sgd_privacy_lib.compute_dp_sgd_privacy_statement(
+        **DP_SGD_STATEMENT_KWARGS,
+        max_examples_per_user=10,
+    )
+    expected_statement = """\
+DP-SGD performed over 10000 examples with 64 examples per iteration, noise
+multiplier 2.0 for 5.0 epochs with microbatching, and at most 10 examples per
+user.
+
+This privacy guarantee protects the release of all model checkpoints in addition
+to the final model.
+
+Example-level DP with add-or-remove-one adjacency at delta = 1e-06 computed with
+RDP accounting:
+    Epsilon with each example occurring once per epoch:        13.376
+    Epsilon assuming Poisson sampling (*):                      1.616
+
+User-level DP with add-or-remove-one adjacency at delta = 1e-06 computed using
+RDP accounting and group privacy:
+    Epsilon with each example occurring once per epoch:      inf (**)
+    Epsilon assuming Poisson sampling (*):                   inf (**)
+
+(*) Poisson sampling is not usually done in training pipelines, but assuming
+that the data was randomly shuffled, it is believed the actual epsilon should be
+closer to this value than the conservative assumption of an arbitrary data
+order.
+
+(**) A finite example-level epsilon implies a finite user-level epsilon at any
+`max_examples_per_user`, but because conversion from example-level to user-level
+DP is not exact, it is possible for the upper bound on the user-level epsilon to
+still be infinite.
+"""
+    self.assertEqual(statement, expected_statement)
 
-  q = batch_size / n  # q - the sampling ratio.
-  if q > 1:
-    raise app.UsageError('n must be larger than the batch size.')
-  orders = ([1.25, 1.5, 1.75, 2., 2.25, 2.5, 3., 3.5, 4., 4.5] +
-            list(range(5, 64)) + [128, 256, 512])
-  steps = int(math.ceil(epochs * n / batch_size))
-  accountant = dp_accounting.rdp.RdpAccountant(orders)
-
-  event = dp_accounting.SelfComposedDpEvent(
-      dp_accounting.PoissonSampledDpEvent(
-          sampling_probability=q,
-          event=dp_accounting.GaussianDpEvent(noise_multiplier),
-      ),
-      steps,
-  )
 
-  accountant.compose(event)
-  return accountant.get_epsilon_and_optimal_order(delta)
+if __name__ == '__main__':
+  absltest.main()
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_noise_from_budget.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_noise_from_budget.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_lib.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/compute_noise_from_budget_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/gdp_accountant.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/gdp_accountant.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tensor_buffer.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tensor_buffer.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tensor_buffer_eager_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tensor_buffer_eager_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tensor_buffer_graph_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tensor_buffer_graph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/analysis/tree_aggregation_accountant_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/losses.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/losses.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/losses_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/losses_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/models.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/models.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/models_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/models_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/optimizers.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/optimizers.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/bolt_on/optimizers_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/bolt_on/optimizers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/discrete_gaussian_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_discrete_gaussian_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_skellam_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_skellam_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/distributed_skellam_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/distributed_skellam_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/dp_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/dp_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/dp_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/dp_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/gaussian_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/gaussian_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/gaussian_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/gaussian_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/nested_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/nested_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/nested_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/nested_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/no_privacy_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/no_privacy_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/no_privacy_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/no_privacy_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/normalized_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/normalized_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/normalized_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/normalized_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_sum_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_adaptive_clip_tree_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_estimator_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_estimator_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/quantile_estimator_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/quantile_estimator_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/restart_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/restart_query.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/restart_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/restart_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/test_utils.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 based on tree aggregation. When using an appropriate noise function (e.g.,
 Gaussian noise), it allows for efficient differentially private algorithms under
 continual observation, without prior subsampling or shuffling assumptions. This
 module implements the core logic of tree aggregation in Tensorflow, which serves
 as helper functions for `tree_aggregation_query`. This module and helper
 functions are publicly accessible.
 """
+
 import abc
 import collections
-from typing import Any, Callable, Collection, Optional, Tuple, Union
+from typing import Any, Callable, Collection, NamedTuple, Optional, Tuple, Union
 
-import attr
 import tensorflow as tf
 
 # TODO(b/192464750): find a proper place for the helper functions, privatize
 # the tree aggregation logic, and encourage users to use the DPQuery API.
 
 
 class ValueGenerator(metaclass=abc.ABCMeta):
@@ -166,30 +166,29 @@
     Returns:
       A pair (value, new_state) where value is the next value and new_state
         is the advanced state.
     """
     return self.value_fn(), state
 
 
-@attr.s(eq=False, frozen=True, slots=True)
-class TreeState(object):
+class TreeState(NamedTuple):
   """Class defining state of the tree.
 
   Attributes:
     level_buffer: A `tf.Tensor` saves the last node value of the left child
       entered for the tree levels recorded in `level_buffer_idx`.
     level_buffer_idx: A `tf.Tensor` for the tree level index of the
       `level_buffer`.  The tree level index starts from 0, i.e.,
       `level_buffer[0]` when `level_buffer_idx[0]==0` recorded the noise value
       for the most recent leaf node.
    value_generator_state: State of a stateful `ValueGenerator` for tree node.
   """
-  level_buffer = attr.ib(type=tf.Tensor)
-  level_buffer_idx = attr.ib(type=tf.Tensor)
-  value_generator_state = attr.ib(type=Any)
+  level_buffer: tf.Tensor
+  level_buffer_idx: tf.Tensor
+  value_generator_state: Any
 
 
 # TODO(b/192464750): move `get_step_idx` to be a property of `TreeState`.
 @tf.function
 def get_step_idx(state: TreeState) -> tf.Tensor:
   """Returns the current leaf node index based on `TreeState.level_buffer_idx`."""
   step_idx = tf.constant(-1, dtype=tf.int32)
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,19 @@
 corresponding epsilon for a `target_delta` and `noise_multiplier` to achieve
 (epsilon,delta)-DP can be computed as:
   orders = [1 + x / 10. for x in range(1, 100)] + list(range(12, 64))
   rdp = compute_rdp_tree_restart(noise_multiplier, [steps], orders)
   eps = rdp_accountant.get_privacy_spent(orders, rdp, target_delta)[0]
 """
 
-import attr
+from typing import Any, NamedTuple
+
 import dp_accounting
 import tensorflow as tf
+
 from tensorflow_privacy.privacy.dp_query import dp_query
 from tensorflow_privacy.privacy.dp_query import tree_aggregation
 
 
 # TODO(b/193679963): define `RestartQuery` and move `RestartIndicator` to be
 # in the same module.
 
@@ -80,27 +82,26 @@
       defined `noise_generator`. `noise_generator` is a
       `tree_aggregation.ValueGenerator` to generate the noise value for a tree
       node. Noise stdandard deviation is specified outside the `dp_query` by the
       user when defining `noise_fn` and should have order
       O(clip_norm*log(T)/eps) to guarantee eps-DP.
   """
 
-  @attr.s(frozen=True)
-  class GlobalState(object):
+  class GlobalState(NamedTuple):
     """Class defining global state for Tree sum queries.
 
     Attributes:
       tree_state: Current state of noise tree keeping track of current leaf and
         each level state.
       clip_value: The clipping value to be passed to clip_fn.
       samples_cumulative_sum: Noiseless cumulative sum of samples over time.
     """
-    tree_state = attr.ib()
-    clip_value = attr.ib()
-    samples_cumulative_sum = attr.ib()
+    tree_state: Any
+    clip_value: Any
+    samples_cumulative_sum: Any
 
   def __init__(self,
                record_specs,
                noise_generator,
                clip_fn,
                clip_value,
                use_efficient=True):
@@ -178,18 +179,19 @@
     """
     new_cumulative_sum = tf.nest.map_structure(
         tf.add, global_state.samples_cumulative_sum, sample_state)
     cumulative_sum_noise, new_tree_state = self._tree_aggregator.get_cumsum_and_update(
         global_state.tree_state)
     noised_cumulative_sum = tf.nest.map_structure(tf.add, new_cumulative_sum,
                                                   cumulative_sum_noise)
-    new_global_state = attr.evolve(
-        global_state,
+    new_global_state = TreeCumulativeSumQuery.GlobalState(
+        tree_state=new_tree_state,
+        clip_value=global_state.clip_value,
         samples_cumulative_sum=new_cumulative_sum,
-        tree_state=new_tree_state)
+    )
     event = dp_accounting.UnsupportedDpEvent()
     return noised_cumulative_sum, new_global_state, event
 
   def reset_state(self, noised_results, global_state):
     """Returns state after resetting the tree.
 
     This function will be used in `restart_query.RestartQuery` after calling
@@ -202,18 +204,19 @@
         cumulative sum.
 
     Returns:
       New global state with current noised cumulative sum and restarted tree
         state for the next cumulative sum.
     """
     new_tree_state = self._tree_aggregator.reset_state(global_state.tree_state)
-    return attr.evolve(
-        global_state,
+    return TreeCumulativeSumQuery.GlobalState(
+        tree_state=new_tree_state,
+        clip_value=global_state.clip_value,
         samples_cumulative_sum=noised_results,
-        tree_state=new_tree_state)
+    )
 
   @classmethod
   def build_l2_gaussian_query(cls,
                               clip_norm,
                               noise_multiplier,
                               record_specs,
                               noise_seed=None,
@@ -308,28 +311,27 @@
       defined `noise_generator`. `noise_generator` is a
       `tree_aggregation.ValueGenerator` to generate the noise value for a tree
       node. Noise stdandard deviation is specified outside the `dp_query` by the
       user when defining `noise_fn` and should have order
       O(clip_norm*log(T)/eps) to guarantee eps-DP.
   """
 
-  @attr.s(frozen=True)
-  class GlobalState(object):
+  class GlobalState(NamedTuple):
     """Class defining global state for Tree sum queries.
 
     Attributes:
       tree_state: Current state of noise tree keeping track of current leaf and
         each level state.
       clip_value: The clipping value to be passed to clip_fn.
       previous_tree_noise: Cumulative noise by tree aggregation from the
         previous time the query is called on a sample.
     """
-    tree_state = attr.ib()
-    clip_value = attr.ib()
-    previous_tree_noise = attr.ib()
+    tree_state: Any
+    clip_value: Any
+    previous_tree_noise: Any
 
   def __init__(self,
                record_specs,
                noise_generator,
                clip_fn,
                clip_value,
                use_efficient=True):
@@ -422,16 +424,19 @@
       A tuple of (noised_cumulative_sum, new_global_state).
     """
     tree_noise, new_tree_state = self._tree_aggregator.get_cumsum_and_update(
         global_state.tree_state)
     noised_sample = tf.nest.map_structure(lambda a, b, c: a + b - c,
                                           sample_state, tree_noise,
                                           global_state.previous_tree_noise)
-    new_global_state = attr.evolve(
-        global_state, previous_tree_noise=tree_noise, tree_state=new_tree_state)
+    new_global_state = TreeResidualSumQuery.GlobalState(
+        tree_state=new_tree_state,
+        clip_value=global_state.clip_value,
+        previous_tree_noise=tree_noise,
+    )
     event = dp_accounting.UnsupportedDpEvent()
     return noised_sample, new_global_state, event
 
   def reset_state(self, noised_results, global_state):
     """Returns state after resetting the tree.
 
     This function will be used in `restart_query.RestartQuery` after calling
@@ -444,29 +449,36 @@
         node, and tree state for the next conceptual cumulative sum.
 
     Returns:
       New global state with zero noise and restarted tree state.
     """
     del noised_results
     new_tree_state = self._tree_aggregator.reset_state(global_state.tree_state)
-    return attr.evolve(
-        global_state,
+    return TreeResidualSumQuery.GlobalState(
+        tree_state=new_tree_state,
+        clip_value=global_state.clip_value,
         previous_tree_noise=self._zero_initial_noise(),
-        tree_state=new_tree_state)
+    )
 
   def reset_l2_clip_gaussian_noise(self, global_state, clip_norm, stddev):
     noise_generator_state = global_state.tree_state.value_generator_state
     assert isinstance(self._tree_aggregator.value_generator,
                       tree_aggregation.GaussianNoiseGenerator)
     noise_generator_state = self._tree_aggregator.value_generator.make_state(
         noise_generator_state.seeds, stddev)
-    new_tree_state = attr.evolve(
-        global_state.tree_state, value_generator_state=noise_generator_state)
-    return attr.evolve(
-        global_state, clip_value=clip_norm, tree_state=new_tree_state)
+    new_tree_state = tree_aggregation.TreeState(
+        level_buffer=global_state.tree_state.level_buffer,
+        level_buffer_idx=global_state.tree_state.level_buffer_idx,
+        value_generator_state=noise_generator_state,
+    )
+    return TreeResidualSumQuery.GlobalState(
+        tree_state=new_tree_state,
+        clip_value=clip_norm,
+        previous_tree_noise=global_state.previous_tree_noise,
+    )
 
   @classmethod
   def build_l2_gaussian_query(cls,
                               clip_norm,
                               noise_multiplier,
                               record_specs,
                               noise_seed=None,
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_aggregation_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_aggregation_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_range_query.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_range_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 """`DPQuery`s for offline differentially private tree aggregation protocols.
 
 'Offline' means all the leaf nodes are ready before the protocol starts.
 """
 
 import distutils
 import math
-from typing import Optional
+from typing import Any, NamedTuple, Optional
 
-import attr
 import dp_accounting
 import tensorflow as tf
 from tensorflow_privacy.privacy.dp_query import distributed_discrete_gaussian_query
 from tensorflow_privacy.privacy.dp_query import dp_query
 from tensorflow_privacy.privacy.dp_query import gaussian_query
 
 
@@ -98,25 +97,24 @@
   necessary for distributed private learning?. Adam Smith, Abhradeep Thakurta,
   Jalaj Upadhyay." Builds a tree on top of the input record and adds noise to
   the tree for differential privacy. Any range query can be decomposed into the
   sum of O(log(n)) nodes in the tree compared to O(n) when using a histogram.
   Improves efficiency and reduces noise scale.
   """
 
-  @attr.s(frozen=True)
-  class GlobalState(object):
+  class GlobalState(NamedTuple):
     """Class defining global state for TreeRangeSumQuery.
 
     Attributes:
       arity: The branching factor of the tree (i.e. the number of children each
         internal node has).
       inner_query_state: The global state of the inner query.
     """
-    arity = attr.ib()
-    inner_query_state = attr.ib()
+    arity: Any
+    inner_query_state: Any
 
   def __init__(self,
                inner_query: dp_query.SumAggregationDPQuery,
                arity: int = 2):
     """Initializes the `TreeRangeSumQuery`.
 
     Args:
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/dp_query/tree_range_query_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/dp_query/tree_range_query_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/binary_class_head.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/binary_class_head.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/binary_class_head_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/binary_class_head_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/dnn.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/dnn.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/dnn_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/dnn_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/head_utils.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/head_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_class_head.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_class_head.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_class_head_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_class_head_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_label_head.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_label_head.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/multi_label_head_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/multi_label_head_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/test_utils.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/dnn.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/dnn.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/dnn_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/dnn_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/head.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/head.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/estimators/v1/head_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/estimators/v1/head_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 clip weights so that the gradient of the loss function, weighted by these
 weights, is equivalent to the gradient of the original loss function but
 with the per-example gradients clipped by some clip weight. Uses a variant
 of the approach given in https://arxiv.org/pdf/2009.03106.pdf (see the
 `compute_gradient_norms()` function).
 """
 
-from typing import Dict, Iterable, Optional, Text, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Text, Tuple, Union
 
 import tensorflow as tf
 from tensorflow_privacy.privacy.fast_gradient_clipping import gradient_clipping_utils
 from tensorflow_privacy.privacy.fast_gradient_clipping import layer_registry as lr
 
 InputTensor = Union[tf.Tensor, Iterable[tf.Tensor], Dict[Text, tf.Tensor]]
 
@@ -50,28 +50,34 @@
               'be used for efficient gradient clipping.'
               % layer_instance.__class__.__name__
           )
         registry_fn = layer_registry.lookup(layer_instance)
         (layer_vars, layer_outputs, layer_sqr_norm_fn) = registry_fn(
             layer_instance, args, kwargs, tape, num_microbatches
         )
-        return layer_outputs, (layer_vars, layer_sqr_norm_fn)
+        return layer_outputs, (
+            layer_vars,
+            layer_sqr_norm_fn,
+            layer_instance.trainable_weights,
+        )
       else:
         # Non-trainable layer.
         return layer_instance(*args, **kwargs), None
 
   return registry_generator_fn
 
 
 def compute_gradient_norms(
     input_model: tf.keras.Model,
     x_batch: InputTensor,
     y_batch: tf.Tensor,
     layer_registry: lr.LayerRegistry,
+    per_example_loss_fn: Optional[Callable[[tf.Tensor, Any], tf.Tensor]] = None,
     num_microbatches: Optional[lr.BatchSize] = None,
+    trainable_vars: Optional[List[tf.Variable]] = None,
 ):
   """Computes the per-example loss gradient norms for given data.
 
   Applies a variant of the approach given in
     https://arxiv.org/pdf/2009.03106.pdf
 
   Args:
@@ -82,20 +88,27 @@
     y_batch: A `tf.Tensor` representing a batch of output labels. The first axis
       must be the batch dimension. The number of examples should match the
       number of examples in `x_batch`.
     layer_registry: A `LayerRegistry` instance containing functions that help
       compute gradient norms quickly. See
       `tensorflow_privacy.privacy.fast_gradient_clipping.layer_registry` for
       more details.
+    per_example_loss_fn: If not None, used as the function to compute the
+      vectorized per example loss. Otherwise, we derive it from `input_model`'s
+      loss function.
     num_microbatches: An optional number or scalar `tf.Tensor` for the number of
       microbatches. If not None, indicates that the loss is grouped into
       num_microbatches (in this case, the batch dimension needs to be a multiple
       of num_microbatches). When there is microbatches, we always assume the
       loss is the mean over a microbatch. And the gradient norm is computed for
       each microbatch.
+    trainable_vars: The list of variables included in computing the gradient
+      norm. When a layer has multiple variables, we include all the variables if
+      any of the variables is in the list. If `trainable_vars` is None, all the
+      variables are included.
 
   Returns:
     A 1D `tf.Tensor` whose i-th entry is the norm of the gradient of the i-th
     per-example loss function.
   """
   tape = tf.GradientTape(persistent=True, watch_accessed_variables=False)
   registry_generator_fn = get_registry_generator_fn(
@@ -105,34 +118,49 @@
   with tape:
     model_outputs, generator_outputs_list = (
         gradient_clipping_utils.model_forward_pass(
             input_model, x_batch, generator_fn=registry_generator_fn
         )
     )
     # Ignore the original loss function's reduction to get per-example loss.
-    loss_config = input_model.loss.get_config()
-    loss_config['reduction'] = tf.keras.losses.Reduction.NONE
-    per_example_loss_fn = input_model.loss.from_config(loss_config)
+    if per_example_loss_fn is None:
+      loss_config = input_model.loss.get_config()
+      loss_config['reduction'] = tf.keras.losses.Reduction.NONE
+      per_example_loss_fn = input_model.loss.from_config(loss_config)
     losses = per_example_loss_fn(y_batch, model_outputs)
     if num_microbatches is not None:
       losses = tf.reduce_mean(
           lr.add_microbatch_axis(losses, num_microbatches), axis=1
       )
     summed_loss = tf.reduce_sum(losses)
   # Unwrap the generator outputs so that the next loop avoids duplicating
   # backprop ops.
   filtered_outputs = [t for t in generator_outputs_list if t is not None]
-  vars_list = [a for (a, b) in filtered_outputs]
-  sqr_norm_fns_list = [b for (a, b) in filtered_outputs]
+  vars_list = []
+  sqr_norm_fns_list = []
+  if trainable_vars is not None:
+    # Create a set using `ref()` for fast set membership check. tf.Variable
+    # itself is not hashable.
+    trainable_vars = set([v.ref() for v in trainable_vars])
+  for v, f, weights_list in filtered_outputs:
+    if trainable_vars is None or any(
+        w.ref() in trainable_vars for w in weights_list
+    ):
+      # Include only those variables in trainable_vars.
+      vars_list.append(v)
+      sqr_norm_fns_list.append(f)
   # Second loop evaluates the squared L2 norm functions and appends the results.
-  grads_list = tape.gradient(summed_loss, vars_list)
+  grads_list = tape.gradient(
+      summed_loss,
+      vars_list,
+      unconnected_gradients=tf.UnconnectedGradients.ZERO,
+  )
   sqr_norm_list = []
   for grads, f in zip(grads_list, sqr_norm_fns_list):
     sqr_norm_list.append(f(grads))
-  del tape
   sqr_norm_tsr = tf.stack(sqr_norm_list, axis=1)
   return tf.sqrt(tf.reduce_sum(sqr_norm_tsr, axis=1))
 
 
 def compute_clip_weights(l2_norm_clip: float, gradient_norms: tf.Tensor):
   """Computes the per-example loss/clip weights for clipping.
 
@@ -154,32 +182,31 @@
     `|G[i]| * C[i] == l2_norm_clip` otherwise.
   """
   if l2_norm_clip is None:
     return None
   return l2_norm_clip / tf.math.maximum(l2_norm_clip, gradient_norms)
 
 
-def compute_pred_and_clipped_gradients(
+def compute_clipped_gradients_and_outputs(
     input_model: tf.keras.Model,
     x_batch: InputTensor,
     y_batch: tf.Tensor,
     l2_norm_clip: float,
     layer_registry: lr.LayerRegistry,
     num_microbatches: Optional[lr.BatchSize] = None,
-):
-  """Computes the per-example predictions and per-example clipped loss gradient.
+) -> Tuple[List[tf.Tensor], tf.Tensor, float]:
+  """Computes the per-example clipped loss gradient and other useful outputs.
 
   Given a batch of observations `(x_batch, y_batch)`, the main steps of this
   function are: (i) compute the l2-norm of the gradients of the trainable
   variables of `input_model` for each example in the batch; (ii) use the norms
   computed in (i) to obtain "clip_weights" that are used to generate a weighted
   loss function whose gradient for each example has l2-norm at most
-  `l2_norm_clip`; (iii) output the clipped gradients in (ii) and the
-  `tf.Tensor` generated by `input_model` when it is given `x_batch` as its
-  input.
+  `l2_norm_clip`; (iii) output the clipped gradients in (ii) and other useful
+  outputs to the caller.
 
   Args:
     input_model: The `tf.keras.Model` from which to obtain the layers from.
     x_batch: An `InputTensor` representing a batch of inputs to the model. The
       first axis must be the batch dimension.
     y_batch: A `tf.Tensor` representing a batch of output labels. The first axis
       must be the batch dimension. The number of examples should match the
@@ -195,31 +222,57 @@
       trainable weights (see `layer_registry_factories.py` for examples).
     num_microbatches: An optional number or scalar `tf.Tensor` for the number of
       microbatches. If not None, indicates that the loss is grouped into
       num_microbatches (in this case, the batch dimension needs to be a multiple
       of num_microbatches).
 
   Returns:
-    A `tuple` `(y_pred, grad)`. The first element is the prediction generated by
-    the model on the input `x_batch`. The second element is the clipped
-    gradient of the loss function.
+    A `tuple` `(grad, y_pred, weighted_loss_value)`. The first element is the
+    clipped gradient of the loss function, the second is the result of
+    applying `input_model` to `x_batch`, and the third is loss value of
+    `input_model`, weighted by the loss weights generated by a specific
+    `compute_clip_weights()` call.
   """
   gradient_norms = compute_gradient_norms(
-      input_model, x_batch, y_batch, layer_registry, num_microbatches
+      input_model,
+      x_batch,
+      y_batch,
+      layer_registry,
+      num_microbatches=num_microbatches,
+      trainable_vars=input_model.trainable_variables,
   )
   loss_weights = compute_clip_weights(l2_norm_clip, gradient_norms)
   with tf.GradientTape() as tape:
-    y_pred = input_model(x_batch, training=True)
-    if num_microbatches is not None:
-      y_batch = lr.add_microbatch_axis(y_batch, num_microbatches)
-      y_pred = lr.add_microbatch_axis(y_pred, num_microbatches)
-    # Warning: When num_microbatches is not None, we need to be sure that
+    # WARNING: When num_microbatches is not None, we need to be sure that
     # `compute_loss` always computes the mean over the microbatches
     # as it is the assumption made when computing the gradient norm.
     # It is indeed the case for multiple keras loss functions
     # (e.g. mean_squared_error and binary_crossentropy). However it
     # is not defined in the contract so may not hold, especially for
     # custom losses.
-    loss_value = input_model.compute_loss(
-        x_batch, y_batch, y_pred, loss_weights
+    y_pred = input_model(x_batch, training=True)
+    loss_y_batch = (
+        y_batch
+        if num_microbatches is None
+        else lr.add_microbatch_axis(y_batch, num_microbatches)
+    )
+    loss_y_pred = (
+        y_pred
+        if num_microbatches is None
+        else lr.add_microbatch_axis(y_pred, num_microbatches)
     )
-  return y_pred, tape.gradient(loss_value, input_model.trainable_variables)
+    # NOTE: We do not log the loss values here. The caller should invoke
+    # `input_model.compute_loss()` to log loss values. Specifically,
+    # calling `input_model.compute_loss()` performs the following steps:
+    #
+    #   (i) sums `input_model.loss` with the regularization losses given in
+    #       `input_model.losses` to obtain the total loss
+    #   (ii) evaluates the total loss with sample weights (if given)
+    weighted_loss_value = input_model.loss(
+        loss_y_batch, loss_y_pred, loss_weights
+    )
+  clipped_grads = tape.gradient(
+      weighted_loss_value,
+      input_model.trainable_variables,
+      unconnected_gradients=tf.UnconnectedGradients.ZERO,
+  )
+  return clipped_grads, y_pred, weighted_loss_value
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,57 +67,70 @@
     norms1 = sqr_norm_fn1(base_vars[0])
     norms2 = sqr_norm_fn2(base_vars[1])
     return norms1 + norms2
 
   return [vars1, vars2], outputs, sqr_norm_fn
 
 
+def test_loss_fn(x: tf.Tensor, y: tf.Tensor) -> tf.Tensor:
+  x = tf.reshape(x, (tf.shape(x)[0], -1))
+  y = tf.reshape(y, (tf.shape(y)[0], -1))
+  # Define a loss function which is unlikely to be coincidently defined.
+  return 3.14 * tf.reduce_sum(tf.square(x - y), axis=1)
+
+
 def compute_true_gradient_norms(
     input_model: tf.keras.Model,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
+    per_example_loss_fn: Optional[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]],
     num_microbatches: Optional[int],
+    trainable_vars: Optional[tf.Variable] = None,
 ) -> layer_registry.OutputTensor:
   """Computes the real gradient norms for an input `(model, x, y)`."""
-  loss_config = input_model.loss.get_config()
-  loss_config['reduction'] = tf.keras.losses.Reduction.NONE
-  per_example_loss_fn = input_model.loss.from_config(loss_config)
+  if per_example_loss_fn is None:
+    loss_config = input_model.loss.get_config()
+    loss_config['reduction'] = tf.keras.losses.Reduction.NONE
+    per_example_loss_fn = input_model.loss.from_config(loss_config)
   with tf.GradientTape(persistent=True) as tape:
     y_pred = input_model(x_batch)
     loss = per_example_loss_fn(y_batch, y_pred)
     if num_microbatches is not None:
       loss = tf.reduce_mean(
           tf.reshape(
               loss,
               tf.concat([[num_microbatches, -1], tf.shape(loss)[1:]], axis=0),
           ),
           axis=1,
       )
     if isinstance(loss, tf.RaggedTensor):
       loss = loss.to_tensor()
   sqr_norms = []
-  for var in input_model.trainable_variables:
+  trainable_vars = trainable_vars or input_model.trainable_variables
+  for var in trainable_vars:
     jacobian = tape.jacobian(loss, var, experimental_use_pfor=False)
     reduction_axes = tf.range(1, len(jacobian.shape))
     sqr_norm = tf.reduce_sum(tf.square(jacobian), axis=reduction_axes)
     sqr_norms.append(sqr_norm)
   sqr_norm_tsr = tf.stack(sqr_norms, axis=1)
   return tf.sqrt(tf.reduce_sum(sqr_norm_tsr, axis=1))
 
 
 def get_computed_and_true_norms(
     model_generator: ModelGenerator,
     layer_generator: LayerGenerator,
     input_dims: Union[int, List[int]],
     output_dim: int,
+    per_example_loss_fn: Optional[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]],
     num_microbatches: Optional[int],
     is_eager: bool,
     x_input: tf.Tensor,
     rng_seed: int = 777,
     registry: layer_registry.LayerRegistry = None,
+    partial: bool = False,
 ) -> Tuple[tf.Tensor, tf.Tensor]:
   """Obtains the true and computed gradient norms for a model and batch input.
 
   Helpful testing wrapper function used to avoid code duplication.
 
   Args:
     model_generator: A function which takes in three arguments:
@@ -126,19 +139,23 @@
       dimension `odim`. Layers of the model are based on the `layer_generator`
       (see below for its description).
     layer_generator: A function which takes in two arguments: `idim` and `odim`.
       Returns a `tf.keras.layers.Layer` that accepts input tensors of dimension
       `idim` and returns output tensors of dimension `odim`.
     input_dims: The input dimension(s) of the test `tf.keras.Model` instance.
     output_dim: The output dimension of the test `tf.keras.Model` instance.
+    per_example_loss_fn: If not None, used as vectorized per example loss
+      function.
     num_microbatches: The number of microbatches. None or an integer.
     is_eager: A `bool` that is `True` if the model should be run eagerly.
     x_input: `tf.Tensor` inputs to be tested.
     rng_seed: An `int` used to initialize model weights.
     registry: A `layer_registry.LayerRegistry` instance.
+    partial: Whether to compute the gradient norm with respect to a partial set
+      of varibles. If True, only consider the variables in the first layer.
 
   Returns:
     A `tuple` `(computed_norm, true_norms)`. The first element contains the
     clipped gradient norms that are generated by
     `clip_grads.compute_gradient_norms()` under the setting given by the given
     model and layer generators. The second element contains the true clipped
     gradient norms under the aforementioned setting.
@@ -147,27 +164,41 @@
   model.compile(
       optimizer=tf.keras.optimizers.SGD(learning_rate=1.0),
       loss=tf.keras.losses.MeanSquaredError(
           reduction=tf.keras.losses.Reduction.SUM_OVER_BATCH_SIZE
       ),
       run_eagerly=is_eager,
   )
+  trainable_vars = None
+  if partial:
+    # Gets the first layer with variables.
+    for l in model.layers:
+      trainable_vars = l.trainable_variables
+      if trainable_vars:
+        break
   y_pred = model(x_input)
   y_batch = tf.ones_like(y_pred)
   tf.keras.utils.set_random_seed(rng_seed)
   computed_norms = clip_grads.compute_gradient_norms(
       model,
       x_input,
       y_batch,
       layer_registry=registry,
+      per_example_loss_fn=per_example_loss_fn,
       num_microbatches=num_microbatches,
+      trainable_vars=trainable_vars,
   )
   tf.keras.utils.set_random_seed(rng_seed)
   true_norms = compute_true_gradient_norms(
-      model, x_input, y_batch, num_microbatches
+      model,
+      x_input,
+      y_batch,
+      per_example_loss_fn,
+      num_microbatches,
+      trainable_vars=trainable_vars,
   )
   return (computed_norms, true_norms)
 
 
 # ==============================================================================
 # Model generators.
 # ==============================================================================
@@ -343,26 +374,30 @@
 
 class ClipGradsDenseLayerTest(tf.test.TestCase, parameterized.TestCase):
 
   @parameterized.product(
       model_name=list(get_dense_model_generators().keys()),
       layer_name=list(get_dense_layer_generators().keys()),
       input_dim=[4],
-      output_dim=[1, 2],
+      output_dim=[2],
+      per_example_loss_fn=[None, test_loss_fn],
       num_microbatches=[None, 1, 2],
       is_eager=[True, False],
+      partial=[True, False],
   )
   def test_gradient_norms_on_various_models(
       self,
       model_name,
       layer_name,
       input_dim,
       output_dim,
+      per_example_loss_fn,
       num_microbatches,
       is_eager,
+      partial,
   ):
     model_generator = get_dense_model_generators()[model_name]
     layer_generator = get_dense_layer_generators()[layer_name]
     x_batches = get_nd_test_batches(input_dim)
     default_registry = layer_registry.make_default_layer_registry()
     for x_batch in x_batches:
       if (
@@ -375,18 +410,20 @@
       else:
         x_input = x_batch
       (computed_norms, true_norms) = get_computed_and_true_norms(
           model_generator,
           layer_generator,
           input_dim,
           output_dim,
+          per_example_loss_fn,
           num_microbatches,
           is_eager,
           x_input,
           registry=default_registry,
+          partial=partial,
       )
       self.assertAllClose(computed_norms, true_norms, rtol=1e-3, atol=1e-2)
 
 
 class ClipGradsEmbeddingLayerTest(tf.test.TestCase, parameterized.TestCase):
 
   # TODO(wkong): Test sparse input tensors when the GitHub CI environment
@@ -415,19 +452,28 @@
           tf.ragged.constant(
               [[[0]], [[1]], [], [[0, 0]], [[0, 1]], [[1, 0]], [[1, 1]], [[0]]],
               dtype=tf.int32,
           ),
       ],
       model_name=list(get_embedding_model_generators().keys()),
       output_dim=[2],
-      num_microbatches=[None, 1, 2],
-      is_eager=[True],
+      per_example_loss_fn=[None, test_loss_fn],
+      num_microbatches=[None, 2],
+      is_eager=[True, False],
+      partial=[True, False],
   )
   def test_gradient_norms_on_various_models(
-      self, x_batch, model_name, output_dim, num_microbatches, is_eager
+      self,
+      x_batch,
+      model_name,
+      output_dim,
+      per_example_loss_fn,
+      num_microbatches,
+      is_eager,
+      partial,
   ):
     if (
         num_microbatches is not None
         and x_batch.shape[0] % num_microbatches != 0
     ):
       return
     valid_test_input = (
@@ -438,32 +484,42 @@
       default_registry = layer_registry.make_default_layer_registry()
       model_generator = get_embedding_model_generators()[model_name]
       (computed_norms, true_norms) = get_computed_and_true_norms(
           model_generator=model_generator,
           layer_generator=None,
           input_dims=x_batch.shape[1:],
           output_dim=output_dim,
+          per_example_loss_fn=per_example_loss_fn,
           num_microbatches=num_microbatches,
           is_eager=is_eager,
           x_input=x_batch,
           registry=default_registry,
+          partial=partial,
       )
       self.assertAllClose(computed_norms, true_norms, rtol=1e-3, atol=1e-2)
 
 
 class ClipGradsCustomLayerTest(tf.test.TestCase, parameterized.TestCase):
 
   @parameterized.product(
-      input_dim=[1, 2],
-      output_dim=[1, 2],
-      num_microbatches=[None, 1, 2],
+      input_dim=[3],
+      output_dim=[2],
+      per_example_loss_fn=[None, test_loss_fn],
+      num_microbatches=[None, 2],
       is_eager=[True, False],
+      partial=[True, False],
   )
   def test_gradient_norms_on_various_models(
-      self, input_dim, output_dim, num_microbatches, is_eager
+      self,
+      input_dim,
+      output_dim,
+      per_example_loss_fn,
+      num_microbatches,
+      is_eager,
+      partial,
   ):
     registry = layer_registry.make_default_layer_registry()
     registry.insert(DoubleDense, double_dense_layer_computation)
     x_batches = get_nd_test_batches(input_dim)
     for x_batch in x_batches:
       if (
           num_microbatches is not None
@@ -471,17 +527,19 @@
       ):
         continue
       (computed_norms, true_norms) = get_computed_and_true_norms(
           model_generator=make_two_layer_sequential_model,
           layer_generator=lambda a, b: DoubleDense(b),
           input_dims=input_dim,
           output_dim=output_dim,
+          per_example_loss_fn=per_example_loss_fn,
           num_microbatches=num_microbatches,
           is_eager=is_eager,
           x_input=x_batch,
           registry=registry,
+          partial=partial,
       )
       self.assertAllClose(computed_norms, true_norms, rtol=1e-3, atol=1e-2)
 
 
 if __name__ == '__main__':
   tf.test.main()
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/gradient_clipping_utils.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/gradient_clipping_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utility functions that help in the computation of per-example gradient norms."""
 
-from typing import Any, Callable, Dict, Iterable, List, Optional, Text, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Text, Tuple, Union
 
 from absl import logging
 import tensorflow as tf
 
 from tensorflow_privacy.privacy.fast_gradient_clipping import layer_registry as lr
 
-InputTensor = Union[tf.Tensor, Iterable[tf.Tensor], Dict[Text, tf.Tensor]]
+PackedTensors = Union[tf.Tensor, Iterable[tf.Tensor], Dict[Text, tf.Tensor]]
 
 GeneratorFunction = Optional[Callable[[Any, Tuple, Dict], Tuple[Any, Any]]]
 
 
 def has_internal_compute_graph(input_object: Any):
   """Checks if input is a TF model and has a TF internal compute graph."""
   return (
@@ -32,32 +32,19 @@
       and hasattr(input_object, '_flatten_to_reference_inputs')
       and hasattr(input_object, '_tensor_usage_count')
       and hasattr(input_object, '_conform_to_reference_input')
       and hasattr(input_object, '_nodes_by_depth')
   )
 
 
-def _get_internal_layers(
-    input_layer: tf.keras.layers.Layer,
-) -> List[tf.keras.layers.Layer]:
-  """Returns a list of layers that are nested within a given layer."""
-  internal_layers = []
-  if isinstance(input_layer, tf.keras.Model) and hasattr(input_layer, 'layers'):
-    for layer in input_layer.layers:
-      internal_layers.extend(_get_internal_layers(layer))
-  else:
-    internal_layers.append(input_layer)
-  return internal_layers
-
-
 def model_forward_pass(
     input_model: tf.keras.Model,
-    inputs: InputTensor,
+    inputs: PackedTensors,
     generator_fn: GeneratorFunction = None,
-) -> Tuple[tf.Tensor, List[Any]]:
+) -> Tuple[PackedTensors, List[Any]]:
   """Does a forward pass of a model and returns useful intermediates.
 
   NOTE: the graph traversal algorithm is an adaptation of the logic in the
     _run_internal_graph() method in the functional.Functional class. Hence,
     forward_norm_pass should only be invoked if the generated model
     instance is an instance of the functional.Functional class.
 
@@ -68,15 +55,15 @@
     generator_fn: A function with signature `(tf.keras.layers.Layer, Any, Any)
       -> (tf.Tensor, Any)`, where we require `generator_fn(layer_instance, args,
       kwargs)[0] == layer_instance(*args, **kwargs)`. If `None`, then
       `layer_fn(layer_instance, args, kwargs)[1] == None`.
 
   Returns:
     A `tuple` `(outputs, generator_outputs_list)`. `outputs` is the
-    `tf.Tensor` that is generated as a result of a forward pass.
+    `PackedTensor` that is generated as a result of a forward pass.
     `generator_outputs_list` is a `list` whose i-th entry is the output of
     `generator_fn(lyr, args, kwargs)[1]` where `lyr` is the i-th
     layer when the compute graph of `input_model` is traversed in BFS order.
   """
   # TODO: Avoid or remove the references to protected methods of `input_model`.  # pylint: disable=g-bad-todo
 
   # Default generator.
@@ -110,34 +97,36 @@
         # If this node has an internal computational graph, we can recurse.
         node_layer_outputs, node_generator_outputs = model_forward_pass(
             node.layer, args, generator_fn
         )
         generator_outputs_list.extend(node_generator_outputs)
       else:
         # Otherwise, we parse the node directly.
-        node_layers = _get_internal_layers(node.layer)
-        for layer in node_layers:
-          node_layer_outputs, layer_generator_outputs = generator_fn(
-              layer, args, kwargs
-          )
-          generator_outputs_list.append(layer_generator_outputs)
-          args = (
-              node_layer_outputs
-              if isinstance(node_layer_outputs, tuple)
-              else (node_layer_outputs,)
-          )
-          kwargs = {}
+        node_layer_outputs, layer_generator_outputs = generator_fn(
+            node.layer, args, kwargs
+        )
+        generator_outputs_list.append(layer_generator_outputs)
 
       # Update the current dictionary of inputs for the next node.
       for x_id, y in zip(
           node.flat_output_ids, tf.nest.flatten(node_layer_outputs)
       ):
         tensor_dict[x_id] = [y] * tensor_usage_count[x_id]
 
-  return node_layer_outputs, generator_outputs_list
+  # Gather outputs (in case there are multiple) and return.
+  output_tensors = []
+  for x in input_model.outputs:
+    x_id = str(id(x))
+    output_tensors.append(tensor_dict[x_id].pop())
+  model_outputs = tf.nest.pack_sequence_as(
+      input_model._nested_outputs,  # pylint: disable=protected-access
+      output_tensors,
+  )
+
+  return model_outputs, generator_outputs_list
 
 
 def all_trainable_layers_are_registered(
     input_model: tf.keras.Model, layer_registry: lr.LayerRegistry
 ) -> bool:
   """Check if an input model's trainable layers are all registered.
 
@@ -149,17 +138,16 @@
       more details.
 
   Returns:
     True if all the trainable layers in `input_model` are in `layer_registry`.
     False otherwise.
   """
   for layer in input_model.layers:
-    for sublayer in _get_internal_layers(layer):
-      if not layer_registry.is_elem(sublayer) and sublayer.trainable_variables:
-        return False
+    if not layer_registry.is_elem(layer) and layer.trainable_variables:
+      return False
   return True
 
 
 def add_aggregate_noise(
     input_model: tf.keras.Model,
     clipped_grads: list[tf.Tensor],
     batch_size: tf.Tensor,
@@ -199,21 +187,57 @@
     )
 
   return tf.nest.map_structure(add_noise, clipped_grads)
 
 
 def generate_model_outputs_using_core_keras_layers(
     input_model: tf.keras.Model,
-) -> tf.Tensor:
-  """Returns the model outputs generated by only core Keras layers."""
-  cust_obj_dict = dict.copy(tf.keras.utils.get_custom_objects())
-  cust_hash_set = set([hash(v) for v in cust_obj_dict.values()])
+    custom_layer_set: Optional[Set[type]] = None,  # pylint: disable=g-bare-generic
+) -> PackedTensors:
+  """Returns the model outputs generated by only core Keras layers.
+
+  Args:
+    input_model: A `tf.keras.Model` instance to obtain outputs from.
+    custom_layer_set: An optional `set` of custom layers to expand. If `None`,
+      then this is the set of all registered custom Keras layers.
+
+  Returns:
+    A `tf.Tensor` that is the result of `input_model(input_model.inputs)`
+    using only Keras layers that are not in `custom_layer_set`.
+  """
+  # Set up helper variables and functions.
+  custom_layer_set = (
+      custom_layer_set or tf.keras.utils.get_custom_objects().values()
+  )
+
+  def _is_core(layer_instance):
+    return type(layer_instance) not in custom_layer_set
 
   def generator_fn(layer_instance, args, kwargs):
-    if hash(layer_instance.__class__) in cust_hash_set:
-      # Using `.call()` does not register the layer in the compute graph of
-      # a forward pass.
-      return layer_instance.call(*args, **kwargs), None
-    else:
-      return layer_instance(*args, **kwargs), None
+    # Using `.call()` does not register the layer in the compute graph of
+    # a forward pass.
+    layer_outputs = (
+        layer_instance(*args, **kwargs)
+        if _is_core(layer_instance)
+        else layer_instance.call(*args, **kwargs)
+    )
+    return layer_outputs, None
 
-  return model_forward_pass(input_model, input_model.inputs, generator_fn)[0]
+  # Return early if all the existing layers contain only core layers.
+  if all(_is_core(layer) for layer in input_model.layers):
+    return model_forward_pass(input_model, input_model.inputs)[0]
+
+  # Do a forward pass to expand the outermost layers.
+  candidate_outputs, _ = model_forward_pass(
+      input_model, input_model.inputs, generator_fn
+  )
+
+  # The following recursion is inefficient because it recursively builds `n`
+  # Keras model graphs, where `n` is the number of recursive calls. However,
+  # it appears to be the only valid approach without accessing Keras's internal
+  # functions (e.g., `keras.engine.functional._map_graph_network()`).
+  cleaned_model = tf.keras.Model(
+      inputs=input_model.inputs, outputs=candidate_outputs
+  )
+  return generate_model_outputs_using_core_keras_layers(
+      cleaned_model, custom_layer_set
+  )
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/fast_gradient_clipping/layer_registry.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/fast_gradient_clipping/layer_registry.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/keras_models/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/keras_models/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/keras_models/dp_keras_model.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_vectorized.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,262 +1,259 @@
-# Copyright 2021, The TensorFlow Authors.
+# Copyright 2020 The TensorFlow Authors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Keras Model for vectorized dpsgd with XLA acceleration."""
+# ==============================================================================
+"""Differentially private version of Keras optimizer v2."""
 
-from absl import logging
 import tensorflow as tf
-from tensorflow_privacy.privacy.fast_gradient_clipping import clip_grads
-from tensorflow_privacy.privacy.fast_gradient_clipping import gradient_clipping_utils
 
+from tensorflow_privacy.privacy.dp_query import gaussian_query
 
-def make_dp_model_class(cls):
-  """Given a subclass of `tf.keras.Model`, returns a DP-SGD version of it."""
 
-  class DPModelClass(cls):  # pylint: disable=missing-class-docstring
-    __doc__ = (
-        """DP subclass of `{base_model}`.
-
-        This can be used as a differentially private replacement for
-        {base_model}. This class implements DP-SGD using the standard
-        Gaussian mechanism.
-
-        This class also utilizes a faster gradient clipping algorithm if the
-        following two conditions hold:
-        (i)  the trainable layers of the model are keys in the `dict` input
-             `layer_registry`,
-        (ii) the loss `tf.Tensor` for a given batch of examples is either a
-             scalar or a 2D `tf.Tensor` that has only one column
-             `(i.e., tf.shape(loss)[1] == 1)` and whose i-th row corresponds to
-             the loss of the i-th example.
-        This clipping algorithm specifically computes clipped gradients at the
-        per-example or per microbatch (when `num_microbatches` is not None)
-        level using the layer registry functions in `layer_registry` (see
-        clip_grads.py for more information about the algorithm).
-
-        WARNING: with faster gradient clipping, and when num_microbatches is not
-        None, the per microbatch loss is assumed to be computed as the mean
-        of the loss over the microbatch, or effectively, by reshaping the loss
-        from the shape [batch_size, ...] to the shape
-        [num_microbatches, batch_size/num_microbatches, ...] and computing the
-        mean of the loss over the microbatches. This would require that the loss
-        function behaves accordingly. This is true for multiple common
-        predefined keras loss functions (e.g. mean_squared_loss,
-        binary_crossentropy) but may not hold for custom losses (and how such
-        aggregation is done is not exposed by the loss function, unfortunately).
-        It is the caller's responsibility to make sure that the loss function
-        does behave this way.
-
-        When instantiating this class, you need to supply several
-        DP-related arguments followed by the standard arguments for
-        `{short_base_model}`.
-
-          Examples:
-
-        ```python
-        # Create Model instance.
-        model = {dp_model_class}(l2_norm_clip=1.0, noise_multiplier=0.5, use_xla=True,
-                 <standard arguments>)
-        ```
-
-        You should use your {dp_model_class} instance with a standard instance
-        of `tf.keras.Optimizer` as the optimizer, and a standard reduced loss.
-        You do not need to use a differentially private optimizer.
-
-        ```python
-        # Use a standard (non-DP) optimizer.
-        optimizer = tf.keras.optimizers.SGD(learning_rate=0.01)
-
-        # Use a standard reduced loss.
-        loss = tf.keras.losses.MeanSquaredError()
-
-        model.compile(optimizer=optimizer, loss=loss)
-        model.fit(train_data, train_labels, epochs=1, batch_size=32)
-        ```
-
-        """
-    ).format(
-        base_model='tf.keras.' + cls.__name__,
-        short_base_model=cls.__name__,
-        dp_model_class='DP' + cls.__name__,
-    )
+def clip_gradients_vmap(g, l2_norm_clip):
+  """Clips gradients in a way that is compatible with vectorized_map."""
+  grads_flat = tf.nest.flatten(g)
+  squared_l2_norms = [
+      tf.reduce_sum(input_tensor=tf.square(g)) for g in grads_flat
+  ]
+  global_norm = tf.sqrt(tf.add_n(squared_l2_norms))
+  div = tf.maximum(global_norm / l2_norm_clip, 1.)
+  clipped_flat = [g / div for g in grads_flat]
+  clipped_grads = tf.nest.pack_sequence_as(g, clipped_flat)
+  return clipped_grads
+
+
+def make_vectorized_keras_optimizer_class(cls):
+  """Given a subclass of `tf.keras.optimizers.Optimizer`, returns a vectorized DP-SGD subclass of it.
+
+  Args:
+    cls: Class from which to derive a DP subclass. Should be a subclass of
+      `tf.keras.optimizers.Optimizer`.
+
+  Returns:
+    A vectorized DP-SGD subclass of `cls`.
+  """
+
+  class DPOptimizerClass(cls):  # pylint: disable=empty-docstring
+    __doc__ = """Vectorized differentially private subclass of given class
+    `{base_class}`.
+
+    You can use this as a differentially private replacement for
+    `{base_class}`. This optimizer implements DP-SGD using
+    the standard Gaussian mechanism. It differs from `{dp_keras_class}` in that
+    it attempts to vectorize the gradient computation and clipping of
+    microbatches.
+
+    When instantiating this optimizer, you need to supply several
+    DP-related arguments followed by the standard arguments for
+    `{short_base_class}`.
+
+    Examples:
+
+    ```python
+    # Create optimizer.
+    opt = {dp_vectorized_keras_class}(l2_norm_clip=1.0, noise_multiplier=0.5, num_microbatches=1,
+            <standard arguments>)
+    ```
+
+    When using the optimizer, be sure to pass in the loss as a
+    rank-one tensor with one entry for each example.
+
+    The optimizer can be used directly via its `minimize` method, or
+    through a Keras `Model`.
+
+    ```python
+    # Compute loss as a tensor by using tf.losses.Reduction.NONE.
+    # Compute vector of per-example loss rather than its mean over a minibatch.
+    # (Side note: Always verify that the output shape when using
+    # tf.losses.Reduction.NONE-- it can sometimes be surprising.
+    loss = tf.keras.losses.CategoricalCrossentropy(
+        from_logits=True, reduction=tf.losses.Reduction.NONE)
+
+    # Use optimizer in a Keras model.
+    opt.minimize(loss, var_list=[var])
+    ```
+
+    ```python
+    # Compute loss as a tensor by using tf.losses.Reduction.NONE.
+    # Compute vector of per-example loss rather than its mean over a minibatch.
+    loss = tf.keras.losses.CategoricalCrossentropy(
+        from_logits=True, reduction=tf.losses.Reduction.NONE)
+
+    # Use optimizer in a Keras model.
+    model = tf.keras.Sequential(...)
+    model.compile(optimizer=opt, loss=loss, metrics=['accuracy'])
+    model.fit(...)
+    ```
+
+    """.format(
+        base_class='tf.keras.optimizers.' + cls.__name__,
+        dp_keras_class='DPKeras' + cls.__name__,
+        short_base_class=cls.__name__,
+        dp_vectorized_keras_class='VectorizedDPKeras' + cls.__name__)
 
     def __init__(
         self,
         l2_norm_clip,
         noise_multiplier,
         num_microbatches=None,
-        use_xla=True,
-        layer_registry=None,
+        unconnected_gradients_to_zero=False,
         *args,  # pylint: disable=keyword-arg-before-vararg, g-doc-args
-        **kwargs,
-    ):
-      """Initializes the DPModelClass.
+        **kwargs):
+      """Initialize the DPOptimizerClass.
 
       Args:
         l2_norm_clip: Clipping norm (max L2 norm of per microbatch gradients).
         noise_multiplier: Ratio of the standard deviation to the clipping norm.
-        num_microbatches: Number of microbatches.
-        use_xla: If `True`, compiles train_step to XLA.
-        layer_registry: A `LayerRegistry` instance containing functions that
-          help compute gradient norms quickly. See
-          `tensorflow_privacy.privacy.fast_gradient_clipping.layer_registry` for
-          more details.
+        num_microbatches: Number of microbatches into which each minibatch is
+          split.
+        unconnected_gradients_to_zero: The Jacobian is used to compute the
+          microbatch losses. If a node in the graph is deliberately not
+          connected, then the Jacobian computation will return a `None` for that
+          node. Set this flag to True to treat these Jacobians as zero.
         *args: These will be passed on to the base class `__init__` method.
         **kwargs: These will be passed on to the base class `__init__` method.
       """
       super().__init__(*args, **kwargs)
       self._l2_norm_clip = l2_norm_clip
       self._noise_multiplier = noise_multiplier
-      self._layer_registry = layer_registry
-
-      # Given that `num_microbatches` was added as an argument after the fact,
-      # this check helps detect unintended calls to the earlier API.
-      # In particular, boolean values supplied to `use_xla` in the earlier API
-      # will raise an error.
-      if isinstance(num_microbatches, bool):
-        raise ValueError('Boolean value supplied for `num_microbatches`. '
-                         'Did you intend it for `use_xla`?')
       self._num_microbatches = num_microbatches
+      self._unconnected_gradients_to_zero = unconnected_gradients_to_zero
+      self._dp_sum_query = gaussian_query.GaussianSumQuery(
+          l2_norm_clip, l2_norm_clip * noise_multiplier)
+      self._global_state = None
+      self._was_dp_gradients_called = False
+
+    def _compute_gradients(self, loss, var_list, grad_loss=None, tape=None):
+      """DP-SGD version of base class method."""
+
+      self._was_dp_gradients_called = True
+      # Compute loss.
+      if not callable(loss) and tape is None:
+        raise ValueError('`tape` is required when a `Tensor` loss is passed.')
+      tape = tape if tape is not None else tf.GradientTape()
+
+      if callable(loss):
+        with tape:
+          if not callable(var_list):
+            tape.watch(var_list)
+
+          loss = loss()
+          if self._num_microbatches is None:
+            num_microbatches = tf.shape(input=loss)[0]
+          else:
+            num_microbatches = self._num_microbatches
+          microbatch_losses = tf.reduce_mean(
+              tf.reshape(loss, [num_microbatches, -1]), axis=1)
 
-      # If all the trainable layers are in the input layer registry, we
-      # don't need to use microbatching and can instead use the "fast"
-      # chain rule trick for computing per-example gradients (peg).
-      if (
-          layer_registry is not None
-          and gradient_clipping_utils.all_trainable_layers_are_registered(
-              self, layer_registry
-          )
-          and gradient_clipping_utils.has_internal_compute_graph(self)
-      ):
-        self._enable_fast_peg_computation = True
+          if callable(var_list):
+            var_list = var_list()
       else:
-        self._enable_fast_peg_computation = False
-
-      if use_xla:
-        self.train_step = tf.function(
-            self.train_step, experimental_compile=True)
-
-    def _process_per_example_grads(self, grads):
-      grads_flat = tf.nest.flatten(grads)
-      squared_l2_norms = [
-          tf.reduce_sum(input_tensor=tf.square(g)) for g in grads_flat
-      ]
-      global_norm = tf.sqrt(tf.add_n(squared_l2_norms))
-      div = tf.maximum(global_norm / self._l2_norm_clip, 1.)
-      clipped_flat = [g / div for g in grads_flat]
-      return tf.nest.pack_sequence_as(grads, clipped_flat)
-
-    def _reduce_per_example_grads(self, stacked_grads):
-      summed_grads = tf.reduce_sum(input_tensor=stacked_grads, axis=0)
-      noise_stddev = self._l2_norm_clip * self._noise_multiplier
-      noise = tf.random.normal(
-          tf.shape(input=summed_grads), stddev=noise_stddev)
-      noised_grads = summed_grads + noise
-      return noised_grads / tf.cast(stacked_grads.shape[0], noised_grads.dtype)
-
-    def _compute_per_example_grads(self, data):
-      x, y = data
-      with tf.GradientTape() as tape:
-        y_pred = self(x, training=True)
-        loss = self.compiled_loss(y, y_pred, regularization_losses=self.losses)
-
-      grads_list = tape.gradient(loss, self.trainable_variables)
-      clipped_grads = self._process_per_example_grads(grads_list)
-      return y_pred, loss, clipped_grads
-
-    def train_step(self, data):
-      """DP-SGD version of base class method.
-
-      Uses the "fast" gradient clipping algorithm to generate per-example
-      clipped gradients if (i) all the trainable layers of the model are
-      registered in the layer_registry input of the model constructor and
-      (ii) if the model contains an internal compute graph (e.g., this
-      condition is satisfied if the model subclasses the keras.Sequential or
-      keras.engine.functional.Functional class).
+        with tape:
+          if self._num_microbatches is None:
+            num_microbatches = tf.shape(input=loss)[0]
+          else:
+            num_microbatches = self._num_microbatches
+          microbatch_losses = tf.reduce_mean(
+              tf.reshape(loss, [num_microbatches, -1]), axis=1)
+
+      var_list = tf.nest.flatten(var_list)
+
+      # Compute the per-microbatch losses using helpful jacobian method.
+      with tf.keras.backend.name_scope(self._name + '/gradients'):
+        jacobian = tape.jacobian(
+            microbatch_losses,
+            var_list,
+            unconnected_gradients=(tf.UnconnectedGradients.ZERO
+                                   if self._unconnected_gradients_to_zero else
+                                   tf.UnconnectedGradients.NONE))
+
+        clipped_gradients = tf.vectorized_map(
+            lambda g: clip_gradients_vmap(g, self._l2_norm_clip), jacobian)
+
+        def reduce_noise_normalize_batch(g):
+          # Sum gradients over all microbatches.
+          summed_gradient = tf.reduce_sum(g, axis=0)
+
+          # Add noise to summed gradients.
+          noise_stddev = self._l2_norm_clip * self._noise_multiplier
+          noise = tf.random.normal(
+              tf.shape(input=summed_gradient), stddev=noise_stddev)
+          noised_gradient = tf.add(summed_gradient, noise)
+
+          # Normalize by number of microbatches and return.
+          return tf.truediv(noised_gradient,
+                            tf.cast(num_microbatches, tf.float32))
+
+        final_gradients = tf.nest.map_structure(reduce_noise_normalize_batch,
+                                                clipped_gradients)
+
+      return list(zip(final_gradients, var_list))
+
+    def get_gradients(self, loss, params):
+      """DP-SGD version of base class method."""
+
+      self._was_dp_gradients_called = True
+      if self._global_state is None:
+        self._global_state = self._dp_sum_query.initial_global_state()
 
-      If (i) and (ii) above do not hold, then clips and aggregates
-      gradients at the microbatch level.
-
-      Args:
-        data: see the base class.
-
-      Returns:
-        See the base class.
-      """
-      if self._enable_fast_peg_computation:
-        logging.info(
-            'Computing gradients using the fast per-example gradient '
-            'norm algorithm.'
-        )
-        # Computes the per-example gradient norms using a "fast" clipping
-        # trick, and uses these norms to clip the per-example gradients.
-        x, y, _ = tf.keras.utils.unpack_x_y_sample_weight(data)
-        y_pred, clipped_grads = clip_grads.compute_pred_and_clipped_gradients(
-            self,
-            x,
-            y,
-            self._l2_norm_clip,
-            self._layer_registry,
-            self._num_microbatches,
-        )
-        batch_size = self._num_microbatches or tf.shape(y)[0]
-        grads = gradient_clipping_utils.add_aggregate_noise(
-            self,
-            clipped_grads,
-            batch_size,
-            self._l2_norm_clip,
-            self._noise_multiplier,
-        )
+      if self._num_microbatches is None:
+        num_microbatches = tf.shape(input=loss)[0]
       else:
-        logging.info('Computing gradients using microbatching.')
-        # Computes per-example clipped gradients directly. This is called
-        # if at least one of the layers cannot use the "fast" gradient clipping
-        # algorithm.
-        # TODO(wkong): check if the following is valid with sample weights.
-        _, y = data
-        batch_size = y.shape[0]
-
-        if self._num_microbatches is None:
-          self._num_microbatches = batch_size
-        if batch_size % self._num_microbatches != 0:
-          raise ValueError('Number of_microbatches must divide batch size.')
-
-        def reshape_fn(x):
-          new_shape = (
-              self._num_microbatches,
-              batch_size // self._num_microbatches,
-          ) + x.shape[1:]
-          return tf.reshape(x, new_shape)
-
-        data = tf.nest.map_structure(reshape_fn, data)
-
-        y_pred, _, per_eg_grads = tf.vectorized_map(
-            self._compute_per_example_grads, data
-        )
-
-        y_pred = tf.reshape(y_pred, (batch_size) + y_pred.shape[2:])
-
-        grads = tf.nest.map_structure(
-            self._reduce_per_example_grads, per_eg_grads
-        )
-
-      # Forward the private gradients to the optimizer and return the results.
-      self.optimizer.apply_gradients(zip(grads, self.trainable_variables))
-      self.compiled_metrics.update_state(y, y_pred)
-      return {m.name: m.result() for m in self.metrics}
-
-  return DPModelClass
+        num_microbatches = self._num_microbatches
 
+      microbatch_losses = tf.reshape(loss, [num_microbatches, -1])
 
-DPModel = make_dp_model_class(tf.keras.Model)
-DPSequential = make_dp_model_class(tf.keras.Sequential)
+      def process_microbatch(microbatch_loss):
+        """Compute clipped grads for one microbatch."""
+        mean_loss = tf.reduce_mean(input_tensor=microbatch_loss)
+        grads = cls.get_gradients(self, mean_loss, params)
+        grads_list = [
+            g if g is not None else tf.zeros_like(v)
+            for (g, v) in zip(list(grads), params)
+        ]
+        clipped_grads = clip_gradients_vmap(grads_list, self._l2_norm_clip)
+        return clipped_grads
+
+      clipped_grads = tf.vectorized_map(process_microbatch, microbatch_losses)
+
+      def reduce_noise_normalize_batch(stacked_grads):
+        summed_grads = tf.reduce_sum(input_tensor=stacked_grads, axis=0)
+        noise_stddev = self._l2_norm_clip * self._noise_multiplier
+        noise = tf.random.normal(
+            tf.shape(input=summed_grads), stddev=noise_stddev)
+        noised_grads = summed_grads + noise
+        return noised_grads / tf.cast(num_microbatches, tf.float32)
+
+      final_grads = tf.nest.map_structure(reduce_noise_normalize_batch,
+                                          clipped_grads)
+      return final_grads
+
+    def apply_gradients(self, *args, **kwargs):
+      """DP-SGD version of base class method."""
+      assert self._was_dp_gradients_called, (
+          'Neither _compute_gradients() or get_gradients() on the '
+          'differentially private optimizer was called. This means the '
+          'training is not differentially private. It may be the case that '
+          'you need to upgrade to TF 2.4 or higher to use this particular '
+          'optimizer.')
+      return super(DPOptimizerClass, self).apply_gradients(*args, **kwargs)
+
+  return DPOptimizerClass
+
+
+VectorizedDPKerasAdagradOptimizer = make_vectorized_keras_optimizer_class(
+    tf.keras.optimizers.legacy.Adagrad)
+VectorizedDPKerasAdamOptimizer = make_vectorized_keras_optimizer_class(
+    tf.keras.optimizers.legacy.Adam)
+VectorizedDPKerasSGDOptimizer = make_vectorized_keras_optimizer_class(
+    tf.keras.optimizers.legacy.SGD)
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/keras_models/dp_keras_model_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/keras_models/dp_keras_model_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -278,9 +278,97 @@
               tf.keras.layers.Dense(
                   2, use_bias=False, kernel_initializer='zeros'
               ),
               tf.keras.layers.Dense(1),
           ],
       )
 
+  # Simple test to check that regularizer gradients are contributing to the
+  # final gradient.
+  @parameterized.named_parameters(
+      ('no_registry', None),
+      ('default_registry', layer_registry.make_default_layer_registry()),
+  )
+  def testRegularizationGradient(self, registry):
+    input_dim = 10
+    batch_size = 2
+    regularizer_multiplier = 0.025
+    inputs = tf.keras.layers.Input((input_dim,))
+    dense_lyr = tf.keras.layers.Dense(
+        1,
+        kernel_initializer='ones',
+        use_bias=False,
+        kernel_regularizer=tf.keras.regularizers.L2(regularizer_multiplier),
+    )
+    # Zero-out outputs to avoid contributions from the main loss function.
+    outputs = tf.multiply(dense_lyr(inputs), 0.0)
+    model = dp_keras_model.DPModel(
+        inputs=inputs,
+        outputs=outputs,
+        l2_norm_clip=1e9,
+        noise_multiplier=0.0,
+        layer_registry=registry,
+    )
+    model.compile(
+        loss=tf.keras.losses.MeanSquaredError(),
+        optimizer=tf.keras.optimizers.SGD(1.0),
+        run_eagerly=True,
+    )
+    x_batch = tf.reshape(
+        tf.range(input_dim * batch_size, dtype=tf.float32),
+        [batch_size, input_dim],
+    )
+    y_batch = tf.zeros([batch_size, 1])
+    model.fit(x=x_batch, y=y_batch)
+
+    self.assertAllClose(
+        model.trainable_variables,
+        tf.multiply(
+            tf.ones_like(model.trainable_variables),
+            1.0 - 2.0 * regularizer_multiplier,
+        ),
+    )
+
+  # Simple test to check that custom input regularization does NOT contribute
+  # to the gradient.
+  @parameterized.named_parameters(
+      ('no_registry', None),
+      ('default_registry', layer_registry.make_default_layer_registry()),
+  )
+  def testCustomRegularizationZeroGradient(self, registry):
+    input_dim = 10
+    batch_size = 2
+    inputs = tf.keras.layers.Input((input_dim,))
+    dense_lyr = tf.keras.layers.Dense(
+        1,
+        kernel_initializer='ones',
+        use_bias=False,
+    )
+    # Zero-out outputs to avoid contributions from the main loss function.
+    outputs = tf.multiply(dense_lyr(inputs), 0.0)
+    model = dp_keras_model.DPModel(
+        inputs=inputs,
+        outputs=outputs,
+        l2_norm_clip=1e9,
+        noise_multiplier=0.0,
+        layer_registry=registry,
+    )
+    model.add_loss(tf.reduce_sum(inputs))
+    model.compile(
+        loss=tf.keras.losses.MeanSquaredError(),
+        optimizer=tf.keras.optimizers.SGD(1.0),
+        run_eagerly=True,
+    )
+    x_batch = tf.reshape(
+        tf.range(input_dim * batch_size, dtype=tf.float32),
+        [batch_size, input_dim],
+    )
+    y_batch = tf.zeros([batch_size, 1])
+    model.fit(x=x_batch, y=y_batch)
+
+    self.assertAllClose(
+        model.trainable_variables, tf.ones_like(model.trainable_variables)
+    )
+
+
 if __name__ == '__main__':
   tf.test.main()
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/datasets.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/datasets.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/datasets_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/datasets_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/multinomial_logistic_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/logistic_regression/single_layer_softmax_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/data_structures.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/data_structures.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/dataset_slicing.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/dataset_slicing.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/keras_evaluation.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/keras_evaluation.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/membership_inference_attack.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/membership_inference_attack.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/models.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/models.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/plotting.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/plotting.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/privacy_report.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/privacy_report.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/seq2seq_mia.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/seq2seq_mia.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/membership_inference_attack/tf_estimator_evaluation.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/membership_inference_attack/tf_estimator_evaluation.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_eager_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_eager_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -181,14 +181,15 @@
       super().__init__(*args, **kwargs)
       self.gradient_accumulation_steps = gradient_accumulation_steps
       self._l2_norm_clip = l2_norm_clip
       self._noise_multiplier = noise_multiplier
       self._num_microbatches = num_microbatches
       self._was_dp_gradients_called = False
       self._noise_stddev = None
+      self._acc_iterations = None
       if self._num_microbatches is not None:
         # The loss/gradients is the mean over the microbatches so we
         # divide the noise by num_microbatches too to obtain the correct
         # normalized noise.  If _num_microbatches is not set, the noise stddev
         # will be set later when the loss is given.
         self._noise_stddev = (self._l2_norm_clip * self._noise_multiplier /
                               self._num_microbatches)
@@ -198,31 +199,45 @@
       if self._noise_stddev is None:
         raise ValueError('noise_stddev is not set yet.')
       return tf.random.normal(tf.shape(input=g), stddev=self._noise_stddev)
 
     def _create_slots(self, var_list):
       super()._create_slots(var_list)  # pytype: disable=attribute-error
       if self.gradient_accumulation_steps > 1:
+        # Slots for accumulating gradients.
         for var in var_list:
           self.add_slot(var, 'grad_acc')
+        if self._acc_iterations is None:
+          # Variable for the iterations, used for bookkeeping when to accumulate
+          # and when to update.
+          self._acc_iterations = self.add_weight(
+              'acc_iterations',
+              shape=[],
+              trainable=False,
+              dtype=tf.int64,
+              aggregation=tf.VariableAggregation.ONLY_FIRST_REPLICA,
+          )
 
     def _prepare_local(self, var_device, var_dtype, apply_state):
       super()._prepare_local(var_device, var_dtype, apply_state)  # pytype: disable=attribute-error
       if self.gradient_accumulation_steps > 1:
         apply_update = tf.math.equal(
-            tf.math.floormod(self.iterations + 1,
-                             self.gradient_accumulation_steps), 0)
+            tf.math.floormod(
+                self._acc_iterations + 1, self.gradient_accumulation_steps
+            ),
+            0,
+        )
         grad_scaler = tf.cast(1. / self.gradient_accumulation_steps, var_dtype)
         apply_state[(var_device, var_dtype)].update({
             'apply_update': apply_update,
             'grad_scaler': grad_scaler
         })
 
     def _resource_apply(self, accum_op, grad, var, apply_state=None):
-      """Help method for _resource_apply_dense and _resource_apply_sparse."""
+      """Helper method for _resource_apply_dense and _resource_apply_sparse."""
       if self.gradient_accumulation_steps > 1:
         var_device, var_dtype = var.device, var.dtype.base_dtype
         coefficients = ((apply_state or {}).get((var_device, var_dtype)) or
                         self._fallback_apply_state(var_device, var_dtype))
         grad_acc = self.get_slot(var, 'grad_acc')
 
         def _update_grad():
@@ -231,28 +246,29 @@
               noisy_grad * coefficients['grad_scaler'],
               var, apply_state)  # pytype: disable=attribute-error
           with tf.control_dependencies([apply_grad_op]):
             return grad_acc.assign(
                 tf.zeros_like(grad_acc),
                 use_locking=self._use_locking,
                 read_value=False)
-        accum_op(grad_acc, grad, use_locking=self._use_locking)
-        return tf.cond(
-            coefficients['apply_update'], _update_grad, lambda: tf.no_op())  # pylint: disable=unnecessary-lambda
+        with tf.control_dependencies([accum_op(grad_acc, grad)]):
+          return tf.cond(coefficients['apply_update'], _update_grad, tf.no_op)
       else:
         grad = tf.convert_to_tensor(grad)
         grad = grad + self._generate_noise(grad)
         return super()._resource_apply_dense(
             grad, var, apply_state)  # pytype: disable=attribute-error
 
     def _resource_apply_dense(self, grad, var, apply_state=None):
       """Handles dense gradients."""
-      def _accum_op(grad_acc, grad, use_locking):
+      def _accum_op(grad_acc, grad):
         return grad_acc.assign_add(
-            grad, use_locking=use_locking, read_value=False)
+            grad, use_locking=self._use_locking, read_value=False
+        )
+
       return self._resource_apply(_accum_op, grad, var, apply_state)
 
     # This method is implemented the same as that in optimizer_v2.py. We
     # redefine it here because it gets overridden by the SGD optimizer (and
     # potentially other optimizers too). If we omit it, it would cause an error
     # if the parent optimizer is the SGD optimizer.
     def _resource_apply_sparse_duplicate_indices(
@@ -267,21 +283,57 @@
       summed_grad, unique_indices = _deduplicate_indexed_slices(
           values=grad, indices=indices)
       return self._resource_apply_sparse(
           summed_grad, var, unique_indices, **kwargs)  # pytype: disable=attribute-error
 
     def _resource_apply_sparse(self, grad, var, indices, apply_state=None):
       """Handles deduped sparse gradients."""
-      def _accum_op(grad_acc, sparse_delta, use_locking):
+      def _accum_op(grad_acc, sparse_delta):
         return grad_acc.scatter_add(
-            sparse_delta=sparse_delta, use_locking=use_locking)
+            sparse_delta=sparse_delta, use_locking=self._use_locking
+        )
+
       sparse_delta = tf.IndexedSlices(
           values=grad, indices=indices, dense_shape=var.shape)
       return self._resource_apply(_accum_op, sparse_delta, var, apply_state)
 
+    def _distributed_apply(
+        self, distribution, grads_and_vars, apply_state, name
+    ):
+      apply_op = super()._distributed_apply(
+          distribution, grads_and_vars, apply_state, name
+      )
+      if self.gradient_accumulation_steps > 1:
+        # The original _distributed_apply increments self.iterations after each
+        # call. But we want to increment it only after each logical batch is
+        # processed, so optimizers that explicitly use self.iterations in their
+        # updates (such as Adam) can use the correct value.
+        def increment_acc_iterations():
+          # Always use locking when updating the steps, so we don't under-count
+          # the steps (which could invalidate privacy accounting).
+          return self._acc_iterations.assign_add(
+              1, use_locking=True, read_value=False
+          )
+
+        def assign_iterations():
+          return self.iterations.assign(
+              tf.math.floordiv(
+                  self._acc_iterations, self.gradient_accumulation_steps
+              ),
+              use_locking=True,
+              read_value=False,
+          )
+
+        with tf.control_dependencies([apply_op]):
+          with tf.control_dependencies([increment_acc_iterations()]):
+            return assign_iterations()
+      else:
+        # No accumulation.
+        return apply_op
+
     def _compute_gradients(self, loss, var_list, grad_loss=None, tape=None):
       """DP-SGD version of base class method."""
       self._was_dp_gradients_called = True
 
       # Computes loss.
       if not callable(loss) and tape is None:
         raise ValueError('`tape` is required when a `Tensor` loss is passed.')
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,29 +334,33 @@
     self.assertAllCloseAccordingToType([[1.0, 2.0]], var0)
     self.assertAllCloseAccordingToType([3.0], var1)
 
     opt.minimize(loss1, [var0, var1])
     # After first call to optimizer values didn't change
     self.assertAllCloseAccordingToType([[1.0, 2.0]], var0)
     self.assertAllCloseAccordingToType([3.0], var1)
+    self.assertEqual(opt.iterations, 0)
 
     opt.minimize(loss2, [var0, var1])
     # After second call to optimizer updates were applied
     self.assertAllCloseAccordingToType([[-1.0, 1.0]], var0)
     self.assertAllCloseAccordingToType([2.0], var1)
+    self.assertEqual(opt.iterations, 1)
 
     opt.minimize(loss2, [var0, var1])
     # After third call to optimizer values didn't change
     self.assertAllCloseAccordingToType([[-1.0, 1.0]], var0)
     self.assertAllCloseAccordingToType([2.0], var1)
+    self.assertEqual(opt.iterations, 1)
 
     opt.minimize(loss2, [var0, var1])
     # After fourth call to optimizer updates were applied again
     self.assertAllCloseAccordingToType([[-4.0, -0.5]], var0)
     self.assertAllCloseAccordingToType([1.0], var1)
+    self.assertEqual(opt.iterations, 2)
 
   @parameterized.named_parameters(
       ('DPSparseKerasSGDOptimizer 1',
        dp_optimizer.DPSparseKerasSGDOptimizer, 1),
       ('DPSparseKerasSGDOptimizer 2',
        dp_optimizer.DPSparseKerasSGDOptimizer, 2),
       ('DPSparseKerasSGDOptimizer 4',
@@ -384,14 +388,15 @@
     for _ in range(gradient_accumulation_steps):
       self.assertAllCloseAccordingToType([[1.0, 2.0]], var0)
       self.assertAllCloseAccordingToType([3.0], var1)
       opt.minimize(loss, [var0, var1])
 
     self.assertNotAllClose([[1.0, 2.0]], var0)
     self.assertNotAllClose([3.0], var1)
+    self.assertEqual(opt.iterations, 1)
 
   def testKerasModelBaselineSaving(self):
     """Tests that DP optimizers work with tf.keras.Model."""
 
     model = tf.keras.models.Sequential(layers=[
         tf.keras.layers.Dense(
             1,
@@ -451,43 +456,51 @@
     model.predict(train_data, batch_size=8)
     tempdir = self.create_tempdir()
     model.save(tempdir, save_format='tf')
     model.load_weights(tempdir)
 
     model.fit(train_data, train_labels, batch_size=8, epochs=1, shuffle=False)
 
-  @parameterized.named_parameters(('1', 1), ('None', None))
-  def testKerasModelBaselineNoNoise(self, num_microbatches):
+  @parameterized.named_parameters(
+      ('no_microbatch_no_accumulation', False, False),
+      ('no_microbatch_accumulation', False, True),
+      ('microbatch_no_accumulation', True, False),
+      ('microbatch_accumulation', True, True),
+  )
+  def testKerasModelBaselineNoNoise(self, microbatch, accumulate):
     """Tests that DP optimizers work with tf.keras.Model."""
-
+    acc_steps = 2 if accumulate else 1
     model = tf.keras.models.Sequential(layers=[
         tf.keras.layers.Dense(
             1,
             activation='linear',
             name='dense',
             kernel_initializer='zeros',
             bias_initializer='zeros')
     ])
 
     optimizer = dp_optimizer.DPSparseKerasSGDOptimizer(
         l2_norm_clip=100.0,
         noise_multiplier=0.0,
-        num_microbatches=num_microbatches,
-        learning_rate=0.05)
+        num_microbatches=None if microbatch else 1,
+        learning_rate=0.05,
+        gradient_accumulation_steps=acc_steps,
+    )
     loss = tf.keras.losses.MeanSquaredError(reduction='none')
     model.compile(optimizer, loss)
 
     true_weights = np.array([[-5], [4], [3], [2]]).astype(np.float32)
     true_bias = np.array([6.0]).astype(np.float32)
-    train_data = np.random.normal(scale=3.0, size=(1000, 4)).astype(np.float32)
-    train_labels = np.matmul(train_data,
-                             true_weights) + true_bias + np.random.normal(
-                                 scale=0.0, size=(1000, 1)).astype(np.float32)
+    train_data = np.random.normal(scale=3.0, size=(2000, 4)).astype(np.float32)
+    train_labels = np.matmul(train_data, true_weights) + true_bias
 
-    model.fit(train_data, train_labels, batch_size=8, epochs=1, shuffle=False)
+    model.fit(train_data, train_labels, batch_size=10, epochs=1, shuffle=False)
 
     self.assertAllClose(model.get_weights()[0], true_weights, atol=0.05)
     self.assertAllClose(model.get_weights()[1], true_bias, atol=0.05)
+    # Check that the optimizer's iterations equal the number of logical batches.
+    total_batches = 200
+    self.assertEqual(optimizer.iterations.numpy(), total_batches / acc_steps)
 
 
 if __name__ == '__main__':
   tf.test.main()
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_vectorized.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,259 +1,201 @@
-# Copyright 2020 The TensorFlow Authors. All Rights Reserved.
+# Copyright 2020, The TensorFlow Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
-"""Differentially private version of Keras optimizer v2."""
+"""Vectorized differentially private optimizers for TensorFlow."""
 
+from absl import logging
 import tensorflow as tf
 
-from tensorflow_privacy.privacy.dp_query import gaussian_query
+AdagradOptimizer = tf.compat.v1.train.AdagradOptimizer
+AdamOptimizer = tf.compat.v1.train.AdamOptimizer
+GradientDescentOptimizer = tf.compat.v1.train.GradientDescentOptimizer
+parent_code = tf.compat.v1.train.Optimizer.compute_gradients.__code__
+GATE_OP = tf.compat.v1.train.Optimizer.GATE_OP  # pylint: disable=invalid-name
 
 
-def clip_gradients_vmap(g, l2_norm_clip):
-  """Clips gradients in a way that is compatible with vectorized_map."""
-  grads_flat = tf.nest.flatten(g)
-  squared_l2_norms = [
-      tf.reduce_sum(input_tensor=tf.square(g)) for g in grads_flat
-  ]
-  global_norm = tf.sqrt(tf.add_n(squared_l2_norms))
-  div = tf.maximum(global_norm / l2_norm_clip, 1.)
-  clipped_flat = [g / div for g in grads_flat]
-  clipped_grads = tf.nest.pack_sequence_as(g, clipped_flat)
-  return clipped_grads
-
-
-def make_vectorized_keras_optimizer_class(cls):
-  """Given a subclass of `tf.keras.optimizers.Optimizer`, returns a vectorized DP-SGD subclass of it.
+def make_vectorized_optimizer_class(cls):
+  """Given a subclass of `tf.compat.v1.train.Optimizer`, returns a vectorized DP-SGD subclass of it.
 
   Args:
     cls: Class from which to derive a DP subclass. Should be a subclass of
-      `tf.keras.optimizers.Optimizer`.
+      `tf.compat.v1.train.Optimizer`.
 
   Returns:
-    A vectorized DP-SGD subclass of `cls`.
+    A DP-SGD subclass of `cls`.
   """
+  child_code = cls.compute_gradients.__code__
+  if child_code is not parent_code:
+    logging.warning(
+        'WARNING: Calling make_optimizer_class() on class %s that overrides '
+        'method compute_gradients(). Check to ensure that '
+        'make_optimizer_class() does not interfere with overridden version.',
+        cls.__name__)
 
   class DPOptimizerClass(cls):  # pylint: disable=empty-docstring
-    __doc__ = """Vectorized differentially private subclass of given class
-    `{base_class}`.
+    __doc__ = ("""Vectorized DP subclass of `{base_class}` using Gaussian
+       averaging.
 
-    You can use this as a differentially private replacement for
-    `{base_class}`. This optimizer implements DP-SGD using
-    the standard Gaussian mechanism. It differs from `{dp_keras_class}` in that
-    it attempts to vectorize the gradient computation and clipping of
-    microbatches.
-
-    When instantiating this optimizer, you need to supply several
-    DP-related arguments followed by the standard arguments for
-    `{short_base_class}`.
-
-    Examples:
-
-    ```python
-    # Create optimizer.
-    opt = {dp_vectorized_keras_class}(l2_norm_clip=1.0, noise_multiplier=0.5, num_microbatches=1,
-            <standard arguments>)
-    ```
-
-    When using the optimizer, be sure to pass in the loss as a
-    rank-one tensor with one entry for each example.
-
-    The optimizer can be used directly via its `minimize` method, or
-    through a Keras `Model`.
-
-    ```python
-    # Compute loss as a tensor by using tf.losses.Reduction.NONE.
-    # Compute vector of per-example loss rather than its mean over a minibatch.
-    # (Side note: Always verify that the output shape when using
-    # tf.losses.Reduction.NONE-- it can sometimes be surprising.
-    loss = tf.keras.losses.CategoricalCrossentropy(
-        from_logits=True, reduction=tf.losses.Reduction.NONE)
-
-    # Use optimizer in a Keras model.
-    opt.minimize(loss, var_list=[var])
-    ```
-
-    ```python
-    # Compute loss as a tensor by using tf.losses.Reduction.NONE.
-    # Compute vector of per-example loss rather than its mean over a minibatch.
-    loss = tf.keras.losses.CategoricalCrossentropy(
-        from_logits=True, reduction=tf.losses.Reduction.NONE)
-
-    # Use optimizer in a Keras model.
-    model = tf.keras.Sequential(...)
-    model.compile(optimizer=opt, loss=loss, metrics=['accuracy'])
-    model.fit(...)
-    ```
-
-    """.format(
-        base_class='tf.keras.optimizers.' + cls.__name__,
-        dp_keras_class='DPKeras' + cls.__name__,
-        short_base_class=cls.__name__,
-        dp_vectorized_keras_class='VectorizedDPKeras' + cls.__name__)
+       You can use this as a differentially private replacement for
+       `{base_class}`. This optimizer implements DP-SGD using
+       the standard Gaussian mechanism. It differs from `{dp_class}` in that
+       it attempts to vectorize the gradient computation and clipping of
+       microbatches.
+
+       When instantiating this optimizer, you need to supply several
+       DP-related arguments followed by the standard arguments for
+       `{short_base_class}`.
+
+       Examples:
+
+       ```python
+       # Create optimizer.
+       opt = {dp_vectorized_class}(l2_norm_clip=1.0, noise_multiplier=0.5, num_microbatches=1,
+                <standard arguments>)
+       ```
+
+       When using the optimizer, be sure to pass in the loss as a
+       rank-one tensor with one entry for each example.
+
+       ```python
+       # Compute loss as a tensor. Do not call tf.reduce_mean as you
+       # would with a standard optimizer.
+       loss = tf.nn.sparse_softmax_cross_entropy_with_logits(
+           labels=labels, logits=logits)
+
+       train_op = opt.minimize(loss, global_step=global_step)
+       ```
+       """).format(
+           base_class='tf.compat.v1.train.' + cls.__name__,
+           dp_class='DP' +
+           cls.__name__.replace('Optimizer', 'GaussianOptimizer'),
+           short_base_class=cls.__name__,
+           dp_vectorized_class='VectorizedDP' + cls.__name__)
 
     def __init__(
         self,
         l2_norm_clip,
         noise_multiplier,
         num_microbatches=None,
-        unconnected_gradients_to_zero=False,
         *args,  # pylint: disable=keyword-arg-before-vararg, g-doc-args
         **kwargs):
       """Initialize the DPOptimizerClass.
 
       Args:
         l2_norm_clip: Clipping norm (max L2 norm of per microbatch gradients).
         noise_multiplier: Ratio of the standard deviation to the clipping norm.
         num_microbatches: Number of microbatches into which each minibatch is
-          split.
-        unconnected_gradients_to_zero: The Jacobian is used to compute the
-          microbatch losses. If a node in the graph is deliberately not
-          connected, then the Jacobian computation will return a `None` for that
-          node. Set this flag to True to treat these Jacobians as zero.
+          split. If `None`, will default to the size of the minibatch, and
+          per-example gradients will be computed.
         *args: These will be passed on to the base class `__init__` method.
         **kwargs: These will be passed on to the base class `__init__` method.
       """
       super().__init__(*args, **kwargs)
       self._l2_norm_clip = l2_norm_clip
       self._noise_multiplier = noise_multiplier
       self._num_microbatches = num_microbatches
-      self._unconnected_gradients_to_zero = unconnected_gradients_to_zero
-      self._dp_sum_query = gaussian_query.GaussianSumQuery(
-          l2_norm_clip, l2_norm_clip * noise_multiplier)
-      self._global_state = None
-      self._was_dp_gradients_called = False
+      self._was_compute_gradients_called = False
 
-    def _compute_gradients(self, loss, var_list, grad_loss=None, tape=None):
+    def compute_gradients(self,
+                          loss,
+                          var_list,
+                          gate_gradients=GATE_OP,
+                          aggregation_method=None,
+                          colocate_gradients_with_ops=False,
+                          grad_loss=None,
+                          gradient_tape=None):
       """DP-SGD version of base class method."""
-
-      self._was_dp_gradients_called = True
-      # Compute loss.
-      if not callable(loss) and tape is None:
-        raise ValueError('`tape` is required when a `Tensor` loss is passed.')
-      tape = tape if tape is not None else tf.GradientTape()
-
+      self._was_compute_gradients_called = True
       if callable(loss):
-        with tape:
-          if not callable(var_list):
-            tape.watch(var_list)
-
-          loss = loss()
-          if self._num_microbatches is None:
-            num_microbatches = tf.shape(input=loss)[0]
-          else:
-            num_microbatches = self._num_microbatches
-          microbatch_losses = tf.reduce_mean(
-              tf.reshape(loss, [num_microbatches, -1]), axis=1)
-
-          if callable(var_list):
-            var_list = var_list()
+        # TF is running in Eager mode
+        raise NotImplementedError('Vectorized optimizer unavailable for TF2.')
       else:
-        with tape:
-          if self._num_microbatches is None:
-            num_microbatches = tf.shape(input=loss)[0]
-          else:
-            num_microbatches = self._num_microbatches
-          microbatch_losses = tf.reduce_mean(
-              tf.reshape(loss, [num_microbatches, -1]), axis=1)
-
-      var_list = tf.nest.flatten(var_list)
-
-      # Compute the per-microbatch losses using helpful jacobian method.
-      with tf.keras.backend.name_scope(self._name + '/gradients'):
-        jacobian = tape.jacobian(
-            microbatch_losses,
-            var_list,
-            unconnected_gradients=(tf.UnconnectedGradients.ZERO
-                                   if self._unconnected_gradients_to_zero else
-                                   tf.UnconnectedGradients.NONE))
-
-        clipped_gradients = tf.vectorized_map(
-            lambda g: clip_gradients_vmap(g, self._l2_norm_clip), jacobian)
-
-        def reduce_noise_normalize_batch(g):
-          # Sum gradients over all microbatches.
-          summed_gradient = tf.reduce_sum(g, axis=0)
+        # TF is running in graph mode, check we did not receive a gradient tape.
+        if gradient_tape:
+          raise ValueError('When in graph mode, a tape should not be passed.')
+
+        batch_size = tf.shape(input=loss)[0]
+        if self._num_microbatches is None:
+          self._num_microbatches = batch_size
+
+        # Note: it would be closer to the correct i.i.d. sampling of records if
+        # we sampled each microbatch from the appropriate binomial distribution,
+        # although that still wouldn't be quite correct because it would be
+        # sampling from the dataset without replacement.
+        microbatch_losses = tf.reshape(loss, [self._num_microbatches, -1])
+
+        if var_list is None:
+          var_list = (
+              tf.compat.v1.trainable_variables() + tf.compat.v1.get_collection(
+                  tf.compat.v1.GraphKeys.TRAINABLE_RESOURCE_VARIABLES))
+
+        def process_microbatch(microbatch_loss):
+          """Compute clipped grads for one microbatch."""
+          microbatch_loss = tf.reduce_mean(input_tensor=microbatch_loss)
+          grads, _ = zip(*super(DPOptimizerClass, self).compute_gradients(
+              microbatch_loss, var_list, gate_gradients, aggregation_method,
+              colocate_gradients_with_ops, grad_loss))
+          grads_list = [
+              g if g is not None else tf.zeros_like(v)
+              for (g, v) in zip(list(grads), var_list)
+          ]
+          # Clip gradients to have L2 norm of l2_norm_clip.
+          # Here, we use TF primitives rather than the built-in
+          # tf.clip_by_global_norm() so that operations can be vectorized
+          # across microbatches.
+          grads_flat = tf.nest.flatten(grads_list)
+          squared_l2_norms = [
+              tf.reduce_sum(input_tensor=tf.square(g)) for g in grads_flat
+          ]
+          global_norm = tf.sqrt(tf.add_n(squared_l2_norms))
+          div = tf.maximum(global_norm / self._l2_norm_clip, 1.)
+          clipped_flat = [g / div for g in grads_flat]
+          clipped_grads = tf.nest.pack_sequence_as(grads_list, clipped_flat)
+          return clipped_grads
+
+        clipped_grads = tf.vectorized_map(process_microbatch, microbatch_losses)
 
-          # Add noise to summed gradients.
+        def reduce_noise_normalize_batch(stacked_grads):
+          summed_grads = tf.reduce_sum(input_tensor=stacked_grads, axis=0)
           noise_stddev = self._l2_norm_clip * self._noise_multiplier
           noise = tf.random.normal(
-              tf.shape(input=summed_gradient), stddev=noise_stddev)
-          noised_gradient = tf.add(summed_gradient, noise)
-
-          # Normalize by number of microbatches and return.
-          return tf.truediv(noised_gradient,
-                            tf.cast(num_microbatches, tf.float32))
-
-        final_gradients = tf.nest.map_structure(reduce_noise_normalize_batch,
-                                                clipped_gradients)
-
-      return list(zip(final_gradients, var_list))
-
-    def get_gradients(self, loss, params):
-      """DP-SGD version of base class method."""
-
-      self._was_dp_gradients_called = True
-      if self._global_state is None:
-        self._global_state = self._dp_sum_query.initial_global_state()
-
-      if self._num_microbatches is None:
-        num_microbatches = tf.shape(input=loss)[0]
-      else:
-        num_microbatches = self._num_microbatches
+              tf.shape(input=summed_grads), stddev=noise_stddev)
+          noised_grads = summed_grads + noise
+          return noised_grads / tf.cast(self._num_microbatches, tf.float32)
 
-      microbatch_losses = tf.reshape(loss, [num_microbatches, -1])
+        final_grads = tf.nest.map_structure(reduce_noise_normalize_batch,
+                                            clipped_grads)
 
-      def process_microbatch(microbatch_loss):
-        """Compute clipped grads for one microbatch."""
-        mean_loss = tf.reduce_mean(input_tensor=microbatch_loss)
-        grads = cls.get_gradients(self, mean_loss, params)
-        grads_list = [
-            g if g is not None else tf.zeros_like(v)
-            for (g, v) in zip(list(grads), params)
-        ]
-        clipped_grads = clip_gradients_vmap(grads_list, self._l2_norm_clip)
-        return clipped_grads
-
-      clipped_grads = tf.vectorized_map(process_microbatch, microbatch_losses)
-
-      def reduce_noise_normalize_batch(stacked_grads):
-        summed_grads = tf.reduce_sum(input_tensor=stacked_grads, axis=0)
-        noise_stddev = self._l2_norm_clip * self._noise_multiplier
-        noise = tf.random.normal(
-            tf.shape(input=summed_grads), stddev=noise_stddev)
-        noised_grads = summed_grads + noise
-        return noised_grads / tf.cast(num_microbatches, tf.float32)
-
-      final_grads = tf.nest.map_structure(reduce_noise_normalize_batch,
-                                          clipped_grads)
-      return final_grads
+        return list(zip(final_grads, var_list))
 
-    def apply_gradients(self, *args, **kwargs):
+    def apply_gradients(self, grads_and_vars, global_step=None, name=None):
+      # pylint: disable=g-doc-args, g-doc-return-or-yield
       """DP-SGD version of base class method."""
-      assert self._was_dp_gradients_called, (
-          'Neither _compute_gradients() or get_gradients() on the '
-          'differentially private optimizer was called. This means the '
-          'training is not differentially private. It may be the case that '
-          'you need to upgrade to TF 2.4 or higher to use this particular '
-          'optimizer.')
-      return super(DPOptimizerClass, self).apply_gradients(*args, **kwargs)
+      assert self._was_compute_gradients_called, (
+          'compute_gradients() on the differentially private optimizer was not'
+          ' called. Which means that the training is not differentially '
+          'private. It happens for example in Keras training in TensorFlow '
+          '2.0+.')
+      return super(DPOptimizerClass, self).apply_gradients(
+          grads_and_vars=grads_and_vars, global_step=global_step, name=name)
 
   return DPOptimizerClass
 
 
-VectorizedDPKerasAdagradOptimizer = make_vectorized_keras_optimizer_class(
-    tf.keras.optimizers.legacy.Adagrad)
-VectorizedDPKerasAdamOptimizer = make_vectorized_keras_optimizer_class(
-    tf.keras.optimizers.legacy.Adam)
-VectorizedDPKerasSGDOptimizer = make_vectorized_keras_optimizer_class(
-    tf.keras.optimizers.legacy.SGD)
+VectorizedDPAdagradOptimizer = make_vectorized_optimizer_class(AdagradOptimizer)
+VectorizedDPAdamOptimizer = make_vectorized_optimizer_class(AdamOptimizer)
+VectorizedDPSGDOptimizer = make_vectorized_optimizer_class(
+    GradientDescentOptimizer)
+
+VectorizedDPAdagrad = VectorizedDPAdagradOptimizer
+VectorizedDPAdam = VectorizedDPAdamOptimizer
+VectorizedDPSGD = VectorizedDPSGDOptimizer
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,201 +1,227 @@
-# Copyright 2020, The TensorFlow Authors.
+# Copyright 2019, The TensorFlow Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Vectorized differentially private optimizers for TensorFlow."""
 
-from absl import logging
+import unittest
+
+from absl.testing import parameterized
+import numpy as np
 import tensorflow as tf
+from tensorflow import estimator as tf_estimator
+from tensorflow.compat.v1 import estimator as tf_compat_v1_estimator
+from tensorflow_privacy.privacy.optimizers import dp_optimizer_vectorized
+from tensorflow_privacy.privacy.optimizers.dp_optimizer_vectorized import VectorizedDPAdagrad
+from tensorflow_privacy.privacy.optimizers.dp_optimizer_vectorized import VectorizedDPAdam
+from tensorflow_privacy.privacy.optimizers.dp_optimizer_vectorized import VectorizedDPSGD
+
+
+class DPOptimizerTest(tf.test.TestCase, parameterized.TestCase):
+
+  @classmethod
+  def setUpClass(cls):
+    super(DPOptimizerTest, cls).setUpClass()
+    tf.compat.v1.disable_eager_execution()
+
+  def _loss(self, val0, val1):
+    """Loss function that is minimized at the mean of the input points."""
+    return 0.5 * tf.reduce_sum(
+        input_tensor=tf.math.squared_difference(val0, val1), axis=1)
+
+  # Parameters for testing: optimizer, num_microbatches, expected answer.
+  @parameterized.named_parameters(
+      ('DPGradientDescent 1', VectorizedDPSGD, 1, [-2.5, -2.5]),
+      ('DPGradientDescent 2', VectorizedDPSGD, 2, [-2.5, -2.5]),
+      ('DPGradientDescent 4', VectorizedDPSGD, 4, [-2.5, -2.5]),
+      ('DPAdagrad 1', VectorizedDPAdagrad, 1, [-2.5, -2.5]),
+      ('DPAdagrad 2', VectorizedDPAdagrad, 2, [-2.5, -2.5]),
+      ('DPAdagrad 4', VectorizedDPAdagrad, 4, [-2.5, -2.5]),
+      ('DPAdam 1', VectorizedDPAdam, 1, [-2.5, -2.5]),
+      ('DPAdam 2', VectorizedDPAdam, 2, [-2.5, -2.5]),
+      ('DPAdam 4', VectorizedDPAdam, 4, [-2.5, -2.5]))
+  def testBaseline(self, cls, num_microbatches, expected_answer):
+    with self.cached_session() as sess:
+      var0 = tf.Variable([1.0, 2.0])
+      data0 = tf.Variable([[3.0, 4.0], [5.0, 6.0], [7.0, 8.0], [-1.0, 0.0]])
+
+      opt = cls(
+          l2_norm_clip=1.0e9,
+          noise_multiplier=0.0,
+          num_microbatches=num_microbatches,
+          learning_rate=2.0)
+
+      self.evaluate(tf.compat.v1.global_variables_initializer())
+      # Fetch params to validate initial values
+      self.assertAllClose([1.0, 2.0], self.evaluate(var0))
+
+      # Expected gradient is sum of differences divided by number of
+      # microbatches.
+      gradient_op = opt.compute_gradients(self._loss(data0, var0), [var0])
+      grads_and_vars = sess.run(gradient_op)
+      self.assertAllCloseAccordingToType(expected_answer, grads_and_vars[0][0])
+
+  @parameterized.named_parameters(('DPGradientDescent', VectorizedDPSGD),
+                                  ('DPAdagrad', VectorizedDPAdagrad),
+                                  ('DPAdam', VectorizedDPAdam))
+  def testClippingNorm(self, cls):
+    with self.cached_session() as sess:
+      var0 = tf.Variable([0.0, 0.0])
+      data0 = tf.Variable([[3.0, 4.0], [6.0, 8.0]])
+
+      opt = cls(
+          l2_norm_clip=1.0,
+          noise_multiplier=0.,
+          num_microbatches=1,
+          learning_rate=2.0)
+
+      self.evaluate(tf.compat.v1.global_variables_initializer())
+      # Fetch params to validate initial values
+      self.assertAllClose([0.0, 0.0], self.evaluate(var0))
+
+      # Expected gradient is sum of differences.
+      gradient_op = opt.compute_gradients(self._loss(data0, var0), [var0])
+      grads_and_vars = sess.run(gradient_op)
+      self.assertAllCloseAccordingToType([-0.6, -0.8], grads_and_vars[0][0])
+
+  @parameterized.named_parameters(('DPGradientDescent', VectorizedDPSGD),
+                                  ('DPAdagrad', VectorizedDPAdagrad),
+                                  ('DPAdam', VectorizedDPAdam))
+  def testNoiseMultiplier(self, cls):
+    with self.cached_session() as sess:
+      var0 = tf.Variable([0.0])
+      data0 = tf.Variable([[0.0]])
+
+      opt = cls(
+          l2_norm_clip=4.0,
+          noise_multiplier=8.0,
+          num_microbatches=1,
+          learning_rate=2.0)
+
+      self.evaluate(tf.compat.v1.global_variables_initializer())
+      # Fetch params to validate initial values
+      self.assertAllClose([0.0], self.evaluate(var0))
+
+      gradient_op = opt.compute_gradients(self._loss(data0, var0), [var0])
+      grads = []
+      for _ in range(5000):
+        grads_and_vars = sess.run(gradient_op)
+        grads.append(grads_and_vars[0][0])
+
+      # Test standard deviation is close to l2_norm_clip * noise_multiplier.
+      self.assertNear(np.std(grads), 4.0 * 8.0, 0.5)
+
+  @unittest.mock.patch('absl.logging.warning')
+  def testComputeGradientsOverrideWarning(self, mock_logging):
+
+    class SimpleOptimizer(tf.compat.v1.train.Optimizer):
+
+      def compute_gradients(self):
+        return 0
 
-AdagradOptimizer = tf.compat.v1.train.AdagradOptimizer
-AdamOptimizer = tf.compat.v1.train.AdamOptimizer
-GradientDescentOptimizer = tf.compat.v1.train.GradientDescentOptimizer
-parent_code = tf.compat.v1.train.Optimizer.compute_gradients.__code__
-GATE_OP = tf.compat.v1.train.Optimizer.GATE_OP  # pylint: disable=invalid-name
-
-
-def make_vectorized_optimizer_class(cls):
-  """Given a subclass of `tf.compat.v1.train.Optimizer`, returns a vectorized DP-SGD subclass of it.
-
-  Args:
-    cls: Class from which to derive a DP subclass. Should be a subclass of
-      `tf.compat.v1.train.Optimizer`.
-
-  Returns:
-    A DP-SGD subclass of `cls`.
-  """
-  child_code = cls.compute_gradients.__code__
-  if child_code is not parent_code:
-    logging.warning(
+    dp_optimizer_vectorized.make_vectorized_optimizer_class(SimpleOptimizer)
+    mock_logging.assert_called_once_with(
         'WARNING: Calling make_optimizer_class() on class %s that overrides '
         'method compute_gradients(). Check to ensure that '
         'make_optimizer_class() does not interfere with overridden version.',
-        cls.__name__)
+        'SimpleOptimizer')
+
+  def testEstimator(self):
+    """Tests that DP optimizers work with tf.estimator."""
+
+    def linear_model_fn(features, labels, mode):
+      preds = tf.keras.layers.Dense(
+          1, activation='linear', name='dense')(
+              features['x'])
+
+      vector_loss = tf.math.squared_difference(labels, preds)
+      scalar_loss = tf.reduce_mean(input_tensor=vector_loss)
+      optimizer = VectorizedDPSGD(
+          l2_norm_clip=1.0,
+          noise_multiplier=0.,
+          num_microbatches=1,
+          learning_rate=1.0)
+      global_step = tf.compat.v1.train.get_global_step()
+      train_op = optimizer.minimize(loss=vector_loss, global_step=global_step)
+      return tf_estimator.EstimatorSpec(
+          mode=mode, loss=scalar_loss, train_op=train_op)
+
+    linear_regressor = tf_estimator.Estimator(model_fn=linear_model_fn)
+    true_weights = np.array([[-5], [4], [3], [2]]).astype(np.float32)
+    true_bias = 6.0
+    train_data = np.random.normal(scale=3.0, size=(200, 4)).astype(np.float32)
+
+    train_labels = np.matmul(train_data,
+                             true_weights) + true_bias + np.random.normal(
+                                 scale=0.1, size=(200, 1)).astype(np.float32)
+
+    train_input_fn = tf_compat_v1_estimator.inputs.numpy_input_fn(
+        x={'x': train_data},
+        y=train_labels,
+        batch_size=20,
+        num_epochs=10,
+        shuffle=True)
+    linear_regressor.train(input_fn=train_input_fn, steps=100)
+    self.assertAllClose(
+        linear_regressor.get_variable_value('dense/kernel'),
+        true_weights,
+        atol=1.0)
+
+  @parameterized.named_parameters(('DPGradientDescent', VectorizedDPSGD),
+                                  ('DPAdagrad', VectorizedDPAdagrad),
+                                  ('DPAdam', VectorizedDPAdam))
+  def testDPGaussianOptimizerClass(self, cls):
+    with self.cached_session() as sess:
+      var0 = tf.Variable([0.0])
+      data0 = tf.Variable([[0.0]])
+
+      opt = cls(
+          l2_norm_clip=4.0,
+          noise_multiplier=2.0,
+          num_microbatches=1,
+          learning_rate=2.0)
+
+      self.evaluate(tf.compat.v1.global_variables_initializer())
+      # Fetch params to validate initial values
+      self.assertAllClose([0.0], self.evaluate(var0))
+
+      gradient_op = opt.compute_gradients(self._loss(data0, var0), [var0])
+      grads = []
+      for _ in range(1000):
+        grads_and_vars = sess.run(gradient_op)
+        grads.append(grads_and_vars[0][0])
+
+      # Test standard deviation is close to l2_norm_clip * noise_multiplier.
+      self.assertNear(np.std(grads), 2.0 * 4.0, 0.5)
+
+  @parameterized.named_parameters(('DPGradientDescent', VectorizedDPSGD),
+                                  ('DPAdagrad', VectorizedDPAdagrad),
+                                  ('DPAdam', VectorizedDPAdam))
+  def testAssertOnNoCallOfComputeGradients(self, cls):
+    opt = cls(
+        l2_norm_clip=4.0,
+        noise_multiplier=2.0,
+        num_microbatches=1,
+        learning_rate=2.0)
+
+    with self.assertRaises(AssertionError):
+      grads_and_vars = tf.Variable([0.0])
+      opt.apply_gradients(grads_and_vars)
+
+    # Expect no call exception if compute_gradients is called.
+    var0 = tf.Variable([0.0])
+    data0 = tf.Variable([[0.0]])
+    grads_and_vars = opt.compute_gradients(self._loss(data0, var0), [var0])
+    opt.apply_gradients(grads_and_vars)
+
 
-  class DPOptimizerClass(cls):  # pylint: disable=empty-docstring
-    __doc__ = ("""Vectorized DP subclass of `{base_class}` using Gaussian
-       averaging.
-
-       You can use this as a differentially private replacement for
-       `{base_class}`. This optimizer implements DP-SGD using
-       the standard Gaussian mechanism. It differs from `{dp_class}` in that
-       it attempts to vectorize the gradient computation and clipping of
-       microbatches.
-
-       When instantiating this optimizer, you need to supply several
-       DP-related arguments followed by the standard arguments for
-       `{short_base_class}`.
-
-       Examples:
-
-       ```python
-       # Create optimizer.
-       opt = {dp_vectorized_class}(l2_norm_clip=1.0, noise_multiplier=0.5, num_microbatches=1,
-                <standard arguments>)
-       ```
-
-       When using the optimizer, be sure to pass in the loss as a
-       rank-one tensor with one entry for each example.
-
-       ```python
-       # Compute loss as a tensor. Do not call tf.reduce_mean as you
-       # would with a standard optimizer.
-       loss = tf.nn.sparse_softmax_cross_entropy_with_logits(
-           labels=labels, logits=logits)
-
-       train_op = opt.minimize(loss, global_step=global_step)
-       ```
-       """).format(
-           base_class='tf.compat.v1.train.' + cls.__name__,
-           dp_class='DP' +
-           cls.__name__.replace('Optimizer', 'GaussianOptimizer'),
-           short_base_class=cls.__name__,
-           dp_vectorized_class='VectorizedDP' + cls.__name__)
-
-    def __init__(
-        self,
-        l2_norm_clip,
-        noise_multiplier,
-        num_microbatches=None,
-        *args,  # pylint: disable=keyword-arg-before-vararg, g-doc-args
-        **kwargs):
-      """Initialize the DPOptimizerClass.
-
-      Args:
-        l2_norm_clip: Clipping norm (max L2 norm of per microbatch gradients).
-        noise_multiplier: Ratio of the standard deviation to the clipping norm.
-        num_microbatches: Number of microbatches into which each minibatch is
-          split. If `None`, will default to the size of the minibatch, and
-          per-example gradients will be computed.
-        *args: These will be passed on to the base class `__init__` method.
-        **kwargs: These will be passed on to the base class `__init__` method.
-      """
-      super().__init__(*args, **kwargs)
-      self._l2_norm_clip = l2_norm_clip
-      self._noise_multiplier = noise_multiplier
-      self._num_microbatches = num_microbatches
-      self._was_compute_gradients_called = False
-
-    def compute_gradients(self,
-                          loss,
-                          var_list,
-                          gate_gradients=GATE_OP,
-                          aggregation_method=None,
-                          colocate_gradients_with_ops=False,
-                          grad_loss=None,
-                          gradient_tape=None):
-      """DP-SGD version of base class method."""
-      self._was_compute_gradients_called = True
-      if callable(loss):
-        # TF is running in Eager mode
-        raise NotImplementedError('Vectorized optimizer unavailable for TF2.')
-      else:
-        # TF is running in graph mode, check we did not receive a gradient tape.
-        if gradient_tape:
-          raise ValueError('When in graph mode, a tape should not be passed.')
-
-        batch_size = tf.shape(input=loss)[0]
-        if self._num_microbatches is None:
-          self._num_microbatches = batch_size
-
-        # Note: it would be closer to the correct i.i.d. sampling of records if
-        # we sampled each microbatch from the appropriate binomial distribution,
-        # although that still wouldn't be quite correct because it would be
-        # sampling from the dataset without replacement.
-        microbatch_losses = tf.reshape(loss, [self._num_microbatches, -1])
-
-        if var_list is None:
-          var_list = (
-              tf.compat.v1.trainable_variables() + tf.compat.v1.get_collection(
-                  tf.compat.v1.GraphKeys.TRAINABLE_RESOURCE_VARIABLES))
-
-        def process_microbatch(microbatch_loss):
-          """Compute clipped grads for one microbatch."""
-          microbatch_loss = tf.reduce_mean(input_tensor=microbatch_loss)
-          grads, _ = zip(*super(DPOptimizerClass, self).compute_gradients(
-              microbatch_loss, var_list, gate_gradients, aggregation_method,
-              colocate_gradients_with_ops, grad_loss))
-          grads_list = [
-              g if g is not None else tf.zeros_like(v)
-              for (g, v) in zip(list(grads), var_list)
-          ]
-          # Clip gradients to have L2 norm of l2_norm_clip.
-          # Here, we use TF primitives rather than the built-in
-          # tf.clip_by_global_norm() so that operations can be vectorized
-          # across microbatches.
-          grads_flat = tf.nest.flatten(grads_list)
-          squared_l2_norms = [
-              tf.reduce_sum(input_tensor=tf.square(g)) for g in grads_flat
-          ]
-          global_norm = tf.sqrt(tf.add_n(squared_l2_norms))
-          div = tf.maximum(global_norm / self._l2_norm_clip, 1.)
-          clipped_flat = [g / div for g in grads_flat]
-          clipped_grads = tf.nest.pack_sequence_as(grads_list, clipped_flat)
-          return clipped_grads
-
-        clipped_grads = tf.vectorized_map(process_microbatch, microbatch_losses)
-
-        def reduce_noise_normalize_batch(stacked_grads):
-          summed_grads = tf.reduce_sum(input_tensor=stacked_grads, axis=0)
-          noise_stddev = self._l2_norm_clip * self._noise_multiplier
-          noise = tf.random.normal(
-              tf.shape(input=summed_grads), stddev=noise_stddev)
-          noised_grads = summed_grads + noise
-          return noised_grads / tf.cast(self._num_microbatches, tf.float32)
-
-        final_grads = tf.nest.map_structure(reduce_noise_normalize_batch,
-                                            clipped_grads)
-
-        return list(zip(final_grads, var_list))
-
-    def apply_gradients(self, grads_and_vars, global_step=None, name=None):
-      # pylint: disable=g-doc-args, g-doc-return-or-yield
-      """DP-SGD version of base class method."""
-      assert self._was_compute_gradients_called, (
-          'compute_gradients() on the differentially private optimizer was not'
-          ' called. Which means that the training is not differentially '
-          'private. It happens for example in Keras training in TensorFlow '
-          '2.0+.')
-      return super(DPOptimizerClass, self).apply_gradients(
-          grads_and_vars=grads_and_vars, global_step=global_step, name=name)
-
-  return DPOptimizerClass
-
-
-VectorizedDPAdagradOptimizer = make_vectorized_optimizer_class(AdagradOptimizer)
-VectorizedDPAdamOptimizer = make_vectorized_optimizer_class(AdamOptimizer)
-VectorizedDPSGDOptimizer = make_vectorized_optimizer_class(
-    GradientDescentOptimizer)
-
-VectorizedDPAdagrad = VectorizedDPAdagradOptimizer
-VectorizedDPAdam = VectorizedDPAdamOptimizer
-VectorizedDPSGD = VectorizedDPSGDOptimizer
+if __name__ == '__main__':
+  tf.test.main()
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/epsilon_lower_bound_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_example.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_example.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/advanced_mia_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,18 @@
 
   Each variable which is set specifies a slicing by different dimension.
   """
 
   # When is set to true, one of the slices is the whole dataset.
   entire_dataset: bool = True
 
-  # Used in classification tasks for slicing by classes. It is assumed that
-  # classes are integers 0, 1, ... number of classes. When true one slice per
-  # each class is generated.
+  # Used in classification tasks for slicing by classes. When true one slice per
+  # each class is generated. Classes can either be
+  #  - integers 0, 1, ..., (for single label) or
+  #  - an array of integers (for multi-label).
   by_class: Union[bool, Iterable[int], int] = False
 
   # if true, it generates 10 slices for percentiles of the loss - 0-10%, 10-20%,
   # ... 90-100%.
   by_percentiles: bool = False
 
   # When true, a slice for correctly classifed and a slice for misclassifed
@@ -234,16 +235,18 @@
   logits_test: Optional[np.ndarray] = None
 
   # Predicted probabilities for each class. They can be derived from logits,
   # so they can be set only if logits are not explicitly provided.
   probs_train: Optional[np.ndarray] = None
   probs_test: Optional[np.ndarray] = None
 
-  # Contains ground-truth classes. Classes are assumed to be integers starting
-  # from 0.
+  # Contains ground-truth classes. For single-label classification, classes are
+  # assumed to be integers starting from 0. For multi-label classification,
+  # label is assumed to be multi-hot, i.e., labels is a binary array of shape
+  # (num_examples, num_classes).
   labels_train: Optional[np.ndarray] = None
   labels_test: Optional[np.ndarray] = None
 
   # Sample weights, if provided.
   sample_weight_train: Optional[np.ndarray] = None
   sample_weight_test: Optional[np.ndarray] = None
 
@@ -286,15 +289,17 @@
 
   @property
   def num_classes(self):
     if self.labels_train is None or self.labels_test is None:
       raise ValueError(
           'Can\'t identify the number of classes as no labels were provided. '
           'Please set labels_train and labels_test')
-    return int(max(np.max(self.labels_train), np.max(self.labels_test))) + 1
+    if not self.multilabel_data:
+      return int(max(np.max(self.labels_train), np.max(self.labels_test))) + 1
+    return self.labels_train.shape[1]
 
   @property
   def logits_or_probs_train(self):
     """Returns train logits or probs whatever is not None."""
     if self.logits_train is not None:
       return self.logits_train
     return self.probs_train
@@ -582,14 +587,16 @@
       #   (num_samples, num_classes).
       _is_array_two_dimensional(self.loss_train, 'loss_train')
       _is_array_two_dimensional(self.loss_test, 'loss_test')
       _is_array_two_dimensional(self.entropy_train, 'entropy_train')
       _is_array_two_dimensional(self.entropy_test, 'entropy_test')
       _is_array_two_dimensional(self.labels_train, 'labels_train')
       _is_array_two_dimensional(self.labels_test, 'labels_test')
+      self.is_multihot_labels(self.labels_train, 'labels_train')
+      self.is_multihot_labels(self.labels_test, 'labels_test')
     else:
       _is_array_one_dimensional(self.loss_train, 'loss_train')
       _is_array_one_dimensional(self.loss_test, 'loss_test')
       _is_array_one_dimensional(self.entropy_train, 'entropy_train')
       _is_array_one_dimensional(self.entropy_test, 'entropy_test')
       _is_array_one_dimensional(self.labels_train, 'labels_train')
       _is_array_one_dimensional(self.labels_test, 'labels_test')
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/data_structures_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,18 +68,26 @@
   # of the original dataset.
   result.multilabel_data = data.is_multilabel_data()
 
   return result
 
 
 def _slice_by_class(data: AttackInputData, class_value: int) -> AttackInputData:
-  if data.is_multilabel_data():
-    raise ValueError("Slicing by class not supported for multilabel data.")
-  idx_train = data.labels_train == class_value
-  idx_test = data.labels_test == class_value
+  """Gets the indices (boolean) for examples belonging to the given class."""
+  if not data.is_multilabel_data():
+    idx_train = data.labels_train == class_value
+    idx_test = data.labels_test == class_value
+  else:
+    if class_value >= data.num_classes:
+      raise ValueError(
+          f"class_value ({class_value}) is larger than the number of classes"
+          " (data.num_classes)."
+      )
+    idx_train = data.labels_train[:, class_value].astype(bool)
+    idx_test = data.labels_test[:, class_value].astype(bool)
   return _slice_data_by_indices(data, idx_train, idx_test)
 
 
 def _slice_by_percentiles(data: AttackInputData, from_percentile: float,
                           to_percentile: float):
   """Slices samples by loss percentiles."""
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/dataset_slicing_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,18 +354,28 @@
   def test_slice_entire_dataset(self):
     entire_dataset_slice = SingleSliceSpec()
     output = get_slice(self.input_data, entire_dataset_slice)
     expected = self.input_data
     expected.slice_spec = entire_dataset_slice
     self.assertTrue(_are_all_fields_equal(output, self.input_data))
 
-  def test_slice_by_class_fails(self):
+  def test_slice_by_class(self):
     class_index = 1
     class_slice = SingleSliceSpec(SlicingFeature.CLASS, class_index)
-    self.assertRaises(ValueError, get_slice, self.input_data, class_slice)
+    output = get_slice(self.input_data, class_slice)
+    expected_indices_train = np.array([0, 2, 3])
+    expected_indices_test = np.array([1, 2])
+
+    np.testing.assert_array_equal(
+        output.logits_train,
+        self.input_data.logits_train[expected_indices_train],
+    )
+    np.testing.assert_array_equal(
+        output.logits_test, self.input_data.logits_test[expected_indices_test]
+    )
 
   @mock.patch('logging.Logger.info', wraps=logging.Logger)
   def test_slice_by_percentile_logs_multilabel_data(self, mock_logger):
     percentile_slice = SingleSliceSpec(SlicingFeature.PERCENTILE, (0, 50))
     _ = get_slice(self.input_data, percentile_slice)
     mock_logger.assert_called_with(
         ('For multilabel data, when slices by percentiles are '
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_example.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_example.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/keras_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,26 +116,29 @@
   # Predict the left out with the last attacker
   if left_out_indices.size:
     assert np.all(np.isnan(scores[left_out_indices]))
     scores[left_out_indices] = attacker.predict(features[left_out_indices])
   assert not np.any(np.isnan(scores))
 
   # Generate ROC curves with scores.
+  # Different from the threshold attacker which uses the loss, we do not negate
+  # the scores here, because the attacker returns the probability of the
+  # positive class.
   fpr, tpr, thresholds = metrics.roc_curve(labels, scores)
   # 'test_train_ratio' is the ratio of test data size to train data size. It is
   # used to compute the Positive Predictive Value.
   test_train_ratio = ((prepared_attacker_data.data_size.ntest) /
                       (prepared_attacker_data.data_size.ntrain))
   roc_curve = RocCurve(
       tpr=tpr,
       fpr=fpr,
       thresholds=thresholds,
       test_train_ratio=test_train_ratio)
 
-  in_train_indices = (labels == 0)
+  in_train_indices = labels == 1
   return SingleAttackResult(
       slice_spec=_get_slice_spec(attack_input),
       data_size=prepared_attacker_data.data_size,
       attack_type=attack_type,
       membership_scores_train=scores[in_train_indices],
       membership_scores_test=scores[~in_train_indices],
       roc_curve=roc_curve)
@@ -150,25 +153,30 @@
     raise ValueError('Not possible to run threshold attack without losses.')
   if attack_input.is_multilabel_data():
     logging.info(('For multilabel data, when a threshold attack is requested, '
                   'losses are summed over the class axis before slicing.'))
     loss_train = np.sum(loss_train, axis=1)
     loss_test = np.sum(loss_test, axis=1)
   fpr, tpr, thresholds = metrics.roc_curve(
-      np.concatenate((np.zeros(ntrain), np.ones(ntest))),
-      np.concatenate((loss_train, loss_test)))
+      np.concatenate((np.ones(ntrain), np.zeros(ntest))),
+      # roc_curve uses classifier in the form of
+      # "score >= threshold ==> predict positive", while training data has lower
+      # loss, so we negate the loss.
+      -np.concatenate((loss_train, loss_test)),
+  )
   # 'test_train_ratio' is the ratio of test data size to train data size. It is
   # used to compute the Positive Predictive Value.
   test_train_ratio = ntest / ntrain
 
   roc_curve = RocCurve(
       tpr=tpr,
       fpr=fpr,
-      thresholds=thresholds,
-      test_train_ratio=test_train_ratio)
+      thresholds=-thresholds,  # negate because we negated the loss
+      test_train_ratio=test_train_ratio,
+  )
 
   return SingleAttackResult(
       slice_spec=_get_slice_spec(attack_input),
       data_size=DataSize(ntrain=ntrain, ntest=ntest),
       attack_type=AttackType.THRESHOLD_ATTACK,
       membership_scores_train=attack_input.get_loss_train(),
       membership_scores_test=attack_input.get_loss_test(),
@@ -178,26 +186,31 @@
 def _run_threshold_entropy_attack(attack_input: AttackInputData):
   """Runs threshold entropy attack on single label data."""
   if attack_input.is_multilabel_data():
     raise NotImplementedError(('Entropy-based attacks are not implemented for '
                                'multilabel data.'))
   ntrain, ntest = attack_input.get_train_size(), attack_input.get_test_size()
   fpr, tpr, thresholds = metrics.roc_curve(
-      np.concatenate((np.zeros(ntrain), np.ones(ntest))),
-      np.concatenate(
-          (attack_input.get_entropy_train(), attack_input.get_entropy_test())))
+      np.concatenate((np.ones(ntrain), np.zeros(ntest))),
+      # Similar as in loss, we negate the entropy becase training examples are
+      # expected to have lower entropy.
+      -np.concatenate(
+          (attack_input.get_entropy_train(), attack_input.get_entropy_test())
+      ),
+  )
   # 'test_train_ratio' is the ratio of test data size to train data size. It is
   # used to compute the Positive Predictive Value.
   test_train_ratio = ntest / ntrain
 
   roc_curve = RocCurve(
       tpr=tpr,
       fpr=fpr,
-      thresholds=thresholds,
-      test_train_ratio=test_train_ratio)
+      thresholds=-thresholds,  # negate because we negated the loss
+      test_train_ratio=test_train_ratio,
+  )
 
   return SingleAttackResult(
       slice_spec=_get_slice_spec(attack_input),
       data_size=DataSize(ntrain=ntrain, ntest=ntest),
       attack_type=AttackType.THRESHOLD_ENTROPY_ATTACK,
       membership_scores_train=-attack_input.get_entropy_train(),
       membership_scores_test=-attack_input.get_entropy_test(),
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/membership_inference_attack_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -210,17 +210,19 @@
         result.membership_scores_train,
         result.membership_scores_train[0],
         rtol=1e-3)
     np.testing.assert_allclose(
         result.membership_scores_test,
         result.membership_scores_test[0],
         rtol=1e-3)
-    # Training score should be smaller than test score
-    self.assertLess(result.membership_scores_train[0],
-                    result.membership_scores_test[0])
+    # Training score should be larger than test score, as training set is set
+    # to be positive.
+    self.assertGreater(
+        result.membership_scores_train[0], result.membership_scores_test[0]
+    )
 
   def test_run_attack_threshold_calculates_correct_auc(self):
     result = mia._run_attack(
         AttackInputData(
             loss_train=np.array([0.1, 0.2, 1.3, 0.4, 0.5, 0.6]),
             loss_test=np.array([1.1, 1.2, 1.3, 0.4, 1.5, 1.6])),
         AttackType.THRESHOLD_ATTACK)
@@ -232,20 +234,47 @@
         AttackInputData(
             entropy_train=np.array([0.1, 0.2, 1.3, 0.4, 0.5, 0.6]),
             entropy_test=np.array([1.1, 1.2, 1.3, 0.4, 1.5, 1.6])),
         AttackType.THRESHOLD_ENTROPY_ATTACK)
 
     np.testing.assert_almost_equal(result.roc_curve.get_auc(), 0.83, decimal=2)
 
+  @parameterized.parameters(
+      [AttackType.THRESHOLD_ATTACK],
+      [AttackType.THRESHOLD_ENTROPY_ATTACK],
+  )
+  def test_calculates_correct_tpr_fpr(self, attack_type):
+    rng = np.random.RandomState(27)
+    loss_train = rng.rand(100)
+    loss_test = rng.rand(50) + 0.1
+    result = mia._run_attack(
+        AttackInputData(
+            loss_train=loss_train,
+            loss_test=loss_test,
+            entropy_train=loss_train,
+            entropy_test=loss_test,
+        ),
+        attack_type,
+    )
+    self.assertEqual(attack_type, result.attack_type)
+    for tpr, fpr, threshold in zip(
+        result.roc_curve.tpr, result.roc_curve.fpr, result.roc_curve.thresholds
+    ):
+      self.assertAlmostEqual(tpr, np.mean(loss_train <= threshold))
+      self.assertAlmostEqual(fpr, np.mean(loss_test <= threshold))
+
   @mock.patch('sklearn.metrics.roc_curve')
   def test_run_attack_threshold_entropy_small_tpr_fpr_correct_ppv(
       self, patched_fn):
     # sklearn.metrics.roc_curve returns (fpr, tpr, thresholds).
-    patched_fn.return_value = ([0.2, 0.04, 0.0003], [0.1, 0.0001,
-                                                     0.0002], [0.2, 0.4, 0.6])
+    patched_fn.return_value = (
+        np.array([0.2, 0.04, 0.0003]),
+        np.array([0.1, 0.0001, 0.0002]),
+        np.array([0.2, 0.4, 0.6]),
+    )
     result = mia._run_attack(
         AttackInputData(
             entropy_train=np.array([0.1, 0.2, 1.3, 0.4, 0.5, 0.6]),
             entropy_test=np.array([1.1, 1.2, 1.3, 0.4, 1.5, 1.6]),
             force_multilabel_data=False), AttackType.THRESHOLD_ENTROPY_ATTACK)
     # PPV = TPR / (TPR + test_train_ratio * FPR), except when both TPR and FPR
     # are close to 0. Then PPV = 1/ (1 + test_train_ratio)
@@ -376,16 +405,19 @@
 
     np.testing.assert_almost_equal(result.roc_curve.get_ppv(), 1.0, decimal=2)
 
   @mock.patch('sklearn.metrics.roc_curve')
   def test_run_multilabel_attack_threshold_small_tpr_fpr_correct_ppv(
       self, patched_fn):
     # sklearn.metrics.roc_curve returns (fpr, tpr, thresholds).
-    patched_fn.return_value = ([0.2, 0.04, 0.0003], [0.1, 0.0001,
-                                                     0.0002], [0.2, 0.4, 0.6])
+    patched_fn.return_value = (
+        np.array([0.2, 0.04, 0.0003]),
+        np.array([0.1, 0.0001, 0.0002]),
+        np.array([0.2, 0.4, 0.6]),
+    )
     result = mia._run_attack(
         AttackInputData(
             loss_train=np.array([[0.1, 0.2], [1.3, 0.4], [0.5, 0.6], [0.9,
                                                                       0.6]]),
             loss_test=np.array([[1.1, 1.2], [1.3, 0.4], [1.5, 1.6]]),
             force_multilabel_data=True), AttackType.THRESHOLD_ATTACK)
     # PPV = TPR / (TPR + test_train_ratio * FPR), except when both TPR and FPR
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
   attack_input_train = _column_stack(attack_input_data.logits_or_probs_train,
                                      attack_input_data.get_loss_train())
   attack_input_test = _column_stack(attack_input_data.logits_or_probs_test,
                                     attack_input_data.get_loss_test())
 
   ntrain, ntest = attack_input_train.shape[0], attack_input_test.shape[0]
   features_all = np.concatenate((attack_input_train, attack_input_test))
-  labels_all = np.concatenate((np.zeros(ntrain), np.ones(ntest)))
+  labels_all = np.concatenate((np.ones(ntrain), np.zeros(ntest)))
   if attack_input_data.has_nonnull_sample_weights():
     sample_weights_all = np.concatenate((attack_input_data.sample_weight_train,
                                          attack_input_data.sample_weight_test),
                                         axis=0)
   else:
     sample_weights_all = None
 
@@ -278,20 +278,24 @@
       }
       model = model_selection.GridSearchCV(
           knn_model, param_grid=param_grid, cv=3, n_jobs=self.n_jobs, verbose=0)
       model.fit(input_features, is_training_labels)
     self.model = model
 
 
-def create_attacker(attack_type,
-                    backend: Optional[str] = None) -> TrainedAttacker:
+def create_attacker(
+    attack_type: data_structures.AttackType, backend: Optional[str] = None
+) -> TrainedAttacker:
   """Returns the corresponding attacker for the provided attack_type."""
   # Compare by name instead of the variable itself to support module reload.
   if attack_type.name == data_structures.AttackType.LOGISTIC_REGRESSION.name:
     return LogisticRegressionAttacker(backend=backend)
-  if attack_type.name == data_structures.AttackType.MULTI_LAYERED_PERCEPTRON.name:
+  if (
+      attack_type.name
+      == data_structures.AttackType.MULTI_LAYERED_PERCEPTRON.name
+  ):
     return MultilayerPerceptronAttacker(backend=backend)
   if attack_type.name == data_structures.AttackType.RANDOM_FOREST.name:
     return RandomForestAttacker(backend=backend)
   if attack_type.name == data_structures.AttackType.K_NEAREST_NEIGHBORS.name:
     return KNearestNeighborsAttacker(backend=backend)
   raise NotImplementedError('Attack type %s not implemented yet.' % attack_type)
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/models_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/plotting.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/plotting.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/privacy_report_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/seq2seq_mia_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_example.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_example.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/tf_estimator_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/utils_tensorboard.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/membership_inference_attack/utils_tensorboard.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/exposures_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/secret_sharer/generate_secrets_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/utils.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/privacy/privacy_tests/utils_test.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/privacy/privacy_tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/v1/__init__.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy/version.py` & `tensorflow_privacy-0.8.9/tensorflow_privacy/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """TensorFlow Privacy version."""
 
-__version__ = '0.8.8'
+__version__ = '0.8.9'
```

### Comparing `tensorflow_privacy-0.8.8/tensorflow_privacy.egg-info/SOURCES.txt` & `tensorflow_privacy-0.8.9/tensorflow_privacy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 tensorflow_privacy/privacy/estimators/v1/dnn_test.py
 tensorflow_privacy/privacy/estimators/v1/head.py
 tensorflow_privacy/privacy/estimators/v1/head_test.py
 tensorflow_privacy/privacy/fast_gradient_clipping/__init__.py
 tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads.py
 tensorflow_privacy/privacy/fast_gradient_clipping/clip_grads_test.py
 tensorflow_privacy/privacy/fast_gradient_clipping/gradient_clipping_utils.py
+tensorflow_privacy/privacy/fast_gradient_clipping/gradient_clipping_utils_test.py
 tensorflow_privacy/privacy/fast_gradient_clipping/layer_registry.py
 tensorflow_privacy/privacy/keras_models/__init__.py
 tensorflow_privacy/privacy/keras_models/dp_keras_model.py
 tensorflow_privacy/privacy/keras_models/dp_keras_model_test.py
 tensorflow_privacy/privacy/logistic_regression/__init__.py
 tensorflow_privacy/privacy/logistic_regression/datasets.py
 tensorflow_privacy/privacy/logistic_regression/datasets_test.py
@@ -107,14 +108,15 @@
 tensorflow_privacy/privacy/optimizers/__init__.py
 tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients.py
 tensorflow_privacy/privacy/optimizers/clip_and_aggregate_gradients_test.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_eager_test.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_keras.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse.py
+tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse_distributed_test.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_sparse_test.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_test.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_keras_vectorized.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_test.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized.py
 tensorflow_privacy/privacy/optimizers/dp_optimizer_vectorized_test.py
 tensorflow_privacy/privacy/privacy_tests/__init__.py
```

