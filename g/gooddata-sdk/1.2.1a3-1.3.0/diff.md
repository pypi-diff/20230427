# Comparing `tmp/gooddata-sdk-1.2.1a3.tar.gz` & `tmp/gooddata-sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-sdk-1.2.1a3.tar", last modified: Mon Feb  6 14:22:52 2023, max compression
+gzip compressed data, was "gooddata-sdk-1.3.0.tar", last modified: Fri Mar 10 09:53:34 2023, max compression
```

## Comparing `gooddata-sdk-1.2.1a3.tar` & `gooddata-sdk-1.3.0.tar`

### file list

```diff
@@ -1,123 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.118307 gooddata-sdk-1.2.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-02-06 14:22:52.118307 gooddata-sdk-1.2.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.090306 gooddata-sdk-1.2.1a3/gooddata_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.094306 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/catalog_service_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.094306 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.098307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/action_requests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/action_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/action_requests/ldm_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/action_requests/scan_model_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.098307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.098307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.098307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.098307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.102306 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/validation/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/validation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.102306 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.102306 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/entity_model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.102306 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.102306 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/declarative_model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.106307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.106307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.106307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/entity_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/entity_model/user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.110307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21781 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/content_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.110307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.110307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.110307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.110307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.110307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.114307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.114307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.114307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.114307 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/model_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.114307 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.118307 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/compute/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/insight.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-02-06 14:22:36.000000 gooddata-sdk-1.2.1a3/gooddata_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 14:22:52.090306 gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-02-06 14:22:52.000000 gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-02-06 14:22:52.000000 gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 14:22:52.000000 gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-06 14:22:52.000000 gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-06 14:22:52.000000 gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 14:22:52.118307 gooddata-sdk-1.2.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-06 14:22:43.000000 gooddata-sdk-1.2.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/catalog_service_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/sql_column.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/validation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/entity_model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/declarative_model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/entity_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/entity_model/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21781 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/content_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.371024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/model_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/gooddata_sdk/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/gooddata_sdk/compute/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/model/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/model/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/compute/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/gooddata_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.367024 gooddata-sdk-1.3.0/gooddata_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-10 09:53:34.000000 gooddata-sdk-1.3.0/gooddata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-03-10 09:53:34.000000 gooddata-sdk-1.3.0/gooddata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:53:34.000000 gooddata-sdk-1.3.0/gooddata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-10 09:53:34.000000 gooddata-sdk-1.3.0/gooddata_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-10 09:53:34.000000 gooddata-sdk-1.3.0/gooddata_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:53:34.375024 gooddata-sdk-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-03-10 09:53:24.000000 gooddata-sdk-1.3.0/tests/test_type_converter.py
```

### Comparing `gooddata-sdk-1.2.1a3/LICENSE.txt` & `gooddata-sdk-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/PKG-INFO` & `gooddata-sdk-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.2.1a3
+Version: 1.3.0
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-sdk.readthedocs.io/en/v1.2.1a3
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,15 +34,15 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.3) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
 -  Python 3.7 or newer
 
 ## Installation
```

### Comparing `gooddata-sdk-1.2.1a3/README.md` & `gooddata-sdk-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.3) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
 -  Python 3.7 or newer
 
 ## Installation
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/__init__.py` & `gooddata-sdk-1.3.0/gooddata_sdk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,35 +3,46 @@
 
 At the moment the SDK provides services to inspect and interact with the Semantic Model and consume analytics.
 """
 
 import logging
 
 from gooddata_sdk._version import __version__
-from gooddata_sdk.catalog.data_source.action_requests.ldm_request import CatalogGenerateLdmRequest
-from gooddata_sdk.catalog.data_source.action_requests.scan_model_request import CatalogScanModelRequest
+from gooddata_sdk.catalog.data_source.action_model.requests.ldm_request import (
+    CatalogGenerateLdmRequest,
+    CatalogPdmLdmRequest,
+    CatalogPdmSql,
+)
+from gooddata_sdk.catalog.data_source.action_model.requests.scan_model_request import CatalogScanModelRequest
+from gooddata_sdk.catalog.data_source.action_model.requests.scan_sql_request import ScanSqlRequest
+from gooddata_sdk.catalog.data_source.action_model.responses.scan_sql_response import ScanSqlResponse
+from gooddata_sdk.catalog.data_source.action_model.sql_column import SqlColumn
 from gooddata_sdk.catalog.data_source.declarative_model.data_source import (
     CatalogDeclarativeDataSource,
     CatalogDeclarativeDataSources,
     CatalogDeclarativeTables,
 )
 from gooddata_sdk.catalog.data_source.declarative_model.physical_model.table import (
     CatalogDeclarativeColumn,
     CatalogDeclarativeTable,
 )
 from gooddata_sdk.catalog.data_source.entity_model.content_objects.table import CatalogDataSourceTable
 from gooddata_sdk.catalog.data_source.entity_model.data_source import (
     CatalogDataSource,
     CatalogDataSourceBigQuery,
+    CatalogDataSourceDatabricks,
     CatalogDataSourceGreenplum,
+    CatalogDataSourceMsSql,
     CatalogDataSourcePostgres,
     CatalogDataSourceRedshift,
     CatalogDataSourceSnowflake,
     CatalogDataSourceVertica,
+    DatabricksAttributes,
     GreenplumAttributes,
+    MsSqlAttributes,
     PostgresAttributes,
     RedshiftAttributes,
     SnowflakeAttributes,
     VerticaAttributes,
 )
 from gooddata_sdk.catalog.data_source.service import CatalogDataSourceService
 from gooddata_sdk.catalog.data_source.validation.data_source import DataSourceValidator
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/base.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/catalog_service_base.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/catalog_service_base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/action_requests/scan_model_request.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # (C) 2022 GoodData Corporation
 from __future__ import annotations
 
-from typing import Any, Optional, Type
+from typing import Any, List, Optional, Type
 
 import attr
 from attr import field
 
 from gooddata_api_client.model.scan_request import ScanRequest
 from gooddata_sdk.catalog.base import Base
 
@@ -18,12 +18,12 @@
 @attr.s(auto_attribs=True, kw_only=True)
 class CatalogScanModelRequest(Base):
     separator: str = "__"
     scan_tables: bool = field(default=True, validator=one_scan_true)
     scan_views: bool = field(default=False, validator=one_scan_true)
     table_prefix: Optional[str] = None
     view_prefix: Optional[str] = None
-    schemata: Optional[list[str]] = None
+    schemata: Optional[List[str]] = None
 
     @staticmethod
     def client_class() -> Type[ScanRequest]:
         return ScanRequest
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/data_source.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/entity_model/data_source.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/entity_model/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,7 +202,45 @@
     type: str = "BIGQUERY"
 
 
 @attr.s(auto_attribs=True, kw_only=True)
 class CatalogDataSourceGreenplum(CatalogDataSourcePostgres):
     type: str = "GREENPLUM"
     db_vendor: str = "postgresql"
+
+
+@attr.s(auto_attribs=True, kw_only=True)
+class MsSqlAttributes(DatabaseAttributes):
+    host: str
+    db_name: str
+    port: str = "1433"
+
+
+@attr.s(auto_attribs=True, kw_only=True)
+class CatalogDataSourceMsSql(CatalogDataSource):
+    _URL_TMPL: ClassVar[str] = "jdbc:{db_vendor}://{host}:{port};databaseName={db_name}"
+    type: str = "MSSQL"
+    db_vendor: str = "sqlserver"
+    db_specific_attributes: MsSqlAttributes
+
+
+@attr.s(auto_attribs=True, kw_only=True)
+class DatabricksAttributes(DatabaseAttributes):
+    host: str
+    http_path: str
+    port: str = "443"
+
+
+@attr.s(auto_attribs=True, kw_only=True)
+class CatalogDataSourceDatabricks(CatalogDataSource):
+    _URL_TMPL: ClassVar[str] = "jdbc:{db_vendor}://{host}:{port}/default;httpPath={http_path}"
+    type: str = "DATABRICKS"
+    parameters: List[Dict[str, str]]
+    db_specific_attributes: DatabricksAttributes
+
+    def __attrs_post_init__(self) -> None:
+        mandatory_parameter = [parameter.get("name") == "catalog" for parameter in self.parameters]
+        if not any(mandatory_parameter):
+            raise ValueError(f"'catalog' is mandatory parameter for data source type {self.type}")
+
+        self.db_vendor = self.type.lower()
+        self.url = self._make_url()
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/service.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import functools
 from pathlib import Path
 from typing import Any, List, Optional
 
 from gooddata_api_client.exceptions import NotFoundException
 from gooddata_api_client.model.declarative_pdm import DeclarativePdm
 from gooddata_sdk.catalog.catalog_service_base import CatalogServiceBase
-from gooddata_sdk.catalog.data_source.action_requests.ldm_request import CatalogGenerateLdmRequest
-from gooddata_sdk.catalog.data_source.action_requests.scan_model_request import CatalogScanModelRequest
+from gooddata_sdk.catalog.data_source.action_model.requests.ldm_request import CatalogGenerateLdmRequest
+from gooddata_sdk.catalog.data_source.action_model.requests.scan_model_request import CatalogScanModelRequest
+from gooddata_sdk.catalog.data_source.action_model.requests.scan_sql_request import ScanSqlRequest
+from gooddata_sdk.catalog.data_source.action_model.responses.scan_sql_response import ScanSqlResponse
 from gooddata_sdk.catalog.data_source.declarative_model.data_source import (
     BIGQUERY_TYPE,
     CatalogDeclarativeDataSource,
     CatalogDeclarativeDataSources,
 )
 from gooddata_sdk.catalog.data_source.declarative_model.physical_model.pdm import (
     CatalogDeclarativeTables,
@@ -40,14 +42,15 @@
     # Entities methods are listed below
 
     def create_or_update_data_source(
         self,
         data_source: CatalogDataSource,
     ) -> None:
         """Pushes the Data Source to the GoodData environment.
+
         Automatically decides, whether to create or update.
 
         Args:
             data_source (CatalogDataSource):
                 Catalog Data Source object
 
         Returns:
@@ -180,14 +183,15 @@
         if test_data_sources:
             self.test_data_sources_connection(declarative_data_sources, credentials_path)
         credentials = self._credentials_from_file(credentials_path) if credentials_path is not None else dict()
         self._layout_api.put_data_sources_layout(declarative_data_sources.to_api(credentials))
 
     def store_declarative_data_sources(self, layout_root_path: Path = Path.cwd()) -> None:
         """Store data sources layouts in a directory hierarchy.
+
             gooddata_layouts
             └── organization_id
                     └── data_sources
                             ├── data_source_a
                             │       ├── pdm
                             │       │   ├── table_A.yaml
                             │       │   └── table_B.yaml
@@ -222,16 +226,18 @@
 
     def load_and_put_declarative_data_sources(
         self,
         layout_root_path: Path = Path.cwd(),
         credentials_path: Optional[Path] = None,
         test_data_sources: bool = False,
     ) -> None:
-        """This method combines load_declarative_data_sources and put_declarative_data_sources
-            methods to load and set layouts stored using store_declarative_data_sources.
+        """Loads and sets layouts stored using `store_declarative_data_sources`.
+
+        This method combines `load_declarative_data_sources` and `put_declarative_data_sources`
+        methods to load and set layouts stored using `store_declarative_data_sources`.
 
         Args:
             layout_root_path (Optional[Path], optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
             credentials_path (Optional[Path], optional):
                 Path to the credentials. Defaults to Path.cwd().
             test_data_sources (bool, optional):
@@ -269,14 +275,15 @@
             None
         """
         declarative_pdm = DeclarativePdm(pdm=declarative_tables.to_api())
         self._layout_api.set_pdm_layout(data_source_id, declarative_pdm)
 
     def store_declarative_pdm(self, data_source_id: str, layout_root_path: Path = Path.cwd()) -> None:
         """Store physical data model layout in directory hierarchy for a given data source.
+
         gooddata_layouts
         └── organization_id
                 └── data_sources
                         └── data_source_a
                                 └── pdm
                                     ├── table_A.yaml
                                     └── table_B.yaml
@@ -292,51 +299,56 @@
         """
         data_source_folder = self.data_source_folder(data_source_id, layout_root_path)
         self.get_declarative_pdm(data_source_id).store_to_disk(data_source_folder)
 
     def load_declarative_pdm(
         self, data_source_id: str, layout_root_path: Path = Path.cwd()
     ) -> CatalogDeclarativeTables:
-        """Load declarative physical data model layout,
-        which was stored using store_declarative_pdm for a given data source.
+        """Load declarative physical data model layout.
+
+        Load declarative physical data model layout, which was stored using
+        `store_declarative_pdm` for a given data source.
 
         Args:
             data_source_id (str):
                 Data Source identification string. e.g. "demo"
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
         Returns:
             CatalogDeclarativeTables: Physical Data Model object.
         """
         data_source_folder = self.data_source_folder(data_source_id, layout_root_path)
         return CatalogDeclarativeTables.load_from_disk(data_source_folder)
 
     def load_and_put_declarative_pdm(self, data_source_id: str, layout_root_path: Path = Path.cwd()) -> None:
-        """This method combines load_declarative_pdm and put_declarative_pdm methods
-            to load and set layouts stored using store_declarative_pdm.
+        """Loads and sets layouts stored using `store_declarative_pdm`.
+
+        This method combines load_declarative_pdm and `put_declarative_pdm` methods
+        to load and set layouts stored using `store_declarative_pdm`.
 
         Args:
             data_source_id (str):
                 Data Source identification string. e.g. "demo"
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
         Returns:
             None
         """
         self.put_declarative_pdm(data_source_id, self.load_declarative_pdm(data_source_id, layout_root_path))
 
     def store_pdm_to_disk(self, datasource_id: str, path: Path = Path.cwd()) -> None:
         """Store the physical data model layout in the directory for a given data source.
-            The directory structure below shows the output for the path set to Path("pdm_location").
-            pdm_location
-                └── pdm
-                    ├── table_A.yaml
-                    └── table_B.yaml
+
+        The directory structure below shows the output for the path set to Path("pdm_location").
+        pdm_location
+            └── pdm
+                ├── table_A.yaml
+                └── table_B.yaml
 
         Args:
             datasource_id (str):
                 Data Source identification string. e.g. "demo"
             path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
@@ -397,14 +409,15 @@
     def scan_data_source(
         self,
         data_source_id: str,
         scan_request: CatalogScanModelRequest = CatalogScanModelRequest(),
         report_warnings: bool = False,
     ) -> CatalogScanResultPdm:
         """Scan data source specified by its id and optionally by specified scan request.
+
         CatalogScanResultPdm contains PDM and warnings. Warnings contain information about
         columns which were not added to the PDM because their data types are not supported.
         Additional parameter report_warnings can be passed to suppress or to report warnings.
         By default warnings are returned but not reported to STDOUT. If you set report_warnings
         to True, warnings are reported to STDOUT.
 
         Args:
@@ -440,16 +453,17 @@
 
         Returns:
             None
         """
         self.put_declarative_pdm(data_source_id, self.scan_data_source(data_source_id, scan_request).pdm)
 
     def scan_schemata(self, data_source_id: str) -> list[str]:
-        """Returns a list of schemas that exist in the database
-        and can be configured in the data source entity. Data source
+        """Returns a list of schemas that exist in the database.
+
+        Can be configured in the data source entity. Data source
         managers like Dremio or Drill can work with multiple schemas
         and schema names can be injected into scan_request to filter
         out tables stored in the different schemas.
 
         Args:
             data_source_id (str):
                 Data Source identification string. e.g. "demo"
@@ -457,23 +471,42 @@
         Returns:
             list[str]:
                 List of schema names for the given data source specified by its id.
         """
         response = self._actions_api.get_data_source_schemata(data_source_id)
         return response.get("schema_names", [])
 
+    def scan_sql(self, data_source_id: str, sql_request: ScanSqlRequest) -> ScanSqlResponse:
+        """Analyze SELECT SQL query in a given request.
+
+        Return description of SQL result-set as list of column names with GoodData data types
+        and list of example data returned by SELECT query.
+
+        Args:
+            data_source_id (str):
+                Data Source identification string. e.g. "demo"
+            sql_request (ScanSqlRequest):
+                SELECT SQL query to analyze
+
+        Returns:
+            ScanSqlResponse:
+                SELECT query analysis result
+        """
+        return ScanSqlResponse.from_api(self._actions_api.scan_sql(data_source_id, sql_request.to_api()))
+
     def test_data_sources_connection(
         self, declarative_data_sources: CatalogDeclarativeDataSources, credentials_path: Optional[Path] = None
     ) -> None:
         """Tests connection to declarative data sources.
-        If credentials_path is omitted then the connection
+
+        If `credentials_path` is omitted then the connection
         is tested with empty credentials. In case some connection
-        failed the ValueError is raised with information about why
+        failed the `ValueError` is raised with information about why
         the connection to the data source failed, e.g. host
-        unreachable or invalid login or password”.
+        unreachable or invalid login or password.
 
         Args:
             declarative_data_sources (CatalogDeclarativeDataSources):
                 Declarative Data Sources object
             credentials_path (Optional[Path], optional):
                 Path to the credentials. Defaults to None.
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/data_source/validation/data_source.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/data_source/validation/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/entity.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/entity.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/identifier.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/identifier.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/entity_model/organization.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/entity_model/organization.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/organization/service.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/organization/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/declarative_model/permission.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/declarative_model/permission.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/permission/service.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/permission/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/setting.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/user.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/declarative_model/user_group.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/declarative_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/entity_model/user_group.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/entity_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/user/service.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/user/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,16 +203,18 @@
         Returns:
             CatalogDeclarativeUsers:
                 Declarative Users object, incuding authetication properties.
         """
         return CatalogDeclarativeUsers.load_from_disk(self.layout_organization_folder(layout_root_path))
 
     def load_and_put_declarative_users(self, layout_root_path: Path = Path.cwd()) -> None:
-        """This method combines load_declarative_users and put_declarative_users
-            methods to load and set layouts stored using store_declarative_users.
+        """Loads and sets the layouts stored using `store_declarative_users`.
+
+        This method combines `load_declarative_users` and `put_declarative_users`
+        methods to load and set layouts stored using `store_declarative_users`.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory.. Defaults to Path.cwd().
 
         Returns:
             None
@@ -245,15 +247,15 @@
 
         Returns:
             None
         """
         self._layout_api.put_user_groups_layout(user_groups.to_api())
 
     def load_declarative_user_groups(self, layout_root_path: Path = Path.cwd()) -> CatalogDeclarativeUserGroups:
-        """Load declarative users groups layout, which was stored using store_declarative_user_groups.
+        """Load declarative users groups layout, which was stored using `store_declarative_user_groups`.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory.. Defaults to Path.cwd().
 
         Returns:
             CatalogDeclarativeUserGroups:
@@ -271,16 +273,18 @@
 
         Returns:
             None
         """
         self.get_declarative_user_groups().store_to_disk(self.layout_organization_folder(layout_root_path))
 
     def load_and_put_declarative_user_groups(self, layout_root_path: Path = Path.cwd()) -> None:
-        """This method combines load_declarative_users and put_declarative_users
-            methods to load and set layouts stored using store_declarative_users.
+        """Loads and sets the layouts stored using `store_declarative_users`.
+
+        This method combines load_declarative_users and put_declarative_users
+        methods to load and set layouts stored using store_declarative_users.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory.. Defaults to Path.cwd().
 
 
         Returns:
@@ -315,15 +319,15 @@
             None
         """
         self._layout_api.put_users_user_groups_layout(declarative_users_user_groups=users_user_groups.to_api())
 
     def load_declarative_users_user_groups(
         self, layout_root_path: Path = Path.cwd()
     ) -> CatalogDeclarativeUsersUserGroups:
-        """Load declarative users and user groups layout, which was stored using store_declarative_users_user_groups.
+        """Load declarative users and user groups layout, which was stored using `store_declarative_users_user_groups`.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory.. Defaults to Path.cwd().
 
         Returns:
             CatalogDeclarativeUsersUserGroups:
@@ -344,16 +348,18 @@
 
         Returns:
             None
         """
         self.get_declarative_users_user_groups().store_to_disk(self.layout_organization_folder(layout_root_path))
 
     def load_and_put_declarative_users_user_groups(self, layout_root_path: Path = Path.cwd()) -> None:
-        """This method combines load_declarative_users and put_declarative_users_user_groups
-            methods to load and set layouts stored using store_declarative_users_user_groups.
+        """Loads and sets the layouts stored using `store_declarative_users_user_groups`.
+
+        This method combines `load_declarative_users` and `put_declarative_users_user_groups`
+        methods to load and set layouts stored using `store_declarative_users_user_groups`.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory.. Defaults to Path.cwd().
 
 
         Returns:
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/content_service.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/content_service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List, Optional, Type
 
 import attr
 
 from gooddata_api_client.model.data_source_table_identifier import DataSourceTableIdentifier
 from gooddata_api_client.model.declarative_attribute import DeclarativeAttribute
 from gooddata_api_client.model.declarative_dataset import DeclarativeDataset
+from gooddata_api_client.model.declarative_dataset_sql import DeclarativeDatasetSql
 from gooddata_api_client.model.declarative_fact import DeclarativeFact
 from gooddata_api_client.model.declarative_label import DeclarativeLabel
 from gooddata_api_client.model.declarative_reference import DeclarativeReference
 from gooddata_sdk.catalog.base import Base
 from gooddata_sdk.catalog.identifier import CatalogGrainIdentifier, CatalogLabelIdentifier, CatalogReferenceIdentifier
 from gooddata_sdk.utils import read_layout_from_file, write_layout_to_file
 
@@ -25,15 +26,17 @@
     title: str
     grain: List[CatalogGrainIdentifier]
     references: List[CatalogDeclarativeReference]
     description: Optional[str] = None
     attributes: Optional[List[CatalogDeclarativeAttribute]] = None
     facts: Optional[List[CatalogDeclarativeFact]] = None
     data_source_table_id: Optional[CatalogDataSourceTableIdentifier] = None
+    sql: Optional[CatalogDeclarativeDatasetSql] = None
     tags: Optional[List[str]] = None
+    workspace_data_filter_columns: Optional[List[str]] = None
 
     @staticmethod
     def client_class() -> Type[DeclarativeDataset]:
         return DeclarativeDataset
 
     def store_to_disk(self, datasets_folder: Path) -> None:
         dataset_file = datasets_folder / f"{self.id}.yaml"
@@ -47,14 +50,15 @@
 
 @attr.s(auto_attribs=True, kw_only=True)
 class CatalogDeclarativeAttribute(Base):
     id: str
     title: str
     source_column: str
     labels: List[CatalogDeclarativeLabel]
+    source_column_data_type: Optional[str] = None
     default_view: Optional[CatalogLabelIdentifier] = None
     sort_column: Optional[str] = None
     sort_direction: Optional[str] = None
     description: Optional[str] = None
     tags: Optional[List[str]] = None
 
     @staticmethod
@@ -63,14 +67,15 @@
 
 
 @attr.s(auto_attribs=True, kw_only=True)
 class CatalogDeclarativeFact(Base):
     id: str
     title: str
     source_column: str
+    source_column_data_type: Optional[str] = None
     description: Optional[str] = None
     tags: Optional[List[str]] = None
 
     @staticmethod
     def client_class() -> Type[DeclarativeFact]:
         return DeclarativeFact
 
@@ -82,29 +87,41 @@
 
     @staticmethod
     def client_class() -> Type[DataSourceTableIdentifier]:
         return DataSourceTableIdentifier
 
 
 @attr.s(auto_attribs=True, kw_only=True)
+class CatalogDeclarativeDatasetSql(Base):
+    statement: str
+    data_source_id: str
+
+    @staticmethod
+    def client_class() -> Type[DeclarativeDatasetSql]:
+        return DeclarativeDatasetSql
+
+
+@attr.s(auto_attribs=True, kw_only=True)
 class CatalogDeclarativeLabel(Base):
     id: str
     title: str
     source_column: str
+    source_column_data_type: Optional[str] = None
     description: Optional[str] = None
     tags: Optional[List[str]] = None
     value_type: Optional[str] = None
 
     @staticmethod
     def client_class() -> Type[DeclarativeLabel]:
         return DeclarativeLabel
 
 
 @attr.s(auto_attribs=True, kw_only=True)
 class CatalogDeclarativeReference(Base):
     identifier: CatalogReferenceIdentifier
     multivalue: bool
     source_columns: List[str]
+    source_column_data_types: Optional[List[str]] = None
 
     @staticmethod
     def client_class() -> Type[DeclarativeReference]:
         return DeclarativeReference
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/entity_model/workspace.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/entity_model/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/model_container.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/model_container.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/catalog/workspace/service.py` & `gooddata-sdk-1.3.0/gooddata_sdk/catalog/workspace/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,28 +153,30 @@
 
         Returns:
             None
         """
         self.get_declarative_workspaces().store_to_disk(self.layout_organization_folder(layout_root_path))
 
     def load_declarative_workspaces(self, layout_root_path: Path = Path.cwd()) -> CatalogDeclarativeWorkspaces:
-        """Load declarative workspaces layout, which was stored using store_declarative_workspaces
+        """Load declarative workspaces layout, which was stored using `store_declarative_workspaces`
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
         Returns:
             CatalogDeclarativeWorkspaces:
                 Declarative Workspaces Object
         """
         return CatalogDeclarativeWorkspaces.load_from_disk(self.layout_organization_folder(layout_root_path))
 
     def load_and_put_declarative_workspaces(self, layout_root_path: Path = Path.cwd()) -> None:
-        """This method combines load_declarative_workspaces and put_declarative_workspaces
-        methods to load and set layouts stored using store_declarative_workspaces.
+        """Loads and sets the layouts stored using `store_declarative_workspaces`.
+
+        This method combines `load_declarative_workspaces` and `put_declarative_workspaces`
+        methods to load and set layouts stored using `store_declarative_workspaces`.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
         Returns:
             None
@@ -224,15 +226,15 @@
             workspace_id=workspace_id, layout_organization_folder=self.layout_organization_folder(layout_root_path)
         )
         self.get_declarative_workspace(workspace_id=workspace_id).store_to_disk(workspace_folder=workspace_folder)
 
     def load_declarative_workspace(
         self, workspace_id: str, layout_root_path: Path = Path.cwd()
     ) -> CatalogDeclarativeWorkspaceModel:
-        """Load declarative workspaces layout, which was stored using store_declarative_workspace.
+        """Load declarative workspaces layout, which was stored using `store_declarative_workspace`.
 
         Args:
             workspace_id (str):
                 Workspace identification string e.g. "demo"
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
@@ -242,16 +244,18 @@
         """
         workspace_folder = get_workspace_folder(
             workspace_id=workspace_id, layout_organization_folder=self.layout_organization_folder(layout_root_path)
         )
         return CatalogDeclarativeWorkspaceModel.load_from_disk(workspace_folder=workspace_folder)
 
     def load_and_put_declarative_workspace(self, workspace_id: str, layout_root_path: Path = Path.cwd()) -> None:
-        """This method combines load_declarative_workspace and put_declarative_workspace methods
-        to load and set layouts stored using store_declarative_workspace.
+        """Loads and sets the layouts stored using `store_declarative_workspace`.
+
+        This method combines `load_declarative_workspace` and `put_declarative_workspace` methods
+        to load and set layouts stored using `store_declarative_workspace`.
 
         Args:
             workspace_id (str):
                 Workspace identification string e.g. "demo"
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
@@ -269,14 +273,15 @@
         target_workspace_id: Optional[str] = None,
         target_workspace_name: Optional[str] = None,
         overwrite_existing: Optional[bool] = None,
         data_source_mapping: Optional[dict] = None,
         upper_case: Optional[bool] = True,
     ) -> None:
         """Clone workspace from existing workspace.
+
         Clones complete workspace content - LDM, ADM, permissions.
 
         If the target workspace already exists, it's content is overwritten.
         This can be useful when testing changes in the clone
           - once you are satisfied, you can clone it back to the origin workspace.
         For the safety, you have to enforce this behavior by the dedicated input argument `overwrite_existing`.
 
@@ -355,15 +360,15 @@
                 Object containing List of declarative workspace data filters.
         """
         return CatalogDeclarativeWorkspaceDataFilters.from_api(self._layout_api.get_workspace_data_filters_layout())
 
     def put_declarative_workspace_data_filters(
         self, workspace_data_filters: CatalogDeclarativeWorkspaceDataFilters
     ) -> None:
-        """Set workspace data filers layout.
+        """Set workspace data filters layout.
 
         Args:
             workspace_data_filters (CatalogDeclarativeWorkspaceDataFilters):
                 Object containing List of declarative workspace data filters.
 
         Returns:
             None
@@ -383,29 +388,31 @@
             None
         """
         self.get_declarative_workspace_data_filters().store_to_disk(self.layout_organization_folder(layout_root_path))
 
     def load_declarative_workspace_data_filters(
         self, layout_root_path: Path = Path.cwd()
     ) -> CatalogDeclarativeWorkspaceDataFilters:
-        """Loads workspace data filters layout, which was stored using store_declarative_workspace_data_filters.
+        """Loads workspace data filters layout, which was stored using `store_declarative_workspace_data_filters`.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
         Returns:
             CatalogDeclarativeWorkspaceDataFilters:
                 Object containing List of declarative workspace data filters.
         """
         return CatalogDeclarativeWorkspaceDataFilters.load_from_disk(self.layout_organization_folder(layout_root_path))
 
     def load_and_put_declarative_workspace_data_filters(self, layout_root_path: Path = Path.cwd()) -> None:
-        """This method combines load_declarative_workspace_data_filters and put_declarative_workspace_data_filters
-        methods to load and set layouts stored using store_declarative_workspace_data_filters.
+        """Loads and sets the layouts stored using `store_declarative_workspace_data_filters`.
+
+        This method combines `load_declarative_workspace_data_filters` and `put_declarative_workspace_data_filters`
+        methods to load and set layouts stored using `store_declarative_workspace_data_filters`.
 
         Args:
             layout_root_path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
         Returns:
             None
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/client.py` & `gooddata-sdk-1.3.0/gooddata_sdk/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,24 +34,27 @@
 
         `extra_user_agent` is optional string to be added to default http User-Agent
         header. This takes precedence over custom_headers setting.
         """
         self._hostname = host
         self._token = token
         self._custom_headers = custom_headers or {}
+        self._default_headers = {"Accept-Encoding": "br, gzip, deflate"}
 
         user_agent = f"{USER_AGENT} {extra_user_agent}" if extra_user_agent is not None else USER_AGENT
 
         self._api_config = api_client.Configuration(host=host)
         self._api_client = api_client.ApiClient(
             configuration=self._api_config,
             header_name="Authorization",
             header_value=f"Bearer {token}",
         )
         self._set_default_headers(self._api_client.default_headers)
+        for header_name, header_value in self._default_headers.items():
+            self._api_client.default_headers[header_name] = header_value
         for header_name, header_value in self._custom_headers.items():
             self._api_client.default_headers[header_name] = header_value
         self._api_client.user_agent = user_agent
 
         self._entities_api = apis.EntitiesApi(self._api_client)
         self._layout_api = apis.LayoutApi(self._api_client)
         self._actions_api = apis.ActionsApi(self._api_client)
@@ -60,36 +63,42 @@
         self._metadata_config = metadata_client.Configuration(host=host)
         self._metadata_client = metadata_client.ApiClient(
             configuration=self._metadata_config,
             header_name="Authorization",
             header_value=f"Bearer {token}",
         )
         self._set_default_headers(self._metadata_client.default_headers)
+        for header_name, header_value in self._default_headers.items():
+            self._metadata_client.default_headers[header_name] = header_value
         for header_name, header_value in self._custom_headers.items():
             self._metadata_client.default_headers[header_name] = header_value
         self._metadata_client.user_agent = user_agent
 
         self._scan_config = scan_client.Configuration(host=host)
         self._scan_client = scan_client.ApiClient(
             configuration=self._scan_config,
             header_name="Authorization",
             header_value=f"Bearer {token}",
         )
         self._set_default_headers(self._scan_client.default_headers)
+        for header_name, header_value in self._default_headers.items():
+            self._scan_client.default_headers[header_name] = header_value
         for header_name, header_value in self._custom_headers.items():
             self._scan_client.default_headers[header_name] = header_value
         self._scan_client.user_agent = user_agent
 
         self._afm_config = afm_client.Configuration(host=host)
         self._afm_client = afm_client.ApiClient(
             configuration=self._afm_config,
             header_name="Authorization",
             header_value=f"Bearer {token}",
         )
         self._set_default_headers(self._afm_client.default_headers)
+        for header_name, header_value in self._default_headers.items():
+            self._afm_client.default_headers[header_name] = header_value
         for header_name, header_value in self._custom_headers.items():
             self._afm_client.default_headers[header_name] = header_value
         self._afm_client.user_agent = user_agent
 
     @staticmethod
     def _set_default_headers(headers: dict) -> None:
         headers["X-Requested-With"] = "XMLHttpRequest"
@@ -98,35 +107,35 @@
     @property
     def custom_headers(self) -> dict[str, str]:
         return self._custom_headers
 
     @property
     def afm_client(self) -> afm_client.ApiClient:
         warn(
-            "This property is deprecated and it will be removed in PythonSDK 2.0. "
+            "This property is deprecated and it will be removed in the upcoming release. "
             "Please use entities_api, layout_api, actions_api properties instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._afm_client
 
     @property
     def metadata_client(self) -> metadata_client.ApiClient:
         warn(
-            "This property is deprecated and it will be removed in PythonSDK 2.0. "
+            "This property is deprecated and it will be removed in the upcoming release. "
             "Please use entities_api, layout_api, actions_api properties instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._metadata_client
 
     @property
     def scan_client(self) -> scan_client.ApiClient:
         warn(
-            "This property is deprecated and it will be removed in PythonSDK 2.0. "
+            "This property is deprecated and it will be removed in the upcoming release. "
             "Please use entities_api, layout_api, actions_api properties instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         return self._scan_client
 
     @property
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/base.py` & `gooddata-sdk-1.3.0/gooddata_sdk/compute/model/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/execution.py` & `gooddata-sdk-1.3.0/gooddata_sdk/compute/model/execution.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/filter.py` & `gooddata-sdk-1.3.0/gooddata_sdk/compute/model/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/compute/model/metric.py` & `gooddata-sdk-1.3.0/gooddata_sdk/compute/model/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/compute/service.py` & `gooddata-sdk-1.3.0/gooddata_sdk/compute/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/insight.py` & `gooddata-sdk-1.3.0/gooddata_sdk/insight.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,22 +316,26 @@
     def alias(self) -> Optional[str]:
         return self._a["alias"] if "alias" in self._a else None
 
     @property
     def label(self) -> dict[str, Any]:
         return self._a["displayForm"]
 
+    @property
+    def show_all_values(self) -> Optional[bool]:
+        return self._a.get("showAllValues")
+
     def as_computable(self) -> Attribute:
-        return Attribute(local_id=self.local_id, label=_ref_extract(self.label))
+        return Attribute(local_id=self.local_id, label=_ref_extract(self.label), show_all_values=self.show_all_values)
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
-        return f"attribute(local_id={self.local_id})"
+        return f"attribute(local_id={self.local_id}, show_all_values={self.show_all_values})"
 
 
 class InsightFilter:
     def __init__(self, f: dict[str, Any]) -> None:
         self._filter = f
 
     def as_computable(self) -> Filter:
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/sdk.py` & `gooddata-sdk-1.3.0/gooddata_sdk/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,26 @@
 
 
 class GoodDataSdk:
     """Top-level class that wraps all the functionality together."""
 
     @classmethod
     def create_from_profile(cls, profile: str = "default", profiles_path: Path = PROFILES_FILE_PATH) -> GoodDataSdk:
+        """Convenient method to initialize the SDK from config file.
+
+        Args:
+            profile (str, optional):
+                Profile Name. Defaults to "default".
+            profiles_path (Path, optional):
+                File path for the profiles. Defaults to PROFILES_FILE_PATH.
+
+        Returns:
+            GoodDataSdk:
+                Initialized SDK.
+        """
         content = profile_content(profile, profiles_path)
         client = GoodDataApiClient(**content)
         return cls(client)
 
     @classmethod
     def create(
         cls,
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/support.py` & `gooddata-sdk-1.3.0/gooddata_sdk/support.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/table.py` & `gooddata-sdk-1.3.0/gooddata_sdk/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/type_converter.py` & `gooddata-sdk-1.3.0/gooddata_sdk/type_converter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk/utils.py` & `gooddata-sdk-1.3.0/gooddata_sdk/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import functools
 import os
 import re
 import typing
 from collections.abc import KeysView
 from pathlib import Path
 from shutil import rmtree
-from typing import Any, Callable, Dict, NamedTuple, Union, cast
+from typing import Any, Callable, Dict, NamedTuple, Tuple, Union, cast
 
 import yaml
 
 from gooddata_api_client import ApiAttributeError
 from gooddata_sdk.compute.model.base import ObjId
 
 # Use typing collection types to support python < py3.9
@@ -199,25 +199,83 @@
     temp = dict()
     for k, v in dictionary.items():
         temp[case(k)] = change_case_helper(v, case)
     return temp
 
 
 def mandatory_profile_content_check(profile: str, profile_content_keys: KeysView) -> None:
+    """Check, whether the mandatory profile content is valid.
+
+    Args:
+        profile (str):
+            Profile name
+        profile_content_keys (KeysView):
+            Dictionary keys from loaded configuration file under specific profile.
+
+    Retruns:
+        None
+
+    Raises:
+        ValueError:
+            Missing mandatory parameter or parameters.
+    """
     mandatory_parameters = ["host", "token"]
     missing = []
     for mandatory_parameter in mandatory_parameters:
         if mandatory_parameter not in profile_content_keys:
             missing.append(mandatory_parameter)
     if missing:
         missing_str = " and ".join(missing)
         raise ValueError(f"Profile {profile} is missing mandatory parameter or parameters {missing_str}.")
 
 
 def profile_content(profile: str = "default", profiles_path: Path = PROFILES_FILE_PATH) -> dict[str, Any]:
+    """Get the profile content from a given file.
+
+    Args:
+        profile (str, optional):
+            Profile name. Defaults to "default".
+        profiles_path (Path, optional):
+            File path for the profiles. Defaults to PROFILES_FILE_PATH.
+
+    Raises:
+        ValueError:
+            There is no profile file located for the given path.
+        ValueError:
+            Profile file does not contain the specified profile.
+
+    Returns:
+        dict[str, Any]:
+            Profile content as a dictionary.
+    """
     if not profiles_path.exists():
         raise ValueError(f"There is no profiles file located for path {profiles_path}.")
     content = read_layout_from_file(profiles_path)
     if not content.get(profile):
         raise ValueError(f"Profiles file does not contain profile {profile}.")
     mandatory_profile_content_check(profile, content.get(profile).keys())
     return content.get(profile)
+
+
+def good_pandas_profile_content(
+    profile: str = "default", profiles_path: Path = PROFILES_FILE_PATH
+) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+    """Load the profiles for GoodPandas
+
+    This is workaround for GoodPandas. We should only use profile_content in the future.
+    For that we need to unify GoodPandas and GoodDataSdk interface.
+
+    Args:
+        profile (str, optional):
+            Profile name. Defaults to "default".
+        profiles_path (Path, optional):
+            File path for the profiles. Defaults to PROFILES_FILE_PATH.
+
+    Returns:
+        Tuple[Dict[str, Any], Dict[str, Any]]:
+            The content and custom Headers.
+    """
+    content = profile_content(profile, profiles_path)
+    custom_headers = content["custom_headers"]
+    del content["extra_user_agent"]
+    del content["custom_headers"]
+    return content, custom_headers
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/PKG-INFO` & `gooddata-sdk-1.3.0/gooddata_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.2.1a3
+Version: 1.3.0
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-sdk.readthedocs.io/en/v1.2.1a3
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,15 +34,15 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.3) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
 -  Python 3.7 or newer
 
 ## Installation
```

### Comparing `gooddata-sdk-1.2.1a3/gooddata_sdk.egg-info/SOURCES.txt` & `gooddata-sdk-1.3.0/gooddata_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,22 @@
 gooddata_sdk/catalog/entity.py
 gooddata_sdk/catalog/identifier.py
 gooddata_sdk/catalog/parameter.py
 gooddata_sdk/catalog/setting.py
 gooddata_sdk/catalog/types.py
 gooddata_sdk/catalog/data_source/__init__.py
 gooddata_sdk/catalog/data_source/service.py
-gooddata_sdk/catalog/data_source/action_requests/__init__.py
-gooddata_sdk/catalog/data_source/action_requests/ldm_request.py
-gooddata_sdk/catalog/data_source/action_requests/scan_model_request.py
+gooddata_sdk/catalog/data_source/action_model/__init__.py
+gooddata_sdk/catalog/data_source/action_model/sql_column.py
+gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
+gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
+gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
+gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
+gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
+gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
 gooddata_sdk/catalog/data_source/declarative_model/__init__.py
 gooddata_sdk/catalog/data_source/declarative_model/data_source.py
 gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
 gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
 gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
 gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
 gooddata_sdk/catalog/data_source/entity_model/__init__.py
@@ -84,8 +89,10 @@
 gooddata_sdk/compute/__init__.py
 gooddata_sdk/compute/service.py
 gooddata_sdk/compute/model/__init__.py
 gooddata_sdk/compute/model/attribute.py
 gooddata_sdk/compute/model/base.py
 gooddata_sdk/compute/model/execution.py
 gooddata_sdk/compute/model/filter.py
-gooddata_sdk/compute/model/metric.py
+gooddata_sdk/compute/model/metric.py
+tests/test_client.py
+tests/test_type_converter.py
```

### Comparing `gooddata-sdk-1.2.1a3/setup.py` & `gooddata-sdk-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,42 +3,43 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-afm-client~=1.2.1a3",
-    "gooddata-metadata-client~=1.2.1a3",
-    "gooddata-scan-client~=1.2.1a3",
-    "gooddata-api-client~=1.2.1a3",
+    "gooddata-afm-client~=1.3.0",
+    "gooddata-metadata-client~=1.3.0",
+    "gooddata-scan-client~=1.3.0",
+    "gooddata-api-client~=1.3.0",
     'importlib-metadata >= 1.0 ; python_version >= "3.7"',
     "python-dateutil>=2.5.3",
     "pyyaml>=5.1",
     "attrs==21.4.0",
     "cattrs==22.1.0",
+    "brotli==1.0.9",
 ]
 
 
 setup(
     name="gooddata-sdk",
     description="GoodData.CN Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.2.1a3",
+    version="1.3.0",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.7.0",
     project_urls={
-        "Documentation": "https://gooddata-sdk.readthedocs.io/en/v1.2.1a3",
+        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.3",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

