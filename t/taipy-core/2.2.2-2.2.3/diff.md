# Comparing `tmp/taipy-core-2.2.2.tar.gz` & `tmp/taipy-core-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.2.2.tar", last modified: Fri Apr 14 17:12:46 2023, max compression
+gzip compressed data, was "taipy-core-2.2.3.tar", last modified: Thu Apr 27 12:02:02 2023, max compression
```

## Comparing `taipy-core-2.2.2.tar` & `taipy-core-2.2.3.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-14 17:12:36.000000 taipy-core-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 17:12:36.000000 taipy-core-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-14 17:12:46.616891 taipy-core-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-14 17:12:36.000000 taipy-core-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 17:12:36.000000 taipy-core-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:12:46.616891 taipy-core-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-14 17:12:36.000000 taipy-core-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.596891 taipy-core-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.596891 taipy-core-2.2.2/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.596891 taipy-core-2.2.2/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_abstract_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.604891 taipy-core-2.2.2/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_get_valid_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/default_custom_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.604891 taipy-core-2.2.2/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.604891 taipy-core-2.2.2/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    32343 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.608891 taipy-core-2.2.2/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:12:39.000000 taipy-core-2.2.2/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-14 17:12:36.000000 taipy-core-2.2.2/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-04-14 17:12:36.000000 taipy-core-2.2.2/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.591877 taipy-core-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-27 12:01:50.000000 taipy-core-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 12:01:50.000000 taipy-core-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-27 12:02:02.591877 taipy-core-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-27 12:01:50.000000 taipy-core-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 12:01:50.000000 taipy-core-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:02:02.591877 taipy-core-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-27 12:01:50.000000 taipy-core-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.571875 taipy-core-2.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.571875 taipy-core-2.2.3/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.571875 taipy-core-2.2.3/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_abstract_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.575876 taipy-core-2.2.3/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_get_valid_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/common/default_custom_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32343 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.579876 taipy-core-2.2.3/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/cycle/cycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.583876 taipy-core-2.2.3/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.583876 taipy-core-2.2.3/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.583876 taipy-core-2.2.3/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 12:01:50.000000 taipy-core-2.2.3/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:01:55.000000 taipy-core-2.2.3/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 12:02:02.000000 taipy-core-2.2.3/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:02:02.587876 taipy-core-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-27 12:01:50.000000 taipy-core-2.2.3/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-04-27 12:01:50.000000 taipy-core-2.2.3/tests/test_taipy.py
```

### Comparing `taipy-core-2.2.2/LICENSE` & `taipy-core-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/PKG-INFO` & `taipy-core-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.2.2/README.md` & `taipy-core-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/setup.py` & `taipy-core-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/__init__.py` & `taipy-core-2.2.3/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/__init__.py` & `taipy-core-2.2.3/src/taipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_core.py` & `taipy-core-2.2.3/src/taipy/core/_core.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_manager/__init__.py` & `taipy-core-2.2.3/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_manager/_manager.py` & `taipy-core-2.2.3/src/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_repository/__init__.py` & `taipy-core-2.2.3/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-2.2.3/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_repository/_repository.py` & `taipy-core-2.2.3/src/taipy/core/_repository/_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-2.2.3/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_repository/_sql_model.py` & `taipy-core-2.2.3/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/__init__.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/_abstract_scheduler.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/_abstract_scheduler.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/__init__.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler_factory.py` & `taipy-core-2.2.3/src/taipy/core/_scheduler/_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/__init__.py` & `taipy-core-2.2.3/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_utils.py` & `taipy-core-2.2.3/src/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_cli.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_manager.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # specific language governing permissions and limitations under the License.
 
 import uuid
 from typing import List, Optional, Union
 
 from taipy.config import Config
 from taipy.config._config_comparator import _ConfigComparator
+from taipy.config.exceptions.exceptions import InconsistentEnvVariableError
 from taipy.logger._taipy_logger import _TaipyLogger
 
 from .._manager._manager import _Manager
 from ..exceptions.exceptions import ModelNotFound, NonExistingVersion, VersionConflictWithPythonConfig
 from ._version import _Version
 from ._version_repository_factory import _VersionRepositoryFactory
 
@@ -173,15 +174,19 @@
             return cls._get_latest_version()
         if version_number in cls.__DEVELOPMENT_VERSION:
             return cls._get_development_version()
         if version_number in cls.__PRODUCTION_VERSION:
             return cls._get_production_version()
         if version_number in cls.__ALL_VERSION:
             return ""
-        if version := cls._get(version_number):
-            return version.id
+
+        try:
+            if version := cls._get(version_number):
+                return version.id
+        except InconsistentEnvVariableError:  # The version exist but the Config is alternated
+            return version_number
 
         raise NonExistingVersion(version_number)
 
     @classmethod
     def _delete_entities_of_multiple_types(cls, _entity_ids):
         return NotImplementedError
```

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_model.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_repository.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/__init__.py` & `taipy-core-2.2.3/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_entity.py` & `taipy-core-2.2.3/src/taipy/core/common/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_entity_ids.py` & `taipy-core-2.2.3/src/taipy/core/common/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_get_valid_filename.py` & `taipy-core-2.2.3/src/taipy/core/common/_get_valid_filename.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_listattributes.py` & `taipy-core-2.2.3/src/taipy/core/common/_listattributes.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_properties.py` & `taipy-core-2.2.3/src/taipy/core/common/_properties.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_reload.py` & `taipy-core-2.2.3/src/taipy/core/common/_reload.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_repr_enum.py` & `taipy-core-2.2.3/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_utils.py` & `taipy-core-2.2.3/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/_warnings.py` & `taipy-core-2.2.3/src/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/alias.py` & `taipy-core-2.2.3/src/taipy/core/common/alias.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/common/default_custom_document.py` & `taipy-core-2.2.3/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/__init__.py` & `taipy-core-2.2.3/src/taipy/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/checkers/__init__.py` & `taipy-core-2.2.3/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-2.2.3/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-2.2.3/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-2.2.3/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-2.2.3/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-2.2.3/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/config.schema.json` & `taipy-core-2.2.3/src/taipy/core/config/config.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997500644031643%*

 * *Differences: {"'properties'": "{'DATA_NODE': {'additionalProperties': {'properties': {'scope': {'enum': "*

 * *                 "{insert: [(0, 'GLOBAL:SCOPE'), (1, 'CYCLE:SCOPE'), (2, 'SCENARIO:SCOPE'), (3, "*

 * *                 "'PIPELINE:SCOPE')], delete: [3, 2, 1, 0]}, 'default': 'SCENARIO:SCOPE'}, 'else': "*

 * *                 "{'else': {'then': {'then': {'if': {'properties': {'storage_type': {replace: "*

 * *                 "OrderedDict([('const', 'sql')])}}}, 'else': {replace: OrderedDict([('required', "*

 * *                 "['tabl […]*

```diff
@@ -81,19 +81,17 @@
                                             "mongo_collection"
                                         ]
                                     }
                                 }
                             },
                             "then": {
                                 "else": {
-                                    "then": {
-                                        "required": [
-                                            "collection_name"
-                                        ]
-                                    }
+                                    "required": [
+                                        "collection_name"
+                                    ]
                                 },
                                 "if": {
                                     "properties": {
                                         "storage_type": {
                                             "enum": [
                                                 "sql",
                                                 "sql_table"
@@ -102,24 +100,22 @@
                                     }
                                 },
                                 "required": [
                                     "db_name"
                                 ],
                                 "then": {
                                     "else": {
-                                        "then": {
-                                            "required": [
-                                                "table_name"
-                                            ]
-                                        }
+                                        "required": [
+                                            "table_name"
+                                        ]
                                     },
                                     "if": {
                                         "properties": {
                                             "storage_type": {
-                                                "constant": "sql"
+                                                "const": "sql"
                                             }
                                         }
                                     },
                                     "required": [
                                         "db_username",
                                         "db_password",
                                         "db_engine"
@@ -189,21 +185,21 @@
                         "type": "object"
                     },
                     "read_query": {
                         "description": "storage_type: sql, mongo_collection specific. The query that will be used by Taipy to read the data from the database.",
                         "type": "string"
                     },
                     "scope": {
-                        "default": "SCENARIO",
+                        "default": "SCENARIO:SCOPE",
                         "description": "An enum value among GLOBAL, CYCLE, SCENARIO or PIPELINE that represents the visibility of the data node in the graph of entities.",
                         "enum": [
-                            "GLOBAL",
-                            "CYCLE",
-                            "SCENARIO",
-                            "PIPELINE",
+                            "GLOBAL:SCOPE",
+                            "CYCLE:SCOPE",
+                            "SCENARIO:SCOPE",
+                            "PIPELINE:SCOPE",
                             ""
                         ],
                         "type": "string"
                     },
                     "sheet_name": {
                         "description": "storage_type: excel specific. If sheet_name is provided with a list of sheet names, the data node will return a dictionary with the key being the sheet name and the value being the data of the corresponding sheet. If a string is provided, the data node will read only the data of the corresponding sheet. The default value of sheet_name is None and the data node will return all sheets in the provided Excel file when reading it.",
                         "type": "string"
@@ -261,22 +257,26 @@
             "type": "object"
         },
         "JOB": {
             "description": "Job",
             "properties": {
                 "max_nb_of_workers": {
                     "description": "mode: standalone specific. The maximum number of jobs able to run in parallel.",
-                    "type": "int"
+                    "type": [
+                        "integer",
+                        "string"
+                    ]
                 },
                 "mode": {
                     "default": "standalone",
                     "enum": [
                         "standalone",
                         "development"
-                    ]
+                    ],
+                    "type": "string"
                 }
             },
             "type": "object"
         },
         "PIPELINE": {
             "additionalProperties": {
                 "properties": {
@@ -306,19 +306,20 @@
                             "type": "string"
                         },
                         "type": "array"
                     },
                     "frequency": {
                         "description": "The recurrence of the scenarios instantiated from this configuration. Based on this frequency the scenarios will be attached to the right cycles.",
                         "enum": [
-                            "DAILY",
-                            "WEEKLY",
-                            "MONTHLY",
-                            "QUARTERLY",
-                            "YEARLY"
+                            "DAILY:FREQUENCY",
+                            "WEEKLY:FREQUENCY",
+                            "MONTHLY:FREQUENCY",
+                            "QUARTERLY:FREQUENCY",
+                            "YEARLY:FREQUENCY",
+                            ""
                         ],
                         "type": "string"
                     },
                     "pipelines": {
                         "description": "The list of pipeline configs.",
                         "items": {
                             "type": "string"
@@ -339,30 +340,35 @@
             "properties": {
                 "clean_entities_enabled": {
                     "default": "False:bool",
                     "description": "Boolean field to activate/deactivate the clean entities feature.",
                     "enum": [
                         "True:bool",
                         "False:bool"
-                    ]
+                    ],
+                    "type": "string"
                 },
                 "read_entity_retry": {
                     "description": "Number of times to retry before return failure to read an entity.",
-                    "type": "int"
+                    "type": [
+                        "integer",
+                        "string"
+                    ]
                 },
                 "repository_properties": {
                     "type": "object"
                 },
                 "repository_type": {
                     "default": "filesystem",
                     "description": "The repository type that is used to store the entities.",
                     "enum": [
                         "sql",
                         "filesystem"
-                    ]
+                    ],
+                    "type": "string"
                 },
                 "root_folder": {
                     "description": "Path of the base folder for the taipy application. The default value is ./taipy/",
                     "type": "string"
                 },
                 "storage_folder": {
                     "description": "Folder name used to store Taipy data. The default value is .data/. It is used in conjunction with the root_folder field",
@@ -393,15 +399,15 @@
                             "type": "string"
                         },
                         "type": "array",
                         "uniqueItems": true
                     },
                     "skippable": {
                         "default": "False:bool",
-                        "description": "A boolean value. True if the task can be skipped if the inputs have been updated since last run.",
+                        "description": "A boolean value as a string: one of [False:bool, True:bool].",
                         "enum": [
                             "False:bool",
                             "True:bool"
                         ],
                         "type": "string"
                     }
                 },
```

### Comparing `taipy-core-2.2.2/src/taipy/core/config/data_node_config.py` & `taipy-core-2.2.3/src/taipy/core/config/data_node_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/job_config.py` & `taipy-core-2.2.3/src/taipy/core/config/job_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/pipeline_config.py` & `taipy-core-2.2.3/src/taipy/core/config/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/scenario_config.py` & `taipy-core-2.2.3/src/taipy/core/config/scenario_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/config/task_config.py` & `taipy-core-2.2.3/src/taipy/core/config/task_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/__init__.py` & `taipy-core-2.2.3/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/cycle/cycle.py` & `taipy-core-2.2.3/src/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/__init__.py` & `taipy-core-2.2.3/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-2.2.3/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_data_manager.py` & `taipy-core-2.2.3/src/taipy/core/data/_data_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_data_model.py` & `taipy-core-2.2.3/src/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_data_repository.py` & `taipy-core-2.2.3/src/taipy/core/data/_data_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/_filter.py` & `taipy-core-2.2.3/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/abstract_sql.py` & `taipy-core-2.2.3/src/taipy/core/data/abstract_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/csv.py` & `taipy-core-2.2.3/src/taipy/core/data/csv.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/data_node.py` & `taipy-core-2.2.3/src/taipy/core/data/data_node.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/excel.py` & `taipy-core-2.2.3/src/taipy/core/data/excel.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/generic.py` & `taipy-core-2.2.3/src/taipy/core/data/generic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/in_memory.py` & `taipy-core-2.2.3/src/taipy/core/data/in_memory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/json.py` & `taipy-core-2.2.3/src/taipy/core/data/json.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/mongo.py` & `taipy-core-2.2.3/src/taipy/core/data/mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/operator.py` & `taipy-core-2.2.3/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/parquet.py` & `taipy-core-2.2.3/src/taipy/core/data/parquet.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/pickle.py` & `taipy-core-2.2.3/src/taipy/core/data/pickle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/sql.py` & `taipy-core-2.2.3/src/taipy/core/data/sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/data/sql_table.py` & `taipy-core-2.2.3/src/taipy/core/data/sql_table.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/exceptions/__init__.py` & `taipy-core-2.2.3/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/exceptions/exceptions.py` & `taipy-core-2.2.3/src/taipy/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/__init__.py` & `taipy-core-2.2.3/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-2.2.3/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/_job_manager.py` & `taipy-core-2.2.3/src/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/_job_model.py` & `taipy-core-2.2.3/src/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/_job_repository.py` & `taipy-core-2.2.3/src/taipy/core/job/_job_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/job.py` & `taipy-core-2.2.3/src/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/job/status.py` & `taipy-core-2.2.3/src/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/__init__.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/pipeline/pipeline.py` & `taipy-core-2.2.3/src/taipy/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/__init__.py` & `taipy-core-2.2.3/src/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/scenario/scenario.py` & `taipy-core-2.2.3/src/taipy/core/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/taipy.py` & `taipy-core-2.2.3/src/taipy/core/taipy.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/__init__.py` & `taipy-core-2.2.3/src/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-2.2.3/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/_task_manager.py` & `taipy-core-2.2.3/src/taipy/core/task/_task_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-2.2.3/src/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/_task_model.py` & `taipy-core-2.2.3/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/_task_repository.py` & `taipy-core-2.2.3/src/taipy/core/task/_task_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-2.2.3/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-2.2.3/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy/core/task/task.py` & `taipy-core-2.2.3/src/taipy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-2.2.3/src/taipy_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.2.2/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-2.2.3/src/taipy_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/tests/test_complex_application.py` & `taipy-core-2.2.3/tests/test_complex_application.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.2/tests/test_taipy.py` & `taipy-core-2.2.3/tests/test_taipy.py`

 * *Files identical despite different names*

