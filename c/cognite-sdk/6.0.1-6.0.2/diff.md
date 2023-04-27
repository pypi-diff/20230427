# Comparing `tmp/cognite_sdk-6.0.1.tar.gz` & `tmp/cognite_sdk-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.0.1.tar", max compression
+gzip compressed data, was "cognite_sdk-6.0.2.tar", max compression
```

## Comparing `cognite_sdk-6.0.1.tar` & `cognite_sdk-6.0.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11349 2023-04-20 06:39:23.077254 cognite_sdk-6.0.1/LICENSE
--rw-r--r--   0        0        0     3945 2023-04-20 06:39:23.077254 cognite_sdk-6.0.1/README.md
--rw-r--r--   0        0        0      503 2023-04-20 06:39:23.077254 cognite_sdk-6.0.1/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 06:39:23.077254 cognite_sdk-6.0.1/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-04-20 06:39:23.077254 cognite_sdk-6.0.1/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54659 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    86986 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17436 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44656 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49923 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24600 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37993 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21069 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     2111 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-04-20 06:39:23.081255 cognite_sdk-6.0.1/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/config.py
--rw-r--r--   0        0        0    16247 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/credentials.py
--rw-r--r--   0        0        0     8878 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34145 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33929 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14287 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12271 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17669 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    22621 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    13108 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-04-20 06:39:23.085255 cognite_sdk-6.0.1/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/testing.py
--rw-r--r--   0        0        0      533 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9511 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    21942 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3313 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     1971 2023-04-20 06:39:23.089254 cognite_sdk-6.0.1/pyproject.toml
--rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 cognite_sdk-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/LICENSE
+-rw-r--r--   0        0        0     3945 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/README.md
+-rw-r--r--   0        0        0      503 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    11025 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54659 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87006 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17436 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-04-27 09:04:25.766256 cognite_sdk-6.0.2/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44656 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49923 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24600 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32132 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21039 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     2111 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    36997 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5245 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/config.py
+-rw-r--r--   0        0        0    16261 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34160 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33929 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14287 2023-04-27 09:04:25.770257 cognite_sdk-6.0.2/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    22565 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    13108 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/py.typed
+-rw-r--r--   0        0        0     8194 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9511 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5919 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    22892 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2109 2023-04-27 09:04:25.774257 cognite_sdk-6.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 cognite_sdk-6.0.2/PKG-INFO
```

### Comparing `cognite_sdk-6.0.1/LICENSE` & `cognite_sdk-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/README.md` & `cognite_sdk-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/annotations.py` & `cognite_sdk-6.0.2/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/assets.py` & `cognite_sdk-6.0.2/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/data_sets.py` & `cognite_sdk-6.0.2/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.0.2/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/datapoints.py` & `cognite_sdk-6.0.2/cognite/client/_api/datapoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1013,16 +1013,16 @@
 
         Note:
             This is a convenience method. It builds on top of the methods ``retrieve_arrays`` and ``retrieve_dataframe``.
             It enables you to get correct aggregates in your local time zone with daily, weekly, monthly, quarterly, and yearly
             aggregates with automatic handling for daylight saving time (DST) transitions. If your time zone observes DST,
             and your query crosses at least one DST-boundary, granularities like "3 days" or "1 week", that used to represent
             fixed durations, no longer do so. To understand why, let's illustrate with an example: A typical time zone
-            that observes DST will skip one hour ahead during spring, leading to a day that is only 23 hours long, and oppositely
-            in the fall, turning back the clock one hour, yielding a 25-hour long day.
+            (above the equator) that observes DST will skip one hour ahead during spring, leading to a day that is only
+            23 hours long, and oppositely in the fall, turning back the clock one hour, yielding a 25-hour-long day.
 
         In short, this method works as follows:
             1. Get the time zone from start and end (must be equal).
             2. Split the time range from start to end into intervals based on DST boundaries.
             3. Create a query for each interval and pass all to the retrieve_arrays method.
             4. Stack the resulting arrays into a single column in the resulting DataFrame.
```

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/diagrams.py` & `cognite_sdk-6.0.2/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.0.2/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/events.py` & `cognite_sdk-6.0.2/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.0.2/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/files.py` & `cognite_sdk-6.0.2/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/functions.py` & `cognite_sdk-6.0.2/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/geospatial.py` & `cognite_sdk-6.0.2/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/iam.py` & `cognite_sdk-6.0.2/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/labels.py` & `cognite_sdk-6.0.2/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/raw.py` & `cognite_sdk-6.0.2/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/relationships.py` & `cognite_sdk-6.0.2/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/sequences.py` & `cognite_sdk-6.0.2/cognite/client/_api/sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import copy
 import math
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Union, cast, overload
 from typing import Sequence as SequenceType
-from typing import Tuple, Union, cast, overload
 
 from cognite.client import utils
 from cognite.client._api_client import APIClient
 from cognite.client._constants import LIST_LIMIT_DEFAULT
 from cognite.client.data_classes import (
     Sequence,
     SequenceAggregate,
```

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.0.2/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/templates.py` & `cognite_sdk-6.0.2/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/three_d.py` & `cognite_sdk-6.0.2/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/time_series.py` & `cognite_sdk-6.0.2/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.0.2/cognite/client/_api/transformations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
-from typing import Any, Awaitable, Dict, List, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union
 
 from cognite.client._api.transformations.jobs import TransformationJobsAPI
 from cognite.client._api.transformations.notifications import TransformationNotificationsAPI
 from cognite.client._api.transformations.schedules import TransformationSchedulesAPI
 from cognite.client._api.transformations.schema import TransformationSchemaAPI
 from cognite.client._api_client import APIClient
+from cognite.client._constants import LIST_LIMIT_DEFAULT
 from cognite.client.data_classes import Transformation, TransformationJob, TransformationList
 from cognite.client.data_classes.shared import TimestampRange
 from cognite.client.data_classes.transformations import (
     TagsFilter,
     TransformationFilter,
     TransformationPreviewResult,
     TransformationUpdate,
 )
 from cognite.client.data_classes.transformations.common import NonceCredentials
 from cognite.client.utils._identifier import IdentifierSequence
-from typing import TYPE_CHECKING
-from cognite.client._constants import LIST_LIMIT_DEFAULT
-
 
 if TYPE_CHECKING:
-    from cognite.client.config import ClientConfig
     from cognite.client import CogniteClient
+    from cognite.client.config import ClientConfig
 
 __all__ = [
     "TransformationSchemaAPI",
     "TransformationsAPI",
     "TransformationSchedulesAPI",
     "TransformationNotificationsAPI",
     "TransformationJobsAPI",
```

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.0.2/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.0.2/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.0.2/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.0.2/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api/vision.py` & `cognite_sdk-6.0.2/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_api_client.py` & `cognite_sdk-6.0.2/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_cognite_client.py` & `cognite_sdk-6.0.2/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_http_client.py` & `cognite_sdk-6.0.2/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.0.2/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.0.2/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.0.2/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.0.2/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/config.py` & `cognite_sdk-6.0.2/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/credentials.py` & `cognite_sdk-6.0.2/cognite/client/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         accounts = self.__app.get_accounts()
         credentials = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0]) if accounts else None
 
         # If not, we acquire a new token interactively
         if credentials is None:
             device_flow = self.__app.initiate_device_flow(scopes=self.__scopes)
             # print device code user instructions to screen
-            print(f"Device code: {device_flow['message']}")
+            print(f"Device code: {device_flow['message']}")  # noqa: T201
             credentials = self.__app.acquire_token_by_device_flow(flow=device_flow)
 
         self._verify_credentials(credentials)
         return credentials["access_token"], time.time() + credentials["expires_in"]
 
 
 class OAuthInteractive(_OAuthCredentialProviderWithTokenRefresh, _WithMsalSerializableTokenCache):
```

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,30 @@
     ContextualizationJobList,
     ContextualizationJobType,
     EntityMatchingModel,
     EntityMatchingModelList,
     EntityMatchingModelUpdate,
     JobStatus,
 )
+from cognite.client.data_classes.data_sets import (
+    DataSet,
+    DataSetAggregate,
+    DataSetFilter,
+    DataSetList,
+    DataSetUpdate,
+)
+from cognite.client.data_classes.datapoints import (
+    Datapoint,
+    Datapoints,
+    DatapointsArray,
+    DatapointsArrayList,
+    DatapointsList,
+    LatestDatapointQuery,
+)
+from cognite.client.data_classes.events import EndTimeFilter, Event, EventFilter, EventList, EventUpdate
 from cognite.client.data_classes.extractionpipelines import (
     ExtractionPipeline,
     ExtractionPipelineConfig,
     ExtractionPipelineConfigRevision,
     ExtractionPipelineConfigRevisionList,
     ExtractionPipelineContact,
     ExtractionPipelineList,
@@ -37,14 +53,40 @@
 from cognite.client.data_classes.files import (
     FileAggregate,
     FileMetadata,
     FileMetadataFilter,
     FileMetadataList,
     FileMetadataUpdate,
 )
+from cognite.client.data_classes.functions import (
+    Function,
+    FunctionCall,
+    FunctionCallList,
+    FunctionCallLog,
+    FunctionCallLogEntry,
+    FunctionFilter,
+    FunctionList,
+    FunctionSchedule,
+    FunctionSchedulesFilter,
+    FunctionSchedulesList,
+    FunctionsLimits,
+)
+from cognite.client.data_classes.geospatial import (
+    CoordinateReferenceSystem,
+    CoordinateReferenceSystemList,
+    Feature,
+    FeatureAggregate,
+    FeatureAggregateList,
+    FeatureList,
+    FeatureType,
+    FeatureTypeList,
+    FeatureTypePatch,
+    FeatureTypeUpdate,
+    FeatureTypeUpdateList,
+)
 from cognite.client.data_classes.iam import (
     ClientCredentials,
     CreatedSession,
     Group,
     GroupList,
     SecurityCategory,
     SecurityCategoryList,
@@ -54,14 +96,15 @@
 from cognite.client.data_classes.labels import (
     Label,
     LabelDefinition,
     LabelDefinitionFilter,
     LabelDefinitionList,
     LabelFilter,
 )
+from cognite.client.data_classes.raw import Database, DatabaseList, Row, RowList, Table, TableList
 from cognite.client.data_classes.relationships import (
     Relationship,
     RelationshipFilter,
     RelationshipList,
     RelationshipUpdate,
 )
 from cognite.client.data_classes.sequences import (
@@ -70,14 +113,23 @@
     SequenceColumnUpdate,
     SequenceData,
     SequenceDataList,
     SequenceFilter,
     SequenceList,
     SequenceUpdate,
 )
+from cognite.client.data_classes.shared import (
+    AggregateResult,
+    AggregateUniqueValuesResult,
+    GeoLocation,
+    GeoLocationFilter,
+    Geometry,
+    GeometryFilter,
+    TimestampRange,
+)
 from cognite.client.data_classes.templates import (
     ConstantResolver,
     Source,
     TemplateGroup,
     TemplateGroupList,
     TemplateGroupVersion,
     TemplateGroupVersionList,
@@ -133,75 +185,19 @@
     TransformationNotificationList,
 )
 from cognite.client.data_classes.transformations.schedules import (
     TransformationSchedule,
     TransformationScheduleList,
     TransformationScheduleUpdate,
 )
-
 from cognite.client.data_classes.transformations.schema import (
     TransformationSchemaColumn,
     TransformationSchemaColumnList,
 )
 
-from cognite.client.data_classes.data_sets import (
-    DataSet,
-    DataSetAggregate,
-    DataSetFilter,
-    DataSetList,
-    DataSetUpdate,
-)
-
-from cognite.client.data_classes.shared import (
-    AggregateResult,
-    AggregateUniqueValuesResult,
-    GeoLocation,
-    GeoLocationFilter,
-    Geometry,
-    GeometryFilter,
-    TimestampRange,
-)
-
-from cognite.client.data_classes.datapoints import (
-    Datapoint,
-    Datapoints,
-    DatapointsList,
-    DatapointsArray,
-    DatapointsArrayList,
-    LatestDatapointQuery,
-)
-from cognite.client.data_classes.events import EndTimeFilter, Event, EventFilter, EventList, EventUpdate
-from cognite.client.data_classes.raw import Database, DatabaseList, Row, RowList, Table, TableList
-from cognite.client.data_classes.functions import (
-    Function,
-    FunctionFilter,
-    FunctionSchedule,
-    FunctionSchedulesFilter,
-    FunctionSchedulesList,
-    FunctionList,
-    FunctionCall,
-    FunctionCallList,
-    FunctionCallLogEntry,
-    FunctionCallLog,
-    FunctionsLimits,
-)
-from cognite.client.data_classes.geospatial import (
-    Feature,
-    FeatureList,
-    FeatureType,
-    FeatureTypeList,
-    FeatureTypePatch,
-    FeatureAggregate,
-    FeatureTypeUpdate,
-    FeatureAggregateList,
-    FeatureTypeUpdateList,
-    CoordinateReferenceSystemList,
-    CoordinateReferenceSystem,
-)
-
 __all__ = [
     "Annotation",
     "AnnotationFilter",
     "AnnotationList",
     "AnnotationUpdate",
     "AggregateResultItem",
     "Asset",
@@ -239,24 +235,20 @@
     "EventList",
     "EventUpdate",
     "FileAggregate",
     "FileMetadata",
     "FileMetadataFilter",
     "FileMetadataList",
     "FileMetadataUpdate",
-    "APIKey",
-    "APIKeyList",
     "ClientCredentials",
     "CreatedSession",
     "Group",
     "GroupList",
     "SecurityCategory",
     "SecurityCategoryList",
-    "ServiceAccount",
-    "ServiceAccountList",
     "Session",
     "SessionList",
     "Label",
     "LabelDefinition",
     "LabelDefinitionFilter",
     "LabelDefinitionList",
     "LabelFilter",
```

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/_base.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/assets.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import itertools
 import operator as op
 import textwrap
 import threading
 import warnings
 from collections import Counter, defaultdict
 from functools import lru_cache
-from graphlib import TopologicalSorter
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Collection,
     Dict,
     List,
@@ -23,14 +22,16 @@
     TextIO,
     Tuple,
     Type,
     Union,
     cast,
 )
 
+from graphlib import TopologicalSorter
+
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteLabelUpdate,
     CogniteListUpdate,
     CogniteObjectUpdate,
     CognitePrimitiveUpdate,
     CognitePropertyClassUtil,
@@ -743,15 +744,15 @@
                 has_cycles |= seen
                 return
 
     @staticmethod
     def print_to(*args: Any, output_file: Union[Path, TextIO, None]) -> None:
         out = "\n".join(s.rstrip() for s in map(str, args))
         if output_file is None:
-            print(out)
+            print(out)  # noqa: T201
         elif isinstance(output_file, Path):
             with output_file.open("a") as file:
                 print(out, file=file)
         else:
             try:
                 # There are no isinstance checks for TextIO
                 output_file.write(out + "\n")
```

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/events.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/files.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/functions.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/iam.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/labels.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/raw.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/relationships.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import copy
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union, cast
 from typing import Sequence as SequenceType
-from typing import Type, Union, cast
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteLabelUpdate,
     CognitePrimitiveUpdate,
     CogniteResource,
     CogniteResourceList,
```

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import json
 import math
-from typing import TYPE_CHECKING, Any, Dict, Generator, List
+from typing import TYPE_CHECKING, Any, Dict, Generator, List, Tuple, Union, cast
 from typing import Sequence as SequenceType
-from typing import Tuple, Union, cast
 
 from cognite.client import utils
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteLabelUpdate,
     CogniteListUpdate,
     CogniteObjectUpdate,
```

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/shared.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/templates.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,27 +10,24 @@
     CogniteResource,
     CogniteResourceList,
     CogniteUpdate,
 )
 from cognite.client.data_classes.iam import ClientCredentials
 from cognite.client.data_classes.shared import TimestampRange
 from cognite.client.data_classes.transformations.common import (
-    DataModelInstances,
     NonceCredentials,
     OidcCredentials,
-    RawTable,
-    SequenceRows,
     TransformationBlockedInfo,
     TransformationDestination,
     _load_destination_dct,
 )
 from cognite.client.data_classes.transformations.jobs import TransformationJob, TransformationJobList
 from cognite.client.data_classes.transformations.schedules import TransformationSchedule
 from cognite.client.data_classes.transformations.schema import TransformationSchemaColumnList
-from cognite.client.utils._text import convert_all_keys_to_snake_case, convert_all_keys_to_camel_case
+from cognite.client.utils._text import convert_all_keys_to_camel_case, convert_all_keys_to_snake_case
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
 
 class SessionDetails:
     """Details of a session which provid.
```

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.0.2/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/exceptions.py` & `cognite_sdk-6.0.2/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/testing.py` & `cognite_sdk-6.0.2/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.0.2/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.0.2/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_graph.py` & `cognite_sdk-6.0.2/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_identifier.py` & `cognite_sdk-6.0.2/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_logging.py` & `cognite_sdk-6.0.2/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.0.2/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.0.2/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.0.2/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_text.py` & `cognite_sdk-6.0.2/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_time.py` & `cognite_sdk-6.0.2/cognite/client/utils/_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -480,23 +480,21 @@
 def _to_fixed_utc_intervals_fixed_unit_length(
     start: datetime, end: datetime, multiplier: int, unit: str
 ) -> list[dict[str, datetime | str]]:
     pd = cast(Any, local_import("pandas"))
     utc = get_utc_zoneinfo()
 
     freq = multiplier * GRANULARITY_IN_HOURS[unit]
-    index = pandas_date_range_tz(start, end, f"{freq}H")
-    expected_freq = pd.Timedelta(hours=freq)
-    next_mask = (index - index.to_series().shift(1)) != expected_freq
-    last_mask = (index.to_series().shift(-1) - index) != expected_freq
-    index = index[last_mask | next_mask]
+    index = pandas_date_range_tz(start, end, to_pandas_freq(f"{multiplier}{unit}", start))
+    utc_offsets = pd.Series([t.utcoffset() for t in index], index=index)
+    transition_raw = index[(utc_offsets != utc_offsets.shift(-1)) | (utc_offsets != utc_offsets.shift(1))]
 
     hour, zero = pd.Timedelta(hours=1), pd.Timedelta(0)
     transitions = []
-    for start, end in zip(index[:-1], index[1:]):
+    for start, end in zip(transition_raw[:-1], transition_raw[1:]):
         if start.dst() == end.dst():
             dst_adjustment = 0
         elif start.dst() == hour and end.dst() == zero:
             # Fall, going away from summer.
             dst_adjustment = 1
         elif start.dst() == zero and end.dst() == hour:
             # Spring, going to summer.
@@ -514,18 +512,37 @@
     return transitions
 
 
 def pandas_date_range_tz(start: datetime, end: datetime, freq: str, inclusive: str = "both") -> pandas.DatetimeIndex:
     """
     Pandas date_range struggles with time zone aware datetimes.
     This function overcomes that limitation.
+
+    Assumes that start and end have the same timezone.
     """
     pd = local_import("pandas")
-    # Pandas seems to have issues with ZoneInfo object, so removing the timezone and adding it back.
-    return pd.date_range(start.replace(tzinfo=None), end.replace(tzinfo=None), freq=freq, inclusive=inclusive).tz_localize(start.tzinfo.key)  # type: ignore [union-attr]
+    # There is a bug in date_range which makes it fail to handle ambiguous timestamps when you use time zone aware
+    # datetimes. This is a workaround by passing the time zone as an argument to the function.
+    # In addition, pandas struggle with ZoneInfo objects, so we convert them to string so that pandas can use its own
+    # tzdata implementation.
+
+    # An ambiguous timestamp is for example 1916-10-01 00:00:00 Europe/Oslo, as this corresponds to two different points in time,
+    # 1916-10-01 00:00:00+02:00 and 1916-10-01 00:00:00+01:00; before and after the DST transition.
+    # (Back in 1916 they did not consider the needs of software engineers in 2023 :P).
+    # Setting ambiguous=True will make pandas ignore the ambiguity and use the DST timestamp. This is what we want;
+    # for a user requesting monthly aggregates, we don't want to miss the first hour of the month.
+    return pd.date_range(  # type: ignore [union-attr]
+        start.replace(tzinfo=None),
+        end.replace(tzinfo=None),
+        tz=str(start.tzinfo),
+        freq=freq,
+        inclusive=inclusive,
+        nonexistent="shift_forward",
+        ambiguous=True,
+    )
 
 
 def validate_timezone(start: datetime, end: datetime) -> ZoneInfo:
     ZoneInfo = import_zoneinfo()
 
     if missing := [name for name, timestamp in zip(("start", "end"), (start, end)) if not timestamp.tzinfo]:
         names = " and ".join(missing)
```

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_validation.py` & `cognite_sdk-6.0.2/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.0.1/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.0.2/cognite/client/utils/_version_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,10 +79,10 @@
     parser.add_argument("-p", "--package", required=True)
     parser.add_argument("-v", "--version", required=True)
     args = parser.parse_args()
 
     version_exists = check_if_version_exists(args.package, args.version)
 
     if version_exists:
-        print("yes")
+        print("yes")  # noqa: T201
     else:
-        print("no")
+        print("no")  # noqa: T201
```

### Comparing `cognite_sdk-6.0.1/pyproject.toml` & `cognite_sdk-6.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.0.1"
+version = "6.0.2"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
 
+[tool.ruff.pyupgrade]
+keep-runtime-typing = true
+
+[tool.ruff.per-file-ignores]
+# let scripts use print statements
+"scripts/*" = ["T201"]
+
 [tool.poetry.dependencies]
 python = "^3.8"
 
 requests = "^2"
 requests_oauthlib = "^1"
 msal = "^1"
 sortedcontainers = "^2.2"
```

### Comparing `cognite_sdk-6.0.1/PKG-INFO` & `cognite_sdk-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.0.1
+Version: 6.0.2
 Summary: Cognite Python SDK
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.0.1 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.0.2 Summary: Cognite Python
 SDK Author: Erlend Vollset Author-email: erlend.vollset@cognite.com Requires-
 Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
 functions Provides-Extra: geo Provides-Extra: numpy Provides-Extra: pandas
 Provides-Extra: pyodide Provides-Extra: sympy Requires-Dist: backports-zoneinfo
```

