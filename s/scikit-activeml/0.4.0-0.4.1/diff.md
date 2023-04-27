# Comparing `tmp/scikit-activeml-0.4.0.tar.gz` & `tmp/scikit-activeml-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-activeml-0.4.0.tar", last modified: Wed Dec 21 13:35:15 2022, max compression
+gzip compressed data, was "scikit-activeml-0.4.1.tar", last modified: Thu Apr 27 09:12:16 2023, max compression
```

## Comparing `scikit-activeml-0.4.0.tar` & `scikit-activeml-0.4.1.tar`

### file list

```diff
@@ -1,139 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.962426 scikit-activeml-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2022-12-21 13:35:15.962426 scikit-activeml-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.942426 scikit-activeml-0.4.0/scikit_activeml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2022-12-21 13:35:15.000000 scikit-activeml-0.4.0/scikit_activeml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2022-12-21 13:35:15.000000 scikit-activeml-0.4.0/scikit_activeml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 13:35:15.000000 scikit-activeml-0.4.0/scikit_activeml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 13:35:15.000000 scikit-activeml-0.4.0/scikit_activeml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-21 13:35:15.000000 scikit-activeml-0.4.0/scikit_activeml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-21 13:35:15.000000 scikit-activeml-0.4.0/scikit_activeml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 13:35:15.962426 scikit-activeml-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.942426 scikit-activeml-0.4.0/skactiveml/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58779 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.942426 scikit-activeml-0.4.0/skactiveml/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/_mixture_model_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/_parzen_window_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    28372 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.942426 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/_annotator_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    24839 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/_annotator_logistic_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.942426 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/tests/test_annotator_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/tests/test_annotator_logistic_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.946426 scikit-activeml-0.4.0/skactiveml/classifier/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19556 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/tests/test_mixture_model_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/tests/test_parzen_window_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/classifier/tests/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.946426 scikit-activeml-0.4.0/skactiveml/pool/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_cost_embedding_al.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_discriminative_al.py
--rw-r--r--   0 runner    (1001) docker     (123)    24199 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_epistemic_uncertainty_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    35076 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_expected_error_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_expected_model_change_maximization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_expected_model_output_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_expected_model_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_four_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_greedy_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_information_gain_maximization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13149 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_probabilistic_al.py
--rw-r--r--   0 runner    (1001) docker     (123)    12792 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_query_by_committee.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_quire.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    15652 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/_uncertainty_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.950425 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15738 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/_interval_estimation_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.950425 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16310 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/tests/test_interval_estimation_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)    19570 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/multiannotator/tests/test_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.954426 scikit-activeml-0.4.0/skactiveml/pool/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_cost_embedding_al.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_discriminative_al.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_epistemic_uncertainty_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    28107 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_error_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_model_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_model_output_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_model_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_four_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_greedy_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_information_gain_maximization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_probabilistic_al.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_query_by_committee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_quire.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_uncertainty_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    33207 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41416 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/pool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.954426 scikit-activeml-0.4.0/skactiveml/regressor/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/regressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/regressor/_nic_kernel_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/regressor/_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.954426 scikit-activeml-0.4.0/skactiveml/regressor/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/regressor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/regressor/tests/test_nic_kernel_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/regressor/tests/test_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.954426 scikit-activeml-0.4.0/skactiveml/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13895 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/_stream_baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/_stream_probabilistic_al.py
--rw-r--r--   0 runner    (1001) docker     (123)    20189 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/_uncertainty_zliobaite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.954426 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/_balanced_incremental_quantile_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25107 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/_estimated_budget_zliobaite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.958426 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/test_balanced_incremental_quantile_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/test_budget_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/test_estimated_budget_zliobaite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.958426 scikit-activeml-0.4.0/skactiveml/stream/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/tests/test_stream_baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/tests/test_stream_probabilistic_al.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/stream/tests/test_uncertainty_zliobaite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.958426 scikit-activeml-0.4.0/skactiveml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26892 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/tests/template_query_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/tests/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.958426 scikit-activeml-0.4.0/skactiveml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/_multi_annot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    27965 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.962426 scikit-activeml-0.4.0/skactiveml/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/test_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/test_multi_annot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/utils/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.962426 scikit-activeml-0.4.0/skactiveml/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/visualization/_feature_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/visualization/_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 13:35:15.962426 scikit-activeml-0.4.0/skactiveml/visualization/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/visualization/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19456 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/visualization/tests/test_feature_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-21 13:34:40.000000 scikit-activeml-0.4.0/skactiveml/visualization/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.885205 scikit-activeml-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-04-27 09:12:16.885205 scikit-activeml-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.869205 scikit-activeml-0.4.1/scikit_activeml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-04-27 09:12:16.000000 scikit-activeml-0.4.1/scikit_activeml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-27 09:12:16.000000 scikit-activeml-0.4.1/scikit_activeml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:12:16.000000 scikit-activeml-0.4.1/scikit_activeml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:12:16.000000 scikit-activeml-0.4.1/scikit_activeml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 09:12:16.000000 scikit-activeml-0.4.1/scikit_activeml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 09:12:16.000000 scikit-activeml-0.4.1/scikit_activeml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:12:16.885205 scikit-activeml-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.869205 scikit-activeml-0.4.1/skactiveml/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58674 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.873205 scikit-activeml-0.4.1/skactiveml/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/_mixture_model_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/_parzen_window_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28453 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.873205 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/_annotator_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24839 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/_annotator_logistic_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.873205 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/tests/test_annotator_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/tests/test_annotator_logistic_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.873205 scikit-activeml-0.4.1/skactiveml/classifier/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19556 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/tests/test_mixture_model_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/tests/test_parzen_window_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20043 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/classifier/tests/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.873205 scikit-activeml-0.4.1/skactiveml/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_batch_bald.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_cost_embedding_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_discriminative_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24199 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_epistemic_uncertainty_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35076 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_expected_error_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_expected_model_change_maximization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_expected_model_output_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_expected_model_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_four_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_greedy_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_information_gain_maximization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_probabilistic_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_query_by_committee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_quire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/_uncertainty_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.873205 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/_interval_estimation_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.877205 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/tests/test_interval_estimation_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/multiannotator/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.877205 scikit-activeml-0.4.1/skactiveml/pool/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_batch_bald.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_cost_embedding_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_discriminative_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_epistemic_uncertainty_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28107 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_error_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_model_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_model_output_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_model_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_four_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_greedy_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_information_gain_maximization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_probabilistic_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_query_by_committee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_quire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_uncertainty_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33919 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42406 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/pool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.877205 scikit-activeml-0.4.1/skactiveml/regressor/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/regressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/regressor/_nic_kernel_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/regressor/_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.877205 scikit-activeml-0.4.1/skactiveml/regressor/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/regressor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/regressor/tests/test_nic_kernel_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/regressor/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.877205 scikit-activeml-0.4.1/skactiveml/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55730 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/_density_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/_stream_baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/_stream_probabilistic_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/_uncertainty_zliobaite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.877205 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/_balanced_incremental_quantile_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33120 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/_estimated_budget_zliobaite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/_threshold_budget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.881205 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/test_balanced_incremental_quantile_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/test_budget_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/test_estimated_budget_zliobaite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/test_threshold_budget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.881205 scikit-activeml-0.4.1/skactiveml/stream/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/tests/test_density_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/tests/test_stream_baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/tests/test_stream_probabilistic_al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/stream/tests/test_uncertainty_zliobaite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.881205 scikit-activeml-0.4.1/skactiveml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26892 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/tests/template_query_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.881205 scikit-activeml-0.4.1/skactiveml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/_multi_annot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27965 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.881205 scikit-activeml-0.4.1/skactiveml/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/test_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/test_multi_annot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/utils/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.881205 scikit-activeml-0.4.1/skactiveml/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26367 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/visualization/_feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/visualization/_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:12:16.881205 scikit-activeml-0.4.1/skactiveml/visualization/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/visualization/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/visualization/tests/test_feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-27 09:11:49.000000 scikit-activeml-0.4.1/skactiveml/visualization/tests/test_misc.py
```

### Comparing `scikit-activeml-0.4.0/LICENSE.txt` & `scikit-activeml-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/PKG-INFO` & `scikit-activeml-0.4.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-activeml
-Version: 0.4.0
+Version: 0.4.1
 Summary: Our package scikit-activeml is a Python library for active learning on top of SciPy and scikit-learn.
 Home-page: https://github.com/scikit-activeml/scikit-activeml
 Author: Marek Herde
 Author-email: marek.herde@uni-kassel.de
 License: BSD 3-Clause License
 Keywords: active learning,machine learning,semi-supervised learning,data mining,pattern recognition,artificial intelligence
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 .. intro_start
 
-|Doc|_ |Codecov|_ |PythonVersion|_ |PyPi|_ |Paper|_
+|Doc|_ |Codecov|_ |PythonVersion|_ |PyPi|_ |Paper|_ |Black|_
 
 .. |Doc| image:: https://img.shields.io/badge/docs-latest-green
 .. _Doc: https://scikit-activeml.github.io/scikit-activeml-docs/
 
 .. |Codecov| image:: https://codecov.io/gh/scikit-activeml/scikit-activeml/branch/master/graph/badge.svg
 .. _Codecov: https://app.codecov.io/gh/scikit-activeml/scikit-activeml
 
@@ -35,14 +35,17 @@
 
 .. |PyPi| image:: https://badge.fury.io/py/scikit-activeml.svg
 .. _PyPi: https://badge.fury.io/py/scikit-activeml
 
 .. |Paper| image:: https://img.shields.io/badge/paper-10.20944/preprints202103.0194.v1-blue
 .. _Paper: https://www.preprints.org/manuscript/202103.0194/v1
 
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. _Black: https://github.com/psf/black
+
 |
 
 .. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/scikit-activeml-logo.png
    :width: 200
 
 |
 
@@ -57,145 +60,102 @@
 on top of `scikit-learn <https://scikit-learn.org/stable/>`_. The project was initiated in 2020 by the
 `Intelligent Embedded Systems Group <https://www.uni-kassel.de/eecs/en/sections/intelligent-embedded-systems/home>`_
 at the University of Kassel and is distributed under the `3-Clause BSD licence
 <https://github.com/scikit-activeml/scikit-activeml/blob/master/LICENSE.txt>`_.
 
 .. intro_end
 
-.. overview_start
-
-Overview
-========
-
-Our philosophy is to extend the ``sklearn`` eco-system with the most relevant
-query strategies for active learning and to implement tools for working with partially
-unlabeled data. An overview of our repository's structure is given in the image below.
-Each node represents a class or interface. The arrows illustrate the inheritance
-hierarchy among them. The functionality of a dashed node is not yet available in our library.
-
-.. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/scikit-activeml-structure.png
-   :width: 1000
-
-In our package ``skactiveml``, there three major components, i.e., ``SkactivemlClassifier``,
-``QueryStrategy``, and the not yet supported ``SkactivemlRegressor``.
-The classifier and regressor modules are necessary to deal with partially unlabeled
-data and to implement active-learning specific estimators. This way, an active learning
-cycle can be easily implemented to start with zero initial labels. Regarding the
-active learning query strategies, we currently differ between
-the pool-based (a large pool of unlabeled samples is available) and stream-based
-(unlabeled samples arrive sequentially, i.e., as a stream) paradigm.
-On top of both paradigms, we also distinguish the single- and multi-annotator
-setting. In the latter setting, multiple error-prone annotators are queried
-to provide labels. As a result, an active learning query strategy not only decides
-which samples but also which annotators should be queried.
-
-.. overview_end
-
 .. user_installation_start
 
 User Installation
 =================
 
 The easiest way of installing scikit-activeml is using ``pip``:
 
 ::
 
     pip install -U scikit-activeml
 
-.. install_end
+.. user_installation_end
 
 .. examples_start
 
 Examples
 ========
-In the following, there are two simple examples illustrating the straightforwardness
-of implementing active learning cycles with our Python package ``skactiveml``.
-For more in-depth examples, we refer to our
-`tutorial section <https://scikit-activeml.github.io/scikit-activeml-docs/>`_ offering
-a broad overview of different use-cases:
-
-- `pool-based active learning -- getting started <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/00_pool_getting_started.ipynb>`_,
-- `deep pool-based active learning -- scikit-activeml with skorch <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/01_deep_pool_al_with_skorch.ipynb>`_,
-- `multi-annotator pool-based active learning -- getting started <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/10_multiple_annotators_getting_started.ipynb>`_,
-- `stream-based active learning -- getting started <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/20_stream_getting_started.ipynb>`_,
-- and `batch stream-based active learning with pool-based query strategies <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/21_stream_batch_with_pool_al.ipynb>`_.
+We provide a broad overview of different use-cases in our `tutorial section <https://scikit-activeml.github.io/scikit-activeml-docs/tutorials.html>`_ offering
+
+- `Pool-based Active Learning - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/00_pool_getting_started.html>`_,
+- `Deep Pool-based Active Learning - scikit-activeml with Skorch <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/01_deep_pool_al_with_skorch.html>`_,
+- `Pool-based Active Learning for Regression - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/02_pool_regression_getting_started.html>`_,
+- `Multi-annotator Pool-based Active Learning - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/10_multiple_annotators_getting_started.html>`_,
+- `Stream-based Active Learning - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/20_stream_getting_started.html>`_,
+- and `Batch Stream-based Active Learning with Pool Query Strategies <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/21_stream_batch_with_pool_al.html>`_.
+
+Two simple examples illustrating the straightforwardness of implementing active learning cycles with our Python package ``skactiveml`` are given in the following.
 
 Pool-based Active Learning
 ##########################
 
-The following code implements an active learning cycle with 20 iterations using a Gaussian process
+The following code snippet implements an active learning cycle with 20 iterations using a Gaussian process
 classifier and uncertainty sampling. To use other classifiers, you can simply wrap classifiers from
 ``sklearn`` or use classifiers provided by ``skactiveml``. Note that the main difficulty using
 active learning with ``sklearn`` is the ability to handle unlabeled data, which we denote as a specific value
 (``MISSING_LABEL``) in the label vector ``y``. More query strategies can be found in the documentation.
 
 .. code-block:: python
-    
+
     import numpy as np
-    import matplotlib.pyplot as plt
     from sklearn.gaussian_process import GaussianProcessClassifier
     from sklearn.datasets import make_blobs
     from skactiveml.pool import UncertaintySampling
     from skactiveml.utils import unlabeled_indices, MISSING_LABEL
     from skactiveml.classifier import SklearnClassifier
-    from skactiveml.visualization import plot_decision_boundary, plot_utilities
 
     # Generate data set.
     X, y_true = make_blobs(n_samples=200, centers=4, random_state=0)
     y = np.full(shape=y_true.shape, fill_value=MISSING_LABEL)
 
-    # GaussianProcessClassifier needs initial training data otherwise a warning will
-    # be raised by SklearnClassifier. Therefore, the first 10 instances are used as
-    # training data.
+    # Use the first 10 instances as initial training data.
     y[:10] = y_true[:10]
 
     # Create classifier and query strategy.
-    clf = SklearnClassifier(GaussianProcessClassifier(random_state=0),classes=np.unique(y_true), random_state=0)
+    clf = SklearnClassifier(
+        GaussianProcessClassifier(random_state=0),
+        classes=np.unique(y_true),
+        random_state=0
+    )
     qs = UncertaintySampling(method='entropy')
 
     # Execute active learning cycle.
     n_cycles = 20
     for c in range(n_cycles):
         query_idx = qs.query(X=X, y=y, clf=clf)
         y[query_idx] = y_true[query_idx]
 
     # Fit final classifier.
     clf.fit(X, y)
 
-    # Visualize resulting classifier and current utilities.
-    bound = [[min(X[:, 0]), min(X[:, 1])], [max(X[:, 0]), max(X[:, 1])]]
-    unlbld_idx = unlabeled_indices(y)
-    fig, ax = plt.subplots(1, 1, figsize=(8, 8))
-    ax.set_title(f'Accuracy score: {clf.score(X,y_true)}', fontsize=15)
-    plot_utilities(qs, X=X, y=y, clf=clf, feature_bound=bound, ax=ax)
-    plot_decision_boundary(clf, feature_bound=bound, confidence=0.6)
-    plt.scatter(X[unlbld_idx,0], X[unlbld_idx,1], c='gray')
-    plt.scatter(X[:,0], X[:,1], c=y, cmap='jet')
-    plt.show()
-
-As output of this code snippet, we obtain the actively trained Gaussian process classifier
-including a visualization of its decision boundary and the sample utilities computed with
-uncertainty sampling.
+As a result, we obtain an actively trained Gaussian process classifier.
+A corresponding visualization of its decision boundary (black line) and the
+sample utilities (greenish contours) is given below.
 
 .. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/pal-example-output.png
    :width: 400
 
 Stream-based Active Learning
 ############################
 
-The following code implements an active learning cycle with 200 data points and
+The following code snippet implements an active learning cycle with 200 data points and
 the default budget of 10% using a pwc classifier and split uncertainty sampling. 
 Like in the pool-based example you can wrap other classifiers from ``sklearn``,
 ``sklearn`` compatible classifiers or like the example classifiers provided by ``skactiveml``.
 
 .. code-block:: python
 
     import numpy as np
-    import matplotlib.pyplot as plt
-    from scipy.ndimage import gaussian_filter1d
     from sklearn.datasets import make_blobs
     from skactiveml.classifier import ParzenWindowClassifier
     from skactiveml.stream import Split
     from skactiveml.utils import MISSING_LABEL
 
     # Generate data set.
     X, y_true = make_blobs(n_samples=200, centers=4, random_state=0)
@@ -218,39 +178,52 @@
         clf.fit(X_train, y_train)
         correct_classifications.append(clf.predict(X_cand)[0] == y_cand)
         sampled_indices = qs.query(candidates=X_cand, clf=clf)
         qs.update(candidates=X_cand, queried_indices=sampled_indices)
         X_train.append(x_t)
         y_train.append(y_cand if len(sampled_indices) > 0 else MISSING_LABEL)
 
-    # Plot the classifier's learning accuracy.
-    fig, ax = plt.subplots(1, 1, figsize=(8, 6))
-    ax.set_title(f'Learning curve', fontsize=15)
-    ax.set_xlabel('number of learning cycles')
-    ax.set_ylabel('accuracy')
-    ax.plot(gaussian_filter1d(np.array(correct_classifications, dtype=float), 4))
-    plt.show()
-
-As output of this code snippet, we obtain the actively trained pwc classifier incuding
-a visualization of its accuracy over the 200 samples.
+As a result, we obtain an actively trained Parzen window classifier.
+A corresponding visualization of its accuracy curve accross the active learning
+cycle is given below.
 
 .. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/stream-example-output.png
    :width: 400
 
+Query Strategy Overview
+#######################
+
+For better orientation, we provide an `overview <https://scikit-activeml.github.io/scikit-activeml-docs/generated/strategy_overview.html>`_
+(incl. paper references and `visualizations <https://scikit-activeml.github.io/scikit-activeml-docs/generated/sphinx_gallery_examples/index.html>`_)
+of the query strategies implemented by ``skactiveml``.
+
+|Overview| |Visualization|
+
+.. |Overview| image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/strategy-overview.gif
+   :width: 400
+   
+.. |Visualization| image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/example-overview.gif
+   :width: 400
+
 .. examples_end
 
+.. citing_start
+
 Citing
 ======
-If you use ``scikit-activeml`` in one of your research projects and find it helpful,
+If you use ``skactiveml`` in one of your research projects and find it helpful,
 please cite the following:
 
 ::
 
     @article{skactiveml2021,
-        title={scikitactiveml: {A} {L}ibrary and {T}oolbox for {A}ctive {L}}earning {A}lgorithms},
+        title={scikit-activeml: {A} {L}ibrary and {T}oolbox for {A}ctive {L}earning {A}lgorithms},
         author={Daniel Kottke and Marek Herde and Tuan Pham Minh and Alexander Benz and Pascal Mergard and Atal Roghman and Christoph Sandrock and Bernhard Sick},
         journal={Preprints},
         doi={10.20944/preprints202103.0194.v1},
         year={2021},
         url={https://github.com/scikit-activeml/scikit-activeml}
     }
 
+.. citing_end
+
+
```

### Comparing `scikit-activeml-0.4.0/README.rst` & `scikit-activeml-0.4.1/scikit_activeml.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,32 @@
+Metadata-Version: 2.1
+Name: scikit-activeml
+Version: 0.4.1
+Summary: Our package scikit-activeml is a Python library for active learning on top of SciPy and scikit-learn.
+Home-page: https://github.com/scikit-activeml/scikit-activeml
+Author: Marek Herde
+Author-email: marek.herde@uni-kassel.de
+License: BSD 3-Clause License
+Keywords: active learning,machine learning,semi-supervised learning,data mining,pattern recognition,artificial intelligence
+Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 .. intro_start
 
-|Doc|_ |Codecov|_ |PythonVersion|_ |PyPi|_ |Paper|_
+|Doc|_ |Codecov|_ |PythonVersion|_ |PyPi|_ |Paper|_ |Black|_
 
 .. |Doc| image:: https://img.shields.io/badge/docs-latest-green
 .. _Doc: https://scikit-activeml.github.io/scikit-activeml-docs/
 
 .. |Codecov| image:: https://codecov.io/gh/scikit-activeml/scikit-activeml/branch/master/graph/badge.svg
 .. _Codecov: https://app.codecov.io/gh/scikit-activeml/scikit-activeml
 
@@ -13,14 +35,17 @@
 
 .. |PyPi| image:: https://badge.fury.io/py/scikit-activeml.svg
 .. _PyPi: https://badge.fury.io/py/scikit-activeml
 
 .. |Paper| image:: https://img.shields.io/badge/paper-10.20944/preprints202103.0194.v1-blue
 .. _Paper: https://www.preprints.org/manuscript/202103.0194/v1
 
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. _Black: https://github.com/psf/black
+
 |
 
 .. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/scikit-activeml-logo.png
    :width: 200
 
 |
 
@@ -35,145 +60,102 @@
 on top of `scikit-learn <https://scikit-learn.org/stable/>`_. The project was initiated in 2020 by the
 `Intelligent Embedded Systems Group <https://www.uni-kassel.de/eecs/en/sections/intelligent-embedded-systems/home>`_
 at the University of Kassel and is distributed under the `3-Clause BSD licence
 <https://github.com/scikit-activeml/scikit-activeml/blob/master/LICENSE.txt>`_.
 
 .. intro_end
 
-.. overview_start
-
-Overview
-========
-
-Our philosophy is to extend the ``sklearn`` eco-system with the most relevant
-query strategies for active learning and to implement tools for working with partially
-unlabeled data. An overview of our repository's structure is given in the image below.
-Each node represents a class or interface. The arrows illustrate the inheritance
-hierarchy among them. The functionality of a dashed node is not yet available in our library.
-
-.. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/scikit-activeml-structure.png
-   :width: 1000
-
-In our package ``skactiveml``, there three major components, i.e., ``SkactivemlClassifier``,
-``QueryStrategy``, and the not yet supported ``SkactivemlRegressor``.
-The classifier and regressor modules are necessary to deal with partially unlabeled
-data and to implement active-learning specific estimators. This way, an active learning
-cycle can be easily implemented to start with zero initial labels. Regarding the
-active learning query strategies, we currently differ between
-the pool-based (a large pool of unlabeled samples is available) and stream-based
-(unlabeled samples arrive sequentially, i.e., as a stream) paradigm.
-On top of both paradigms, we also distinguish the single- and multi-annotator
-setting. In the latter setting, multiple error-prone annotators are queried
-to provide labels. As a result, an active learning query strategy not only decides
-which samples but also which annotators should be queried.
-
-.. overview_end
-
 .. user_installation_start
 
 User Installation
 =================
 
 The easiest way of installing scikit-activeml is using ``pip``:
 
 ::
 
     pip install -U scikit-activeml
 
-.. install_end
+.. user_installation_end
 
 .. examples_start
 
 Examples
 ========
-In the following, there are two simple examples illustrating the straightforwardness
-of implementing active learning cycles with our Python package ``skactiveml``.
-For more in-depth examples, we refer to our
-`tutorial section <https://scikit-activeml.github.io/scikit-activeml-docs/>`_ offering
-a broad overview of different use-cases:
-
-- `pool-based active learning -- getting started <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/00_pool_getting_started.ipynb>`_,
-- `deep pool-based active learning -- scikit-activeml with skorch <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/01_deep_pool_al_with_skorch.ipynb>`_,
-- `multi-annotator pool-based active learning -- getting started <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/10_multiple_annotators_getting_started.ipynb>`_,
-- `stream-based active learning -- getting started <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/20_stream_getting_started.ipynb>`_,
-- and `batch stream-based active learning with pool-based query strategies <https://github.com/scikit-activeml/scikit-activeml/blob/master/tutorials/21_stream_batch_with_pool_al.ipynb>`_.
+We provide a broad overview of different use-cases in our `tutorial section <https://scikit-activeml.github.io/scikit-activeml-docs/tutorials.html>`_ offering
+
+- `Pool-based Active Learning - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/00_pool_getting_started.html>`_,
+- `Deep Pool-based Active Learning - scikit-activeml with Skorch <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/01_deep_pool_al_with_skorch.html>`_,
+- `Pool-based Active Learning for Regression - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/02_pool_regression_getting_started.html>`_,
+- `Multi-annotator Pool-based Active Learning - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/10_multiple_annotators_getting_started.html>`_,
+- `Stream-based Active Learning - Getting Started <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/20_stream_getting_started.html>`_,
+- and `Batch Stream-based Active Learning with Pool Query Strategies <https://scikit-activeml.github.io/scikit-activeml-docs/generated/tutorials/21_stream_batch_with_pool_al.html>`_.
+
+Two simple examples illustrating the straightforwardness of implementing active learning cycles with our Python package ``skactiveml`` are given in the following.
 
 Pool-based Active Learning
 ##########################
 
-The following code implements an active learning cycle with 20 iterations using a Gaussian process
+The following code snippet implements an active learning cycle with 20 iterations using a Gaussian process
 classifier and uncertainty sampling. To use other classifiers, you can simply wrap classifiers from
 ``sklearn`` or use classifiers provided by ``skactiveml``. Note that the main difficulty using
 active learning with ``sklearn`` is the ability to handle unlabeled data, which we denote as a specific value
 (``MISSING_LABEL``) in the label vector ``y``. More query strategies can be found in the documentation.
 
 .. code-block:: python
-    
+
     import numpy as np
-    import matplotlib.pyplot as plt
     from sklearn.gaussian_process import GaussianProcessClassifier
     from sklearn.datasets import make_blobs
     from skactiveml.pool import UncertaintySampling
     from skactiveml.utils import unlabeled_indices, MISSING_LABEL
     from skactiveml.classifier import SklearnClassifier
-    from skactiveml.visualization import plot_decision_boundary, plot_utilities
 
     # Generate data set.
     X, y_true = make_blobs(n_samples=200, centers=4, random_state=0)
     y = np.full(shape=y_true.shape, fill_value=MISSING_LABEL)
 
-    # GaussianProcessClassifier needs initial training data otherwise a warning will
-    # be raised by SklearnClassifier. Therefore, the first 10 instances are used as
-    # training data.
+    # Use the first 10 instances as initial training data.
     y[:10] = y_true[:10]
 
     # Create classifier and query strategy.
-    clf = SklearnClassifier(GaussianProcessClassifier(random_state=0),classes=np.unique(y_true), random_state=0)
+    clf = SklearnClassifier(
+        GaussianProcessClassifier(random_state=0),
+        classes=np.unique(y_true),
+        random_state=0
+    )
     qs = UncertaintySampling(method='entropy')
 
     # Execute active learning cycle.
     n_cycles = 20
     for c in range(n_cycles):
         query_idx = qs.query(X=X, y=y, clf=clf)
         y[query_idx] = y_true[query_idx]
 
     # Fit final classifier.
     clf.fit(X, y)
 
-    # Visualize resulting classifier and current utilities.
-    bound = [[min(X[:, 0]), min(X[:, 1])], [max(X[:, 0]), max(X[:, 1])]]
-    unlbld_idx = unlabeled_indices(y)
-    fig, ax = plt.subplots(1, 1, figsize=(8, 8))
-    ax.set_title(f'Accuracy score: {clf.score(X,y_true)}', fontsize=15)
-    plot_utilities(qs, X=X, y=y, clf=clf, feature_bound=bound, ax=ax)
-    plot_decision_boundary(clf, feature_bound=bound, confidence=0.6)
-    plt.scatter(X[unlbld_idx,0], X[unlbld_idx,1], c='gray')
-    plt.scatter(X[:,0], X[:,1], c=y, cmap='jet')
-    plt.show()
-
-As output of this code snippet, we obtain the actively trained Gaussian process classifier
-including a visualization of its decision boundary and the sample utilities computed with
-uncertainty sampling.
+As a result, we obtain an actively trained Gaussian process classifier.
+A corresponding visualization of its decision boundary (black line) and the
+sample utilities (greenish contours) is given below.
 
 .. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/pal-example-output.png
    :width: 400
 
 Stream-based Active Learning
 ############################
 
-The following code implements an active learning cycle with 200 data points and
+The following code snippet implements an active learning cycle with 200 data points and
 the default budget of 10% using a pwc classifier and split uncertainty sampling. 
 Like in the pool-based example you can wrap other classifiers from ``sklearn``,
 ``sklearn`` compatible classifiers or like the example classifiers provided by ``skactiveml``.
 
 .. code-block:: python
 
     import numpy as np
-    import matplotlib.pyplot as plt
-    from scipy.ndimage import gaussian_filter1d
     from sklearn.datasets import make_blobs
     from skactiveml.classifier import ParzenWindowClassifier
     from skactiveml.stream import Split
     from skactiveml.utils import MISSING_LABEL
 
     # Generate data set.
     X, y_true = make_blobs(n_samples=200, centers=4, random_state=0)
@@ -196,38 +178,52 @@
         clf.fit(X_train, y_train)
         correct_classifications.append(clf.predict(X_cand)[0] == y_cand)
         sampled_indices = qs.query(candidates=X_cand, clf=clf)
         qs.update(candidates=X_cand, queried_indices=sampled_indices)
         X_train.append(x_t)
         y_train.append(y_cand if len(sampled_indices) > 0 else MISSING_LABEL)
 
-    # Plot the classifier's learning accuracy.
-    fig, ax = plt.subplots(1, 1, figsize=(8, 6))
-    ax.set_title(f'Learning curve', fontsize=15)
-    ax.set_xlabel('number of learning cycles')
-    ax.set_ylabel('accuracy')
-    ax.plot(gaussian_filter1d(np.array(correct_classifications, dtype=float), 4))
-    plt.show()
-
-As output of this code snippet, we obtain the actively trained pwc classifier incuding
-a visualization of its accuracy over the 200 samples.
+As a result, we obtain an actively trained Parzen window classifier.
+A corresponding visualization of its accuracy curve accross the active learning
+cycle is given below.
 
 .. image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/stream-example-output.png
    :width: 400
 
+Query Strategy Overview
+#######################
+
+For better orientation, we provide an `overview <https://scikit-activeml.github.io/scikit-activeml-docs/generated/strategy_overview.html>`_
+(incl. paper references and `visualizations <https://scikit-activeml.github.io/scikit-activeml-docs/generated/sphinx_gallery_examples/index.html>`_)
+of the query strategies implemented by ``skactiveml``.
+
+|Overview| |Visualization|
+
+.. |Overview| image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/strategy-overview.gif
+   :width: 400
+   
+.. |Visualization| image:: https://raw.githubusercontent.com/scikit-activeml/scikit-activeml/master/docs/logos/example-overview.gif
+   :width: 400
+
 .. examples_end
 
+.. citing_start
+
 Citing
 ======
-If you use ``scikit-activeml`` in one of your research projects and find it helpful,
+If you use ``skactiveml`` in one of your research projects and find it helpful,
 please cite the following:
 
 ::
 
     @article{skactiveml2021,
-        title={scikitactiveml: {A} {L}ibrary and {T}oolbox for {A}ctive {L}}earning {A}lgorithms},
+        title={scikit-activeml: {A} {L}ibrary and {T}oolbox for {A}ctive {L}earning {A}lgorithms},
         author={Daniel Kottke and Marek Herde and Tuan Pham Minh and Alexander Benz and Pascal Mergard and Atal Roghman and Christoph Sandrock and Bernhard Sick},
         journal={Preprints},
         doi={10.20944/preprints202103.0194.v1},
         year={2021},
         url={https://github.com/scikit-activeml/scikit-activeml}
-    }
+    }
+
+.. citing_end
+
+
```

### Comparing `scikit-activeml-0.4.0/scikit_activeml.egg-info/SOURCES.txt` & `scikit-activeml-0.4.1/scikit_activeml.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 skactiveml/classifier/multiannotator/tests/test_annotator_logistic_regression.py
 skactiveml/classifier/tests/__init__.py
 skactiveml/classifier/tests/test_classifier.py
 skactiveml/classifier/tests/test_mixture_model_classifier.py
 skactiveml/classifier/tests/test_parzen_window_classifier.py
 skactiveml/classifier/tests/test_wrapper.py
 skactiveml/pool/__init__.py
+skactiveml/pool/_batch_bald.py
 skactiveml/pool/_cost_embedding_al.py
 skactiveml/pool/_discriminative_al.py
 skactiveml/pool/_epistemic_uncertainty_sampling.py
 skactiveml/pool/_expected_error_reduction.py
 skactiveml/pool/_expected_model_change_maximization.py
 skactiveml/pool/_expected_model_output_change.py
 skactiveml/pool/_expected_model_variance.py
@@ -45,14 +46,15 @@
 skactiveml/pool/multiannotator/__init__.py
 skactiveml/pool/multiannotator/_interval_estimation_threshold.py
 skactiveml/pool/multiannotator/_wrapper.py
 skactiveml/pool/multiannotator/tests/__init__.py
 skactiveml/pool/multiannotator/tests/test_interval_estimation_threshold.py
 skactiveml/pool/multiannotator/tests/test_wrapper.py
 skactiveml/pool/tests/__init__.py
+skactiveml/pool/tests/test_batch_bald.py
 skactiveml/pool/tests/test_cost_embedding_al.py
 skactiveml/pool/tests/test_discriminative_al.py
 skactiveml/pool/tests/test_epistemic_uncertainty_sampling.py
 skactiveml/pool/tests/test_expected_error_reduction.py
 skactiveml/pool/tests/test_expected_model_change.py
 skactiveml/pool/tests/test_expected_model_output_change.py
 skactiveml/pool/tests/test_expected_model_variance.py
@@ -68,25 +70,29 @@
 skactiveml/regressor/__init__.py
 skactiveml/regressor/_nic_kernel_regressor.py
 skactiveml/regressor/_wrapper.py
 skactiveml/regressor/tests/__init__.py
 skactiveml/regressor/tests/test_nic_kernel_regressor.py
 skactiveml/regressor/tests/test_wrapper.py
 skactiveml/stream/__init__.py
+skactiveml/stream/_density_uncertainty.py
 skactiveml/stream/_stream_baselines.py
 skactiveml/stream/_stream_probabilistic_al.py
 skactiveml/stream/_uncertainty_zliobaite.py
 skactiveml/stream/budgetmanager/__init__.py
 skactiveml/stream/budgetmanager/_balanced_incremental_quantile_filter.py
 skactiveml/stream/budgetmanager/_estimated_budget_zliobaite.py
+skactiveml/stream/budgetmanager/_threshold_budget.py
 skactiveml/stream/budgetmanager/tests/__init__.py
 skactiveml/stream/budgetmanager/tests/test_balanced_incremental_quantile_filter.py
 skactiveml/stream/budgetmanager/tests/test_budget_manager.py
 skactiveml/stream/budgetmanager/tests/test_estimated_budget_zliobaite.py
+skactiveml/stream/budgetmanager/tests/test_threshold_budget.py
 skactiveml/stream/tests/__init__.py
+skactiveml/stream/tests/test_density_uncertainty.py
 skactiveml/stream/tests/test_stream.py
 skactiveml/stream/tests/test_stream_baselines.py
 skactiveml/stream/tests/test_stream_probabilistic_al.py
 skactiveml/stream/tests/test_uncertainty_zliobaite.py
 skactiveml/tests/__init__.py
 skactiveml/tests/template_query_strategy.py
 skactiveml/tests/test_base.py
```

### Comparing `scikit-activeml-0.4.0/setup.py` & `scikit-activeml-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/base.py` & `scikit-activeml-0.4.1/skactiveml/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -834,15 +834,15 @@
         # Check budget
         self._validate_budget()
         return utilities
 
 
 class SingleAnnotatorStreamQueryStrategy(QueryStrategy):
     """Base class for all stream-based active learning query strategies in
-       scikit-activeml.
+    scikit-activeml.
 
     Parameters
     ----------
     budget : float, default=None
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
     random_state : int, RandomState instance, default=None
@@ -856,19 +856,17 @@
     @abstractmethod
     def query(self, candidates, *args, return_utilities=False, **kwargs):
         """Ask the query strategy which instances in candidates to acquire.
 
         The query startegy determines the most useful instances in candidates,
         which can be acquired within the budgeting constraint specified by the
         budgetmanager.
-        Please note that, when the decisions from this function
-        may differ from the final sampling, simulate=True can set, so that the
-        query strategy can be updated later with update(...) with the final
-        sampling. This is especially helpful, when developing wrapper query
-        strategies.
+        Please note that, this method does not alter the internal state of the
+        query strategy. To adapt the query strategy to the selected candidates,
+        use update(...) with the selected candidates.
 
         Parameters
         ----------
         candidates : {array-like, sparse matrix} of shape
         (n_samples, n_features)
             The instances which may be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
```

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/_mixture_model_classifier.py` & `scikit-activeml-0.4.1/skactiveml/classifier/_mixture_model_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/_parzen_window_classifier.py` & `scikit-activeml-0.4.1/skactiveml/classifier/_parzen_window_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,17 +231,17 @@
                 F[i, :] = K[i, indices[i]] @ self.V_[indices[i], :]
         return F
 
     def _calculate_mean_gamma(
         N, variance, n_features, delta=(np.sqrt(2) * 1e-6)
     ):
         denominator = 2 * N * np.sum(variance)
-        numerator = (N - 1) * np.log((N - 1) / delta ** 2)
+        numerator = (N - 1) * np.log((N - 1) / delta**2)
         if denominator <= 0:
-            gamma = 1/n_features
+            gamma = 1 / n_features
             warnings.warn(
                 "The variance of the provided data is 0. Bandwidth of "
                 + f"1/n_features={gamma} is used instead."
-                )
+            )
         else:
             gamma = 0.5 * numerator / denominator
         return gamma
```

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/_wrapper.py` & `scikit-activeml-0.4.1/skactiveml/classifier/_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,17 @@
                 "are counted and will be used to make predictions. "
                 "The class label distribution is `_label_counts={}`.".format(
                     e, self._label_counts
                 )
             )
         return self
 
+    def __sklearn_is_fitted__(self):
+        return hasattr(self, "is_fitted_")
+
     def __getattr__(self, item):
         if "estimator_" in self.__dict__:
             return getattr(self.estimator_, item)
         else:
             return getattr(self.estimator, item)
```

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/_annotator_ensemble_classifier.py` & `scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/_annotator_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/_annotator_logistic_regression.py` & `scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/_annotator_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/tests/test_annotator_ensemble_classifier.py` & `scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/tests/test_annotator_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/multiannotator/tests/test_annotator_logistic_regression.py` & `scikit-activeml-0.4.1/skactiveml/classifier/multiannotator/tests/test_annotator_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/tests/test_classifier.py` & `scikit-activeml-0.4.1/skactiveml/classifier/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/tests/test_mixture_model_classifier.py` & `scikit-activeml-0.4.1/skactiveml/classifier/tests/test_mixture_model_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/tests/test_parzen_window_classifier.py` & `scikit-activeml-0.4.1/skactiveml/classifier/tests/test_parzen_window_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/classifier/tests/test_wrapper.py` & `scikit-activeml-0.4.1/skactiveml/classifier/tests/test_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import unittest
 import warnings
 
 import numpy as np
+from sklearn.datasets import make_blobs
+from sklearn.preprocessing import StandardScaler
 from sklearn.ensemble import BaggingClassifier
 from sklearn.gaussian_process import (
     GaussianProcessClassifier,
     GaussianProcessRegressor,
 )
 from sklearn.linear_model import Perceptron
+from sklearn.pipeline import Pipeline
 from sklearn.naive_bayes import GaussianNB
 from sklearn.utils.validation import NotFittedError, check_is_fitted
 
 from skactiveml.classifier import (
     SklearnClassifier,
     SlidingWindowClassifier,
     ParzenWindowClassifier,
@@ -168,14 +171,37 @@
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter("always")
             y = clf.predict(X=self.X)
             self.assertEqual(len(w), 1)
         y_exp = ["tokyo"] * len(self.X)
         np.testing.assert_array_equal(y_exp, y)
 
+    def test_pipeline(self):
+        X, y_true = make_blobs(100, centers=2, random_state=0)
+        pipline = Pipeline(
+            (
+                ("scaler", StandardScaler()),
+                ("gpc", GaussianProcessClassifier(random_state=0)),
+            )
+        )
+        clf = SklearnClassifier(
+            pipline, classes=[0, 1], missing_label=-1, random_state=0
+        )
+        clf = clf.fit(X, y_true)
+        self.assertTrue(clf.is_fitted_)
+        check_is_fitted(clf)
+        self.assertRaises(NotFittedError, check_is_fitted, pipline)
+        self.assertGreaterEqual(clf.score(X, y_true), 0.9)
+        y_missing = np.full_like(y_true, -1)
+        clf.fit(X, y_missing)
+        self.assertFalse(clf.is_fitted_)
+        check_is_fitted(clf)
+        p = clf.predict_proba(X)
+        np.testing.assert_array_equal(np.full_like(p, 0.5), p)
+
 
 class TestSlidingWindowClassifier(unittest.TestCase):
     def setUp(self):
         self.X = np.zeros((4, 1))
         self.y1 = ["tokyo", "paris", "nan", "tokyo"]
         self.y2 = ["tokyo", "nan", "nan", "tokyo"]
         self.y3 = [0, 1, 0, 0]
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/__init__.py` & `scikit-activeml-0.4.1/skactiveml/pool/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The :mod:`skactiveml.pool` package implements query strategies for
 pool-based active learning.
 """
 
 from . import multiannotator
 from . import utils
+from ._batch_bald import BatchBALD, batch_bald
 from ._cost_embedding_al import CostEmbeddingAL
 from ._discriminative_al import DiscriminativeAL
 from ._epistemic_uncertainty_sampling import EpistemicUncertaintySampling
 from ._expected_error_reduction import MonteCarloEER, ValueOfInformationEER
 from ._expected_model_change_maximization import (
     ExpectedModelChangeMaximization,
 )
@@ -54,8 +55,10 @@
     "ExpectedModelChangeMaximization",
     "ExpectedModelOutputChange",
     "ExpectedModelVarianceReduction",
     "KLDivergenceMaximization",
     "GreedySamplingX",
     "GreedySamplingTarget",
     "DiscriminativeAL",
+    "BatchBALD",
+    "batch_bald",
 ]
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_cost_embedding_al.py` & `scikit-activeml-0.4.1/skactiveml/pool/_cost_embedding_al.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_discriminative_al.py` & `scikit-activeml-0.4.1/skactiveml/pool/_discriminative_al.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_epistemic_uncertainty_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/_epistemic_uncertainty_sampling.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_expected_error_reduction.py` & `scikit-activeml-0.4.1/skactiveml/pool/_expected_error_reduction.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_expected_model_change_maximization.py` & `scikit-activeml-0.4.1/skactiveml/pool/_expected_model_change_maximization.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_expected_model_output_change.py` & `scikit-activeml-0.4.1/skactiveml/pool/_expected_model_output_change.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_expected_model_variance.py` & `scikit-activeml-0.4.1/skactiveml/pool/_expected_model_variance.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_four_ds.py` & `scikit-activeml-0.4.1/skactiveml/pool/_four_ds.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_greedy_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/_greedy_sampling.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_information_gain_maximization.py` & `scikit-activeml-0.4.1/skactiveml/pool/_information_gain_maximization.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_probabilistic_al.py` & `scikit-activeml-0.4.1/skactiveml/pool/_probabilistic_al.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,18 +169,15 @@
                 "clf has no predict_freq and metric was set to None"
             )
 
         # Fit the classifier and predict frequencies.
         if fit_clf:
             clf = clone(clf).fit(X, y, sample_weight)
         if self.metric is not None:
-            if (
-                self.metric_dict is None
-                and self.metric == "rbf"
-            ):
+            if self.metric_dict is None and self.metric == "rbf":
                 self.metric_dict = {"gamma": "mean"}
             pwc = ParzenWindowClassifier(
                 metric=self.metric,
                 metric_dict=self.metric_dict,
                 missing_label=clf.missing_label,
                 classes=clf.classes,
             )
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_query_by_committee.py` & `scikit-activeml-0.4.1/skactiveml/pool/_query_by_committee.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_quire.py` & `scikit-activeml-0.4.1/skactiveml/pool/_quire.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         utilities_cand = np.full((len(X)), fill_value=np.nan)
         y_labeled_ovr = _one_versus_rest_transform(
             y[mask_l], classes_, l_rest=-1
         )
         for i, s in enumerate(mapping):
             mask_u = mask_a.copy()
             mask_u[s] = False
-            L_uu_inv = _del_i_inv(L_aa_inv, i, 'L_aa_inv')
+            L_uu_inv = _del_i_inv(L_aa_inv, i, "L_aa_inv")
 
             utilities_cand[s] = L[s, s] + np.max(
                 [
                     yl.T.dot(L[mask_l][:, mask_l]).dot(yl)
                     + 2 * L[s][mask_l].dot(yl)
                     - (L[mask_u][:, mask_l].dot(yl) + L[mask_u][:, [s]])
                     .T.dot(L_uu_inv)
@@ -229,21 +229,23 @@
     y_ovr = np.full((len(classes), len(y)), fill_value=l_rest, dtype=dtype)
     for i, c in enumerate(classes):
         y_ovr[i, (y == c)] = l_one
         y_ovr[i, (np.isnan(y))] = missing_label
     return y_ovr.T
 
 
-def _del_i_inv(A_inv, s, name='A'):
+def _del_i_inv(A_inv, s, name="A"):
     if not np.allclose(A_inv, A_inv.T):
-        err = (np.abs(A_inv - A_inv.T))
-        warnings.warn(f'The approximation of the inverse of matrix `{name}` '
-                      f'may be inaccurate because the matrix is not symmetric '
-                      f'with an absolut error of \n{err}.\n To avoid this '
-                      f'warning you can increase `lmbda`.')
+        err = np.abs(A_inv - A_inv.T)
+        warnings.warn(
+            f"The approximation of the inverse of matrix `{name}` "
+            f"may be inaccurate because the matrix is not symmetric "
+            f"with an absolut error of \n{err}.\n To avoid this "
+            f"warning you can increase `lmbda`."
+        )
 
     a = A_inv[s, s]
     b = np.delete(A_inv[:, [s]], s, axis=0)
     D = np.delete(np.delete(A_inv, [s], axis=0), [s], axis=1)
     B_inv = D - (1 / a) * np.dot(b, b.T)
     return B_inv
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_random_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/_random_sampling.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/_uncertainty_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/_uncertainty_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
             )
         if mapping is not None and not len(X) == len(utility_weight):
             raise ValueError(
                 f"'utility_weight' must have length 'n_samples' but "
                 f"{len(utility_weight)} != {len(X)}."
             )
 
-
         # Validate method.
         if not isinstance(self.method, str):
             raise TypeError(
                 "{} is an invalid type for method. Type {} is "
                 "expected".format(type(self.method), str)
             )
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/multiannotator/_interval_estimation_threshold.py` & `scikit-activeml-0.4.1/skactiveml/pool/multiannotator/_interval_estimation_threshold.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/multiannotator/_wrapper.py` & `scikit-activeml-0.4.1/skactiveml/pool/multiannotator/_wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/multiannotator/tests/test_interval_estimation_threshold.py` & `scikit-activeml-0.4.1/skactiveml/pool/multiannotator/tests/test_interval_estimation_threshold.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/multiannotator/tests/test_wrapper.py` & `scikit-activeml-0.4.1/skactiveml/pool/multiannotator/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_cost_embedding_al.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_cost_embedding_al.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_discriminative_al.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_discriminative_al.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_epistemic_uncertainty_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_epistemic_uncertainty_sampling.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_error_reduction.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_error_reduction.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_model_change.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_model_change.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_model_output_change.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_model_output_change.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_expected_model_variance.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_expected_model_variance.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_four_ds.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_four_ds.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_greedy_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_greedy_sampling.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_information_gain_maximization.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_information_gain_maximization.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_probabilistic_al.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_probabilistic_al.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,17 @@
         self._test_param("init", "prior", test_cases)
 
     def test_init_param_m_max(self):
         test_cases = [(-2, ValueError), (1.5, TypeError)]
         self._test_param("init", "m_max", test_cases)
 
     def test_init_param_metric_dict(self):
-        pal = ProbabilisticAL(
-            metric="rbf", metric_dict=["gamma"]
-        )
+        pal = ProbabilisticAL(metric="rbf", metric_dict=["gamma"])
         self.assertRaises(TypeError, pal.query, **(self.kwargs))
-        pal = ProbabilisticAL(
-            metric="rbf", metric_dict={"test": 0}
-        )
+        pal = ProbabilisticAL(metric="rbf", metric_dict={"test": 0})
         self.assertRaises(TypeError, pal.query, **(self.kwargs))
 
     def test_init_param_metric(self):
         pal = ProbabilisticAL(metric="string")
         self.assertRaises(ValueError, pal.query, **(self.kwargs))
         pal = ProbabilisticAL(metric=0)
         self.assertRaises(ValueError, pal.query, **(self.kwargs))
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_query_by_committee.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_query_by_committee.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,29 @@
         test_cases = [] if test_cases is None else test_cases
         test_cases += [(1, TypeError), ("string", TypeError)]
         self._test_param("init", "method", test_cases)
 
     def test_query_param_ensemble(self, test_cases=None):
         estimators = [
             ("pwc1", ParzenWindowClassifier()),
-            ("pwc2", ParzenWindowClassifier())
+            ("pwc2", ParzenWindowClassifier()),
         ]
         vote = SklearnClassifier(
             VotingClassifier(estimators=estimators, voting="soft"),
-            classes=[0, 1])
+            classes=[0, 1],
+        )
         test_cases = [(vote, None)]
         self._test_param(
             "query",
             "ensemble",
             test_cases,
-            replace_query_params={"fit_ensemble": True,
-                                  "y": np.full(4, np.nan)}
+            replace_query_params={
+                "fit_ensemble": True,
+                "y": np.full(4, np.nan),
+            },
         )
         test_cases = [] if test_cases is None else test_cases
         test_cases += [
             (None, TypeError),
             ("test", TypeError),
             (1, TypeError),
             (ParzenWindowClassifier(classes=self.classes), TypeError),
@@ -111,18 +114,17 @@
         vote = vote.fit(X=X, y=y)
         pwc_list = [ParzenWindowClassifier(), ParzenWindowClassifier()]
         test_cases = [(vote, None), (pwc_list, NotFittedError)]
         self._test_param(
             "query",
             "ensemble",
             test_cases,
-            replace_query_params={"fit_ensemble": False}
+            replace_query_params={"fit_ensemble": False},
         )
 
-
     def test_query_param_y(self, test_cases=None):
         y = self.query_default_params_clf["y"]
         test_cases = [(y, None), (np.vstack([y, y]), ValueError)]
         self._test_param("query", "y", test_cases, exclude_reg=True)
 
         for ml, classes, t, err in [
             (np.nan, [1.0, 2.0], float, None),
@@ -154,23 +156,32 @@
     def test_query_param_fit_ensemble(self, test_cases=None):
         test_cases = [] if test_cases is None else test_cases
         test_cases += [("string", TypeError), (None, TypeError)]
         self._test_param("query", "fit_ensemble", test_cases)
 
     def test_query(self):
         voting_classifiers = [
-            ("gp1", SklearnClassifier(
-                classes=self.classes, estimator=GaussianProcessClassifier()
-            )),
-            ("gp2", SklearnClassifier(
-                classes=self.classes, estimator=GaussianProcessClassifier()
-            )),
-            ("gp3", SklearnClassifier(
-                classes=self.classes, estimator=GaussianProcessClassifier()
-            )),
+            (
+                "gp1",
+                SklearnClassifier(
+                    classes=self.classes, estimator=GaussianProcessClassifier()
+                ),
+            ),
+            (
+                "gp2",
+                SklearnClassifier(
+                    classes=self.classes, estimator=GaussianProcessClassifier()
+                ),
+            ),
+            (
+                "gp3",
+                SklearnClassifier(
+                    classes=self.classes, estimator=GaussianProcessClassifier()
+                ),
+            ),
         ]
         ensemble_classifiers = [member[1] for member in voting_classifiers]
         gpc = ParzenWindowClassifier(classes=self.classes)
         ensemble_bagging = SklearnClassifier(
             estimator=BaggingClassifier(estimator=gpc),
             classes=self.classes,
         )
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_quire.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_quire.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_random_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_random_sampling.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_uncertainty_sampling.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_uncertainty_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,21 +76,26 @@
         X = self.query_default_params_clf["X"]
         test_cases = [
             ("string", ValueError),
             (X, ValueError),
             (np.empty((len(X) - 1)), ValueError),
         ]
         self._test_param("query", "utility_weight", test_cases)
-        self._test_param("query", "utility_weight", [(np.ones(2), ValueError)],
-                         replace_query_params={'candidates': [2]})
-        self._test_param("query", "utility_weight",
-                         [(np.ones(len(X)-1), ValueError)],
-                         replace_query_params={'candidates': np.ones_like(X)})
-
-
+        self._test_param(
+            "query",
+            "utility_weight",
+            [(np.ones(2), ValueError)],
+            replace_query_params={"candidates": [2]},
+        )
+        self._test_param(
+            "query",
+            "utility_weight",
+            [(np.ones(len(X) - 1), ValueError)],
+            replace_query_params={"candidates": np.ones_like(X)},
+        )
 
     def test_query(self):
         compare_list = []
         random_state = np.random.RandomState(42)
         clf = SklearnClassifier(
             estimator=GaussianProcessClassifier(),
             random_state=random_state,
@@ -100,22 +105,25 @@
         X = random_state.rand(100, 10)
         y = random_state.randint(0, 2, (100,))
 
         # utility_weight
         qs = UncertaintySampling()
         utility_weight = np.arange(len(candidates))
         idx, utils_w = qs.query(
-            X, y, clf, candidates=candidates, utility_weight=utility_weight,
-            return_utilities=True
+            X,
+            y,
+            clf,
+            candidates=candidates,
+            utility_weight=utility_weight,
+            return_utilities=True,
         )
         idx, utils = qs.query(
             X, y, clf, candidates=candidates, return_utilities=True
         )
-        np.testing.assert_array_equal(utils*utility_weight, utils_w)
-
+        np.testing.assert_array_equal(utils * utility_weight, utils_w)
 
         # query
         qs = UncertaintySampling(method="entropy")
         compare_list.append(qs.query(X, y, clf, candidates=candidates))
 
         qs = UncertaintySampling(method="margin_sampling")
         compare_list.append(qs.query(X, y, clf, candidates=candidates))
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/tests/test_utils.py` & `scikit-activeml-0.4.1/skactiveml/pool/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 from scipy.stats import norm
 from sklearn.exceptions import NotFittedError
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import pairwise_kernels
 from sklearn.naive_bayes import GaussianNB
+from sklearn.datasets import make_blobs
 
 from skactiveml.classifier import ParzenWindowClassifier, SklearnClassifier
 from skactiveml.pool.utils import _cross_entropy
 from skactiveml.pool.utils import (
     IndexClassifierWrapper,
     _conditional_expect,
     _reshape_scipy_dist,
@@ -35,15 +36,15 @@
 )
 
 
 class TestIndexClassifierWrapper(unittest.TestCase):
     def setUp(self):
         self.X = np.linspace(0, 1, 4).reshape(-1, 1)
         self.y = np.array([0, 1, MISSING_LABEL, MISSING_LABEL])
-        self.y2 = np.array([0, 1, 0, 1])
+        self.y2 = np.array([0.0, 1.0, 0.0, 1.0])
         self.y3 = np.array([0, MISSING_LABEL, MISSING_LABEL, MISSING_LABEL])
         self.clf = ParzenWindowClassifier(classes=[0, 1])
         self.kwargs = dict(X=self.X, y=self.y, clf=self.clf)
         self.iclf = lambda **kw: IndexClassifierWrapper(
             self.clf, self.X, self.y, **kw
         )
 
@@ -52,14 +53,34 @@
         self.assertRaises(
             TypeError, IndexClassifierWrapper, clf="str", X=self.X, y=self.y
         )
         clf = self.clf.fit(self.X, self.y)
         iclf = IndexClassifierWrapper(clf=clf, X=self.X, y=self.y)
         np.testing.assert_array_equal(clf.X_, iclf.clf_.X_)
 
+    def test_dtype_error(self):
+        X, y = make_blobs(
+            n_samples=2000, centers=[(-2, 2), (2, -2)], n_features=2
+        )
+        clf = ParzenWindowClassifier(
+            classes=np.unique(y), missing_label=MISSING_LABEL
+        )
+        y_known = np.full(len(y), MISSING_LABEL)
+        self.assertRaises(
+            TypeError,
+            IndexClassifierWrapper,
+            clf=clf,
+            X=X,
+            y=y,
+            missing_label=MISSING_LABEL,
+        )
+        y = y.astype(float)
+        id_clf = IndexClassifierWrapper(clf, X, y, missing_label=MISSING_LABEL)
+        id_clf.fit(np.arange(len(X)), y_known, set_base_clf=True)
+
     def test_init_param_X(self):
         self.assertTrue(hasattr(self.iclf(), "X"))
         self.assertRaises(
             (ValueError, TypeError),
             IndexClassifierWrapper,
             clf=self.clf,
             X="str",
```

### Comparing `scikit-activeml-0.4.0/skactiveml/pool/utils.py` & `scikit-activeml-0.4.1/skactiveml/pool/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     clf : skactiveml.base.SkactivemlClassifier
         The base classifier implementing the methods `fit` and `predict_proba`.
     X : array-like of shape (n_samples, n_features)
         Training data set, usually complete, i.e. including the labeled and
         unlabeled samples.
     y : array-like of shape (n_samples)
         Labels of the training data set (possibly including unlabeled ones
-        indicated by self.missing_label.
+        indicated by self.missing_label).
     sample_weight : array-like of shape (n_samples), optional (default=None)
         Weights of training samples in `X`.
     set_base_clf : bool, default=False
         If True, the base classifier will be set to the newly fitted
         classifier
     ignore_partial_fit : bool, optional (default: True)
         Specifies if the `partial_fit` function of `self.clf` should be used
@@ -93,14 +93,21 @@
         self.use_speed_up = use_speed_up
         self.missing_label = missing_label
 
         # Validate classifier type.
         check_type(self.clf, "clf", SkactivemlClassifier)
 
         # Check X, y, sample_weight: will be done by base clf
+        self.X = check_array(self.X, allow_nd="True")
+        self.y = check_array(
+            self.y,
+            ensure_2d=False,
+            force_all_finite=False,
+            dtype=None,
+        )
         check_consistent_length(self.X, self.y)
 
         if self.sample_weight is not None:
             check_consistent_length(self.X, self.sample_weight)
 
         check_type(set_base_clf, "set_base_clf", bool)
 
@@ -138,14 +145,20 @@
 
         # Check use_speed_up
         check_type(self.use_speed_up, "use_speed_up", bool)
 
         # Check missing label
         check_missing_label(self.missing_label)
         self.missing_label_ = self.missing_label
+        if not np.issubdtype(type(self.missing_label), self.y.dtype):
+            raise TypeError(
+                f"`missing_label` has type {type(missing_label)}, "
+                f"which is not compatible with {self.y.dtype} as the "
+                f"type of `y`."
+            )
         check_equal_missing_label(self.clf.missing_label, self.missing_label_)
 
         # prepare ParzenWindowClassifier
         if isinstance(self.clf, ParzenWindowClassifier) and self.use_speed_up:
             self.pwc_metric_ = self.clf.metric
             self.pwc_metric_dict_ = (
                 {} if self.clf.metric_dict is None else self.clf.metric_dict
@@ -176,18 +189,22 @@
             will be used later. Can be of value 'all', 'labeled', or
             'unlabeled'.
         pred_params : string, optional (default='all')
             Parameter to specify if only a subset of the `idx_predict` indices
             will be used later. Can be of value 'all', 'labeled', or
             'unlabeled'.
         """
-        idx_fit = check_array(idx_fit, ensure_2d=False, dtype=int)
+        idx_fit = check_array(
+            idx_fit, ensure_2d=False, dtype=int, input_name="`idx_fit`"
+        )
         idx_fit = check_indices(idx_fit, self.X, dim=0)
 
-        idx_pred = check_array(idx_pred, ensure_2d=False, dtype=int)
+        idx_pred = check_array(
+            idx_pred, ensure_2d=False, dtype=int, input_name="`idx_pred`"
+        )
         idx_pred = check_indices(idx_pred, self.X, dim=0)
 
         # precompute ParzenWindowClassifier
         if isinstance(self.clf, ParzenWindowClassifier) and self.use_speed_up:
             if fit_params == "all":
                 idx_fit_ = idx_fit
             elif fit_params == "labeled":
@@ -253,15 +270,15 @@
         Returns
         -------
         self: IndexClassifierWrapper,
             The fitted IndexClassifierWrapper.
 
         """
         # check idx
-        idx = check_array(idx, ensure_2d=False, dtype=int)
+        idx = check_array(idx, ensure_2d=False, dtype=int, input_name="`idx`")
         idx = check_indices(
             idx, self.X, dim=0, unique=self.enforce_unique_samples
         )
 
         # check set_base_clf
         check_type(set_base_clf, "set_base_clf", bool)
 
@@ -270,27 +287,30 @@
             y = self.y[idx]
             if is_unlabeled(y, missing_label=self.missing_label_).all():
                 warnings.warn("All labels are of `missing_label` in `fit`.")
         else:
             y = check_array(
                 y,
                 ensure_2d=False,
-                force_all_finite="allow-nan",
+                force_all_finite=False,
                 dtype=self.y.dtype,
+                input_name="`y`",
             )
             check_consistent_length(idx, y)
 
         # check sample_weight
         if sample_weight is None:
             sample_weight = self._copy_sw(
                 self._get_sw(self.sample_weight, idx=idx)
             )
             # TODO deepcopy
         else:
-            sample_weight = check_array(sample_weight, ensure_2d=False)
+            sample_weight = check_array(
+                sample_weight, ensure_2d=False, input_name="`sample_weight`"
+            )
             check_consistent_length(sample_weight, y)
 
         # check if a clf_ exists
         if "clf_" not in self.__dict__:
             self.clf_ = clone(self.clf)
 
         # fit classifier
@@ -345,15 +365,17 @@
         -------
         self: IndexClassifierWrapper,
             The fitted IndexClassifierWrapper.
 
         """
 
         # check idx
-        add_idx = check_array(idx, ensure_2d=False, dtype=int)
+        add_idx = check_array(
+            idx, ensure_2d=False, dtype=int, input_name="`add_idx`"
+        )
         add_idx = check_indices(
             add_idx, self.X, dim=0, unique=self.enforce_unique_samples
         )
 
         # check use_base_clf
         check_type(use_base_clf, "use_base_clf", bool)
 
@@ -381,26 +403,29 @@
                 warnings.warn(
                     "All labels are of `missing_label` in " "`partial_fit`."
                 )
         else:
             add_y = check_array(
                 y,
                 ensure_2d=False,
-                force_all_finite="allow-nan",
+                force_all_finite=False,
                 dtype=self.y.dtype,
+                input_name="`y`",
             )
             check_consistent_length(add_idx, add_y)
 
         # check sample_weight
         if sample_weight is None:
             add_sample_weight = self._copy_sw(
                 self._get_sw(self.sample_weight, idx=add_idx)
             )
         else:
-            add_sample_weight = check_array(sample_weight, ensure_2d=False)
+            add_sample_weight = check_array(
+                sample_weight, ensure_2d=False, input_name="`sample_weight`"
+            )
             check_consistent_length(add_idx, add_sample_weight)
 
         # handle case when partial fit of clf is used
         if self.use_partial_fit:
             if use_base_clf:
                 self.clf_ = deepcopy(self.base_clf_)
 
@@ -723,40 +748,47 @@
     -------
     X_new : np.ndarray of shape (n_new_samples, n_features)
         The new training data set.
     y_new : np.ndarray of shape (n_new_samples)
         The new labels.
     """
 
-    X = check_array(X)
-    y = column_or_1d(check_array(y, force_all_finite=False, ensure_2d=False))
+    X = check_array(X, input_name="`X`")
+    y = column_or_1d(
+        check_array(
+            y, force_all_finite=False, ensure_2d=False, input_name="`y`"
+        )
+    )
     check_consistent_length(X, y)
 
     if isinstance(y_update, (int, float)):
         y_update = np.array([y_update])
     else:
         y_update = check_array(
             y_update,
             force_all_finite=False,
             ensure_2d=False,
             ensure_min_samples=0,
+            input_name="`y`",
         )
         y_update = column_or_1d(y_update)
 
     if idx_update is not None:
         if isinstance(idx_update, (int, np.integer)):
             idx_update = np.array([idx_update])
         idx_update = check_indices(idx_update, A=X, unique="check_unique")
         check_consistent_length(y_update, idx_update)
         X_new = X.copy()
         y_new = y.copy()
         y_new[idx_update] = y_update
         return X_new, y_new
     elif X_update is not None:
-        X_update = check_array(X_update, ensure_2d=False)
+        X_update = check_array(
+            X_update, ensure_2d=False, input_name="`X_update`"
+        )
         if X_update.ndim == 1:
             X_update = X_update.reshape(1, -1)
         check_consistent_length(X.T, X_update.T)
         check_consistent_length(y_update, X_update)
         X_new = np.append(X, X_update, axis=0)
         y_new = np.append(y, y_update, axis=0)
         return X_new, y_new
@@ -950,15 +982,15 @@
 
     Returns
     -------
     expectation : numpy.ndarray of shape (n_samples)
         The conditional expectation for each value applied.
     """
 
-    X = check_array(X, allow_nd=True)
+    X = check_array(X, allow_nd=True, input_name="`X`")
 
     check_type(reg, "reg", ProbabilisticRegressor)
     check_type(
         method,
         "method",
         target_vals=[
             "monte_carlo",
```

### Comparing `scikit-activeml-0.4.0/skactiveml/regressor/_nic_kernel_regressor.py` & `scikit-activeml-0.4.1/skactiveml/regressor/_nic_kernel_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/regressor/_wrapper.py` & `scikit-activeml-0.4.1/skactiveml/regressor/_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,17 @@
         """
         check_is_fitted(self)
         if hasattr(self.estimator_, "sample_y"):
             return self.estimator_.sample_y(X, n_samples, random_state)
         else:
             return self.estimator_.sample(X, n_samples)
 
+    def __sklearn_is_fitted__(self):
+        return hasattr(self, "_label_mean")
+
     def __getattr__(self, item):
         if "estimator_" in self.__dict__:
             return getattr(self.estimator_, item)
         else:
             return getattr(self.estimator, item)
```

### Comparing `scikit-activeml-0.4.0/skactiveml/regressor/tests/test_nic_kernel_regressor.py` & `scikit-activeml-0.4.1/skactiveml/regressor/tests/test_nic_kernel_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/regressor/tests/test_wrapper.py` & `scikit-activeml-0.4.1/skactiveml/regressor/tests/test_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import numpy as np
 from sklearn import clone
 from sklearn.exceptions import NotFittedError
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.linear_model import LinearRegression, ARDRegression, SGDRegressor
 from sklearn.neural_network import MLPRegressor
 from sklearn.svm import SVC
+from sklearn.preprocessing import PolynomialFeatures
+from sklearn.pipeline import Pipeline
+from sklearn.utils.validation import check_is_fitted
 
 from skactiveml.base import SkactivemlRegressor
 from skactiveml.regressor._wrapper import (
     SklearnRegressor,
     SklearnNormalRegressor,
 )
 from skactiveml.utils import MISSING_LABEL
@@ -144,14 +147,35 @@
 
         reg_1.partial_fit(X, y)
         reg_2.fit(X, y)
         self.assertTrue(
             np.any(np.not_equal(reg_1.predict(X), reg_2.predict(X)))
         )
 
+    def test_pipeline(self):
+        X = np.linspace(-3, 3, 100)
+        y_true = X**2
+        X = X.reshape(-1, 1)
+        pipline = Pipeline(
+            (
+                ("scaler", PolynomialFeatures(degree=2)),
+                ("lr", LinearRegression()),
+            )
+        )
+        reg = SklearnRegressor(pipline, missing_label=np.nan, random_state=0)
+        reg = reg.fit(X, y_true)
+        check_is_fitted(reg)
+        self.assertRaises(NotFittedError, check_is_fitted, pipline)
+        self.assertGreaterEqual(reg.score(X, y_true), 0.9)
+        y_missing = np.full_like(y_true, np.nan)
+        reg.fit(X, y_missing)
+        check_is_fitted(reg)
+        y_pred = reg.predict(X)
+        np.testing.assert_array_equal(np.zeros_like(y_pred), y_pred)
+
 
 class TestSklearnProbabilisticRegressor(unittest.TestCase):
     def setUp(self):
         self.X = np.array([[0, 1], [1, 0], [2, 3]])
         self.y = np.array([1, 2, 3])
         self.X_cand = np.array([[2, 1], [3, 5]])
```

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/_stream_baselines.py` & `scikit-activeml-0.4.1/skactiveml/stream/_stream_baselines.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,24 @@
     with a probability of 10%. Instances are queried regardless of their
     position in the feature space. As this query strategy disregards any
     information about the instance. Thus, it should only be used as a baseline
     strategy.
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
 
-    allow_exceeding_budget : bool, default=True
+    allow_exceeding_budget : bool, optional (default=True)
         If True, the query strategy is allowed to exceed it's budget as long as
         the average number of queries will be within the budget. If False,
         queries are not allowed if the budget is exhausted.
 
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the estimator.
     """
 
     def __init__(
         self, budget=None, allow_exceeding_budget=True, random_state=None
     ):
         super().__init__(budget=budget, random_state=random_state)
@@ -47,15 +47,15 @@
         Parameters
         ----------
         candidates : array-like or sparse matrix of shape
         (n_samples, n_features)
             The instances which may be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
 
-        return_utilities : bool, optional
+        return_utilities : bool, optional (default=False)
             If true, also return the utilities based on the query strategy.
             The default is False.
 
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances in candidates which should be queried,
@@ -115,17 +115,14 @@
         (n_samples, n_features)
             The instances which could be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
 
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
-        budget_manager_param_dict : kwargs
-            Optional kwargs for budgetmanager.
-
         Returns
         -------
         self : StreamRandomSampling
             The RandomSampling returns itself, after it is updated.
         """
         # check if a random state is set
         self._validate_data([[0]], False)
@@ -151,15 +148,15 @@
         Parameters
         ----------
         candidates: array-like of shape (n_candidates, n_features)
             The instances which could be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
         return_utilities : bool,
             If true, also return the utilities based on the query strategy.
-        reset : bool, default=True
+        reset : bool, optional (default=True)
             Whether to reset the `n_features_in_` attribute.
             If False, the input will be checked for consistency with data
             provided when reset was last True.
         **check_candidates_params : kwargs
             Parameters passed to :func:`sklearn.utils.check_array`.
 
         Returns
@@ -199,19 +196,19 @@
     exhaust a given budget as soon it is available. Instances are queried
     regardless of their position in the feature space. As this query strategy
     disregards any information about the instance. Thus, it should only be used
     as a baseline strategy.
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
 
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the estimator.
     """
 
     def __init__(self, budget=None, random_state=None):
         super().__init__(budget=budget, random_state=random_state)
 
     def query(self, candidates, return_utilities=False):
@@ -228,15 +225,15 @@
         Parameters
         ----------
         candidates : array-like or sparse matrix of shape
         (n_samples, n_features)
             The instances which may be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
 
-        return_utilities : bool, optional
+        return_utilities : bool, optional (default=False)
             If true, also return the utilities based on the query strategy.
             The default is False.
 
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances in candidates which should be queried,
@@ -288,17 +285,14 @@
         (n_samples, n_features)
             The instances which could be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
 
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
-        budget_manager_param_dict : kwargs
-            Optional kwargs for budgetmanager.
-
         Returns
         -------
         self : PeriodicSampling
             The PeriodicSampler returns itself, after it is updated.
         """
         # check if a budgetmanager is set
         self._validate_data(np.array([[0]]), False)
@@ -320,15 +314,15 @@
         Parameters
         ----------
         candidates: array-like of shape (n_candidates, n_features)
             The instances which could be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
         return_utilities : bool,
             If true, also return the utilities based on the query strategy.
-        reset : bool, default=True
+        reset : bool, optional (default=True)
             Whether to reset the `n_features_in_` attribute.
             If False, the input will be checked for consistency with data
             provided when reset was last True.
         **check_candidates_params : kwargs
             Parameters passed to :func:`sklearn.utils.check_array`.
 
         Returns
```

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/_stream_probabilistic_al.py` & `scikit-activeml-0.4.1/skactiveml/stream/_stream_probabilistic_al.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,68 +16,66 @@
     check_scalar,
     call_func,
     check_budget_manager,
 )
 
 
 class StreamProbabilisticAL(SingleAnnotatorStreamQueryStrategy):
-    """Probabilistic Active Learning in Datastreams.
+    """StreamProbabilisticAL
 
     Probabilistic Active Learning in Datastreams (StreamProbabilisticAL) is an
     extension to Multi-Class Probabilistic Active Learning (McPAL)
     (see pool.ProbabilisticAL). It assesses McPAL spatial to assess the spatial
     utility. The Balanced Incremental Quantile Filter
     (BalancedIncrementalQuantileFilter), that is implemented within the
     default budget manager, is used to evaluate the temporal utility
     (see stream.budgetmanager.BalancedIncrementalQuantileFilter).
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
-    budget_manager : BudgetManager, default=None
+    budget_manager : BudgetManager, optional (default=None)
         The BudgetManager which models the budgeting constraint used in
         the stream-based active learning setting. if set to None,
-        FixedUncertaintyBudgetManager will be used by default. The budget
+        BalancedIncrementalQuantileFilter will be used by default. The budget
         manager will be initialized based on the following conditions:
             If only a budget is given the default budget manager is initialized
             with the given budget.
             If only a budget manager is given use the budget manager.
             If both are not given the default budget manager with the
             default budget.
             If both are given and the budget differs from budgetmanager.budget
             a warning is thrown.
-    metric : str or callable, default=None
+    metric : str or callable, optional (default=None)
         The metric must a be None or a valid kernel as defined by the function
         `sklearn.metrics.pairwise.pairwise_kernels`. The kernel is used to
         calculate the frequency of labels near the candidates and multiplied
         with the probabilities returned by the `clf` to get a kernel frequency
         estimate for each class.
         If metric is set to None, the `predict_freq` function of the `clf` will
         be used instead. If this is not defined, an Exception is raised.
-    metric_dict : dict, default=None
+    metric_dict : dict, optional (default=None)
         Any further parameters are passed directly to the kernel function.
         If metric_dict is None and metric is 'rbf' metric_dict is set to
         {'gamma': 'mean'}.
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the query strategy.
-    prior : float
+    prior : float, optional (default=1.0e-3)
         The prior value that is passed onto ProbabilisticAL
         (see pool.ProbabilisticAL).
-    m_max : float
+    m_max : float, optional (default=2)
         The m_max value that is passed onto ProbabilisticAL
         (see pool.ProbabilisticAL).
 
     References
     ----------
-    [1] Kottke D., Krempl G., Spiliopoulou M. (2015) Probabilistic Active
-        Learning in Datastreams. In: Fromont E., De Bie T., van Leeuwen M.
-        (eds) Advances in Intelligent Data Analysis XIV. IDA 2015. Lecture
-        Notes in Computer Science, vol 9385. Springer, Cham.
+    [1] Kottke, M. (2015). Probabilistic Active Learning in Datastreams. In
+        Advances in Intelligent Data Analysis XIV (pp. 145–157). Springer.
     """
 
     def __init__(
         self,
         budget_manager=None,
         budget=None,
         metric=None,
@@ -108,31 +106,39 @@
 
         Parameters
         ----------
         candidates : {array-like, sparse matrix} of shape
         (n_samples, n_features)
             The instances which may be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
+
         clf : SkactivemlClassifier
             Model implementing the methods `fit` and `predict_proba`. If
             `self.metric` is None, the `clf` must also implement
             `predict_freq`.
+
         X : array-like of shape (n_samples, n_features), optional
         (default=None)
             Input samples used to fit the classifier.
+
         y : array-like of shape (n_samples), optional (default=None)
             Labels of the input samples 'X'. There may be missing labels.
-        sample_weight : array-like of shape (n_samples,) (default=None)
+
+        sample_weight : array-like of shape (n_samples,), optional
+        (default=None)
             Sample weights for X, used to fit the clf.
-        fit_clf : bool,
+
+        fit_clf : bool,optional (default=False)
             If True, refit the classifier also requires X and y to be given.
+
         utility_weight : array-like of shape (n_candidate_samples), optional
         (default=None)
             Densities for each sample in `candidates`.
-        return_utilities : bool, optional
+
+        return_utilities : bool, optional (default=False)
             If true, also return the utilities based on the query strategy.
             The default is False.
 
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances in candidates which should be queried,
@@ -157,18 +163,15 @@
             y=y,
             sample_weight=sample_weight,
             fit_clf=fit_clf,
             utility_weight=utility_weight,
             return_utilities=return_utilities,
         )
         if self.metric is not None:
-            if (
-                self.metric_dict is None
-                and self.metric == "rbf"
-            ):
+            if self.metric_dict is None and self.metric == "rbf":
                 self.metric_dict = {"gamma": "mean"}
             pwc = ParzenWindowClassifier(
                 metric=self.metric,
                 metric_dict=self.metric_dict,
                 missing_label=clf.missing_label,
                 classes=clf.classes,
             )
@@ -197,17 +200,19 @@
 
         Parameters
         ----------
         candidates : {array-like, sparse matrix} of shape
         (n_samples, n_features)
             The instances which could be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
+
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
-        budget_manager_param_dict : kwargs, optional
+
+        budget_manager_param_dict : kwargs, optional (default=None)
             Optional kwargs for budgetmanager.
 
         Returns
         -------
         self : StreamProbabilisticAL
             PALS returns itself, after it is updated.
         """
@@ -260,24 +265,23 @@
             Model implementing the methods `fit` and `predict_proba`. If
             `self.metric` is None, the `clf` must also implement
             `predict_freq`.
         X : array-like of shape (n_samples, n_features)
             Input samples used to fit the classifier.
         y : array-like of shape (n_samples)
             Labels of the input samples 'X'. There may be missing labels.
-        sample_weight : array-like of shape (n_samples,) (default=None)
+        sample_weight : array-like of shape (n_samples,)
             Sample weights for X, used to fit the clf.
         fit_clf : bool,
             If true, refit the classifier also requires X and y to be given.
-        utility_weight: array-like of shape (n_candidate_samples), optional
-        (default=None)
+        utility_weight: array-like of shape (n_candidate_samples)
             Densities for each sample in `candidates`.
         return_utilities : bool,
             If true, also return the utilities based on the query strategy.
-        reset : bool, default=True
+        reset : bool, optional (default=True)
             Whether to reset the `n_features_in_` attribute.
             If False, the input will be checked for consistency with data
             provided when reset was last True.
         **check_candidates_params : kwargs
             Parameters passed to :func:`sklearn.utils.check_array`.
 
         Returns
@@ -290,16 +294,15 @@
             Checked training samples
         y: np.ndarray, shape (n_candidates)
             Checked training labels
         sampling_weight: np.ndarray, shape (n_candidates)
             Checked training sample weight
         fit_clf : bool,
             Checked boolean value of `fit_clf`
-        utility_weight: array-like of shape (n_candidate_samples), optional
-        (default=None)
+        utility_weight: array-like of shape (n_candidate_samples)
             Checked densities for each sample in `candidates`.
         candidates: np.ndarray, shape (n_candidates, n_features)
             Checked candidate samples
         return_utilities : bool,
             Checked boolean value of `return_utilities`.
         """
         candidates, return_utilities = super()._validate_data(
@@ -358,15 +361,15 @@
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             Input samples used to fit the classifier.
         y : array-like of shape (n_samples)
             Labels of the input samples 'X'. There may be missing labels.
-        sample_weight : array-like of shape (n_samples,) (default=None)
+        sample_weight : array-like of shape (n_samples,)
             Sample weights for X, used to fit the clf.
 
         Returns
         -------
         X : array-like of shape (n_samples, n_features)
             Checked Input samples.
         y : array-like of shape (n_samples)
@@ -390,15 +393,15 @@
         ----------
         clf : SkactivemlClassifier
             Model implementing the methods `fit` and `predict_freq`.
         X : array-like of shape (n_samples, n_features)
             Input samples used to fit the classifier.
         y : array-like of shape (n_samples)
             Labels of the input samples 'X'. There may be missing labels.
-        sample_weight : array-like of shape (n_samples,) (default=None)
+        sample_weight : array-like of shape (n_samples,)
             Sample weights for X, used to fit the clf.
 
         Returns
         -------
         clf : SkactivemlClassifier
             Checked model implementing the methods `fit` and `predict_freq`.
         """
@@ -413,22 +416,20 @@
         """Validate if utility_weight is numeric and of equal length as
         candidates.
 
         Parameters
         ----------
         candidates: np.ndarray, shape (n_candidates, n_features)
             Checked candidate samples
-        utility_weight: array-like of shape (n_candidate_samples), optional
-        (default=None)
+        utility_weight: array-like of shape (n_candidate_samples)
             Densities for each sample in `candidates`.
 
         Returns
         -------
-        utility_weight : array-like of shape (n_candidate_samples), optional
-        (default=None)
+        utility_weight : array-like of shape (n_candidate_samples)
             Checked densities for each sample in `candidates`.
         """
         if utility_weight is None:
             utility_weight = np.ones(len(candidates))
         utility_weight = check_array(utility_weight, ensure_2d=False)
         check_consistent_length(utility_weight, candidates)
         return utility_weight
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/_uncertainty_zliobaite.py` & `scikit-activeml-0.4.1/skactiveml/stream/_uncertainty_zliobaite.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,48 +17,47 @@
     check_type,
     call_func,
     check_budget_manager,
 )
 
 
 class UncertaintyZliobaite(SingleAnnotatorStreamQueryStrategy):
-    """The UncertaintyZliobaite (Utility calculation in [1]) query strategy
-    samples instances based on the classifiers uncertainty assessed based on
-    the classifier's predictions. The instance is queried when the probability
-    of the most likely class exceeds a threshold calculated based on the budget
-    and the number of classes. It is used as the base class for uncertainty
-    strategies provided by Zliobaite in [1].
+    """UncertaintyZliobaite
+
+    The UncertaintyZliobaite class provides the base for query strategies
+    proposed by Žliobaitė et al. in [1]. The strategies evaluate the
+    classifier's uncertainty based on its predictions and instances' labels are
+    queried when the uncertainty exceeds a specific threshold. Žliobaitė et al.
+    propose various techniques to calculate such a threshold.
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
-
-    budget_manager : BudgetManager, default=None
+    budget_manager : BudgetManager, optional (default=None)
         The BudgetManager which models the budgeting constraint used in
         the stream-based active learning setting. if set to None,
         FixedUncertaintyBudgetManager will be used by default. The
         budget manager will be initialized based on the following conditions:
             If only a budget is given the default budget manager is initialized
             with the given budget.
             If only a budget manager is given use the budget manager.
             If both are not given the default budget manager with the
             default budget.
             If both are given and the budget differs from budgetmanager.budget
             a warning is thrown.
-
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the estimator.
 
     References
     ----------
-    [1] Zliobaite, Indre & Bifet, Albert & Pfahringer, Bernhard & Holmes,
-        Geoffrey. (2014). Active Learning With Drifting Streaming Data. Neural
-        Networks and Learning Systems, IEEE Transactions on. 25. 27-39.
+    [1] Žliobaitė, I., Bifet, A., Pfahringer, B., & Holmes, G. (2014). Active
+        Learning With Drifting Streaming Data. IEEE Transactions on Neural
+        Networks and Learning Systems, 25(1), 27-39.
 
     """
 
     def __init__(
         self,
         budget_manager=None,
         budget=None,
@@ -75,36 +74,33 @@
         y=None,
         sample_weight=None,
         fit_clf=False,
         return_utilities=False,
     ):
         """Ask the query strategy which instances in candidates to acquire.
 
-        Please note that, when the decisions from this function may differ from
-        the final sampling, simulate=True can be set, so that the query
-        strategy can be updated later with update(...) with the final sampling.
-        This is especially helpful when developing wrapper query strategies.
-
         Parameters
         ----------
         candidates : {array-like, sparse matrix} of shape
         (n_samples, n_features)
             The instances which may be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
         clf : SkactivemlClassifier
             Model implementing the methods `fit` and `predict_freq`.
         X : array-like of shape (n_samples, n_features), optional
+        (default=None)
             Input samples used to fit the classifier.
-        y : array-like of shape (n_samples), optional
+        y : array-like of shape (n_samples), optional (default=None)
             Labels of the input samples 'X'. There may be missing labels.
         sample_weight : array-like of shape (n_samples,), optional
+        (default=None)
             Sample weights for X, used to fit the clf.
-        fit_clf : bool,
+        fit_clf : bool, optional (default=False)
             If true, refit the classifier also requires X and y to be given.
-        return_utilities : bool, optional
+        return_utilities : bool, optional (default=False)
             If true, also return the utilities based on the query strategy.
             The default is False.
 
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances in candidates which should be queried,
@@ -129,15 +125,16 @@
             y=y,
             sample_weight=sample_weight,
             fit_clf=fit_clf,
             return_utilities=return_utilities,
         )
 
         predict_proba = clf.predict_proba(candidates)
-        utilities = np.max(predict_proba, axis=1)
+        confidence = np.max(predict_proba, axis=1)
+        utilities = 1 - confidence
 
         queried_indices = self.budget_manager_.query_by_utility(utilities)
 
         if return_utilities:
             return queried_indices, utilities
         else:
             return queried_indices
@@ -154,15 +151,15 @@
         (n_samples, n_features)
             The instances which could be queried. Sparse matrices are accepted
             only if they are supported by the base query strategy.
 
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
-        budget_manager_param_dict : kwargs
+        budget_manager_param_dict : kwargs, optional (default=None)
             Optional kwargs for budget manager.
 
         Returns
         -------
         self : UncertaintyZliobaite
             The UncertaintyZliobaite returns itself, after it is updated.
         """
@@ -215,21 +212,21 @@
             only if they are supported by the base query strategy.
         clf : SkactivemlClassifier
             Model implementing the methods `fit` and `predict_freq`.
         X : array-like of shape (n_samples, n_features)
             Input samples used to fit the classifier.
         y : array-like of shape (n_samples)
             Labels of the input samples 'X'. There may be missing labels.
-        sample_weight : array-like of shape (n_samples,) (default=None)
+        sample_weight : array-like of shape (n_samples,)
             Sample weights for X, used to fit the clf.
         return_utilities : bool,
             If true, also return the utilities based on the query strategy.
         fit_clf : bool,
             If true, refit the classifier also requires X and y to be given.
-        reset : bool, default=True
+        reset : bool, optional (default=True)
             Whether to reset the `n_features_in_` attribute.
             If False, the input will be checked for consistency with data
             provided when reset was last True.
         **check_candidates_params : kwargs
             Parameters passed to :func:`sklearn.utils.check_array`.
 
         Returns
@@ -287,15 +284,15 @@
         ----------
         clf : SkactivemlClassifier
             Model implementing the methods `fit` and `predict_freq`.
         X : array-like of shape (n_samples, n_features)
             Input samples used to fit the classifier.
         y : array-like of shape (n_samples)
             Labels of the input samples 'X'. There may be missing labels.
-        sample_weight : array-like of shape (n_samples,) (default=None)
+        sample_weight : array-like of shape (n_samples,)
             Sample weights for X, used to fit the clf.
         fit_clf : bool,
             If true, refit the classifier also requires X and y to be given.
         Returns
         -------
         clf : SkactivemlClassifier
             Checked model implementing the methods `fit` and `predict_freq`.
@@ -314,15 +311,15 @@
         ----------
         X : array-like of shape (n_samples, n_features)
             Input samples used to fit the classifier.
 
         y : array-like of shape (n_samples)
             Labels of the input samples 'X'. There may be missing labels.
 
-        sample_weight : array-like of shape (n_samples,) (default=None)
+        sample_weight : array-like of shape (n_samples,)
             Sample weights for X, used to fit the clf.
 
         Returns
         -------
         X : array-like of shape (n_samples, n_features)
             Checked Input samples.
         y : array-like of shape (n_samples)
@@ -336,47 +333,47 @@
             X = check_array(X)
             y = np.array(y)
             check_consistent_length(X, y)
         return X, y, sample_weight
 
 
 class FixedUncertainty(UncertaintyZliobaite):
-    """The FixedUncertainty (Fixed-Uncertainty in [1]) query strategy samples
+    """FixedUncertainty
+
+    The FixedUncertainty (Fixed-Uncertainty in [1]) query strategy samples
     instances based on the classifiers uncertainty assessed based on the
     classifier's predictions. The instance is queried when the probability of
     the most likely class exceeds a threshold calculated based on the budget
     and the number of classes.
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
-
-    budgetmanager : BudgetManager, default=None
+    budgetmanager : BudgetManager, optional (default=None)
         The BudgetManager which models the budgeting constraint used in
         the stream-based active learning setting. if set to None,
         FixedUncertaintyBudgetManager will be used by default. The budget
         manager will be initialized based on the following conditions:
             If only a budget is given the default budget manager is initialized
             with the given budget.
             If only a budget manager is given use the budget manager.
             If both are not given the default budget manager with the
             default budget.
             If both are given and the budget differs from budget manager.budget
             a warning is thrown.
-
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the estimator.
 
     References
     ----------
-    [1] Zliobaite, Indre & Bifet, Albert & Pfahringer, Bernhard & Holmes,
-        Geoffrey. (2014). Active Learning With Drifting Streaming Data. Neural
-        Networks and Learning Systems, IEEE Transactions on. 25. 27-39.
+    [1] Žliobaitė, I., Bifet, A., Pfahringer, B., & Holmes, G. (2014). Active
+        Learning With Drifting Streaming Data. IEEE Transactions on Neural
+        Networks and Learning Systems, 25(1), 27-39.
 
     """
 
     def _get_default_budget_manager(self):
         """Provide the budget manager that will be used as default.
 
         Returns
@@ -384,142 +381,139 @@
         budgetmanager : BudgetManager
             The BudgetManager that should be used by default.
         """
         return FixedUncertaintyBudgetManager
 
 
 class VariableUncertainty(UncertaintyZliobaite):
-    """The VariableUncertainty (Var-Uncertainty in [1]) query strategy samples
+    """VariableUncertainty
+
+    The VariableUncertainty (Var-Uncertainty in [1]) query strategy samples
     instances based on the classifiers uncertainty assessed based on the
     classifier's predictions. The instance is queried when the probability of
     the most likely class exceeds a time-dependent threshold calculated based
     on the budget, the number of classes and the number of observed and
     acquired samples.
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
-
-    budgetmanager : BudgetManager, default=None
+    budgetmanager : BudgetManager, optional (default=None)
         The BudgetManager which models the budgeting constraint used in
         the stream-based active learning setting. if set to None,
-        FixedUncertaintyBudgetManager will be used by default. The budget
+        VariableUncertaintyBudgetManager will be used by default. The budget
         manager will be initialized based on the following conditions:
             If only a budget is given the default budgetmanager is initialized
             with the given budget.
             If only a budgetmanager is given use the budgetmanager.
             If both are not given the default budgetmanager with the
             default budget.
             If both are given and the budget differs from budgetmanager.budget
             a warning is thrown.
-
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the estimator.
 
     References
     ----------
-    [1] Zliobaite, Indre & Bifet, Albert & Pfahringer, Bernhard & Holmes,
-        Geoffrey. (2014). Active Learning With Drifting Streaming Data. Neural
-        Networks and Learning Systems, IEEE Transactions on. 25. 27-39.
-
+    [1] Žliobaitė, I., Bifet, A., Pfahringer, B., & Holmes, G. (2014). Active
+        Learning With Drifting Streaming Data. IEEE Transactions on Neural
+        Networks and Learning Systems, 25(1), 27-39.
     """
 
     def _get_default_budget_manager(self):
         """Provide the budget manager that will be used as default.
 
         Returns
         -------
         budgetmanager : BudgetManager
             The BudgetManager that should be used by default.
         """
         return VariableUncertaintyBudgetManager
 
 
 class RandomVariableUncertainty(UncertaintyZliobaite):
-    """The RandomVariableUncertainty (Ran-Var-Uncertainty in [1]) query
+    """RandomVariableUncertainty
+
+    The RandomVariableUncertainty (Ran-Var-Uncertainty in [1]) query
     strategy samples instances based on the classifier's uncertainty assessed
     based on the classifier's predictions. The instance is queried when the
     probability of the most likely class exceeds a time-dependent threshold
     calculated based on the budget, the number of classes and the number of
     observed and acquired samples. To better adapt at change detection the
     threshold is multiplied by a random number generator with N(1,delta).
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
-
-    budgetmanager : BudgetManager, default=None
+    budgetmanager : BudgetManager, optional (default=None)
         The BudgetManager which models the budgeting constraint used in
         the stream-based active learning setting. if set to None,
-        FixedUncertaintyBudgetManager will be used by default. The budget
-        manager will be initialized based on the following conditions:
+        RandomVariableUncertaintyBudgetManager will be used by default. The
+        budget manager will be initialized based on the following conditions:
             If only a budget is given the default budgetmanager is initialized
             with the given budget.
             If only a budgetmanager is given use the budgetmanager.
             If both are not given the default budgetmanager with the
             default budget.
             If both are given and the budget differs from budgetmanager.budget
             a warning is thrown.
-
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the estimator.
 
     References
     ----------
-    [1] Zliobaite, Indre & Bifet, Albert & Pfahringer, Bernhard & Holmes,
-        Geoffrey. (2014). Active Learning With Drifting Streaming Data. Neural
-        Networks and Learning Systems, IEEE Transactions on. 25. 27-39.
-
+    [1] Žliobaitė, I., Bifet, A., Pfahringer, B., & Holmes, G. (2014). Active
+        Learning With Drifting Streaming Data. IEEE Transactions on Neural
+        Networks and Learning Systems, 25(1), 27-39.
     """
 
     def _get_default_budget_manager(self):
         """Provide the budget manager that will be used as default.
 
         Returns
         -------
         budgetmanager : BudgetManager
             The BudgetManager that should be used by default.
         """
         return RandomVariableUncertaintyBudgetManager
 
 
 class Split(UncertaintyZliobaite):
-    """The Split [1] query strategy samples in 100*v% of instances randomly and
+    """Split
+
+    The Split [1] query strategy samples in 100*v% of instances randomly and
     in 100*(1-v)% of cases according to VariableUncertainty.
 
     Parameters
     ----------
-    budget : float, default=None
+    budget : float, optional (default=None)
         The budget which models the budgeting constraint used in
         the stream-based active learning setting.
-
-    budgetmanager : BudgetManager, default=None
+    budgetmanager : BudgetManager, optional (default=None)
         The BudgetManager which models the budgeting constraint used in
         the stream-based active learning setting. if set to None,
-        FixedUncertaintyBudgetManager will be used by default. The budget
+        SplitBudgetManager will be used by default. The budget
         manager will
         be initialized based on the following conditions:
             If only a budget is given the default budget manager is initialized
             with the given budget.
             If only a budgetmanager is given use the budgetmanager.
             If both are not given the default budgetmanager with the
             default budget.
             If both are given and the budget differs from budgetmanager.budget
             a warning is thrown.
-
-    random_state : int, RandomState instance, default=None
+    random_state : int, RandomState instance, optional (default=None)
         Controls the randomness of the estimator.
 
     References
     ----------
-    [1] Zliobaite, Indre & Bifet, Albert & Pfahringer, Bernhard & Holmes,
-        Geoffrey. (2014). Active Learning With Drifting Streaming Data. Neural
-        Networks and Learning Systems, IEEE Transactions on. 25. 27-39.
-
+    [1] Žliobaitė, I., Bifet, A., Pfahringer, B., & Holmes, G. (2014). Active
+        Learning With Drifting Streaming Data. IEEE Transactions on Neural
+        Networks and Learning Systems, 25(1), 27-39.
     """
 
     def _get_default_budget_manager(self):
         return SplitBudgetManager
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/_balanced_incremental_quantile_filter.py` & `scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/_balanced_incremental_quantile_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     a threshold that is derived from a quantile (budget) of the last w observed
     utilities.
     To balance the number of queries, w_tol is used to increase or decrease the
     threshold based on the number of available acquisitions.
 
     Parameters
     ----------
-    w : int
+    w : int, optional (default=100)
         The number of observed utilities that are used to infer the threshold.
         w should be higher than 0.
 
-    w_tol : int
+    w_tol : int, optional (default=50)
         The window in which the number of acquisitions should stay within the
         budget. w_tol should be higher than 0.
 
-    budget : float
+    budget : float, optional (default=None)
         Specifies the ratio of instances which are allowed to be queried, with
-        0 <= budget <= 1.
+        0 <= budget <= 1. See Also :class:`BudgetManager`.
 
     References
     ----------
     [1] Kottke D., Krempl G., Spiliopoulou M. (2015) Probabilistic Active
         Learning in Datastreams. In: Fromont E., De Bie T., van Leeuwen M.
         (eds) Advances in Intelligent Data Analysis XIV. IDA 2015. Lecture
         Notes in Computer Science, vol 9385. Springer, Cham.
@@ -93,18 +93,23 @@
         return queried_indices
 
     def update(self, candidates, queried_indices, utilities):
         """Updates the budget manager.
 
         Parameters
         ----------
+        candidates : {array-like, sparse matrix} of shape
+        (n_samples, n_features)
+            The instances which could be queried. Sparse matrices are accepted
+            only if they are supported by the base query strategy.
+
         queried_indices : array-like
             Indicates which instances from candidates have been queried.
 
-        utilities : ndarray of shape (n_samples,), optional
+        utilities : ndarray of shape (n_samples,)
             The utilities based on the query strategy.
 
         Returns
         -------
         self : EstimatedBudget
             The EstimatedBudget returns itself, after it is updated.
         """
```

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/_estimated_budget_zliobaite.py` & `scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/_estimated_budget_zliobaite.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,45 +3,58 @@
 import numpy as np
 
 from ...base import BudgetManager
 from ...utils import check_random_state, check_scalar
 
 
 class EstimatedBudgetZliobaite(BudgetManager):
-    """Budget manager which checks, whether the specified budget has been
+    """EstimatedBudgetZliobaite
+
+    Budget manager which checks, whether the specified budget has been
     exhausted already. If not, an instance is queried, when the utility is
     higher than the specified budget.
 
-    This budget manager calculates the estimated budget spent in the last
+    This budget manager calculates the estimated budget [1] spent in the last
     w steps and compares that to the budget. If the ratio is smaller
     than the specified budget, i.e., budget - u_t / w > 0, the budget
     manager samples an instance when its utility is higher than the budget.
     u is the estimate of how many true lables were queried within the last
     w steps. The incremental funktion, u_t = u_t-1 * (w-1) / w + labeling_t,
     is used to calculate u at time t.
 
     Parameters
     ----------
-    budget : float
+    budget : float, optional (default=None)
         Specifies the ratio of instances which are allowed to be queried, with
-        0 <= budget <= 1.
-    w : int
+        0 <= budget <= 1. See Also :class:`BudgetManager`.
+    w : int, optional (default=100)
         Specifies the size of the memory window. Controlles the budget in the
         last w steps taken. Default = 100
+
+    References
+    ----------
+    [1] Žliobaitė, I., Bifet, A., Pfahringer, B., & Holmes, G. (2014). Active
+        Learning With Drifting Streaming Data. IEEE Transactions on Neural
+        Networks and Learning Systems, 25(1), 27-39.
     """
 
     def __init__(self, budget=None, w=100):
         super().__init__(budget)
         self.w = w
 
     def update(self, candidates, queried_indices):
         """Updates the budget manager.
 
         Parameters
         ----------
+        candidates : {array-like, sparse matrix} of shape
+        (n_samples, n_features)
+            The instances which could be queried. Sparse matrices are accepted
+            only if they are supported by the base query strategy.
+
         queried : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
         Returns
         -------
         self : EstimatedBudgetZliobaite
             The EstimatedBudgetZliobaite returns itself, after it is updated.
@@ -75,30 +88,32 @@
         if not hasattr(self, "u_t_"):
             self.u_t_ = 0
 
         return utilities
 
 
 class FixedUncertaintyBudgetManager(EstimatedBudgetZliobaite):
-    """Budget manager which is optimized for FixedUncertainty and checks,
+    """FixedUncertaintyBudgetManager
+
+    Budget manager which is optimized for FixedUncertainty and checks,
     whether the specified budget has been exhausted already. If not, an
     instance is queried, when the utility is higher than the specified budget
     and the probability of the most likely class exceeds a threshold
     calculated based on the budget and the number of classes.
     See also :class:`.EstimatedBudgetZliobaite`
 
     Parameters
     ----------
-    budget : float
+    budget : float, optional (default=None)
         Specifies the ratio of instances which are allowed to be queried, with
-        0 <= budget <= 1.
-    w : int
+        0 <= budget <= 1. See Also :class:`BudgetManager`.
+    w : int, optional (default=100)
         Specifies the size of the memory window. Controlles the budget in the
         last w steps taken. Default = 100
-    num_classes : int
+    num_classes : int, optional (default=2)
         Specifies the number of classes. Default = 2
     """
 
     def __init__(self, budget=None, w=100, num_classes=2):
         super().__init__(budget, w)
         self.num_classes = num_classes
 
@@ -119,46 +134,52 @@
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances represented by utilities which should be
             queried, with 0 <= n_queried_instances <= n_samples.
         """
         utilities = self._validate_data(utilities)
+        confidence = 1 - utilities
 
         # intialize return parameters
         queried_indices = []
         budget_left = []
         # calculate theta with num_classes
         theta = 1 / self.num_classes + self.budget_ * (
             1 - 1 / self.num_classes
         )
 
         # keep the internal state to reset it later if simulate is true
         tmp_u_t = self.u_t_
 
-        samples = np.array(utilities) <= theta
+        samples = np.array(confidence) <= theta
         # check for each sample separately if budget is left and the utility is
         # high enough
         for i, d in enumerate(samples):
             budget_left.append(tmp_u_t / self.w < self.budget_)
             if not budget_left[-1]:
                 d = False
             # u_t = u_t-1 * (w-1)/w + labeling_t
             tmp_u_t = tmp_u_t * ((self.w - 1) / self.w) + d
             # get the indices instances that should be queried
             if d:
                 queried_indices.append(i)
 
-            return queried_indices
+        return queried_indices
 
     def update(self, candidates, queried_indices):
         """Updates the budget manager.
 
         Parameters
         ----------
+        candidates : {array-like, sparse matrix} of shape
+        (n_samples, n_features)
+            The instances which could be queried. Sparse matrices are accepted
+            only if they are supported by the base query strategy.
+
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
         Returns
         -------
         self : FixedUncertaintyBudgetManager
             The FixedUncertaintyBudget returns itself, after it is updated.
@@ -191,15 +212,17 @@
             min_inclusive=False,
         )
 
         return utilities
 
 
 class VariableUncertaintyBudgetManager(EstimatedBudgetZliobaite):
-    """Budget manager which checks, whether the specified budget has been
+    """VariableUncertaintyBudgetManager
+
+    Budget manager which checks, whether the specified budget has been
     exhausted already. If not, an instance is queried, when the utility is
     higher than the specified budget and when the probability of
     the most likely class exceeds a time-dependent threshold calculated based
     on the budget, the number of classes and the number of observed and
     acquired samples.
 
     This budget manager calculates the estimated budget spent in the last
@@ -210,24 +233,24 @@
     u is the estimate of how many true lables were queried within the last
     w steps. The recursive funktion,
     u_t = u_t-1 * (w-1) / w + labeling_t , is used to calculate u at time t.
     See also :class:`.EstimatedBudgetZliobaite`
 
     Parameters
     ----------
-    budget : float
+    budget : float, optional (default=None)
         Specifies the ratio of instances which are allowed to be queried, with
-        0 <= budget <= 1.
-    w : int
+        0 <= budget <= 1. See Also :class:`BudgetManager`.
+    w : int, optional (default=100)
         Specifies the size of the memory window. Controlles the budget in the
         last w steps taken. Default = 100
-    theta : float
+    theta : float, optional (default=1.0)
         Specifies the starting threshold in wich instances are purchased. This
         value of theta will recalculated after each instance. Default = 1
-    s : float
+    s : float, optional (default=0.1)
         Specifies the value in wich theta is decresed or increased based on the
         purchase of the given label. Default = 0.01
     """
 
     def __init__(self, budget=None, w=100, theta=1.0, s=0.01):
         super().__init__(budget, w)
         self.theta = theta
@@ -250,24 +273,25 @@
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances represented by utilities which should be
             queried, with 0 <= n_queried_instances <= n_samples.
         """
         utilities = self._validate_data(utilities)
+        confidence = 1 - utilities
 
         # intialize return parameters
         queried_indices = []
         budget_left = []
         # keep the internal state to reset it later if simulate is true
         tmp_u_t = self.u_t_
         tmp_theta = self.theta_
 
-        # get utilities
-        for i, u in enumerate(utilities):
+        # get confidence
+        for i, u in enumerate(confidence):
             budget_left.append(self.budget_ > tmp_u_t / self.w)
 
             if not budget_left[-1]:
                 sample = False
             else:
                 sample = u < tmp_theta
                 # get the indices instances that should be queried
@@ -282,14 +306,19 @@
         return queried_indices
 
     def update(self, candidates, queried_indices):
         """Updates the budget manager.
 
         Parameters
         ----------
+        candidates : {array-like, sparse matrix} of shape
+        (n_samples, n_features)
+            The instances which could be queried. Sparse matrices are accepted
+            only if they are supported by the base query strategy.
+
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
         Returns
         -------
         self : VariableUncertaintyBudgetManager
             The VariableUncertaintyBudget returns itself, after it is updated.
@@ -341,45 +370,50 @@
         check_scalar(self.theta, "theta", float)
         # check if theta exists
         if not hasattr(self, "theta_"):
             self.theta_ = self.theta
 
 
 class RandomVariableUncertaintyBudgetManager(EstimatedBudgetZliobaite):
-    """Budget manager which checks, whether the specified budget has been
+    """RandomVariableUncertaintyBudgetManager
+
+    Budget manager which checks, whether the specified budget has been
     exhausted already. If not, an instance is queried, when the utility is
     higher than the specified budget and when the probability of
     the most likely class exceeds a time-dependent threshold calculated based
     on the budget, the number of classes and the number of observed and
     acquired samples.
 
     This budget manager calculates the estimated budget spent in the last
     w steps and compares that to the budget. If the ratio is smaller
     than the specified budget, i.e.,
     budget - u_t / w > 0 , the budget
     manager samples an instance when its utility is higher than the budget.
     u is the estimate of how many true lables were queried within the last
     w steps. The recursive funktion,
     u_t = u_t-1 * (w-1) / w + labeling_t , is used to calculate u at time t.
-    See also :class:`.EstimatedBudgetZliobaite`
 
     Parameters
     ----------
-    budget : float
+    budget : float, optional (default=None)
         Specifies the ratio of instances which are allowed to be queried, with
-        0 <= budget <= 1.
-    w : int
+        0 <= budget <= 1. See Also :class:`BudgetManager`.
+    w : int, optional (default=100)
         Specifies the size of the memory window. Controlles the budget in the
         last w steps taken. Default = 100
-    theta : float
+    theta : float, optional (default=1)
         Specifies the starting threshold in wich instances are purchased. This
         value of theta will recalculated after each instance. Default = 1
-    s : float
+    s : float, optional (default=0.01)
         Specifies the value in wich theta is decresed or increased based on the
         purchase of the given label. Default = 0.01
+    delta : float, optional (default=1.0)
+        Specifies the standart deviation of the distribution. Default 1.0
+    random_state : int | np.random.RandomState, optional (default=None)
+        Random state for candidate selection.
     """
 
     def __init__(
         self,
         budget=None,
         w=100,
         theta=1.0,
@@ -410,26 +444,27 @@
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances represented by utilities which should be
             queried, with 0 <= n_queried_instances <= n_samples.
         """
         utilities = self._validate_data(utilities)
+        confidence = 1 - utilities
 
         # intialize return parameters
         queried_indices = []
         budget_left = []
         # keep the internal state to reset it later if simulate is true
         tmp_u_t = self.u_t_
         tmp_theta = self.theta_
 
         prior_random_state = self.random_state_.get_state()
 
-        # get utilities
-        for i, u in enumerate(utilities):
+        # get confidence
+        for i, u in enumerate(confidence):
             budget_left.append(self.budget_ > tmp_u_t / self.w)
 
             if not budget_left[-1]:
                 sample = False
             else:
 
                 eta = self.random_state_.normal(1, self.delta)
@@ -449,14 +484,19 @@
         return queried_indices
 
     def update(self, candidates, queried_indices):
         """Updates the budget manager.
 
         Parameters
         ----------
+        candidates : {array-like, sparse matrix} of shape
+        (n_samples, n_features)
+            The instances which could be queried. Sparse matrices are accepted
+            only if they are supported by the base query strategy.
+
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
         Returns
         -------
         self : RandomVariableUncertaintyBudgetManager
             The RandomVariableUncertaintyBudget returns itself, after it is
@@ -523,15 +563,17 @@
         """
         if not hasattr(self, "random_state_"):
             self.random_state_ = deepcopy(self.random_state)
         self.random_state_ = check_random_state(self.random_state_)
 
 
 class SplitBudgetManager(EstimatedBudgetZliobaite):
-    """Budget manager which checks, whether the specified budget has been
+    """SplitBudgetManager
+
+    Budget manager which checks, whether the specified budget has been
     exhausted already. If not, an instance is queried, when the utility is
     higher than the specified budget. 100*v% of instances will be queried
     randomly and in 100*(1-v)% of will be queried cases according
     to VariableUncertainty
 
     This budget manager calculates the estimated budget spent in the last
     w steps and compares that to the budget. If the ratio is smaller
@@ -540,32 +582,39 @@
     u is the estimate of how many true lables were queried within the last
     w steps. The recursive funktion,
     u_t = u_t-1 * (w-1) / w + labeling_t , is used to calculate u at time t.
     See also :class:`.EstimatedBudgetZliobaite`
 
     Parameters
     ----------
-    budget : float
+    budget : float, optional (default=None)
         Specifies the ratio of instances which are allowed to be queried, with
-        0 <= budget <= 1.
-    w : int
+        0 <= budget <= 1. See Also :class:`BudgetManager`.
+    w : int, optional (default=100)
         Specifies the size of the memory window. Controlles the budget in the
         last w steps taken. Default = 100
-    theta : float
+    theta : float, optional (default=1.0)
         Specifies the starting threshold in wich instances are purchased. This
         value of theta will recalculated after each instance. Default = 1
-    s : float
+    s : float, optional (default=0.01)
         Specifies the value in wich theta is decresed or increased based on the
         purchase of the given label. Default = 0.01
-    v : float
+    v : float, optional (default=0.1)
         Specifies the percent value of instances queried randomly.
+    random_state : int | np.random.RandomState, optional (default=None)
+        Random state for candidate selection.
+
+    See Also
+    --------
+    EstimatedBudgetZliobaite : BudgetManager implementing the base class for
+        Zliobaite based budget managers
     """
 
     def __init__(
-        self, budget=None, w=100, theta=1.0, s=0.01, v=0.1, random_state=0
+        self, budget=None, w=100, theta=1.0, s=0.01, v=0.1, random_state=None
     ):
         super().__init__(budget, w)
         self.v = v
         self.theta = theta
         self.s = s
         self.random_state = random_state
 
@@ -583,26 +632,27 @@
         Returns
         -------
         queried_indices : ndarray of shape (n_queried_instances,)
             The indices of instances represented by utilities which should be
             queried, with 0 <= n_queried_instances <= n_samples.
         """
         utilities = self._validate_data(utilities)
+        confidence = 1 - utilities
 
         # intialise return parameters
         queried_indices = []
         budget_left = []
         # keep the internal state to reset it later if simulate is true
         tmp_u_t = self.u_t_
         tmp_theta = self.theta_
         random_state_state = self.random_state_.get_state()
 
         # check for each queried separately if budget is left and the utility
         # is high enough
-        for i, u in enumerate(utilities):
+        for i, u in enumerate(confidence):
             budget_left.append(tmp_u_t / self.w < self.budget_)
             if not budget_left[-1]:
                 sample = False
             else:
                 # changed self.v < self.rand_.random_sample()
                 random_val = self.random_state_.random_sample()
                 if self.v > random_val:
@@ -627,14 +677,19 @@
         return queried_indices
 
     def update(self, candidates, queried_indices):
         """Updates the budget manager.
 
         Parameters
         ----------
+        candidates : {array-like, sparse matrix} of shape
+        (n_samples, n_features)
+            The instances which could be queried. Sparse matrices are accepted
+            only if they are supported by the base query strategy.
+
         queried_indices : array-like of shape (n_samples,)
             Indicates which instances from candidates have been queried.
 
         Returns
         -------
         self : SplitBudgetManager
             The SplitBudget returns itself, after it is updated.
@@ -698,9 +753,147 @@
 
     def _validate_random_state(self):
         """Creates a copy 'random_state_' if random_state is an instance of
         np.random_state. If not create a new random state. See also
         :func:`~sklearn.utils.check_random_state`
         """
         if not hasattr(self, "random_state_"):
+            self.random_state_ = deepcopy(self.random_state)
+        self.random_state_ = check_random_state(self.random_state_)
+
+
+class RandomBudgetManager(EstimatedBudgetZliobaite):
+    """RandomBudgetManager
+
+    Budget manager which checks, whether the specified budget has been
+    exhausted already. If not, an instance is queried, when the utility is
+    higher than the specified budget. If budget is available, budget% instances
+    are queried randomly.
+
+    This budget manager calculates the estimated budget spent in the last
+    w steps and compares that to the budget. If the ratio is smaller
+    than the specified budget, i.e., budget - u_t / w > 0 , the budget
+    manager samples an instance when its utility is higher than the budget.
+    u is the estimate of how many true lables were queried within the last
+    w steps. The recursive funktion,
+    u_t = u_t-1 * (w-1) / w + labeling_t , is used to calculate u at time t.
+    See also :class:`.EstimatedBudgetZliobaite`
+
+    Parameters
+    ----------
+    budget : float, optional (default=None)
+        Specifies the ratio of instances which are allowed to be queried, with
+        0 <= budget <= 1. See Also :class:`BudgetManager`.
+    w : int, optional (default=100)
+        Specifies the size of the memory window. Controlles the budget in the
+        last w steps taken. Default = 100
+    random_state : int | np.random.RandomState, optional (default=None)
+        Random state for candidate selection.
+    """
+
+    def __init__(self, budget=None, w=100, random_state=None):
+        super().__init__(budget, w)
+        self.random_state = random_state
+
+    def query_by_utility(self, utilities):
+        """Ask the budget manager which utilities are sufficient to query the
+        corresponding instance.
+
+        Parameters
+        ----------
+        utilities : ndarray of shape (n_samples,)
+            The utilities provided by the stream-based active learning
+            strategy, which are used to determine whether sampling an instance
+            is worth it given the budgeting constraint.
+
+        return_utilities : bool, optional
+            If true, also return whether there was budget left for each
+            assessed utility. The default is False.
+
+        Returns
+        -------
+        queried_indices : ndarray of shape (n_queried_instances,)
+            The indices of instances represented by utilities which should be
+            queried, with 0 <= n_queried_instances <= n_samples.
+        """
+        utilities = self._validate_data(utilities)
+        confidence = 1 - utilities
+
+        # intialize return parameters
+        queried_indices = []
+
+        # keep the internal state to reset it later if simulate is true
+        tmp_u_t = self.u_t_
+
+        prior_random_state = self.random_state_.get_state()
+
+        samples = (
+            self.random_state_.random_sample(len(confidence)) <= self.budget_
+        )
+        # check for each sample separately if budget is left and the utility is
+        # high enough
+        for i, d in enumerate(samples):
+            budget_left = tmp_u_t / self.w < self.budget_
+            d = d if budget_left else False
+            tmp_u_t = tmp_u_t * ((self.w - 1) / self.w) + (
+                d and not np.isnan(utilities[i])
+            )
+            # get the indices instances that should be queried
+            if d and not np.isnan(utilities[i]):
+                queried_indices.append(i)
+
+        self.random_state_.set_state(prior_random_state)
+
+        return queried_indices
+
+    def update(self, candidates, queried_indices):
+        """Updates the budget manager.
+
+        Parameters
+        ----------
+        candidates : {array-like, sparse matrix} of shape
+        (n_samples, n_features)
+            The instances which could be queried. Sparse matrices are accepted
+            only if they are supported by the base query strategy.
+
+        queried_indices : array-like of shape (n_samples,)
+            Indicates which instances from candidates have been queried.
+
+        Returns
+        -------
+        self : RandomBudgetManager
+            The RandomBudgetManager returns itself, after it is updated.
+        """
+        self._validate_data(np.array([]))
+        self.random_state_.random_sample(len(candidates))
+        super().update(candidates, queried_indices)
+        return self
+
+    def _validate_data(self, utilities):
+        """Validate input data.
+
+        Parameters
+        ----------
+        utilities: ndarray of shape (n_samples,)
+            The utilities provided by the stream-based active learning
+            strategy.
+
+        Returns
+        -------
+        utilities : ndarray of shape (n_samples,)
+            Checked utilities.
+        """
+
+        utilities = super()._validate_data(utilities)
+        check_scalar(self.w, "w", int, min_val=0, min_inclusive=False)
+        self._validate_random_state()
+
+        return utilities
+
+    def _validate_random_state(self):
+        """Creates a copy 'random_state_' if random_state is an instance of
+        np.random_state. If not create a new random state. See also
+        :func:`~sklearn.utils.check_random_state`
+        """
+        if not hasattr(self, "random_state_"):
             self.random_state_ = deepcopy(self.random_state)
         self.random_state_ = check_random_state(self.random_state_)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/test_balanced_incremental_quantile_filter.py` & `scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/test_balanced_incremental_quantile_filter.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/test_budget_manager.py` & `scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/test_budget_manager.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/budgetmanager/tests/test_estimated_budget_zliobaite.py` & `scikit-activeml-0.4.1/skactiveml/stream/budgetmanager/tests/test_estimated_budget_zliobaite.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 
 from skactiveml.stream.budgetmanager import (
     FixedUncertaintyBudgetManager,
     VariableUncertaintyBudgetManager,
     SplitBudgetManager,
     RandomVariableUncertaintyBudgetManager,
+    RandomBudgetManager,
 )
 
 
 class TemplateTestEstimatedBudgetZliobaite:
     def setUp(self):
         # initialise var for sampled var tests
         self.utilities = np.array([True, False])
@@ -208,7 +209,21 @@
         self.assertRaises(
             ValueError, budget_manager.query_by_utility, self.utilities
         )
         budget_manager = self.get_budget_manager()(v=-1.0)
         self.assertRaises(
             ValueError, budget_manager.query_by_utility, self.utilities
         )
+
+
+class TestRandomBudgetManager(
+    TemplateTestEstimatedBudgetZliobaite, unittest.TestCase
+):
+    def get_budget_manager(self):
+        return RandomBudgetManager
+
+    def test_init_param_random_state(self):
+        # v must be defined as an float with a range of: 0 < v < 1
+        budget_manager = self.get_budget_manager()(random_state="string")
+        self.assertRaises(
+            ValueError, budget_manager.query_by_utility, self.utilities
+        )
```

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/tests/test_stream.py` & `scikit-activeml-0.4.1/skactiveml/stream/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/tests/test_stream_baselines.py` & `scikit-activeml-0.4.1/skactiveml/stream/tests/test_stream_baselines.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/tests/test_stream_probabilistic_al.py` & `scikit-activeml-0.4.1/skactiveml/stream/tests/test_stream_probabilistic_al.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/stream/tests/test_uncertainty_zliobaite.py` & `scikit-activeml-0.4.1/skactiveml/stream/tests/test_uncertainty_zliobaite.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/tests/template_query_strategy.py` & `scikit-activeml-0.4.1/skactiveml/tests/template_query_strategy.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/tests/test_base.py` & `scikit-activeml-0.4.1/skactiveml/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/__init__.py` & `scikit-activeml-0.4.1/skactiveml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/_aggregation.py` & `scikit-activeml-0.4.1/skactiveml/utils/_aggregation.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/_functions.py` & `scikit-activeml-0.4.1/skactiveml/utils/_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 from functools import update_wrapper
 from operator import attrgetter
 
 
 def call_func(
     f_callable, only_mandatory=False, ignore_var_keyword=False, **kwargs
-    ):
+):
     """Calls a function with the given parameters given in kwargs if they
     exist as parameters in f_callable.
 
     Parameters
     ----------
     f_callable : callable
         The function or object that is to be called
```

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/_label.py` & `scikit-activeml-0.4.1/skactiveml/utils/_label.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/_label_encoder.py` & `scikit-activeml-0.4.1/skactiveml/utils/_label_encoder.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/_multi_annot.py` & `scikit-activeml-0.4.1/skactiveml/utils/_multi_annot.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/_selection.py` & `scikit-activeml-0.4.1/skactiveml/utils/_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/_validation.py` & `scikit-activeml-0.4.1/skactiveml/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/tests/test_aggregation.py` & `scikit-activeml-0.4.1/skactiveml/utils/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/tests/test_functions.py` & `scikit-activeml-0.4.1/skactiveml/utils/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,27 @@
 
         result = call_func(test_func_1, arg1=1, arg2=2, arg3=3)
         self.assertEqual(result, 6)
 
         result = call_func(test_func_2, kwarg1=1, arg2=2, arg3=3)
         self.assertEqual(result, 6)
 
-        result = call_func(test_func_1, only_mandatory=True, arg1=1, arg2=2, arg3=3)
+        result = call_func(
+            test_func_1, only_mandatory=True, arg1=1, arg2=2, arg3=3
+        )
         self.assertEqual(result, 1)
 
-        result = call_func(test_func_2, only_mandatory=True, kwarg1=1, arg2=2, arg3=3)
+        result = call_func(
+            test_func_2, only_mandatory=True, kwarg1=1, arg2=2, arg3=3
+        )
         self.assertEqual(result, 0)
 
-        result = call_func(test_func_2, ignore_var_keyword=True, kwarg1=1, arg2=2, arg3=3)
+        result = call_func(
+            test_func_2, ignore_var_keyword=True, kwarg1=1, arg2=2, arg3=3
+        )
         self.assertEqual(result, 1)
 
     def test__available_if(self):
 
         if hasattr(metaestimators, "available_if"):
             wrapper_func = _available_if("a", True)
             self.assertTrue(callable(wrapper_func))
```

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/tests/test_label.py` & `scikit-activeml-0.4.1/skactiveml/utils/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/tests/test_label_encoder.py` & `scikit-activeml-0.4.1/skactiveml/utils/tests/test_label_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,7 @@
 
         # classes=[0, 2, 5, 10], missing_label=np.nan
         cls = [0, 2, 5, 10]
         np.testing.assert_array_equal(
             [-1, 1, 2, 3, -1],
             ExtLabelEncoder(classes=cls).fit_transform(self.y1),
         )
-
```

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/tests/test_multi_annot.py` & `scikit-activeml-0.4.1/skactiveml/utils/tests/test_multi_annot.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/tests/test_selection.py` & `scikit-activeml-0.4.1/skactiveml/utils/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/utils/tests/test_validation.py` & `scikit-activeml-0.4.1/skactiveml/utils/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-activeml-0.4.0/skactiveml/visualization/_feature_space.py` & `scikit-activeml-0.4.1/skactiveml/visualization/_feature_space.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import warnings
 
 import numpy as np
-from matplotlib import pyplot as plt
+from matplotlib import lines, pyplot as plt
 from matplotlib.axes import Axes
 from sklearn.base import ClassifierMixin
 from sklearn.neighbors import KNeighborsRegressor
 from sklearn.utils.validation import (
     check_array,
     check_consistent_length,
     column_or_1d,
@@ -283,15 +283,15 @@
 
 def plot_contour_for_samples(
     X,
     values,
     replace_nan=0.0,
     feature_bound=None,
     ax=None,
-    res=101,
+    res=21,
     contour_dict=None,
 ):
     """Plot the utility for the given query strategy.
 
     Parameters
     ----------
     X : array-like of shape (n_samples, n_features)
@@ -341,14 +341,176 @@
     neighbors.fit(X, values)
 
     scores = neighbors.predict(mesh_instances).reshape(X_mesh.shape)
     ax.contourf(X_mesh, Y_mesh, scores, **contour_args)
     return ax
 
 
+def plot_stream_training_data(
+    ax,
+    X,
+    y,
+    queried_indices,
+    classes,
+    feature_bound,
+    unlabeled_color="grey",
+    cmap="coolwarm",
+    alpha=0.2,
+    linewidth=3,
+    plot_cand_highlight=True,
+):
+    """Plot the utility for the given query strategy.
+
+    Parameters
+    ----------
+    ax : matplotlib.axes.Axes
+        The axis on which the utility is plotted. Only if y.ndim = 1 (single
+        annotator).
+    X : array-like of shape (n_samples, 1)
+        Training data set, usually complete, i.e. including the labeled and
+        unlabeled samples.
+    y : array-like of shape (n_samples, )
+        Labels of the training data set (possibly including unlabeled ones
+        indicated by self.MISSING_LABEL).
+    queried_indices : array-like of shape (n_samples,)
+        Indicates which instances from candidates have been queried.
+    classes : array-like of shape (n_classes)
+        Holds the label for each class.
+    feature_bound : array-like of shape [[xmin, ymin], [xmax, ymax]]
+        Determines the area in which the boundary is plotted. If candidates is
+        not given, bound must not be None. Otherwise, the bound is determined
+        based on the data.
+    unlabeled_color: str | matplotlib.colors.Colormap, optional
+    (default='grey')
+        The color for the unlabled samples.
+    cmap: str | matplotlib.colors.Colormap, optional (default='coolwarm_r')
+        The colormap for the confidence levels.
+    alpha: scalar
+        Set the alpha value used for blending - not supported on all backends.
+    linewidth: float
+        Set the line width in points.
+    plot_cand_highlight: bool
+        The indicator to higlight the current candidate.
+
+    Returns
+    -------
+     axes : array-like of shape (n_annotators_to_plot,)
+         The axes on which the utilities were plotted.
+    """
+    column_or_1d(X)
+    check_array(y, ensure_2d=False, force_all_finite="allow-nan")
+    check_consistent_length(X, y)
+    check_array(queried_indices, ensure_2d=False)
+    check_array(classes, ensure_2d=False)
+    check_type(unlabeled_color, "unlabeled_color", str)
+    check_type(plot_cand_highlight, "plot_cand_highlight", bool)
+    check_type(ax, "ax", Axes)
+
+    data_lines = []
+    cmap = _get_cmap(cmap)
+    norm = plt.Normalize(vmin=min(classes), vmax=max(classes))
+
+    highlight_color = (
+        cmap(norm(y[-1])) if queried_indices[-1] else unlabeled_color
+    )
+
+    if plot_cand_highlight:
+        data_lines.append(
+            lines.Line2D(
+                [0, feature_bound[0][1]],
+                [X[-1], X[-1]],
+                c=highlight_color,
+                alpha=alpha,
+                linewidth=linewidth * 2,
+            )
+        )
+
+    for t, (x_t, a, y_t) in enumerate(zip(X, queried_indices, y)):
+        line_color = cmap(norm(y_t)) if a else unlabeled_color
+        zorder = 3 if a else 2
+        alpha_tmp = alpha * 2 if a else alpha
+        data_lines.append(
+            lines.Line2D(
+                [t, len(X) - 1],
+                [x_t, x_t],
+                zorder=zorder,
+                color=line_color,
+                alpha=alpha_tmp,
+                linewidth=linewidth,
+            )
+        )
+    for d_line in data_lines:
+        ax.add_line(d_line)
+    return data_lines
+
+
+def plot_stream_decision_boundary(
+    ax,
+    t_x,
+    plot_step,
+    clf,
+    X,
+    pred_list,
+    color="k",
+    res=25,
+):
+    """Plot the decision boundary of the given classifier.
+
+    Parameters
+    ----------
+    ax: matplotlib.axes.Axes or List
+        The axis on which the decision boundary is plotted. If ax is a List,
+        each entry has to be an `matplotlib.axes.Axes`.
+    t_x: int
+        The position of the newest instance for the x axies.
+    plot_step: int
+        The interval in which the clf should predict new samples.
+    clf: Sklearn classifier
+        The fitted classifier whose decision boundary is plotted.
+    X : array-like of shape (n_samples, 1)
+        Training data set, usually complete, i.e. including the labeled and
+        unlabeled samples.
+    pred_list: array-like of shape (n_samples, )
+        The list containing classifier prediction for the last steps.
+    color: str | matplotlib.colors.Colormap, optional (default='k')
+        The color for the decision boundary.
+    res : int, optional (default=25)
+        The resolution of the plot.
+
+    Returns
+    -------
+    ax: matplotlib.axes.Axes or List
+        The axis on which the boundary was plotted or the list of axis if ax
+        was a list.
+    pred_list: array-like of shape (n_samples, )
+        The list containing classifier prediction for the last steps.
+    """
+    X = column_or_1d(X)
+    check_array(pred_list, ensure_2d=False, ensure_min_samples=0)
+    check_scalar(t_x, "t_x", int, min_val=0)
+    check_scalar(plot_step, "plot_step", int, min_val=1)
+    check_type(ax, "ax", Axes)
+    check_type(clf, "clf", ClassifierMixin)
+    x_vec = np.linspace(np.min(X), np.max(X), res)
+    t_vec = np.arange(1, t_x // plot_step + 1) * plot_step
+    t_mesh, x_mesh = np.meshgrid(t_vec, x_vec)
+    predictions = np.array([clf.predict(x_vec.reshape([-1, 1]))])
+    pred_list.extend(predictions)
+
+    if len(pred_list) > 2 and np.sum(pred_list) > 0:
+        ax.contour(
+            t_mesh,
+            x_mesh,
+            np.array(pred_list[1:]).T,
+            levels=[0.5],
+            colors=color,
+        )
+    return ax, pred_list
+
+
 def _general_plot_utilities(qs, X, y, candidates=None, **kwargs):
     """Plot the utility for the given query strategy.
 
     Parameters
     ----------
     qs : skactiveml.base.QueryStrategy
         The query strategy for which the utility is plotted.
@@ -357,16 +519,16 @@
         unlabeled samples.
     y : array-like of shape (n_samples, ) or (n_samples, n_annotators)
         Labels of the training data set (possibly including unlabeled ones
         indicated by self.MISSING_LABEL).
     candidates : None or array-like of shape (n_candidates,), dtype=int or
         array-like of shape (n_candidates, n_features),
         optional (default=None)
-        If `candidates` is None, the unlabeled samples from (X,y) are
-        considered as candidates.
+        If `candidates` is None, a mesh with the specified resolution is
+        generated and considered as candidates.
         If `candidates` is of shape (n_candidates,) and of type int,
         candidates is considered as the indices of the samples in (X,y).
         If `candidates` is of shape (n_candidates, n_features), the
         candidates are directly given in candidates (not necessarily
         contained in X). This is not supported by all query strategies.
 
     Other Parameters
```

### Comparing `scikit-activeml-0.4.0/skactiveml/visualization/_misc.py` & `scikit-activeml-0.4.1/skactiveml/visualization/_misc.py`

 * *Files identical despite different names*

