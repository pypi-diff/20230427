# Comparing `tmp/autogluon.timeseries-0.7.1b20230425.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230425.tar", last modified: Tue Apr 25 09:05:02 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230426.tar", last modified: Wed Apr 26 09:04:29 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230425.tar` & `autogluon.timeseries-0.7.1b20230426.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37101 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    42541 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40270 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.389025 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 09:03:53.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:05:02.385025 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:05:02.000000 autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.294592 autogluon.timeseries-0.7.1b20230426/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-26 09:04:29.294592 autogluon.timeseries-0.7.1b20230426/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:04:29.294592 autogluon.timeseries-0.7.1b20230426/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.282592 autogluon.timeseries-0.7.1b20230426/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.286592 autogluon.timeseries-0.7.1b20230426/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.286592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.286592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.286592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37101 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.290592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.294592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46535 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.294592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.294592 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-26 09:03:35.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:04:29.286592 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:04:29.000000 autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230425/PKG-INFO` & `autogluon.timeseries-0.7.1b20230426/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230425
+Version: 0.7.1b20230426
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230425/setup.py` & `autogluon.timeseries-0.7.1b20230426/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,11 +219,9 @@
 
         learner_info.update(trainer_info)
         # self.random_state not used during fitting, so we don't include it in the summary
         # TODO: Report random seed passed to predictor.fit?
         learner_info.pop("random_state", None)
         return learner_info
 
-    def refit_full(self, models="all"):
-        # TODO: Implement refitting
-        # return self.load_trainer().refit_full(models=models)
-        raise NotImplementedError("refitting logic currently not implemented in autogluon.timeseries")
+    def refit_full(self, model: str = "all") -> Dict[str, str]:
+        return self.load_trainer().refit_full(model=model)
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import copy
 import logging
 import os
 import time
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Union
 
 import autogluon.core as ag
 from autogluon.common.loaders import load_pkl
 from autogluon.common.savers import save_pkl
 from autogluon.core.hpo.exceptions import EmptySearchSpace
 from autogluon.core.hpo.executors import HpoExecutor
 from autogluon.core.models import AbstractModel
@@ -445,24 +444,19 @@
 
     def preprocess(self, data: Any, **kwargs) -> Any:
         return data
 
     def get_memory_size(self, **kwargs) -> Optional[int]:
         return None
 
-    def convert_to_refit_full_template(self):
-        params = copy.deepcopy(self.get_params())
-
-        # TODO: Time series models currently do not support incremental training
-        params["hyperparameters"].update(self.params_trained)
-        params["name"] = params["name"] + ag.constants.REFIT_FULL_SUFFIX
-
-        template = self.__class__(**params)
-
-        return template
+    def convert_to_refit_full_via_copy(self) -> "AbstractTimeSeriesModel":
+        refit_model = super().convert_to_refit_full_via_copy()
+        refit_model.val_score = None
+        refit_model.predict_time = None
+        return refit_model
 
     def get_user_params(self) -> dict:
         """Used to access user-specified parameters for the model before initialization."""
         if self._user_params is None:
             return {}
         else:
             return self._user_params.copy()
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,7 +393,10 @@
 
     def _rescale_targets(self, normalized_data: TimeSeriesDataFrame, scale_per_item: pd.Series) -> TimeSeriesDataFrame:
         """Scale all columns in the normalized dataframe back to original scale (inplace)."""
         data = normalized_data
         for col in data.columns:
             data[col] = data[col] * scale_per_item
         return data
+
+    def _more_tags(self) -> dict:
+        return {"can_refit_full": True}
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,7 +57,14 @@
         """Private method for `fit_ensemble`. See `fit_ensemble` for documentation of arguments. Apart from the model
         training logic, `fit_ensemble` additionally implements other logic such as keeping track of the time limit.
         """
         raise NotImplementedError
 
     def predict(self, data: Dict[str, TimeSeriesDataFrame], **kwargs) -> TimeSeriesDataFrame:
         raise NotImplementedError
+
+    def remap_base_models(self, model_full_dict: Dict[str, str]) -> None:
+        """Update names of the base models based on the mapping in model_full_dict.
+
+        This method should be called after performing refit_full to point to the refitted base models, if necessary.
+        """
+        raise NotImplementedError
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,7 +132,14 @@
 
         return sum(pred * w for pred, w in zip(model_preds, weights) if pred is not None)
 
     def get_info(self) -> dict:
         info = super().get_info()
         info["model_weights"] = self.model_to_weight
         return info
+
+    def remap_base_models(self, model_full_dict: Dict[str, str]) -> None:
+        updated_weights = {}
+        for model, weight in self.model_to_weight.items():
+            model_full_name = model_full_dict.get(model, model)
+            updated_weights[model_full_name] = weight
+        self.model_to_weight = updated_weights
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import copy
 import inspect
 import logging
 import os
 import time
+from pathlib import Path
 from typing import Dict, Optional, Type, Union
 
 import numpy as np
 import pandas as pd
 
+import autogluon.core as ag
 from autogluon.common.utils.log_utils import set_logger_verbosity
 from autogluon.timeseries.dataset.ts_dataframe import TimeSeriesDataFrame
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
 
 logger = logging.getLogger(__name__)
 
 
@@ -28,14 +30,16 @@
         which will be used to initialize the model via model_base(**model_base_kwargs).
     model_base_kwargs : Optional[Dict[str, any]], default = None
         kwargs used to initialize model_base if model_base is a class.
     num_val_windows : int, default = 1
         Number of windows to use for backtesting, starting from the end of the training data.
     """
 
+    _most_recent_model_folder: str = "W0"
+
     def __init__(
         self,
         model_base: Union[AbstractTimeSeriesModel, Type[AbstractTimeSeriesModel]],
         model_base_kwargs: Optional[Dict[str, any]] = None,
         **kwargs,
     ):
         if inspect.isclass(model_base) and issubclass(model_base, AbstractTimeSeriesModel):
@@ -124,15 +128,15 @@
     def get_info(self) -> dict:
         info = super().get_info()
         info["info_per_val_window"] = self.info_per_val_window
         return info
 
     def get_child_model(self, window_index: int) -> AbstractTimeSeriesModel:
         model = copy.deepcopy(self.model_base)
-        model.set_contexts(self.path + f"W{window_index}" + os.sep)
+        model.rename(self.name + os.sep + f"W{window_index}")
         return model
 
     def predict(
         self,
         data: TimeSeriesDataFrame,
         known_covariates: Optional[TimeSeriesDataFrame] = None,
         **kwargs,
@@ -180,17 +184,31 @@
             most_recent_model._oof_predictions = None
             most_recent_model.save()
         return save_path
 
     @classmethod
     def load(
         cls, path: str, reset_paths: bool = True, load_oof: bool = False, verbose: bool = True
-    ) -> "AbstractTimeSeriesModel":
+    ) -> AbstractTimeSeriesModel:
         model = super().load(path=path, reset_paths=reset_paths, load_oof=load_oof, verbose=verbose)
-        # Most recent model is always generated for the window W0
-        most_recent_model_path = model.path + os.sep + "W0" + os.sep
+        most_recent_model_path = model.path + os.sep + cls._most_recent_model_folder + os.sep
         model.most_recent_model = model.model_base_type.load(
             most_recent_model_path,
             reset_paths=reset_paths,
             verbose=verbose,
         )
         return model
+
+    def convert_to_refit_full_template(self) -> AbstractTimeSeriesModel:
+        # refit_model is an instance of base model type, not MultiWindowBacktestingModel
+        refit_model = self.most_recent_model.convert_to_refit_full_template()
+        refit_model.rename(self.name + ag.constants.REFIT_FULL_SUFFIX)
+        return refit_model
+
+    def convert_to_refit_full_via_copy(self) -> AbstractTimeSeriesModel:
+        # refit_model is an instance of base model type, not MultiWindowBacktestingModel
+        refit_model = self.most_recent_model.convert_to_refit_full_via_copy()
+        refit_model.rename(self.name + ag.constants.REFIT_FULL_SUFFIX)
+        return refit_model
+
+    def _more_tags(self) -> dict:
+        return self.most_recent_model._get_tags()
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,14 +287,15 @@
         train_data: Union[TimeSeriesDataFrame, pd.DataFrame],
         tuning_data: Optional[Union[TimeSeriesDataFrame, pd.DataFrame]] = None,
         time_limit: Optional[int] = None,
         presets: Optional[str] = None,
         hyperparameters: Dict[Union[str, Type], Any] = None,
         hyperparameter_tune_kwargs: Optional[Union[str, Dict]] = None,
         num_val_windows: int = 1,
+        refit_full: bool = False,
         enable_ensemble: bool = True,
         random_seed: Optional[int] = None,
         verbosity: Optional[int] = None,
     ) -> "TimeSeriesPredictor":
         """Fit probabilistic forecasting models to the given time series dataset.
 
         Parameters
@@ -323,16 +324,16 @@
             to a ``TimeSeriesDataFrame``.
 
         tuning_data : Union[TimeSeriesDataFrame, pd.DataFrame], optional
             Data reserved for model selection and hyperparameter tuning, rather than training individual models. Also
             used to compute the validation scores. Note that only the last ``prediction_length`` time steps of each
             time series are used for computing the validation score.
 
-            If ``tuning_data`` is provided, multi-window backtesting on training data will be disabled and the
-            ``num_val_windows`` argument will be ignored.
+            If ``tuning_data`` is provided, multi-window backtesting on training data will be disabled, the
+            ``num_val_windows`` argument will be ignored, and ``refit_full`` will be set to ``False``.
 
             Leaving this argument empty and letting AutoGluon automatically generate the validation set from
             ``train_data`` is a good default.
 
             If ``known_covariates_names`` were specified when creating the predictor, ``tuning_data`` must also include
             the columns listed in ``known_covariates_names`` with the covariates values aligned with the target time
             series.
@@ -440,15 +441,20 @@
                         "scheduler": "local",
                         "searcher": "auto",
                         "num_trials": 5,
                     }
                 )
         num_val_windows : int, default = 1
             Number of backtests done on ``train_data`` for each trained model to estimate the validation performance.
+            A separate copy of each model is trained for each validation window.
             When ``num_val_windows = k``, training time is increased roughly by a factor of ``k``.
+        refit_full : bool, default = False
+            If True, after training is complete, AutoGluon will attempt to re-train all models using all of training
+            data (including the data initially reserved for validation). This argument has no effect if ``tuning_data``
+            is provided.
         enable_ensemble : bool, default = True
             If True, the ``TimeSeriesPredictor`` will fit a simple weighted ensemble on top of the models specified via
             ``hyperparameters``.
         random_seed : int, optional
             If provided, fixes the seed of the random number generator for all models. This guarantees reproducible
             results for most models (except those trained on GPU because of the non-determinism of GPU operations).
         verbosity : int, optional
@@ -515,14 +521,19 @@
             hyperparameters=hyperparameters,
             hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
             time_limit=time_left,
             verbosity=verbosity,
             num_val_windows=num_val_windows,
             enable_ensemble=enable_ensemble,
         )
+        if refit_full:
+            if tuning_data is None:
+                self.refit_full()
+            else:
+                logger.warning("Skipping `refit_full` because custom `tuning_data` was provided during `fit`.")
 
         self.save()
         return self
 
     def get_model_names(self) -> List[str]:
         """Returns the list of model names trained by this predictor object."""
         return self._trainer.get_model_names()
@@ -684,14 +695,18 @@
 
     def info(self) -> Dict[str, Any]:
         """Returns a dictionary of objects each describing an attribute of the training process and trained models."""
         return self._learner.get_info(include_model_info=True)
 
     def get_model_best(self) -> str:
         """Returns the name of the best model from trainer."""
+        if self._trainer.model_best is not None:
+            models = self._trainer.get_model_names()
+            if self._trainer.model_best in models:
+                return self._trainer.model_best
         return self._trainer.get_model_best()
 
     def leaderboard(
         self, data: Optional[Union[TimeSeriesDataFrame, pd.DataFrame]] = None, silent=False
     ) -> pd.DataFrame:
         """Return a leaderboard showing the performance of every trained model, the output is a
         pandas data frame with columns:
@@ -787,10 +802,68 @@
             print(results["leaderboard"])
             print(f"Number of models trained: {len(results['model_performance'])}")
             print("Types of models trained:")
             print(unique_model_types)
             print("****************** End of fit() summary ******************")
         return results
 
-    # TODO
-    def refit_full(self, models="all"):
-        raise NotImplementedError("Refitting logic not yet implemented in autogluon.timeseries")
+    def refit_full(self, model: str = "all", set_best_to_refit_full: bool = True) -> Dict[str, str]:
+        """Retrain model on all of the data (training + validation).
+
+        This method can only be used if no ``tuning_data`` was passed to :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit`.
+
+        .. warning::
+            This is experimental functionality, many time series models do not yet support ``refit_full`` and will
+            simply be copied.
+
+
+        Parameters
+        ----------
+        model : str, default = "all"
+            Name of the model to refit.
+            All ancestor models will also be refit in the case that the selected model is a weighted ensemble.
+            Valid models are listed in this ``predictor`` by calling :meth:`~autogluon.timeseries.TimeSeriesPredictor.get_model_names`.
+
+            * If "all" then all models are refitted.
+            * If "best" then the model with the highest validation score is refit.
+
+        set_best_to_refit_full : bool, default = True
+            If True, sets best model to the refit_full version of the prior best model. This means the model used when
+            ``predictor.predict(data)`` is called will be the refit_full version instead of the original version of the
+            model. Has no effect if ``model`` is not the best model.
+        """
+        logger.warning(
+            "\tWARNING: refit_full functionality for TimeSeriesPredictor is experimental "
+            "and is not yet supported by all models."
+        )
+
+        logger.info(
+            "Refitting models via `refit_full` using all of the data (combined train and validation)...\n"
+            "\tModels trained in this way will have the suffix '_FULL' and have NaN validation score.\n"
+            "\tThis process is not bound by time_limit, but should take less time than the original `fit` call."
+        )
+        model_best = self.get_model_best()
+        refit_full_dict = self._learner.refit_full(model=model)
+
+        if set_best_to_refit_full:
+            if model_best in refit_full_dict:
+                self._trainer.model_best = refit_full_dict[model_best]
+                self._trainer.save()
+                logger.info(
+                    f"Updated best model to '{self._trainer.model_best}' (Previously '{model_best}'). "
+                    f"AutoGluon will default to using '{self._trainer.model_best}' for predict()."
+                )
+            elif model_best in refit_full_dict.values():
+                # Model best is already a refit full model
+                prev_best = self._trainer.model_best
+                self._trainer.model_best = model_best
+                self._trainer.save()
+                logger.info(
+                    f"Updated best model to '{self._trainer.model_best}' (Previously '{prev_best}'). "
+                    f"AutoGluon will default to using '{self._trainer.model_best}' for predict()."
+                )
+            else:
+                logger.warning(
+                    f"Best model ('{model_best}') is not present in refit_full dictionary. "
+                    f"Training may have failed on the refit model. AutoGluon will default to using '{model_best}' for predict()."
+                )
+        return refit_full_dict
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 import logging
 import os
 import time
 import traceback
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
-from warnings import warn
 
 import networkx as nx
 import pandas as pd
 from tqdm import tqdm
 
 from autogluon.common.utils.log_utils import set_logger_verbosity
 from autogluon.core.models import AbstractModel
 from autogluon.core.utils.loaders import load_pkl
 from autogluon.core.utils.savers import save_json, save_pkl
 from autogluon.timeseries import TimeSeriesDataFrame, TimeSeriesEvaluator
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
 from autogluon.timeseries.models.ensemble import AbstractTimeSeriesEnsembleModel, TimeSeriesGreedyEnsemble
-from autogluon.timeseries.models.multi_window.multi_window_model import MultiWindowBacktestingModel
 from autogluon.timeseries.models.presets import contains_searchspace
 from autogluon.timeseries.utils.features import CovariateMetadata
 from autogluon.timeseries.utils.warning_filters import disable_tqdm
 
 logger = logging.getLogger("autogluon.timeseries.trainer")
 
 
@@ -157,15 +155,15 @@
             self.models[model.name] = model
 
     def load_model(
         self,
         model_name: Union[str, AbstractModel],
         path: Optional[str] = None,
         model_type: Optional[Type[AbstractModel]] = None,
-    ):
+    ) -> AbstractTimeSeriesModel:
         if isinstance(model_name, AbstractModel):
             return model_name
         if model_name in self.models.keys():
             return self.models[model_name]
 
         if path is None:
             path = self.get_model_attribute(model=model_name, attribute="path")
@@ -293,19 +291,17 @@
         self.enable_ensemble = enable_ensemble
         self.ensemble_model_type = TimeSeriesGreedyEnsemble
 
         self.verbosity = verbosity
         set_logger_verbosity(self.verbosity, logger=logger)
 
         # Dict of normal model -> FULL model. FULL models are produced by
-        # self.refit_single_full() and self.refit_ensemble_full().
+        # self.refit_single_full() and self.refit_full().
         self.model_full_dict = {}
 
-        # Dict of FULL model -> normal model validation score in case the normal model had been deleted.
-        self._model_full_dict_val_score = {}
         self.eval_metric = TimeSeriesEvaluator.check_get_evaluation_metric(eval_metric)
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
         self.num_val_windows = num_val_windows
         self.hpo_results = {}
 
     def save_train_data(self, data: TimeSeriesDataFrame, verbose: bool = True) -> None:
         path = self.path_data + "train.pkl"
@@ -315,19 +311,22 @@
         path = self.path_data + "val.pkl"
         save_pkl.save(path=path, object=data, verbose=verbose)
 
     def load_train_data(self) -> TimeSeriesDataFrame:
         path = self.path_data + "train.pkl"
         return load_pkl.load(path=path)
 
-    def load_val_data(self) -> TimeSeriesDataFrame:
+    def load_val_data(self) -> Optional[TimeSeriesDataFrame]:
         path = self.path_data + "val.pkl"
-        return load_pkl.load(path=path)
+        if os.path.exists(path):
+            return load_pkl.load(path=path)
+        else:
+            return None
 
-    def load_data(self) -> Tuple[TimeSeriesDataFrame, TimeSeriesDataFrame]:
+    def load_data(self) -> Tuple[TimeSeriesDataFrame, Optional[TimeSeriesDataFrame]]:
         train_data = self.load_train_data()
         val_data = self.load_val_data()
         return train_data, val_data
 
     def save(self) -> None:
         models = self.models
         self.models = {}
@@ -880,79 +879,100 @@
         **kwargs,
     ) -> TimeSeriesDataFrame:
         if isinstance(model, str):
             model = self.load_model(model)
         data = self.get_inputs_to_model(model=model, X=data, known_covariates=known_covariates)
         return model.predict(data, known_covariates=known_covariates, **kwargs)
 
-    # TODO: experimental
-    def refit_single_full(self, train_data=None, val_data=None, models=None):
-        warn("Refitting logic is experimental for autogluon.timeseries.")
-        models_trained_full = []
-        model_full_dict = {}
+    def _merge_refit_full_data(
+        self, train_data: TimeSeriesDataFrame, val_data: Optional[TimeSeriesDataFrame]
+    ) -> TimeSeriesDataFrame:
+        if val_data is None:
+            return train_data
+        else:
+            # TODO: Implement merging of arbitrary tuning_data with train_data
+            raise NotImplementedError("refit_full is not supported if custom val_data is provided.")
 
-        train_data = train_data or self.load_train_data()  # noqa
-        val_data = val_data or self.load_val_data()
+    def refit_single_full(
+        self,
+        train_data: Optional[TimeSeriesDataFrame] = None,
+        val_data: Optional[TimeSeriesDataFrame] = None,
+        models: List[str] = None,
+    ) -> List[str]:
 
-        # FIXME: implement the append operation below in datasets
-        # refit_full_data = train_data + val_data
-        # for now we assume validation data includes train data (as in GluonTS)
-        refit_full_data = val_data
+        train_data = train_data or self.load_train_data()
+        val_data = val_data or self.load_val_data()
+        refit_full_data = self._merge_refit_full_data(train_data, val_data)
 
         if models is None:
-            self.get_model_names()
+            models = self.get_model_names()
 
-        for model in models:
-            model: AbstractTimeSeriesModel = self.load_model(model)
+        model_to_level = self._get_model_levels()
+        models_sorted_by_level = sorted(models, key=model_to_level.get)
+
+        model_full_dict = {}
+        models_trained_full = []
+        for model in models_sorted_by_level:
+            model = self.load_model(model)
             model_name = model.name
-            model_full = model.convert_to_refit_full_template()  # FIXME: not available
-            models_trained = self._train_multi(
-                train_data=refit_full_data,
-                val_data=None,
-                hyperparameters=None,
-                hyperparameter_tune_kwargs=None,
-                models=[model_full],
-            )
+            if model._get_tags()["can_refit_full"]:
+                model_full = model.convert_to_refit_full_template()
+                logger.info(f"Fitting model: {model_full.name}")
+                models_trained = self._train_and_save(
+                    train_data=refit_full_data,
+                    val_data=None,
+                    model=model_full,
+                )
+            else:
+                model_full = model.convert_to_refit_full_via_copy()
+                logger.info(f"Fitting model: {model_full.name} | Skipping fit via cloning parent ...")
+                models_trained = [model_full.name]
+                if isinstance(model_full, AbstractTimeSeriesEnsembleModel):
+                    model_full.remap_base_models(model_full_dict)
+                    self._add_model(model_full, base_models=model_full.model_names)
+                else:
+                    self._add_model(model_full)
+                self.save_model(model_full)
 
             if len(models_trained) == 1:
                 model_full_dict[model_name] = models_trained[0]
-            for model_trained in models_trained:
-                self._model_full_dict_val_score[model_trained] = self.get_model_attribute(model_name, "val_score")
             models_trained_full += models_trained
 
         self.model_full_dict.update(model_full_dict)
         self.save()
         return models_trained_full
 
-    # TODO: experimental
-    def refit_full(self, models="all"):
-        warn("Refitting logic is experimental for autogluon.timeseries.")
-        if isinstance(models, str):
-            if models == "all":
-                models = self.get_model_names()
-            elif models == "best":
-                models = [self.get_model_best()]
-            else:
-                models = self.load_model(models)
+    def refit_full(self, model: str = "all") -> Dict[str, str]:
+        time_start = time.time()
         existing_models = self.get_model_names()
+        if model == "all":
+            model_names = existing_models
+        elif model == "best":
+            model_names = self.get_minimum_model_set(self.get_model_best())
+        else:
+            model_names = self.get_minimum_model_set(model)
+
         valid_model_set = []
-        for model in models:
-            if model in self.model_full_dict and self.model_full_dict[model] in existing_models:
-                logger.log(
-                    20,
-                    f"Model '{model}' already has a refit _FULL model: "
+        for name in model_names:
+            if name in self.model_full_dict and self.model_full_dict[model] in existing_models:
+                logger.info(
+                    f"Model '{name}' already has a refit _FULL model: "
                     f"'{self.model_full_dict[model]}', skipping refit...",
                 )
             else:
-                valid_model_set.append(model)
+                valid_model_set.append(name)
 
         if valid_model_set:
-            self.refit_single_full(models=valid_model_set)
+            models_trained_full = self.refit_single_full(models=valid_model_set)
+        else:
+            models_trained_full = []
 
         self.save()
+        logger.info(f"Refit complete. Models trained: {models_trained_full}")
+        logger.info(f"Total runtime: {time.time() - time_start:.2f} s")
         return copy.deepcopy(self.model_full_dict)
 
     def construct_model_templates(
         self, hyperparameters: Union[str, Dict[str, Any]], multi_window: bool = False, **kwargs
     ) -> List[AbstractTimeSeriesModel]:
         """Constructs a list of unfit models based on the hyperparameters dict."""
         raise NotImplementedError
@@ -965,9 +985,7 @@
         **kwargs,
     ) -> None:
         raise NotImplementedError
 
     # TODO: def _filter_base_models_via_infer_limit
 
     # TODO: persist and unpersist models
-
-    # TODO: generate weighted ensemble
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230426/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230425
+Version: 0.7.1b20230426
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230425/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230426/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

