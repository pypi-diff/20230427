# Comparing `tmp/zdatasets-0.2.4.tar.gz` & `tmp/zdatasets-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdatasets-0.2.4.tar", max compression
+gzip compressed data, was "zdatasets-0.2.5.tar", max compression
```

## Comparing `zdatasets-0.2.4.tar` & `zdatasets-0.2.5.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0    11357 2022-12-08 20:20:45.697842 zdatasets-0.2.4/LICENSE
--rw-r--r--   0        0        0     1872 2022-12-08 20:20:45.697842 zdatasets-0.2.4/README.md
--rw-r--r--   0        0        0      431 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/__init__.py
--rw-r--r--   0        0        0      387 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/_typing.py
--rw-r--r--   0        0        0      269 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/context.py
--rw-r--r--   0        0        0     8435 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/dataset_plugin.py
--rwxr-xr-x   0        0        0     1828 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/datasets_decorator.py
--rw-r--r--   0        0        0       53 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/exceptions.py
--rw-r--r--   0        0        0     4452 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/metaflow.py
--rw-r--r--   0        0        0      295 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/mode.py
--rw-r--r--   0        0        0      404 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/batch/__init__.py
--rw-r--r--   0        0        0     6064 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/batch/batch_base_plugin.py
--rw-r--r--   0        0        0     9814 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/batch/batch_dataset.py
--rw-r--r--   0        0        0     2084 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/batch/flow_dataset.py
--rw-r--r--   0        0        0    10225 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/batch/hive_dataset.py
--rw-r--r--   0        0        0        0 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/executors/__init__.py
--rw-r--r--   0        0        0     1172 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/executors/metaflow_executor.py
--rw-r--r--   0        0        0      752 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/plugins/register_plugins.py
--rw-r--r--   0        0        0      850 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/program_executor.py
--rw-r--r--   0        0        0        0 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/tests/__init__.py
--rw-r--r--   0        0        0     1887 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/tests/conftest.py
--rw-r--r--   0        0        0    21810 2022-12-08 20:20:45.697842 zdatasets-0.2.4/datasets/tests/data/train/date=2020-07-23/region=king/data.parquet
--rw-r--r--   0        0        0    21810 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/data/train/date=2020-07-23/region=la/data.parquet
--rw-r--r--   0        0        0     9280 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/test_batch_dataset.py
--rw-r--r--   0        0        0    11420 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/test_dataset_plugin.py
--rw-r--r--   0        0        0     1489 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/test_datasets_decorator.py
--rw-r--r--   0        0        0      842 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/test_flow_dataset.py
--rw-r--r--   0        0        0    11095 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/test_hive_dataset.py
--rw-r--r--   0        0        0     4748 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/test_metaflow.py
--rw-r--r--   0        0        0     2173 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/test_tutorials.py
--rw-r--r--   0        0        0        0 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/utils/__init__.py
--rw-r--r--   0        0        0     1270 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/utils/test_case_utils.py
--rw-r--r--   0        0        0     2195 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/utils/test_partitions.py
--rw-r--r--   0        0        0     7252 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tests/utils/test_secret_fetcher.py
--rwxr-xr-x   0        0        0     1433 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/0_hello_dataset_flow.py
--rwxr-xr-x   0        0        0     1093 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/1_input_output_flow.py
--rwxr-xr-x   0        0        0      818 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/2_spark_dask_flow.py
--rwxr-xr-x   0        0        0     1449 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/3_foreach_dataset_flow.py
--rwxr-xr-x   0        0        0      910 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/4_hello_plugin_flow.py
--rwxr-xr-x   0        0        0     1450 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/5_consistent_flow.py
--rwxr-xr-x   0        0        0     1395 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/6_hive_dataset_flow.py
--rw-r--r--   0        0        0     3762 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/README.ipynb
--rw-r--r--   0        0        0     1751 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/tutorials/online_plugin.py
--rw-r--r--   0        0        0       63 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/utils/__init__.py
--rw-r--r--   0        0        0     4075 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/utils/aws.py
--rw-r--r--   0        0        0     1079 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/utils/case_utils.py
--rw-r--r--   0        0        0     2374 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/utils/partitions.py
--rw-r--r--   0        0        0     9584 2022-12-08 20:20:45.701842 zdatasets-0.2.4/datasets/utils/secret_fetcher.py
--rw-r--r--   0        0        0     2073 2022-12-08 20:20:45.701842 zdatasets-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 zdatasets-0.2.4/setup.py
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 zdatasets-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 19:33:50.998113 zdatasets-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1872 2023-04-27 19:33:50.998113 zdatasets-0.2.5/README.md
+-rw-r--r--   0        0        0      431 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/__init__.py
+-rw-r--r--   0        0        0      387 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/_typing.py
+-rw-r--r--   0        0        0      269 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/context.py
+-rw-r--r--   0        0        0     8435 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/dataset_plugin.py
+-rwxr-xr-x   0        0        0     1828 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/datasets_decorator.py
+-rw-r--r--   0        0        0       53 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/exceptions.py
+-rw-r--r--   0        0        0     4452 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/metaflow.py
+-rw-r--r--   0        0        0      295 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/mode.py
+-rw-r--r--   0        0        0      404 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/batch/__init__.py
+-rw-r--r--   0        0        0     6064 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/batch/batch_base_plugin.py
+-rw-r--r--   0        0        0     9814 2023-04-27 19:33:50.998113 zdatasets-0.2.5/datasets/plugins/batch/batch_dataset.py
+-rw-r--r--   0        0        0     2084 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/batch/flow_dataset.py
+-rw-r--r--   0        0        0    10225 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/batch/hive_dataset.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/executors/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/executors/metaflow_executor.py
+-rw-r--r--   0        0        0      752 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/plugins/register_plugins.py
+-rw-r--r--   0        0        0      850 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/program_executor.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/__init__.py
+-rw-r--r--   0        0        0     1887 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/conftest.py
+-rw-r--r--   0        0        0    21810 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=king/data.parquet
+-rw-r--r--   0        0        0    21810 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=la/data.parquet
+-rw-r--r--   0        0        0     9280 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_batch_dataset.py
+-rw-r--r--   0        0        0    11420 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_dataset_plugin.py
+-rw-r--r--   0        0        0     1489 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_datasets_decorator.py
+-rw-r--r--   0        0        0      842 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_flow_dataset.py
+-rw-r--r--   0        0        0    11095 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_hive_dataset.py
+-rw-r--r--   0        0        0     4748 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_metaflow.py
+-rw-r--r--   0        0        0     2173 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/test_tutorials.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1270 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/test_case_utils.py
+-rw-r--r--   0        0        0     2195 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/test_partitions.py
+-rw-r--r--   0        0        0     7252 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tests/utils/test_secret_fetcher.py
+-rwxr-xr-x   0        0        0     1433 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/0_hello_dataset_flow.py
+-rwxr-xr-x   0        0        0     1093 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/1_input_output_flow.py
+-rwxr-xr-x   0        0        0      818 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/2_spark_dask_flow.py
+-rwxr-xr-x   0        0        0     1449 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/3_foreach_dataset_flow.py
+-rwxr-xr-x   0        0        0      910 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/4_hello_plugin_flow.py
+-rwxr-xr-x   0        0        0     1450 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/5_consistent_flow.py
+-rwxr-xr-x   0        0        0     1395 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/6_hive_dataset_flow.py
+-rw-r--r--   0        0        0     3762 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/README.ipynb
+-rw-r--r--   0        0        0     1751 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/tutorials/online_plugin.py
+-rw-r--r--   0        0        0       63 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     4075 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/aws.py
+-rw-r--r--   0        0        0     1079 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/case_utils.py
+-rw-r--r--   0        0        0     2374 2023-04-27 19:33:51.002113 zdatasets-0.2.5/datasets/utils/partitions.py
+-rw-r--r--   0        0        0     9584 2023-04-27 19:33:51.006113 zdatasets-0.2.5/datasets/utils/secret_fetcher.py
+-rw-r--r--   0        0        0     2073 2023-04-27 19:33:51.006113 zdatasets-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 zdatasets-0.2.5/PKG-INFO
```

### Comparing `zdatasets-0.2.4/LICENSE` & `zdatasets-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/README.md` & `zdatasets-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/dataset_plugin.py` & `zdatasets-0.2.5/datasets/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/datasets_decorator.py` & `zdatasets-0.2.5/datasets/datasets_decorator.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/metaflow.py` & `zdatasets-0.2.5/datasets/metaflow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/plugins/batch/batch_base_plugin.py` & `zdatasets-0.2.5/datasets/plugins/batch/batch_base_plugin.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/plugins/batch/batch_dataset.py` & `zdatasets-0.2.5/datasets/plugins/batch/batch_dataset.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/plugins/batch/flow_dataset.py` & `zdatasets-0.2.5/datasets/plugins/batch/flow_dataset.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/plugins/batch/hive_dataset.py` & `zdatasets-0.2.5/datasets/plugins/batch/hive_dataset.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/plugins/executors/metaflow_executor.py` & `zdatasets-0.2.5/datasets/plugins/executors/metaflow_executor.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/plugins/register_plugins.py` & `zdatasets-0.2.5/datasets/plugins/register_plugins.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/program_executor.py` & `zdatasets-0.2.5/datasets/program_executor.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/conftest.py` & `zdatasets-0.2.5/datasets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/data/train/date=2020-07-23/region=king/data.parquet` & `zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=king/data.parquet`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/data/train/date=2020-07-23/region=la/data.parquet` & `zdatasets-0.2.5/datasets/tests/data/train/date=2020-07-23/region=la/data.parquet`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/test_batch_dataset.py` & `zdatasets-0.2.5/datasets/tests/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/test_dataset_plugin.py` & `zdatasets-0.2.5/datasets/tests/test_dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/test_datasets_decorator.py` & `zdatasets-0.2.5/datasets/tests/test_datasets_decorator.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/test_flow_dataset.py` & `zdatasets-0.2.5/datasets/tests/test_flow_dataset.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/test_hive_dataset.py` & `zdatasets-0.2.5/datasets/tests/test_hive_dataset.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/test_metaflow.py` & `zdatasets-0.2.5/datasets/tests/test_metaflow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/test_tutorials.py` & `zdatasets-0.2.5/datasets/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/utils/test_case_utils.py` & `zdatasets-0.2.5/datasets/tests/utils/test_case_utils.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/utils/test_partitions.py` & `zdatasets-0.2.5/datasets/tests/utils/test_partitions.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tests/utils/test_secret_fetcher.py` & `zdatasets-0.2.5/datasets/tests/utils/test_secret_fetcher.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/0_hello_dataset_flow.py` & `zdatasets-0.2.5/datasets/tutorials/0_hello_dataset_flow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/1_input_output_flow.py` & `zdatasets-0.2.5/datasets/tutorials/1_input_output_flow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/2_spark_dask_flow.py` & `zdatasets-0.2.5/datasets/tutorials/2_spark_dask_flow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/3_foreach_dataset_flow.py` & `zdatasets-0.2.5/datasets/tutorials/3_foreach_dataset_flow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/4_hello_plugin_flow.py` & `zdatasets-0.2.5/datasets/tutorials/4_hello_plugin_flow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/5_consistent_flow.py` & `zdatasets-0.2.5/datasets/tutorials/5_consistent_flow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/6_hive_dataset_flow.py` & `zdatasets-0.2.5/datasets/tutorials/6_hive_dataset_flow.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/README.ipynb` & `zdatasets-0.2.5/datasets/tutorials/README.ipynb`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/tutorials/online_plugin.py` & `zdatasets-0.2.5/datasets/tutorials/online_plugin.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/utils/aws.py` & `zdatasets-0.2.5/datasets/utils/aws.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/utils/case_utils.py` & `zdatasets-0.2.5/datasets/utils/case_utils.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/utils/partitions.py` & `zdatasets-0.2.5/datasets/utils/partitions.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/datasets/utils/secret_fetcher.py` & `zdatasets-0.2.5/datasets/utils/secret_fetcher.py`

 * *Files identical despite different names*

### Comparing `zdatasets-0.2.4/pyproject.toml` & `zdatasets-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zdatasets"
-version = "0.2.4"
+version = "0.2.5"
 description = "Dataset SDK for consistent read/write [batch, online, streaming] data."
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
@@ -27,15 +27,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4"
 pandas = ">=1.1.0"
 pyarrow = ">=6.0.0"
 dask = { version = ">=2021.9.1", optional = true }
 pyspark = { version = "^3.2.0", optional = true }
-importlib-metadata = ">=4.8.1"
+importlib-metadata = ">=4.6.1"
 click = ">=7.0,<8.1"
 s3fs = ">=2022.1.0"
 tenacity = ">=5.0"
 kubernetes = { version = ">=12.0.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 mypy = ">=0.910"
```

### Comparing `zdatasets-0.2.4/PKG-INFO` & `zdatasets-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatasets
-Version: 0.2.4
+Version: 0.2.5
 Summary: Dataset SDK for consistent read/write [batch, online, streaming] data.
 Author: Taleb Zeghmi
 Requires-Python: >=3.8.0,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dask
 Provides-Extra: doc
 Provides-Extra: kubernetes
 Provides-Extra: metaflow
 Provides-Extra: spark
 Requires-Dist: click (>=7.0,<8.1)
-Requires-Dist: dask (>=2021.9.1); extra == "dask"
-Requires-Dist: importlib-metadata (>=4.8.1)
-Requires-Dist: kubernetes (>=12.0.0); extra == "kubernetes"
+Requires-Dist: dask (>=2021.9.1) ; extra == "dask"
+Requires-Dist: importlib-metadata (>=4.6.1)
+Requires-Dist: kubernetes (>=12.0.0) ; extra == "kubernetes"
 Requires-Dist: pandas (>=1.1.0)
 Requires-Dist: pyarrow (>=6.0.0)
-Requires-Dist: pyspark (>=3.2.0,<4.0.0); extra == "spark"
+Requires-Dist: pyspark (>=3.2.0,<4.0.0) ; extra == "spark"
 Requires-Dist: s3fs (>=2022.1.0)
 Requires-Dist: tenacity (>=5.0)
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/zillow/datasets/actions/workflows/test.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/zillow/datasets/badge.svg)](https://coveralls.io/github/zillow/datasets)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zillow/datasets/main?urlpath=lab/tree/datasets/tutorials)
```

