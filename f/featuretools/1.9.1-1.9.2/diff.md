# Comparing `tmp/featuretools-1.9.1.tar.gz` & `tmp/featuretools-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/tmpsvoy0xsm/featuretools-1.9.1.tar", last modified: Fri May 27 16:45:35 2022, max compression
+gzip compressed data, was "/github/workspace/dist/tmpa2rqme_b/featuretools-1.9.2.tar", last modified: Fri Jun 10 15:21:55 2022, max compression
```

## Comparing `featuretools-1.9.1.tar` & `featuretools-1.9.2.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/
--rw-r--r--   0 root         (0) root         (0)     1517 2022-05-27 16:45:16.000000 featuretools-1.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13116 2022-05-27 16:45:35.000000 featuretools-1.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11225 2022-05-27 16:45:16.000000 featuretools-1.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/
--rw-r--r--   0 root         (0) root         (0)     2090 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/computational_backends/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/computational_backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)      183 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/computational_backends/api.py
--rw-r--r--   0 root         (0) root         (0)    38333 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/computational_backends/calculate_feature_matrix.py
--rw-r--r--   0 root         (0) root         (0)     9196 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/computational_backends/feature_set.py
--rw-r--r--   0 root         (0) root         (0)    35288 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/computational_backends/feature_set_calculator.py
--rw-r--r--   0 root         (0) root         (0)    14629 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/computational_backends/utils.py
--rw-r--r--   0 root         (0) root         (0)     2078 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/config_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/demo/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/demo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/demo/api.py
--rw-r--r--   0 root         (0) root         (0)     9528 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/demo/flight.py
--rw-r--r--   0 root         (0) root         (0)     4029 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/demo/mock_customer.py
--rw-r--r--   0 root         (0) root         (0)     3486 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/demo/retail.py
--rw-r--r--   0 root         (0) root         (0)      918 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/demo/weather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/entityset/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/entityset/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/entityset/api.py
--rw-r--r--   0 root         (0) root         (0)     6118 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/entityset/deserialize.py
--rw-r--r--   0 root         (0) root         (0)    77954 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/entityset/entityset.py
--rw-r--r--   0 root         (0) root         (0)     6705 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/entityset/relationship.py
--rw-r--r--   0 root         (0) root         (0)     3391 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/entityset/serialize.py
--rw-r--r--   0 root         (0) root         (0)     6558 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/entityset/timedelta.py
--rw-r--r--   0 root         (0) root         (0)      178 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/feature_base/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      407 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/api.py
--rw-r--r--   0 root         (0) root         (0)    35124 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/feature_base.py
--rw-r--r--   0 root         (0) root         (0)     6697 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/feature_descriptions.py
--rw-r--r--   0 root         (0) root         (0)     9650 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/feature_visualizer.py
--rw-r--r--   0 root         (0) root         (0)     4725 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/features_deserializer.py
--rw-r--r--   0 root         (0) root         (0)     4143 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/features_serializer.py
--rw-r--r--   0 root         (0) root         (0)      383 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/feature_base/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/primitives/
--rw-r--r--   0 root         (0) root         (0)     2405 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      223 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/primitives/base/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/base/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1435 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/base/aggregation_primitive_base.py
--rw-r--r--   0 root         (0) root         (0)      175 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/base/api.py
--rw-r--r--   0 root         (0) root         (0)     5322 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/base/primitive_base.py
--rwxr-xr-x   0 root         (0) root         (0)      817 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/base/transform_primitive_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/primitives/data/
--rw-r--r--   0 root         (0) root         (0)        8 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/data/featuretools_unit_test_example.csv
--rw-r--r--   0 root         (0) root         (0)    63370 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/data/free_email_provider_domains.txt
--rw-r--r--   0 root         (0) root         (0)      747 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/data/free_email_provider_domains_license
--rw-r--r--   0 root         (0) root         (0)    12400 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/options_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/primitives/standard/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25967 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/aggregation_primitives.py
--rw-r--r--   0 root         (0) root         (0)      289 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/api.py
--rw-r--r--   0 root         (0) root         (0)    38353 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/binary_transform.py
--rw-r--r--   0 root         (0) root         (0)     4648 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/cum_transform_feature.py
--rw-r--r--   0 root         (0) root         (0)    19903 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/datetime_transform_primitives.py
--rw-r--r--   0 root         (0) root         (0)     8701 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/latlong_transform_primitives.py
--rw-r--r--   0 root         (0) root         (0)    27459 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/rolling_transform_primitive.py
--rw-r--r--   0 root         (0) root         (0)    18445 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/standard/transform_primitive.py
--rw-r--r--   0 root         (0) root         (0)    18565 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/primitives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/selection/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)       40 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/selection/api.py
--rw-r--r--   0 root         (0) root         (0)     8304 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/selection/selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/synthesis/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/synthesis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      193 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/synthesis/api.py
--rw-r--r--   0 root         (0) root         (0)    42995 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/synthesis/deep_feature_synthesis.py
--rw-r--r--   0 root         (0) root         (0)    14366 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/synthesis/dfs.py
--rw-r--r--   0 root         (0) root         (0)     7299 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/synthesis/encode_features.py
--rw-r--r--   0 root         (0) root         (0)     4072 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/synthesis/get_valid_primitives.py
--rw-r--r--   0 root         (0) root         (0)     1836 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/synthesis/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      561 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/cli_tests/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/computational_backend/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/computational_backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82879 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/computational_backend/test_calculate_feature_matrix.py
--rw-r--r--   0 root         (0) root         (0)     1084 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/computational_backend/test_dask_features.py
--rw-r--r--   0 root         (0) root         (0)     6370 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/computational_backend/test_feature_set.py
--rw-r--r--   0 root         (0) root         (0)    37868 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/computational_backend/test_feature_set_calculator.py
--rw-r--r--   0 root         (0) root         (0)     1807 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/computational_backend/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/config_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/config_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      618 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/config_tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    19867 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/demo_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/demo_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2170 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/demo_tests/test_demo_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6334 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_dask_es.py
--rw-r--r--   0 root         (0) root         (0)    81581 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_es.py
--rw-r--r--   0 root         (0) root         (0)     8531 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_es_metadata.py
--rw-r--r--   0 root         (0) root         (0)    17288 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_last_time_index.py
--rw-r--r--   0 root         (0) root         (0)     2355 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_plotting.py
--rw-r--r--   0 root         (0) root         (0)     3115 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_relationship.py
--rw-r--r--   0 root         (0) root         (0)    17468 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_serialization.py
--rw-r--r--   0 root         (0) root         (0)     6654 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_spark_es.py
--rw-r--r--   0 root         (0) root         (0)     7710 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_timedelta.py
--rw-r--r--   0 root         (0) root         (0)    34578 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entityset_tests/test_ww_es.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/featuretools_plugin/
--rw-r--r--   0 root         (0) root         (0)       52 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/featuretools_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      223 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      170 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/existing_primitive.py
--rw-r--r--   0 root         (0) root         (0)       47 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/invalid_primitive.py
--rw-r--r--   0 root         (0) root         (0)      179 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/new_primitive.py
--rw-r--r--   0 root         (0) root         (0)      389 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/setup.py
--rw-r--r--   0 root         (0) root         (0)      671 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/test_plugin.py
--rw-r--r--   0 root         (0) root         (0)     1101 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/test_primitives.py
--rw-r--r--   0 root         (0) root         (0)     1040 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/entry_point_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/integration_data/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/integration_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/bad_primitive_files/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/bad_primitive_files/__init__.py
--rw-r--r--   0 root         (0) root         (0)      472 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/bad_primitive_files/multiple_primitives.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/bad_primitive_files/no_primitives.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/primitives_to_install/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/primitives_to_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)      294 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/primitives_to_install/custom_max.py
--rw-r--r--   0 root         (0) root         (0)      296 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/primitives_to_install/custom_mean.py
--rw-r--r--   0 root         (0) root         (0)      294 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/primitives_to_install/custom_sum.py
--rw-r--r--   0 root         (0) root         (0)    28808 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_agg_feats.py
--rw-r--r--   0 root         (0) root         (0)      994 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_agg_primitives.py
--rw-r--r--   0 root         (0) root         (0)     3891 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_dask_primitives.py
--rw-r--r--   0 root         (0) root         (0)     3567 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_datetoholiday_primitive.py
--rw-r--r--   0 root         (0) root         (0)    10425 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_direct_features.py
--rw-r--r--   0 root         (0) root         (0)     3064 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_distancetoholiday_primitive.py
--rw-r--r--   0 root         (0) root         (0)    14498 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_base.py
--rw-r--r--   0 root         (0) root         (0)    11825 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_descriptions.py
--rw-r--r--   0 root         (0) root         (0)     9771 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_serialization.py
--rw-r--r--   0 root         (0) root         (0)     2027 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_utils.py
--rw-r--r--   0 root         (0) root         (0)    14820 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_visualizer.py
--rw-r--r--   0 root         (0) root         (0)    10326 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_features_deserializer.py
--rw-r--r--   0 root         (0) root         (0)     6728 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_features_serializer.py
--rw-r--r--   0 root         (0) root         (0)    19156 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_groupby_transform_primitives.py
--rw-r--r--   0 root         (0) root         (0)      582 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_identity_features.py
--rw-r--r--   0 root         (0) root         (0)     3004 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_is_federal_holiday.py
--rw-r--r--   0 root         (0) root         (0)     3785 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_latlong_primitives.py
--rw-r--r--   0 root         (0) root         (0)     6014 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_overrides.py
--rw-r--r--   0 root         (0) root         (0)     2874 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_primitive_base.py
--rw-r--r--   0 root         (0) root         (0)    22895 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_primitive_utils.py
--rw-r--r--   0 root         (0) root         (0)    12299 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_rolling_primitive.py
--rw-r--r--   0 root         (0) root         (0)    51676 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_transform_features.py
--rw-r--r--   0 root         (0) root         (0)    19127 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/test_transform_primitive.py
--rw-r--r--   0 root         (0) root         (0)      929 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/primitive_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/selection/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11030 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/selection/test_selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/synthesis/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/synthesis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13390 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/synthesis/test_dask_dfs.py
--rw-r--r--   0 root         (0) root         (0)    67215 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/synthesis/test_deep_feature_synthesis.py
--rw-r--r--   0 root         (0) root         (0)    23089 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/synthesis/test_dfs_method.py
--rw-r--r--   0 root         (0) root         (0)    10876 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/synthesis/test_encode_features.py
--rw-r--r--   0 root         (0) root         (0)     3718 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/synthesis/test_get_valid_primitives.py
--rw-r--r--   0 root         (0) root         (0)    14589 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/synthesis/test_spark_dfs.py
--rw-r--r--   0 root         (0) root         (0)       93 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/testing_utils/
--rw-r--r--   0 root         (0) root         (0)      298 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/testing_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      510 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/testing_utils/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1499 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/testing_utils/es_utils.py
--rw-r--r--   0 root         (0) root         (0)     1967 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/testing_utils/features.py
--rw-r--r--   0 root         (0) root         (0)    47175 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/testing_utils/mock_ds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/tests/utils_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/test_cli_utils.py
--rw-r--r--   0 root         (0) root         (0)     1703 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      787 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/test_description_utils.py
--rw-r--r--   0 root         (0) root         (0)     3446 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/test_entry_point.py
--rw-r--r--   0 root         (0) root         (0)     2853 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/test_gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     3531 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/test_time_utils.py
--rw-r--r--   0 root         (0) root         (0)     1309 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/tests/utils_tests/test_trie.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools/utils/
--rw-r--r--   0 root         (0) root         (0)       34 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      298 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/api.py
--rw-r--r--   0 root         (0) root         (0)     2646 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)     2861 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/common_tld_utils.py
--rw-r--r--   0 root         (0) root         (0)      384 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/description_utils.py
--rw-r--r--   0 root         (0) root         (0)     1551 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/entry_point.py
--rw-r--r--   0 root         (0) root         (0)     4668 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     2233 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/plot_utils.py
--rw-r--r--   0 root         (0) root         (0)     2451 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/s3_utils.py
--rw-r--r--   0 root         (0) root         (0)     1228 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/spark_utils.py
--rw-r--r--   0 root         (0) root         (0)     3008 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/time_utils.py
--rw-r--r--   0 root         (0) root         (0)     3360 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/trie.py
--rw-r--r--   0 root         (0) root         (0)     4537 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/utils/wrangle.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-05-27 16:45:16.000000 featuretools-1.9.1/featuretools/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13116 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8903 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-27 16:45:24.000000 featuretools-1.9.1/featuretools.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1426 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-05-27 16:45:35.000000 featuretools-1.9.1/featuretools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      840 2022-05-27 16:45:16.000000 featuretools-1.9.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     3405 2022-05-27 16:45:35.000000 featuretools-1.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/
+-rw-r--r--   0 root         (0) root         (0)     1517 2022-06-10 15:21:35.000000 featuretools-1.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13116 2022-06-10 15:21:55.000000 featuretools-1.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11225 2022-06-10 15:21:35.000000 featuretools-1.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/
+-rw-r--r--   0 root         (0) root         (0)     2090 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/computational_backends/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/computational_backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      183 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/computational_backends/api.py
+-rw-r--r--   0 root         (0) root         (0)    38333 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/computational_backends/calculate_feature_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     9196 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/computational_backends/feature_set.py
+-rw-r--r--   0 root         (0) root         (0)    35288 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/computational_backends/feature_set_calculator.py
+-rw-r--r--   0 root         (0) root         (0)    14645 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/computational_backends/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/config_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/demo/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/demo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/demo/api.py
+-rw-r--r--   0 root         (0) root         (0)     9528 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/demo/flight.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/demo/mock_customer.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/demo/retail.py
+-rw-r--r--   0 root         (0) root         (0)      918 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/demo/weather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/entityset/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/entityset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/entityset/api.py
+-rw-r--r--   0 root         (0) root         (0)     6118 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/entityset/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)    77954 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/entityset/entityset.py
+-rw-r--r--   0 root         (0) root         (0)     6705 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/entityset/relationship.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/entityset/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     6558 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/entityset/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)      178 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/feature_base/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      407 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/api.py
+-rw-r--r--   0 root         (0) root         (0)    35124 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/feature_base.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/feature_descriptions.py
+-rw-r--r--   0 root         (0) root         (0)     9650 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/feature_visualizer.py
+-rw-r--r--   0 root         (0) root         (0)     4725 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/features_deserializer.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/features_serializer.py
+-rw-r--r--   0 root         (0) root         (0)      383 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/feature_base/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/primitives/
+-rw-r--r--   0 root         (0) root         (0)     2405 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      223 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/primitives/base/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/base/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1435 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/base/aggregation_primitive_base.py
+-rw-r--r--   0 root         (0) root         (0)      175 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/base/api.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/base/primitive_base.py
+-rwxr-xr-x   0 root         (0) root         (0)      817 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/base/transform_primitive_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/primitives/data/
+-rw-r--r--   0 root         (0) root         (0)        8 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/data/featuretools_unit_test_example.csv
+-rw-r--r--   0 root         (0) root         (0)    63370 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/data/free_email_provider_domains.txt
+-rw-r--r--   0 root         (0) root         (0)      747 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/data/free_email_provider_domains_license
+-rw-r--r--   0 root         (0) root         (0)    12400 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/options_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/primitives/standard/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25967 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/aggregation_primitives.py
+-rw-r--r--   0 root         (0) root         (0)      289 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/api.py
+-rw-r--r--   0 root         (0) root         (0)    38353 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/binary_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4648 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/cum_transform_feature.py
+-rw-r--r--   0 root         (0) root         (0)    19903 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/datetime_transform_primitives.py
+-rw-r--r--   0 root         (0) root         (0)     8701 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/latlong_transform_primitives.py
+-rw-r--r--   0 root         (0) root         (0)    27459 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/rolling_transform_primitive.py
+-rw-r--r--   0 root         (0) root         (0)    18445 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/standard/transform_primitive.py
+-rw-r--r--   0 root         (0) root         (0)    18565 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/primitives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/selection/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       40 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/selection/api.py
+-rw-r--r--   0 root         (0) root         (0)     8304 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/selection/selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/synthesis/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/synthesis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      193 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/synthesis/api.py
+-rw-r--r--   0 root         (0) root         (0)    42995 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/synthesis/deep_feature_synthesis.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/synthesis/dfs.py
+-rw-r--r--   0 root         (0) root         (0)     7299 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/synthesis/encode_features.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/synthesis/get_valid_primitives.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/synthesis/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      561 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/cli_tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/computational_backend/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/computational_backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83593 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/computational_backend/test_calculate_feature_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/computational_backend/test_dask_features.py
+-rw-r--r--   0 root         (0) root         (0)     6370 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/computational_backend/test_feature_set.py
+-rw-r--r--   0 root         (0) root         (0)    37868 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/computational_backend/test_feature_set_calculator.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/computational_backend/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/config_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/config_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      618 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/config_tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    19867 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/demo_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/demo_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/demo_tests/test_demo_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6334 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_dask_es.py
+-rw-r--r--   0 root         (0) root         (0)    81581 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_es.py
+-rw-r--r--   0 root         (0) root         (0)     8531 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_es_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    17288 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_last_time_index.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_plotting.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_relationship.py
+-rw-r--r--   0 root         (0) root         (0)    17468 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_serialization.py
+-rw-r--r--   0 root         (0) root         (0)     6654 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_spark_es.py
+-rw-r--r--   0 root         (0) root         (0)     7710 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_timedelta.py
+-rw-r--r--   0 root         (0) root         (0)    34578 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entityset_tests/test_ww_es.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/featuretools_plugin/
+-rw-r--r--   0 root         (0) root         (0)       52 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/featuretools_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      223 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_plugin/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      170 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/existing_primitive.py
+-rw-r--r--   0 root         (0) root         (0)       47 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/invalid_primitive.py
+-rw-r--r--   0 root         (0) root         (0)      179 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/featuretools_primitives/new_primitive.py
+-rw-r--r--   0 root         (0) root         (0)      389 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/add-ons/featuretools_primitives/setup.py
+-rw-r--r--   0 root         (0) root         (0)      671 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/test_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/test_primitives.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/entry_point_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/integration_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/integration_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/bad_primitive_files/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/bad_primitive_files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      472 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/bad_primitive_files/multiple_primitives.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/bad_primitive_files/no_primitives.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/primitives_to_install/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/primitives_to_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      294 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/primitives_to_install/custom_max.py
+-rw-r--r--   0 root         (0) root         (0)      296 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/primitives_to_install/custom_mean.py
+-rw-r--r--   0 root         (0) root         (0)      294 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/primitives_to_install/custom_sum.py
+-rw-r--r--   0 root         (0) root         (0)    28808 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_agg_feats.py
+-rw-r--r--   0 root         (0) root         (0)      994 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_agg_primitives.py
+-rw-r--r--   0 root         (0) root         (0)     3891 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_dask_primitives.py
+-rw-r--r--   0 root         (0) root         (0)     3567 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_datetoholiday_primitive.py
+-rw-r--r--   0 root         (0) root         (0)    10425 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_direct_features.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_distancetoholiday_primitive.py
+-rw-r--r--   0 root         (0) root         (0)    14498 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_base.py
+-rw-r--r--   0 root         (0) root         (0)    11825 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_descriptions.py
+-rw-r--r--   0 root         (0) root         (0)     9771 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_serialization.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_utils.py
+-rw-r--r--   0 root         (0) root         (0)    14820 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_visualizer.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_features_deserializer.py
+-rw-r--r--   0 root         (0) root         (0)     6728 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_features_serializer.py
+-rw-r--r--   0 root         (0) root         (0)    19156 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_groupby_transform_primitives.py
+-rw-r--r--   0 root         (0) root         (0)      582 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_identity_features.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_is_federal_holiday.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_latlong_primitives.py
+-rw-r--r--   0 root         (0) root         (0)     6014 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_overrides.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_primitive_base.py
+-rw-r--r--   0 root         (0) root         (0)    22895 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_primitive_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12299 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_rolling_primitive.py
+-rw-r--r--   0 root         (0) root         (0)    51676 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_transform_features.py
+-rw-r--r--   0 root         (0) root         (0)    19127 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/test_transform_primitive.py
+-rw-r--r--   0 root         (0) root         (0)      929 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/primitive_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/selection/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/selection/test_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/synthesis/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/synthesis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13390 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/synthesis/test_dask_dfs.py
+-rw-r--r--   0 root         (0) root         (0)    67215 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/synthesis/test_deep_feature_synthesis.py
+-rw-r--r--   0 root         (0) root         (0)    23089 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/synthesis/test_dfs_method.py
+-rw-r--r--   0 root         (0) root         (0)    10876 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/synthesis/test_encode_features.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/synthesis/test_get_valid_primitives.py
+-rw-r--r--   0 root         (0) root         (0)    14589 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/synthesis/test_spark_dfs.py
+-rw-r--r--   0 root         (0) root         (0)       93 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/testing_utils/
+-rw-r--r--   0 root         (0) root         (0)      298 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/testing_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      510 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/testing_utils/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/testing_utils/es_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/testing_utils/features.py
+-rw-r--r--   0 root         (0) root         (0)    47175 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/testing_utils/mock_ds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/tests/utils_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/test_cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      787 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/test_description_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3446 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/test_entry_point.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/test_gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/test_time_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/tests/utils_tests/test_trie.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools/utils/
+-rw-r--r--   0 root         (0) root         (0)       34 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      298 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/api.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/common_tld_utils.py
+-rw-r--r--   0 root         (0) root         (0)      384 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/description_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/entry_point.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/plot_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/s3_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/spark_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/time_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/trie.py
+-rw-r--r--   0 root         (0) root         (0)     4537 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/utils/wrangle.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-06-10 15:21:35.000000 featuretools-1.9.2/featuretools/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13116 2022-06-10 15:21:54.000000 featuretools-1.9.2/featuretools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8903 2022-06-10 15:21:55.000000 featuretools-1.9.2/featuretools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 15:21:54.000000 featuretools-1.9.2/featuretools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2022-06-10 15:21:54.000000 featuretools-1.9.2/featuretools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 15:21:43.000000 featuretools-1.9.2/featuretools.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1426 2022-06-10 15:21:54.000000 featuretools-1.9.2/featuretools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-06-10 15:21:54.000000 featuretools-1.9.2/featuretools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      840 2022-06-10 15:21:35.000000 featuretools-1.9.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     3405 2022-06-10 15:21:55.000000 featuretools-1.9.2/setup.cfg
```

### Comparing `featuretools-1.9.1/LICENSE` & `featuretools-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/PKG-INFO` & `featuretools-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuretools
-Version: 1.9.1
+Version: 1.9.2
 Summary: a framework for automated feature engineering
 Home-page: https://github.com/alteryx/featuretools
 Download-URL: https://pypi.org/project/featuretools/
 Author: Alteryx, Inc.
 Author-email: open_source_support@alteryx.com
 License: BSD 3-clause
 Project-URL: Documentation, https://featuretools.alteryx.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: featuretools Version: 1.9.1 Summary: a framework
+Metadata-Version: 2.1 Name: featuretools Version: 1.9.2 Summary: a framework
 for automated feature engineering Home-page: https://github.com/alteryx/
 featuretools Download-URL: https://pypi.org/project/featuretools/ Author:
 Alteryx, Inc. Author-email: open_source_support@alteryx.com License: BSD 3-
 clause Project-URL: Documentation, https://featuretools.alteryx.com Project-
 URL: Source Code, https://github.com/alteryx/featuretools/ Project-URL:
 Changes, https://featuretools.alteryx.com/en/latest/release_notes.html Project-
 URL: Issue Tracker, https://github.com/alteryx/featuretools/issues Project-URL:
```

### Comparing `featuretools-1.9.1/README.md` & `featuretools-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/__init__.py` & `featuretools-1.9.2/featuretools/__init__.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/__main__.py` & `featuretools-1.9.2/featuretools/__main__.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/computational_backends/calculate_feature_matrix.py` & `featuretools-1.9.2/featuretools/computational_backends/calculate_feature_matrix.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/computational_backends/feature_set.py` & `featuretools-1.9.2/featuretools/computational_backends/feature_set.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/computational_backends/feature_set_calculator.py` & `featuretools-1.9.2/featuretools/computational_backends/feature_set_calculator.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/computational_backends/utils.py` & `featuretools-1.9.2/featuretools/computational_backends/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,18 +354,18 @@
         for name in names:
             logical_types[name] = feature.column_schema.logical_type
             semantic_tags[name] = feature.column_schema.semantic_tags.copy()
             semantic_tags[name] -= {"index", "time_index"}
 
             if logical_types[name] is None and "numeric" in semantic_tags[name]:
                 logical_types[name] = Double
-        if all([f.primitive is None for f in feature.get_dependencies(deep=True)]):
-            origins[name] = "base"
-        else:
-            origins[name] = "engineered"
+            if all([f.primitive is None for f in feature.get_dependencies(deep=True)]):
+                origins[name] = "base"
+            else:
+                origins[name] = "engineered"
 
     if pass_columns:
         cutoff_schema = cutoff_time.ww.schema
         for column in pass_columns:
             logical_types[column] = cutoff_schema.logical_types[column]
             semantic_tags[column] = cutoff_schema.semantic_tags[column]
             origins[column] = "base"
```

### Comparing `featuretools-1.9.1/featuretools/config_init.py` & `featuretools-1.9.2/featuretools/config_init.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/demo/flight.py` & `featuretools-1.9.2/featuretools/demo/flight.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/demo/mock_customer.py` & `featuretools-1.9.2/featuretools/demo/mock_customer.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/demo/retail.py` & `featuretools-1.9.2/featuretools/demo/retail.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/demo/weather.py` & `featuretools-1.9.2/featuretools/demo/weather.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/entityset/deserialize.py` & `featuretools-1.9.2/featuretools/entityset/deserialize.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/entityset/entityset.py` & `featuretools-1.9.2/featuretools/entityset/entityset.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/entityset/relationship.py` & `featuretools-1.9.2/featuretools/entityset/relationship.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/entityset/serialize.py` & `featuretools-1.9.2/featuretools/entityset/serialize.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/entityset/timedelta.py` & `featuretools-1.9.2/featuretools/entityset/timedelta.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/feature_base/feature_base.py` & `featuretools-1.9.2/featuretools/feature_base/feature_base.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/feature_base/feature_descriptions.py` & `featuretools-1.9.2/featuretools/feature_base/feature_descriptions.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/feature_base/feature_visualizer.py` & `featuretools-1.9.2/featuretools/feature_base/feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/feature_base/features_deserializer.py` & `featuretools-1.9.2/featuretools/feature_base/features_deserializer.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/feature_base/features_serializer.py` & `featuretools-1.9.2/featuretools/feature_base/features_serializer.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/__init__.py` & `featuretools-1.9.2/featuretools/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/base/aggregation_primitive_base.py` & `featuretools-1.9.2/featuretools/primitives/base/aggregation_primitive_base.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/base/primitive_base.py` & `featuretools-1.9.2/featuretools/primitives/base/primitive_base.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/base/transform_primitive_base.py` & `featuretools-1.9.2/featuretools/primitives/base/transform_primitive_base.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/data/free_email_provider_domains.txt` & `featuretools-1.9.2/featuretools/primitives/data/free_email_provider_domains.txt`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/data/free_email_provider_domains_license` & `featuretools-1.9.2/featuretools/primitives/data/free_email_provider_domains_license`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/options_utils.py` & `featuretools-1.9.2/featuretools/primitives/options_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/standard/aggregation_primitives.py` & `featuretools-1.9.2/featuretools/primitives/standard/aggregation_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/standard/binary_transform.py` & `featuretools-1.9.2/featuretools/primitives/standard/binary_transform.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/standard/cum_transform_feature.py` & `featuretools-1.9.2/featuretools/primitives/standard/cum_transform_feature.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/standard/datetime_transform_primitives.py` & `featuretools-1.9.2/featuretools/primitives/standard/datetime_transform_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/standard/latlong_transform_primitives.py` & `featuretools-1.9.2/featuretools/primitives/standard/latlong_transform_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/standard/rolling_transform_primitive.py` & `featuretools-1.9.2/featuretools/primitives/standard/rolling_transform_primitive.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/standard/transform_primitive.py` & `featuretools-1.9.2/featuretools/primitives/standard/transform_primitive.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/primitives/utils.py` & `featuretools-1.9.2/featuretools/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/selection/selection.py` & `featuretools-1.9.2/featuretools/selection/selection.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/synthesis/deep_feature_synthesis.py` & `featuretools-1.9.2/featuretools/synthesis/deep_feature_synthesis.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/synthesis/dfs.py` & `featuretools-1.9.2/featuretools/synthesis/dfs.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/synthesis/encode_features.py` & `featuretools-1.9.2/featuretools/synthesis/encode_features.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/synthesis/get_valid_primitives.py` & `featuretools-1.9.2/featuretools/synthesis/get_valid_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/synthesis/utils.py` & `featuretools-1.9.2/featuretools/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/cli_tests/test_cli.py` & `featuretools-1.9.2/featuretools/tests/cli_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/computational_backend/test_calculate_feature_matrix.py` & `featuretools-1.9.2/featuretools/tests/computational_backend/test_calculate_feature_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -2240,7 +2240,29 @@
     assert isinstance(es["customers"].ww.logical_types["age"], Age)
     assert isinstance(es["customers"].ww.logical_types["engagement_level"], Integer)
     assert isinstance(es["customers"].ww.logical_types["loves_ice_cream"], Boolean)
 
     assert isinstance(fm.ww.logical_types["age"], AgeNullable)
     assert isinstance(fm.ww.logical_types["engagement_level"], IntegerNullable)
     assert isinstance(fm.ww.logical_types["loves_ice_cream"], BooleanNullable)
+
+
+def test_feature_origins_present_on_all_fm_cols(pd_es):
+    class MultiCumSum(TransformPrimitive):
+        name = "multi_cum_sum"
+        input_types = [ColumnSchema(semantic_tags={"numeric"})]
+        return_type = ColumnSchema(semantic_tags={"numeric"})
+        number_output_features = 3
+
+        def get_function(self):
+            def multi_cum_sum(x):
+                return x.cumsum(), x.cummax(), x.cummin()
+
+            return multi_cum_sum
+
+    feature_matrix, _ = ft.dfs(
+        entityset=pd_es, target_dataframe_name="log", trans_primitives=[MultiCumSum]
+    )
+
+    for col in feature_matrix.columns:
+        origin = feature_matrix.ww[col].ww.origin
+        assert origin in ["base", "engineered"]
```

### Comparing `featuretools-1.9.1/featuretools/tests/computational_backend/test_dask_features.py` & `featuretools-1.9.2/featuretools/tests/computational_backend/test_dask_features.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/computational_backend/test_feature_set.py` & `featuretools-1.9.2/featuretools/tests/computational_backend/test_feature_set.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/computational_backend/test_feature_set_calculator.py` & `featuretools-1.9.2/featuretools/tests/computational_backend/test_feature_set_calculator.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/computational_backend/test_utils.py` & `featuretools-1.9.2/featuretools/tests/computational_backend/test_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/config_tests/test_config.py` & `featuretools-1.9.2/featuretools/tests/config_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/conftest.py` & `featuretools-1.9.2/featuretools/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/demo_tests/test_demo_data.py` & `featuretools-1.9.2/featuretools/tests/demo_tests/test_demo_data.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_dask_es.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_dask_es.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_es.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_es.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_es_metadata.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_es_metadata.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_last_time_index.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_last_time_index.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_plotting.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_relationship.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_relationship.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_serialization.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_spark_es.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_spark_es.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_timedelta.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_timedelta.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entityset_tests/test_ww_es.py` & `featuretools-1.9.2/featuretools/tests/entityset_tests/test_ww_es.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entry_point_tests/test_plugin.py` & `featuretools-1.9.2/featuretools/tests/entry_point_tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entry_point_tests/test_primitives.py` & `featuretools-1.9.2/featuretools/tests/entry_point_tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/entry_point_tests/utils.py` & `featuretools-1.9.2/featuretools/tests/entry_point_tests/utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_agg_feats.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_agg_feats.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_agg_primitives.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_agg_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_dask_primitives.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_dask_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_datetoholiday_primitive.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_datetoholiday_primitive.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_direct_features.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_direct_features.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_distancetoholiday_primitive.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_distancetoholiday_primitive.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_base.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_base.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_descriptions.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_descriptions.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_serialization.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_serialization.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_utils.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_feature_visualizer.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_features_deserializer.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_features_deserializer.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_features_serializer.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_features_serializer.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_groupby_transform_primitives.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_groupby_transform_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_identity_features.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_identity_features.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_is_federal_holiday.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_is_federal_holiday.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_latlong_primitives.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_latlong_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_overrides.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_overrides.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_primitive_base.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_primitive_base.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_primitive_utils.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_primitive_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_rolling_primitive.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_rolling_primitive.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_transform_features.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_transform_features.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/test_transform_primitive.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/test_transform_primitive.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/primitive_tests/utils.py` & `featuretools-1.9.2/featuretools/tests/primitive_tests/utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/selection/test_selection.py` & `featuretools-1.9.2/featuretools/tests/selection/test_selection.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/synthesis/test_dask_dfs.py` & `featuretools-1.9.2/featuretools/tests/synthesis/test_dask_dfs.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/synthesis/test_deep_feature_synthesis.py` & `featuretools-1.9.2/featuretools/tests/synthesis/test_deep_feature_synthesis.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/synthesis/test_dfs_method.py` & `featuretools-1.9.2/featuretools/tests/synthesis/test_dfs_method.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/synthesis/test_encode_features.py` & `featuretools-1.9.2/featuretools/tests/synthesis/test_encode_features.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/synthesis/test_get_valid_primitives.py` & `featuretools-1.9.2/featuretools/tests/synthesis/test_get_valid_primitives.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/synthesis/test_spark_dfs.py` & `featuretools-1.9.2/featuretools/tests/synthesis/test_spark_dfs.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/testing_utils/es_utils.py` & `featuretools-1.9.2/featuretools/tests/testing_utils/es_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/testing_utils/features.py` & `featuretools-1.9.2/featuretools/tests/testing_utils/features.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/testing_utils/mock_ds.py` & `featuretools-1.9.2/featuretools/tests/testing_utils/mock_ds.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/utils_tests/test_cli_utils.py` & `featuretools-1.9.2/featuretools/tests/utils_tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/utils_tests/test_config.py` & `featuretools-1.9.2/featuretools/tests/utils_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/utils_tests/test_description_utils.py` & `featuretools-1.9.2/featuretools/tests/utils_tests/test_description_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/utils_tests/test_entry_point.py` & `featuretools-1.9.2/featuretools/tests/utils_tests/test_entry_point.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/utils_tests/test_gen_utils.py` & `featuretools-1.9.2/featuretools/tests/utils_tests/test_gen_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/utils_tests/test_time_utils.py` & `featuretools-1.9.2/featuretools/tests/utils_tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/tests/utils_tests/test_trie.py` & `featuretools-1.9.2/featuretools/tests/utils_tests/test_trie.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/cli_utils.py` & `featuretools-1.9.2/featuretools/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/common_tld_utils.py` & `featuretools-1.9.2/featuretools/utils/common_tld_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/entry_point.py` & `featuretools-1.9.2/featuretools/utils/entry_point.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/gen_utils.py` & `featuretools-1.9.2/featuretools/utils/gen_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/plot_utils.py` & `featuretools-1.9.2/featuretools/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/s3_utils.py` & `featuretools-1.9.2/featuretools/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/spark_utils.py` & `featuretools-1.9.2/featuretools/utils/spark_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/time_utils.py` & `featuretools-1.9.2/featuretools/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/trie.py` & `featuretools-1.9.2/featuretools/utils/trie.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools/utils/wrangle.py` & `featuretools-1.9.2/featuretools/utils/wrangle.py`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools.egg-info/PKG-INFO` & `featuretools-1.9.2/featuretools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuretools
-Version: 1.9.1
+Version: 1.9.2
 Summary: a framework for automated feature engineering
 Home-page: https://github.com/alteryx/featuretools
 Download-URL: https://pypi.org/project/featuretools/
 Author: Alteryx, Inc.
 Author-email: open_source_support@alteryx.com
 License: BSD 3-clause
 Project-URL: Documentation, https://featuretools.alteryx.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: featuretools Version: 1.9.1 Summary: a framework
+Metadata-Version: 2.1 Name: featuretools Version: 1.9.2 Summary: a framework
 for automated feature engineering Home-page: https://github.com/alteryx/
 featuretools Download-URL: https://pypi.org/project/featuretools/ Author:
 Alteryx, Inc. Author-email: open_source_support@alteryx.com License: BSD 3-
 clause Project-URL: Documentation, https://featuretools.alteryx.com Project-
 URL: Source Code, https://github.com/alteryx/featuretools/ Project-URL:
 Changes, https://featuretools.alteryx.com/en/latest/release_notes.html Project-
 URL: Issue Tracker, https://github.com/alteryx/featuretools/issues Project-URL:
```

### Comparing `featuretools-1.9.1/featuretools.egg-info/SOURCES.txt` & `featuretools-1.9.2/featuretools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/featuretools.egg-info/requires.txt` & `featuretools-1.9.2/featuretools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/pyproject.toml` & `featuretools-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `featuretools-1.9.1/setup.cfg` & `featuretools-1.9.2/setup.cfg`

 * *Files identical despite different names*

