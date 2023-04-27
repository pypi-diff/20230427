# Comparing `tmp/types-influxdb-client-1.36.0.7.tar.gz` & `tmp/types-influxdb-client-1.36.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-influxdb-client-1.36.0.7.tar", last modified: Mon Mar 27 18:25:13 2023, max compression
+gzip compressed data, was "types-influxdb-client-1.36.0.8.tar", last modified: Thu Apr 27 03:16:14 2023, max compression
```

## Comparing `types-influxdb-client-1.36.0.7.tar` & `types-influxdb-client-1.36.0.8.tar`

### file list

```diff
@@ -1,426 +1,426 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.323695 types-influxdb-client-1.36.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-27 18:25:12.000000 types-influxdb-client-1.36.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:25:12.000000 types-influxdb-client-1.36.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-27 18:25:13.323695 types-influxdb-client-1.36.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.279695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-27 18:25:12.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    34856 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.279695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_async/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_async/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_async/api_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_async/rest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.279695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_sync/api_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/_sync/rest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.283695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/authorizations_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/bucket_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/delete_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/delete_api_async.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/flux_csv_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/flux_table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/influxdb_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/influxdb_client_async.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/invokable_scripts_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/labels_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/logging_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/organizations_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/query_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/query_api_async.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/tasks_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/users_api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.283695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/date_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/date_utils_pandas.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/multiprocessing_helper.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/warnings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.283695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/dataframe_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/point.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write_api_async.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/configuration.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.319695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    30203 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/add_resource_member_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/analyze_query_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/analyze_query_response_errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/array_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/ast_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorization_post_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorization_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorizations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/axes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/axis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/axis_scale.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bad_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/band_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/binary_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/block.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/boolean_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_retention_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_shard_mapping.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/buckets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_aggregate_function_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_functions_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_tags_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builtin_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/call_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/cell_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/cell_update.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/cell_with_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_base_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_discriminator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_patch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_status_level.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/column_data_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/column_semantic_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/conditional_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/constant_variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/create_cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/create_dashboard_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/custom_check.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard_color.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard_query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboards.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/date_time_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbr_ps.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbrp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbrp_create.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbrp_get.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbrp_update.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/deadman_check.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/decimal_places.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/delete_predicate_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dialect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dict_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dict_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/duration.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/duration_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/expression_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/field.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/float_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/flux_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/flux_suggestion.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/flux_suggestions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/function_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/gauge_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/greater_threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/health_check.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/heatmap_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/histogram_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/http_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/http_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/http_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/identifier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/import_declaration.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/index_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/integer_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/is_onboarding.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label_mapping.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label_update.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/labels_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/language_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/lesser_threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/line_protocol_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/line_protocol_length_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/list_stacks_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/log_event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/logical_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/logs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/map_variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/markdown_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema_column.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/member_assignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/member_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/metadata_backup.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/model_property.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/mosaic_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/node.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_update.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoints.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_base_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_discriminator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_update.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/object_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/onboarding_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/onboarding_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/option_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/organization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/organization_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/organizations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/package.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/package_clause.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/paren_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/password_reset_body.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_bucket_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_dashboard_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_organization_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_retention_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_stack_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/permission.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/permission_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pipe_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pipe_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_bucket_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_check.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_organization_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_restore_kv_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_stack_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/property_key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/query_edit_mode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/query_variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/query_variable_properties_values.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/range_threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/ready.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/regexp_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/remote_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/remote_connection_creation_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/remote_connection_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/remote_connections.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/renamable_field.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/replication.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/replication_creation_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/replication_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/replications.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_member.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_members.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_members_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_owner.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_owners.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/restored_bucket_mappings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/retention_policy_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/return_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/routes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/routes_external.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/routes_query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/routes_system.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/rule_status_level.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/run.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/run_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/run_manually.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/runs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scatter_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/schema_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scraper_target_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scraper_target_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scraper_target_responses.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script_invocation_params.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script_language.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/secret_keys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/secret_keys_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/shard_group_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/shard_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/shard_owner.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/simple_table_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/single_stat_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/slack_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/slack_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/slack_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/smtp_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/source.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/source_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/sources.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack_associations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack_events.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/statement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/static_legend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/status_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/string_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/subscription_manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/table_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/table_view_properties_table_options.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/tag_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task_status_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugin_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_request_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegrafs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegram_notification_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_apply.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_apply_remotes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_apply_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_name.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_name_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_kind.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_checks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_labels.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_variables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_label.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_label_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_variables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/test_statement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/threshold_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/threshold_check.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/unary_expression.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/unsigned_integer_literal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/user_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/user_response_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/users.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variable_assignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variable_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variable_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/view.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/view_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/write_precision.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/xy_geom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/xy_view_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/extras.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/rest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.323695 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/_base_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/authorizations_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/backup_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/bucket_schemas_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/buckets_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/cells_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/checks_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/config_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/dashboards_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/dbr_ps_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/delete_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/health_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/invokable_scripts_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/labels_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/legacy_authorizations_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/metrics_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/notification_endpoints_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/notification_rules_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/organizations_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/ping_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/query_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/ready_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/remote_connections_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/replications_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/resources_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/restore_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/routes_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/rules_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/scraper_targets_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/secrets_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/setup_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/signin_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/signout_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/sources_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/tasks_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/telegraf_plugins_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/telegrafs_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/templates_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/users_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/variables_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/views_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/write_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:21:24.000000 types-influxdb-client-1.36.0.7/influxdb_client-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:25:13.323695 types-influxdb-client-1.36.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-03-27 18:25:12.000000 types-influxdb-client-1.36.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:13.323695 types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-27 18:25:13.000000 types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-03-27 18:25:13.000000 types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:25:13.000000 types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-27 18:25:13.000000 types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 18:25:13.000000 types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.833520 types-influxdb-client-1.36.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-27 03:16:13.000000 types-influxdb-client-1.36.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 03:16:13.000000 types-influxdb-client-1.36.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-27 03:16:14.833520 types-influxdb-client-1.36.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.797520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 03:16:13.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    34856 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.797520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_async/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_async/api_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_async/rest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.797520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_sync/api_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/_sync/rest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.801520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/authorizations_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/bucket_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/delete_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/delete_api_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/flux_csv_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/flux_table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/influxdb_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/influxdb_client_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/invokable_scripts_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/labels_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/logging_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/organizations_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/query_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/query_api_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/tasks_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/users_api.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.801520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/date_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/date_utils_pandas.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/multiprocessing_helper.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/warnings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.801520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/dataframe_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/point.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write_api_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/configuration.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.829520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    30203 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/add_resource_member_request_body.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/analyze_query_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/analyze_query_response_errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/array_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/ast_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorization_post_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorization_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorizations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/axes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/axis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/axis_scale.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bad_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/band_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/binary_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/block.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/boolean_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_retention_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_shard_mapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/buckets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_aggregate_function_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_functions_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_tags_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builtin_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/call_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/cell_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/cell_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/cell_with_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_base_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_discriminator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_patch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_status_level.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/column_data_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/column_semantic_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/conditional_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/constant_variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/create_cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/create_dashboard_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/custom_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard_color.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboards.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/date_time_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbr_ps.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbrp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbrp_create.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbrp_get.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbrp_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/deadman_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/decimal_places.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/delete_predicate_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dialect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dict_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dict_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/duration.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/duration_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/expression_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/field.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/float_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/flux_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/flux_suggestion.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/flux_suggestions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/function_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/gauge_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/greater_threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/health_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/heatmap_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/histogram_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/http_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/http_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/http_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/identifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/import_declaration.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/index_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/integer_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/is_onboarding.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label_mapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/labels_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/language_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/lesser_threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/line_protocol_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/line_protocol_length_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/list_stacks_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/log_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/logical_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/logs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/map_variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/markdown_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema_column.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/member_assignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/member_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/metadata_backup.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/model_property.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/mosaic_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoints.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_base_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_discriminator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/object_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/onboarding_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/onboarding_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/option_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/organization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/organization_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/organizations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/package.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/package_clause.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/paren_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/password_reset_body.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_bucket_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_dashboard_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_organization_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_retention_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_stack_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/permission.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/permission_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pipe_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pipe_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_bucket_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_organization_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_restore_kv_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_stack_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/property_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/query_edit_mode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/query_variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/query_variable_properties_values.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/range_threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/ready.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/regexp_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/remote_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/remote_connection_creation_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/remote_connection_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/remote_connections.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/renamable_field.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/replication.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/replication_creation_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/replication_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/replications.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_member.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_members.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_members_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_owner.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_owners.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/restored_bucket_mappings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/retention_policy_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/return_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/routes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/routes_external.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/routes_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/routes_system.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/rule_status_level.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/run.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/run_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/run_manually.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/runs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scatter_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/schema_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scraper_target_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scraper_target_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scraper_target_responses.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script_invocation_params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script_language.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/secret_keys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/secret_keys_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/shard_group_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/shard_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/shard_owner.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/simple_table_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/single_stat_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/slack_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/slack_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/slack_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/smtp_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/source.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/source_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/sources.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack_associations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/static_legend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/status_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/string_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/subscription_manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/table_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/table_view_properties_table_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/tag_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task_create_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task_status_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task_update_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugin_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_request_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegrafs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegram_notification_rule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_apply.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_apply_remotes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_apply_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_name.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_name_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_kind.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_labels.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_variables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_label.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_label_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_variables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/test_statement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/threshold_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/threshold_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/unary_expression.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/unsigned_integer_literal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/user_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/user_response_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/users.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variable_assignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variable_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variable_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/view.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/view_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/write_precision.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/xy_geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/xy_view_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/extras.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/rest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.833520 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/_base_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/authorizations_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/backup_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/bucket_schemas_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/buckets_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/cells_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/checks_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/config_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/dashboards_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/dbr_ps_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/delete_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/health_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/invokable_scripts_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/labels_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/legacy_authorizations_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/metrics_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/notification_endpoints_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/notification_rules_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/organizations_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/ping_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/query_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/ready_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/remote_connections_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/replications_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/resources_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/restore_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/routes_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/rules_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/scraper_targets_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/secrets_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/setup_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/signin_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/signout_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/sources_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/tasks_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/telegraf_plugins_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/telegrafs_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/templates_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/users_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/variables_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/views_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/write_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 03:15:54.000000 types-influxdb-client-1.36.0.8/influxdb_client-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:16:14.833520 types-influxdb-client-1.36.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-27 03:16:13.000000 types-influxdb-client-1.36.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:16:14.833520 types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-27 03:16:14.000000 types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-04-27 03:16:14.000000 types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:16:14.000000 types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 03:16:14.000000 types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 03:16:14.000000 types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/top_level.txt
```

### Comparing `types-influxdb-client-1.36.0.7/CHANGELOG.md` & `types-influxdb-client-1.36.0.8/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.36.0.8 (2023-04-27)
+
+influxdb-client: fix stubtest (#10090)
+
 ## 1.36.0.7 (2023-03-27)
 
 Add defaults for third-party stubs I-L (#9955)
 
 ## 1.36.0.6 (2023-02-26)
 
 Improve many `__(a)exit__` annotations (#9696)
```

### Comparing `types-influxdb-client-1.36.0.7/PKG-INFO` & `types-influxdb-client-1.36.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-influxdb-client
-Version: 1.36.0.7
+Version: 1.36.0.8
 Summary: Typing stubs for influxdb-client
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/influxdb-client.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `influxdb-client`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/influxdb-client. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `2dd268d74aaebe4819f55ecb13c03e352bad13a4`.
```

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/__init__.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/_async/api_client.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/_async/api_client.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/_async/rest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/_async/rest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/_sync/api_client.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/_sync/api_client.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/_sync/rest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/_sync/rest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/__init__.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/authorizations_api.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/authorizations_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/bucket_api.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/bucket_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/flux_csv_parser.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/flux_csv_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/flux_table.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/flux_table.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/influxdb_client.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/influxdb_client.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/influxdb_client_async.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/influxdb_client_async.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/invokable_scripts_api.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/invokable_scripts_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/labels_api.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/labels_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/query_api.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/query_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/query_api_async.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/query_api_async.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/tasks_api.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/tasks_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/date_utils.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/date_utils.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/util/multiprocessing_helper.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/util/multiprocessing_helper.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/__init__.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/dataframe_serializer.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/dataframe_serializer.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/point.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/point.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write/retry.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write_api.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write_api.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/client/write_api_async.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/client/write_api_async.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/configuration.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/configuration.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/__init__.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/add_resource_member_request_body.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/add_resource_member_request_body.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/analyze_query_response_errors.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/analyze_query_response_errors.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/array_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/array_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorization.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorization.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorization_post_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorization_post_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorization_update_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorization_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/authorizations.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/authorizations.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/axis.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/axis.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bad_statement.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bad_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/band_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/band_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/binary_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/binary_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/block.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/block.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/boolean_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/boolean_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_metadata_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_retention_rules.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_retention_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/bucket_shard_mapping.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/bucket_shard_mapping.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/buckets.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/buckets.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_config.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_config.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_config_aggregate_window.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builder_tags_type.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builder_tags_type.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/builtin_statement.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/builtin_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/call_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/call_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/cell.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/cell_update.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/cell_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/cell_with_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/cell_with_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_base_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_base_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_discriminator.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_discriminator.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_patch.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_patch.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/check_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/check_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/checks.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/checks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/conditional_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/conditional_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/constant_variable_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/constant_variable_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/create_cell.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/create_cell.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/create_dashboard_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/create_dashboard_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/custom_check.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/custom_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard_color.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard_color.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard_query.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard_query.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboard_with_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dashboards.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dashboards.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/date_time_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/date_time_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbrp.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbrp.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbrp_create.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbrp_create.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dbrp_update.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dbrp_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/deadman_check.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/deadman_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/decimal_places.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/decimal_places.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/delete_predicate_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/delete_predicate_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dialect.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dialect.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dict_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dict_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/dict_item.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/dict_item.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/duration.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/duration.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/duration_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/duration_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/error.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/error.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/expression_statement.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/expression_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/field.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/field.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/file.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/file.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/float_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/float_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/flux_suggestion.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/flux_suggestion.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/function_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/function_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/gauge_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/gauge_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/greater_threshold.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/greater_threshold.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/health_check.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/health_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/heatmap_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/heatmap_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/histogram_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/histogram_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/http_notification_endpoint.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/http_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/http_notification_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/http_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/http_notification_rule_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/http_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/identifier.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/identifier.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/import_declaration.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/import_declaration.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/index_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/index_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/integer_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/integer_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label_create_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label_response.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/label_update.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/label_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/labels_response.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/labels_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/legacy_authorization_post_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/lesser_threshold.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/lesser_threshold.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/line_plus_single_stat_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/line_protocol_error.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/line_protocol_error.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/line_protocol_length_error.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/line_protocol_length_error.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/log_event.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/log_event.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/logical_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/logical_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/map_variable_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/map_variable_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/markdown_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/markdown_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema_column.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema_column.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/measurement_schema_create_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/measurement_schema_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/member_assignment.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/member_assignment.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/member_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/member_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/metadata_backup.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/metadata_backup.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/model_property.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/model_property.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/mosaic_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/mosaic_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_base_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_discriminator.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoint_update.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoint_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_endpoints.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_base_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_base_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_discriminator.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_discriminator.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rule_update.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rule_update.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/notification_rules.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/notification_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/object_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/object_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/onboarding_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/onboarding_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/onboarding_response.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/onboarding_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/option_statement.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/option_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/organization.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/organization.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/organization_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/organization_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/organizations.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/organizations.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/package.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/package.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/package_clause.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/package_clause.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pager_duty_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pager_duty_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pager_duty_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/paren_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/paren_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_bucket_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_bucket_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_dashboard_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_dashboard_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_organization_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_organization_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_retention_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_retention_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_stack_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_stack_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/patch_stack_request_additional_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/permission.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/permission.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/permission_resource.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/permission_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/pipe_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/pipe_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_bucket_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_bucket_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_notification_endpoint.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_notification_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_organization_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_organization_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/post_stack_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/post_stack_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/query.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/query.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/query_variable_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/query_variable_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/query_variable_properties_values.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/query_variable_properties_values.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/range_threshold.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/range_threshold.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/ready.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/ready.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/regexp_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/regexp_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/remote_connection.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/remote_connection.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/remote_connection_creation_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/remote_connection_creation_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/remote_connection_update_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/remote_connection_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/renamable_field.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/renamable_field.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/replication.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/replication.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/replication_creation_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/replication_creation_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/replication_update_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/replication_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_member.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_member.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_members.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_members.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_owner.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_owner.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/resource_owners.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/resource_owners.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/restored_bucket_mappings.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/restored_bucket_mappings.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/retention_policy_manifest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/retention_policy_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/return_statement.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/return_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/routes.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/routes.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/routes_query.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/routes_query.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/routes_system.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/routes_system.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/run.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/run.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/run_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/run_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/runs.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/runs.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scatter_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scatter_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scraper_target_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scraper_target_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/scraper_target_response.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/scraper_target_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script_create_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/script_update_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/script_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/secret_keys_response.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/secret_keys_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/shard_group_manifest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/shard_group_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/shard_manifest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/shard_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/simple_table_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/simple_table_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/single_stat_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/single_stat_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/slack_notification_endpoint.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/slack_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/slack_notification_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/slack_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/slack_notification_rule_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/slack_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/smtp_notification_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/smtp_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/smtp_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/source.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/source.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/source_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/source_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/sources.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/sources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack_associations.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack_associations.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack_events.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack_events.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/stack_resources.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/stack_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/static_legend.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/static_legend.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/status_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/status_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/string_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/string_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/subscription_manifest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/subscription_manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/table_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/table_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/table_view_properties_table_options.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/table_view_properties_table_options.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/tag_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/tag_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task_create_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task_create_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/task_update_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/task_update_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/tasks.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/tasks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugin.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugin_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugin_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugin_request_plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_plugins.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegraf_request.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegraf_request.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegram_notification_endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegram_notification_rule.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegram_notification_rule.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/telegram_notification_rule_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_apply.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_apply.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_apply_remotes.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_apply_remotes.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_apply_template.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_apply_template.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_chart.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id_org_ids.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id_resource_filters.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_id_resources.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_id_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_name.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_name.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_export_by_name_resources.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_export_by_name_resources.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_kind.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_kind.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_buckets.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_buckets_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_checks.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_checks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_dashboards.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_dashboards_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_label_mappings.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_labels.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_labels.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_labels_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_notification_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_notification_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_notification_rules_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_tasks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_tasks_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_telegraf_configs.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_variables.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_variables.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_diff_variables_new_old.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_errors.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_errors.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_label.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_label.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_label_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_label_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_buckets.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_dashboards.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_label_mappings.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_notification_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_status_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_tag_rules.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_tasks.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/template_summary_summary_variables.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/template_summary_summary_variables.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/test_statement.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/test_statement.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/threshold_base.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/threshold_base.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/threshold_check.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/threshold_check.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/unary_expression.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/unary_expression.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/unsigned_integer_literal.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/unsigned_integer_literal.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/user.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/user.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/user_response.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/user_response.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/users.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/users.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variable.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variable.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variable_assignment.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variable_assignment.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/variable_links.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/variable_links.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/view.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/view.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/views.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/views.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/write_precision.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/write_precision.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/domain/xy_view_properties.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/domain/xy_view_properties.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/rest.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/rest.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/__init__.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/authorizations_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/authorizations_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/backup_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/backup_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/bucket_schemas_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/bucket_schemas_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/buckets_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/buckets_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/cells_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/cells_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/checks_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/checks_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/dashboards_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/dashboards_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/dbr_ps_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/dbr_ps_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/invokable_scripts_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/invokable_scripts_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/labels_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/labels_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/legacy_authorizations_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/legacy_authorizations_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/notification_endpoints_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/notification_endpoints_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/notification_rules_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/notification_rules_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/organizations_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/organizations_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/query_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/query_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/remote_connections_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/remote_connections_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/replications_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/replications_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/restore_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/restore_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/scraper_targets_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/scraper_targets_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/secrets_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/secrets_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/setup_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/setup_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/sources_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/sources_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/tasks_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/tasks_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/telegrafs_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/telegrafs_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/templates_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/templates_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/users_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/users_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/variables_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/variables_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/influxdb_client-stubs/service/views_service.pyi` & `types-influxdb-client-1.36.0.8/influxdb_client-stubs/service/views_service.pyi`

 * *Files identical despite different names*

### Comparing `types-influxdb-client-1.36.0.7/setup.py` & `types-influxdb-client-1.36.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `influxdb-client`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/influxdb-client. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `2dd268d74aaebe4819f55ecb13c03e352bad13a4`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.36.0.7",
+      version="1.36.0.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/influxdb-client.md",
```

### Comparing `types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/PKG-INFO` & `types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-influxdb-client
-Version: 1.36.0.7
+Version: 1.36.0.8
 Summary: Typing stubs for influxdb-client
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/influxdb-client.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `influxdb-client`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/influxdb-client. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `2dd268d74aaebe4819f55ecb13c03e352bad13a4`.
```

### Comparing `types-influxdb-client-1.36.0.7/types_influxdb_client.egg-info/SOURCES.txt` & `types-influxdb-client-1.36.0.8/types_influxdb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

