# Comparing `tmp/dagster-1.3.1.tar.gz` & `tmp/dagster-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.1.tar", last modified: Thu Apr 20 20:39:23 2023, max compression
+gzip compressed data, was "dagster-1.3.2.tar", last modified: Thu Apr 27 18:31:49 2023, max compression
```

## Comparing `dagster-1.3.1.tar` & `dagster-1.3.2.tar`

### file list

```diff
@@ -1,625 +1,622 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.236790 dagster-1.3.1/
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-20 20:39:02.000000 dagster-1.3.1/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-20 20:39:02.000000 dagster-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-20 20:39:02.000000 dagster-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-20 20:39:23.236790 dagster-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-04-20 20:39:02.000000 dagster-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.152789 dagster-1.3.1/dagster/
--rw-r--r--   0 root         (0) root         (0)    25230 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.156789 dagster-1.3.1/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.156789 dagster-1.3.1/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.156789 dagster-1.3.1/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27263 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8207 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3456 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5718 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    33891 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5141 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.160790 dagster-1.3.1/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28486 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.160790 dagster-1.3.1/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14686 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18799 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    17554 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.164790 dagster-1.3.1/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    58149 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    16671 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.164790 dagster-1.3.1/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13519 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.164790 dagster-1.3.1/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.180790 dagster-1.3.1/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7997 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28864 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10380 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)    22609 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_group.py
--rw-r--r--   0 root         (0) root         (0)     3817 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36853 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    46445 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    17185 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    58973 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24065 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     2576 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    15537 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45721 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10877 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20634 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    17905 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.180790 dagster-1.3.1/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40545 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9563 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10731 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17810 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14491 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11914 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     6695 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    20547 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31183 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21562 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16178 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44593 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22927 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)    46583 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    18335 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7422 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.180790 dagster-1.3.1/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32712 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/mode.py
--rw-r--r--   0 root         (0) root         (0)    55735 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    21561 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11938 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8044 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     3307 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    20633 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19242 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)    18917 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    44192 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    34900 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/pipeline_definition.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)     9054 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/preset.py
--rw-r--r--   0 root         (0) root         (0)    30644 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.184790 dagster-1.3.1/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    23982 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    19736 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    19180 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8118 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    25522 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14975 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    37627 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    35100 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10753 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    44640 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    14153 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    74443 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15807 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6232 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.184790 dagster-1.3.1/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    65032 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.188790 dagster-1.3.1/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41958 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    25196 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14370 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.188790 dagster-1.3.1/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22487 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    16287 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    27186 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27826 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    34437 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    43261 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    20099 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/context_creation_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     6480 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execute_job_result.py
--rw-r--r--   0 root         (0) root         (0)     9184 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8734 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14650 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23056 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7095 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12568 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16478 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27380 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10255 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    38667 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    60978 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15617 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    16031 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19527 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)    25987 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/results.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10333 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2855 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15452 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14347 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.192790 dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2874 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33996 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    33186 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    69685 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    11276 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4341 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)    17332 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     5205 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/pipeline_index.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   104545 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11577 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24318 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3675 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6413 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17327 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    18194 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.196790 dagster-1.3.1/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20631 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.200790 dagster-1.3.1/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2847 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4019 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12052 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14487 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)    17447 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/snap/pipeline_snapshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.204790 dagster-1.3.1/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.204790 dagster-1.3.1/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7205 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8073 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16259 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9579 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    11527 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14277 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    77841 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7409 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18916 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)     9985 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    26262 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17376 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23190 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)    23993 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/pipeline_run.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15584 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8629 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46721 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6818 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    19749 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.216790 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3660 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    10435 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14729 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15907 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27288 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    18883 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7393 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/utility_solids.py
--rw-r--r--   0 root         (0) root         (0)     4003 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5451 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    26703 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5450 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6882 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9124 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.220790 dagster-1.3.1/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4422 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17726 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8371 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16312 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    35694 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.148790 dagster-1.3.1/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.224790 dagster-1.3.1/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11665 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38179 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18538 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    22252 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5394 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    52644 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26106 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      638 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32009 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    33924 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.228790 dagster-1.3.1/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.232790 dagster-1.3.1/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23212 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8687 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4308 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    23704 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    11139 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.232790 dagster-1.3.1/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10483 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    23902 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.236790 dagster-1.3.1/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-20 20:39:02.000000 dagster-1.3.1/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:39:23.152789 dagster-1.3.1/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24986 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1290 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 20:39:23.000000 dagster-1.3.1/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-20 20:39:23.236790 dagster-1.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6429 2023-04-20 20:39:02.000000 dagster-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.200454 dagster-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-27 18:30:33.000000 dagster-1.3.2/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:33.000000 dagster-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-27 18:30:33.000000 dagster-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-27 18:31:49.200454 dagster-1.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-04-27 18:30:33.000000 dagster-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.808453 dagster-1.3.2/dagster/
+-rw-r--r--   0 root         (0) root         (0)    25278 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.872453 dagster-1.3.2/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/snapshot_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.872453 dagster-1.3.2/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.872453 dagster-1.3.2/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27227 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8207 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5718 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30343 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5141 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19909 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.872453 dagster-1.3.2/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28486 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.876453 dagster-1.3.2/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14686 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18799 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    17554 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.876453 dagster-1.3.2/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    61210 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    16671 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.884453 dagster-1.3.2/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13519 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.884453 dagster-1.3.2/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.968454 dagster-1.3.2/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7771 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28864 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)    22695 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_group.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36853 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5686 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    47123 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    17185 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    60723 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24021 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    15537 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45721 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10877 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20634 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    17905 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.028454 dagster-1.3.2/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42322 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9563 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10731 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17810 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14444 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11914 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    20546 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39915 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31185 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21465 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16178 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44593 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6582 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22927 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)    53618 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    18335 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.028454 dagster-1.3.2/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32315 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    55735 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    21561 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    20633 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19242 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    18917 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    44192 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    46488 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     5988 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    30453 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.028454 dagster-1.3.2/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    18298 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    17823 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    15501 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    24263 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14975 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    38019 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    35004 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    44498 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14153 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    74443 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15962 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.028454 dagster-1.3.2/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    65171 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.032454 dagster-1.3.2/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39644 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    26566 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    15096 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.032454 dagster-1.3.2/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22172 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    27186 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27472 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    34422 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    42790 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18821 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/context_creation_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/execute_job_result.py
+-rw-r--r--   0 root         (0) root         (0)     9184 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.036454 dagster-1.3.2/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23056 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7299 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16478 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27413 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10211 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    38123 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    59748 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15617 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    16031 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19440 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)    25947 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/results.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.036454 dagster-1.3.2/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15407 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.036454 dagster-1.3.2/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14347 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.036454 dagster-1.3.2/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.040454 dagster-1.3.2/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33817 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32501 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    68876 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    11276 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)    17332 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/pipeline_index.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.040454 dagster-1.3.2/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   102984 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11577 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24318 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.040454 dagster-1.3.2/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17327 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.040454 dagster-1.3.2/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.044454 dagster-1.3.2/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18194 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.044454 dagster-1.3.2/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.044454 dagster-1.3.2/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20291 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.044454 dagster-1.3.2/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12052 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14472 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)    16768 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/snap/pipeline_snapshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.108454 dagster-1.3.2/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.112454 dagster-1.3.2/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.124454 dagster-1.3.2/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.124454 dagster-1.3.2/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8073 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16259 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    11544 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.124454 dagster-1.3.2/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14277 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3630 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    77841 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.124454 dagster-1.3.2/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.124454 dagster-1.3.2/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18951 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13227 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    26262 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17376 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.124454 dagster-1.3.2/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23190 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)    23821 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/pipeline_run.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15584 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8629 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46629 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    19749 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14174 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14920 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    28122 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18689 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.128454 dagster-1.3.2/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7393 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/utility_solids.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.132454 dagster-1.3.2/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5432 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    26661 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.132454 dagster-1.3.2/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6882 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9124 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17726 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8371 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16312 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    35637 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.804453 dagster-1.3.2/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-04-27 18:30:33.000000 dagster-1.3.2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.188454 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11665 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38179 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18538 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    22220 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    52639 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26204 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      468 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31924 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37037 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.192454 dagster-1.3.2/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.196454 dagster-1.3.2/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23212 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8667 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    23704 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.196454 dagster-1.3.2/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10463 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    23902 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:49.200454 dagster-1.3.2/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 18:30:34.000000 dagster-1.3.2/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 18:31:48.808453 dagster-1.3.2/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-27 18:31:47.000000 dagster-1.3.2/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24867 2023-04-27 18:31:48.000000 dagster-1.3.2/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 18:31:47.000000 dagster-1.3.2/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-27 18:31:47.000000 dagster-1.3.2/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-04-27 18:31:47.000000 dagster-1.3.2/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-27 18:31:47.000000 dagster-1.3.2/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-27 18:31:49.200454 dagster-1.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-04-27 18:30:35.000000 dagster-1.3.2/setup.py
```

### Comparing `dagster-1.3.1/COPYING` & `dagster-1.3.2/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/LICENSE` & `dagster-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/PKG-INFO` & `dagster-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.1
+Version: 1.3.2
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.1/README.md` & `dagster-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/__init__.py` & `dagster-1.3.2/dagster/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,14 +452,15 @@
 from dagster._core.storage.asset_value_loader import AssetValueLoader as AssetValueLoader
 from dagster._core.storage.file_manager import (
     FileHandle as FileHandle,
     LocalFileHandle as LocalFileHandle,
     local_file_manager as local_file_manager,
 )
 from dagster._core.storage.fs_io_manager import (
+    FilesystemIOManager as FilesystemIOManager,
     custom_path_fs_io_manager as custom_path_fs_io_manager,
     fs_io_manager as fs_io_manager,
 )
 from dagster._core.storage.input_manager import (
     InputManager as InputManager,
     input_manager as input_manager,
 )
```

### Comparing `dagster-1.3.1/dagster/_annotations.py` & `dagster-1.3.2/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/get_server_id.py` & `dagster-1.3.2/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/list_repositories.py` & `dagster-1.3.2/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/notebook_data.py` & `dagster-1.3.2/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.2/dagster/_api/snapshot_execution_plan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TYPE_CHECKING, AbstractSet, Any, Mapping, Optional, Sequence
 
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.errors import DagsterUserCodeProcessError
 from dagster._core.execution.plan.state import KnownExecutionState
+from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 from dagster._core.host_representation.origin import ExternalPipelineOrigin
 from dagster._core.instance import DagsterInstance
 from dagster._core.snap.execution_plan_snapshot import (
     ExecutionPlanSnapshot,
     ExecutionPlanSnapshotErrorData,
 )
 from dagster._grpc.types import ExecutionPlanSnapshotArgs
@@ -17,15 +18,14 @@
     from dagster._grpc.client import DagsterGrpcClient
 
 
 def sync_get_external_execution_plan_grpc(
     api_client: "DagsterGrpcClient",
     pipeline_origin: ExternalPipelineOrigin,
     run_config: Mapping[str, Any],
-    mode: str,
     pipeline_snapshot_id: str,
     asset_selection: Optional[AbstractSet[AssetKey]] = None,
     solid_selection: Optional[Sequence[str]] = None,
     step_keys_to_execute: Optional[Sequence[str]] = None,
     known_state: Optional[KnownExecutionState] = None,
     instance: Optional[DagsterInstance] = None,
 ) -> ExecutionPlanSnapshot:
@@ -34,27 +34,26 @@
     check.inst_param(api_client, "api_client", DagsterGrpcClient)
     check.inst_param(pipeline_origin, "pipeline_origin", ExternalPipelineOrigin)
     solid_selection = check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
     asset_selection = check.opt_nullable_set_param(
         asset_selection, "asset_selection", of_type=AssetKey
     )
     run_config = check.mapping_param(run_config, "run_config", key_type=str)
-    check.str_param(mode, "mode")
     check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
     check.str_param(pipeline_snapshot_id, "pipeline_snapshot_id")
     check.opt_inst_param(known_state, "known_state", KnownExecutionState)
     check.opt_inst_param(instance, "instance", DagsterInstance)
 
     result = deserialize_value(
         api_client.execution_plan_snapshot(
             execution_plan_snapshot_args=ExecutionPlanSnapshotArgs(
                 pipeline_origin=pipeline_origin,
                 solid_selection=solid_selection,
                 run_config=run_config,
-                mode=mode,
+                mode=DEFAULT_MODE_NAME,
                 step_keys_to_execute=step_keys_to_execute,
                 pipeline_snapshot_id=pipeline_snapshot_id,
                 known_state=known_state,
                 instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
                 asset_selection=asset_selection,
             )
         ),
```

### Comparing `dagster-1.3.1/dagster/_api/snapshot_partition.py` & `dagster-1.3.2/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/snapshot_pipeline.py` & `dagster-1.3.2/dagster/_api/snapshot_pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/snapshot_repository.py` & `dagster-1.3.2/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/snapshot_schedule.py` & `dagster-1.3.2/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_api/snapshot_sensor.py` & `dagster-1.3.2/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_check/README.md` & `dagster-1.3.2/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_check/__init__.py` & `dagster-1.3.2/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/__init__.py` & `dagster-1.3.2/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/api.py` & `dagster-1.3.2/dagster/_cli/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,14 @@
             )
         )
 
         execution_plan = create_execution_plan(
             recon_pipeline,
             run_config=pipeline_run.run_config,
             step_keys_to_execute=args.step_keys_to_execute,
-            mode=pipeline_run.mode,
             known_state=args.known_state,
             repository_load_data=repository_load_data,
         )
 
         yield from execute_plan_iterator(
             execution_plan,
             recon_pipeline,
```

### Comparing `dagster-1.3.1/dagster/_cli/asset.py` & `dagster-1.3.2/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/config_scaffolder.py` & `dagster-1.3.2/dagster/_cli/config_scaffolder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Optional
 
 from dagster import _check as check
 from dagster._config import ConfigType, ConfigTypeKind
-from dagster._core.definitions import create_run_config_schema
-from dagster._legacy import PipelineDefinition
+from dagster._core.definitions import JobDefinition
 
 
 def scaffold_pipeline_config(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     skip_non_required: bool = True,
     mode: Optional[str] = None,
 ):
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
     check.bool_param(skip_non_required, "skip_non_required")
 
-    env_config_type = create_run_config_schema(pipeline_def, mode=mode).config_type
+    env_config_type = pipeline_def.run_config_schema.config_type
 
     env_dict = {}
 
     for env_field_name, env_field in env_config_type.fields.items():  # type: ignore
         if skip_non_required and not env_field.is_required:
             continue
```

### Comparing `dagster-1.3.1/dagster/_cli/debug.py` & `dagster-1.3.2/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/dev.py` & `dagster-1.3.2/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/instance.py` & `dagster-1.3.2/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/job.py` & `dagster-1.3.2/dagster/_cli/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,19 @@
     get_job_python_origin_from_kwargs,
     get_workspace_from_kwargs,
     job_repository_target_argument,
     job_target_argument,
     python_job_config_argument,
     python_job_target_argument,
 )
+from dagster._core.definitions import JobDefinition
 from dagster._core.definitions.reconstruct import ReconstructableJob
 from dagster._core.definitions.selector import PipelineSelector
 from dagster._core.definitions.utils import validate_tags
-from dagster._core.errors import DagsterBackfillFailedError, DagsterInvariantViolationError
+from dagster._core.errors import DagsterBackfillFailedError
 from dagster._core.execution.api import create_execution_plan, execute_job
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
 from dagster._core.execution.execution_result import ExecutionResult
 from dagster._core.execution.job_backfill import create_backfill_run
 from dagster._core.host_representation import (
     CodeLocation,
     ExternalPipeline,
@@ -48,15 +49,14 @@
 from dagster._core.instance import DagsterInstance
 from dagster._core.snap import NodeInvocationSnap, PipelineSnapshot
 from dagster._core.storage.pipeline_run import DagsterRun
 from dagster._core.storage.tags import MEMOIZED_RUN_TAG
 from dagster._core.telemetry import log_external_repo_stats, telemetry_wrapper
 from dagster._core.utils import make_new_backfill_id
 from dagster._core.workspace.workspace import IWorkspace
-from dagster._legacy import PipelineDefinition
 from dagster._seven import IS_WINDOWS, JSONDecodeError, json
 from dagster._utils import DEFAULT_WORKSPACE_YAML_FILENAME, PrintFn
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.hosted_user_process import recon_pipeline_from_origin
 from dagster._utils.indenting_printer import IndentingPrinter
 from dagster._utils.interrupts import capture_interrupts
 from dagster._utils.merger import merge_dicts
@@ -261,15 +261,14 @@
     job_origin = get_job_python_origin_from_kwargs(kwargs)
     job = recon_pipeline_from_origin(job_origin)
     run_config = get_run_config_from_file_list(config)
 
     memoized_plan = create_execution_plan(
         job,
         run_config=run_config,
-        mode="default",
         instance_ref=instance.get_ref(),
         tags={MEMOIZED_RUN_TAG: "true"},
     )
 
     add_step_to_table(memoized_plan)
 
 
@@ -319,19 +318,14 @@
 @telemetry_wrapper
 def execute_execute_command(instance: DagsterInstance, kwargs: ClickArgMapping) -> ExecutionResult:
     check.inst_param(instance, "instance", DagsterInstance)
 
     config = list(
         check.opt_tuple_param(cast(Tuple[str, ...], kwargs.get("config")), "config", of_type=str)
     )
-    preset = cast(Optional[str], kwargs.get("preset"))
-    cast(Optional[str], kwargs.get("mode"))
-
-    if preset and config:
-        raise click.UsageError("Can not use --preset with --config.")
 
     tags = get_tags_from_args(kwargs)
 
     pipeline_origin = get_job_python_origin_from_kwargs(kwargs)
     pipeline = recon_pipeline_from_origin(pipeline_origin)
     solid_selection = get_solid_selection_from_args(kwargs)
     result = do_execute_command(pipeline, instance, config, tags, solid_selection)
@@ -440,15 +434,14 @@
 
 @telemetry_wrapper
 def execute_launch_command(
     instance: DagsterInstance,
     kwargs: Mapping[str, str],
 ) -> DagsterRun:
     preset = cast(Optional[str], kwargs.get("preset"))
-    mode = cast(Optional[str], kwargs.get("mode"))
     check.inst_param(instance, "instance", DagsterInstance)
     config = get_config_from_args(kwargs)
 
     with get_workspace_from_kwargs(instance, version=dagster_version, kwargs=kwargs) as workspace:
         code_location = get_code_location_from_workspace(workspace, kwargs.get("location"))
         external_repo = get_external_repository_from_code_location(
             code_location, cast(Optional[str], kwargs.get("repository"))
@@ -474,84 +467,72 @@
 
         pipeline_run = _create_external_pipeline_run(
             instance=instance,
             code_location=code_location,
             external_repo=external_repo,
             external_pipeline=external_pipeline,
             run_config=config,
-            mode=mode,
-            preset=preset,
             tags=run_tags,
             solid_selection=solid_selection,
             run_id=cast(Optional[str], kwargs.get("run_id")),
         )
 
         return instance.submit_run(pipeline_run.run_id, workspace)
 
 
 def _create_external_pipeline_run(
     instance: DagsterInstance,
     code_location: CodeLocation,
     external_repo: ExternalRepository,
     external_pipeline: ExternalPipeline,
     run_config: Mapping[str, object],
-    mode: Optional[str],
-    preset: Optional[str],
     tags: Optional[Mapping[str, str]],
     solid_selection: Optional[Sequence[str]],
     run_id: Optional[str],
 ) -> DagsterRun:
     check.inst_param(instance, "instance", DagsterInstance)
     check.inst_param(code_location, "code_location", CodeLocation)
     check.inst_param(external_repo, "external_repo", ExternalRepository)
     check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
     check.opt_mapping_param(run_config, "run_config", key_type=str)
 
-    check.opt_str_param(mode, "mode")
-    check.opt_str_param(preset, "preset")
     check.opt_mapping_param(tags, "tags", key_type=str)
     check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
     check.opt_str_param(run_id, "run_id")
 
-    run_config, mode, tags, solid_selection = _check_execute_external_pipeline_args(
+    run_config, tags, solid_selection = _check_execute_external_pipeline_args(
         external_pipeline,
         run_config,
-        mode,
-        preset,
         tags,
         solid_selection,
     )
 
     pipeline_name = external_pipeline.name
     pipeline_selector = PipelineSelector(
         location_name=code_location.name,
         repository_name=external_repo.name,
         pipeline_name=pipeline_name,
         solid_selection=solid_selection,
     )
 
     external_pipeline = code_location.get_external_pipeline(pipeline_selector)
 
-    pipeline_mode = mode or external_pipeline.get_default_mode_name()
-
     external_execution_plan = code_location.get_external_execution_plan(
         external_pipeline,
         run_config,
-        pipeline_mode,
         step_keys_to_execute=None,
         known_state=None,
         instance=instance,
     )
     execution_plan_snapshot = external_execution_plan.execution_plan_snapshot
 
     return instance.create_run(
         pipeline_name=pipeline_name,
         run_id=run_id,
         run_config=run_config,
-        mode=pipeline_mode,
         solids_to_execute=external_pipeline.solids_to_execute,
         step_keys_to_execute=execution_plan_snapshot.step_keys_to_execute,
         solid_selection=solid_selection,
         status=None,
         root_run_id=None,
         parent_run_id=None,
         tags=tags,
@@ -563,96 +544,26 @@
         asset_selection=None,
     )
 
 
 def _check_execute_external_pipeline_args(
     external_pipeline: ExternalPipeline,
     run_config: Mapping[str, object],
-    mode: Optional[str],
-    preset: Optional[str],
     tags: Optional[Mapping[str, str]],
     solid_selection: Optional[Sequence[str]],
-) -> Tuple[Mapping[str, object], str, Mapping[str, str], Optional[Sequence[str]]]:
+) -> Tuple[Mapping[str, object], Mapping[str, str], Optional[Sequence[str]]]:
     check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
     run_config = check.opt_mapping_param(run_config, "run_config")
-    check.opt_str_param(mode, "mode")
-    check.opt_str_param(preset, "preset")
-    check.invariant(
-        not (mode is not None and preset is not None),
-        "You may set only one of `mode` (got {mode}) or `preset` (got {preset}).".format(
-            mode=mode, preset=preset
-        ),
-    )
 
     tags = check.opt_mapping_param(tags, "tags", key_type=str)
     check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
-
-    if preset is not None:
-        pipeline_preset = external_pipeline.get_preset(preset)
-
-        if pipeline_preset.run_config is not None:
-            check.invariant(
-                (not run_config) or (pipeline_preset.run_config == run_config),
-                "The environment set in preset '{preset}' does not agree with the environment "
-                "passed in the `run_config` argument.".format(preset=preset),
-            )
-
-            run_config = pipeline_preset.run_config
-
-        # load solid_selection from preset
-        if pipeline_preset.solid_selection is not None:
-            check.invariant(
-                solid_selection is None or solid_selection == pipeline_preset.solid_selection,
-                "The solid_selection set in preset '{preset}', {preset_subset}, does not agree with"
-                " the `solid_selection` argument: {solid_selection}".format(
-                    preset=preset,
-                    preset_subset=pipeline_preset.solid_selection,
-                    solid_selection=solid_selection,
-                ),
-            )
-            solid_selection = pipeline_preset.solid_selection
-
-        check.invariant(
-            mode is None or mode == pipeline_preset.mode,
-            "Mode {mode} does not agree with the mode set in preset '{preset}': "
-            "('{preset_mode}')".format(preset=preset, preset_mode=pipeline_preset.mode, mode=mode),
-        )
-
-        mode = pipeline_preset.mode
-
-        tags = merge_dicts(pipeline_preset.tags, tags)
-
-    if mode is not None:
-        if not external_pipeline.has_mode(mode):
-            raise DagsterInvariantViolationError(
-                (
-                    "You have attempted to execute pipeline {name} with mode {mode}. "
-                    "Available modes: {modes}"
-                ).format(
-                    name=external_pipeline.name,
-                    mode=mode,
-                    modes=external_pipeline.available_modes,
-                )
-            )
-    else:
-        if len(external_pipeline.available_modes) > 1:
-            raise DagsterInvariantViolationError(
-                (
-                    "Pipeline {name} has multiple modes (Available modes: {modes}) and you have "
-                    "attempted to execute it without specifying a mode. Set "
-                    "mode property on the PipelineRun object."
-                ).format(name=external_pipeline.name, modes=external_pipeline.available_modes)
-            )
-        mode = external_pipeline.get_default_mode_name()
-
     tags = merge_dicts(external_pipeline.tags, tags)
 
     return (
         run_config,
-        mode,
         validate_tags(tags),
         solid_selection,
     )
 
 
 @job_cli.command(
     name="scaffold_config",
@@ -670,19 +581,19 @@
     pipeline_origin = get_job_python_origin_from_kwargs(cli_args)
     pipeline = recon_pipeline_from_origin(pipeline_origin)
     skip_non_required = cli_args["print_only_required"]
     do_scaffold_command(pipeline.get_definition(), print_fn, skip_non_required)
 
 
 def do_scaffold_command(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     printer: Callable[..., Any],
     skip_non_required: bool,
 ):
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
     check.callable_param(printer, "printer")
     check.bool_param(skip_non_required, "skip_non_required")
 
     config_dict = scaffold_pipeline_config(pipeline_def, skip_non_required=skip_non_required)
     yaml_string = dump_run_config_yaml(config_dict)
     printer(yaml_string)
```

### Comparing `dagster-1.3.1/dagster/_cli/load_handle.py` & `dagster-1.3.2/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/project.py` & `dagster-1.3.2/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/run.py` & `dagster-1.3.2/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/schedule.py` & `dagster-1.3.2/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/sensor.py` & `dagster-1.3.2/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/utils.py` & `dagster-1.3.2/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.2/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/__init__.py` & `dagster-1.3.2/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/config_schema.py` & `dagster-1.3.2/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/config_type.py` & `dagster-1.3.2/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/errors.py` & `dagster-1.3.2/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/evaluate_value_result.py` & `dagster-1.3.2/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/field.py` & `dagster-1.3.2/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/field_utils.py` & `dagster-1.3.2/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/post_process.py` & `dagster-1.3.2/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/primitive_mapping.py` & `dagster-1.3.2/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.2/dagster/_config/pythonic_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,42 @@
                 raise
 
     def _is_field_internal(self, name: str) -> bool:
         return name.endswith(INTERNAL_MARKER)
 
 
 class Config(MakeConfigCacheable):
-    """Base class for Dagster configuration models."""
+    """Base class for Dagster configuration models, used to specify config schema for
+    ops and assets. Subclasses :py:class:`pydantic.BaseModel`.
+
+    Example definition:
+
+    .. code-block:: python
+
+        from pydantic import Field
+
+        class MyAssetConfig(Config):
+            my_str: str = "my_default_string"
+            my_int_list: List[int]
+            my_bool_with_metadata: bool = Field(default=False, description="A bool field")
+
+
+    Example usage:
+
+    .. code-block:: python
+
+        @asset
+        def asset_with_config(config: MyAssetConfig):
+            assert config.my_str == "my_default_string"
+            assert config.my_int_list == [1, 2, 3]
+            assert config.my_bool_with_metadata == False
+
+        asset_with_config(MyAssetConfig(my_int_list=[1, 2, 3], my_bool_with_metadata=True))
+
+    """
 
     def __init__(self, **config_dict) -> None:
         """This constructor is overridden to handle any remapping of raw config dicts to
         the appropriate config classes. For example, discriminated unions are represented
         in Dagster config as dicts with a single key, which is the discriminator value.
         """
         modified_data = {}
@@ -215,23 +242,51 @@
         This is useful when interacting with legacy code that expects a dictionary of fields but you
         want the source of truth to be a config class.
         """
         return cast(Shape, cls.to_config_schema().as_field().config_type).fields
 
 
 class PermissiveConfig(Config):
+    """Subclass of :py:class:`Config` that allows arbitrary extra fields. This is useful for
+    config classes which may have open-ended inputs.
+
+    Example definition:
+
+    .. code-block:: python
+
+        class MyPermissiveOpConfig(PermissiveConfig):
+            my_explicit_parameter: bool
+            my_other_explicit_parameter: str
+
+
+    Example usage:
+
+    .. code-block:: python
+
+        @op
+        def op_with_config(config: MyPermissiveOpConfig):
+            assert config.my_explicit_parameter == True
+            assert config.my_other_explicit_parameter == "foo"
+            assert config.dict().get("my_implicit_parameter") == "bar"
+
+        op_with_config(
+            MyPermissiveOpConfig(
+                my_explicit_parameter=True,
+                my_other_explicit_parameter="foo",
+                my_implicit_parameter="bar"
+            )
+        )
+
+    """
+
     # Pydantic config for this class
     # Cannot use kwargs for base class as this is not support for pydantic<1.8
     class Config:
         extra = "allow"
 
-    """
-    Base class for Dagster configuration models that allow arbitrary extra fields.
-    """
-
 
 # This is from https://github.com/dagster-io/dagster/pull/11470
 def _apply_defaults_to_schema_field(field: Field, additional_default_values: Any) -> Field:
     # This work by validating the top-level config and then
     # just setting it at that top-level field. Config fields
     # can actually take nested values so we only need to set it
     # at a single level
@@ -789,15 +844,15 @@
                 my_str: str
 
             @resource(config_schema=MyResource.to_config_schema())
             def my_resource(context: InitResourceContext) -> MyResource:
                 return MyResource.from_resource_context(context)
 
         """
-        return cls(**context.resource_config or {}).create_resource(context)
+        return cls(**context.resource_config or {})._create_object_fn(context)  # noqa: SLF001
 
 
 class ConfigurableResource(ConfigurableResourceFactory[TResValue]):
     """Base class for Dagster resources that utilize structured config.
 
     This class is a subclass of both :py:class:`ResourceDefinition` and :py:class:`Config`.
 
@@ -807,16 +862,14 @@
 
         class WriterResource(ConfigurableResource):
             prefix: str
 
             def output(self, text: str) -> None:
                 print(f"{self.prefix}{text}")
 
-        # which can be used in a pipeline like so:
-
     Example usage:
 
     .. code-block:: python
 
         @asset
         def asset_that_uses_writer(writer: WriterResource):
             writer.output("text")
@@ -990,14 +1043,49 @@
     """Base class for Dagster IO managers that utilize structured config. This base class
     is useful for cases in which the returned IO manager is not the same as the class itself
     (e.g. when it is a wrapper around the actual IO manager implementation).
 
     This class is a subclass of both :py:class:`IOManagerDefinition` and :py:class:`Config`.
     Implementers should provide an implementation of the :py:meth:`resource_function` method,
     which should return an instance of :py:class:`IOManager`.
+
+
+    Example definition:
+
+    .. code-block:: python
+
+        class ExternalIOManager(IOManager):
+
+            def __init__(self, connection):
+                self._connection = connection
+
+            def handle_output(self, context, obj):
+                ...
+
+            def load_input(self, context):
+                ...
+
+        class ConfigurableExternalIOManager(ConfigurableIOManagerFactory):
+            username: str
+            password: str
+
+            def create_io_manager(self, context) -> IOManager:
+                with database.connect(username, password) as connection:
+                    return MyExternalIOManager(connection)
+
+        defs = Definitions(
+            ...,
+            resources={
+                "io_manager": ConfigurableExternalIOManager(
+                    username="dagster",
+                    password=EnvVar("DB_PASSWORD")
+                )
+            }
+        )
+
     """
 
     def __init__(self, **data: Any):
         ConfigurableResourceFactory.__init__(self, **data)
 
     @abstractmethod
     def create_io_manager(self, context) -> TIOManagerValue:
@@ -1049,14 +1137,38 @@
 
 class ConfigurableIOManager(ConfigurableIOManagerFactory, IOManager):
     """Base class for Dagster IO managers that utilize structured config.
 
     This class is a subclass of both :py:class:`IOManagerDefinition`, :py:class:`Config`,
     and :py:class:`IOManager`. Implementers must provide an implementation of the
     :py:meth:`handle_output` and :py:meth:`load_input` methods.
+
+    Example definition:
+
+    .. code-block:: python
+
+        class MyIOManager(ConfigurableIOManager):
+            path_prefix: List[str]
+
+            def _get_path(self, context) -> str:
+                return "/".join(context.asset_key.path)
+
+            def handle_output(self, context, obj):
+                write_csv(self._get_path(context), obj)
+
+            def load_input(self, context):
+                return read_csv(self._get_path(context))
+
+        defs = Definitions(
+            ...,
+            resources={
+                "io_manager": MyIOManager(path_prefix=["my", "prefix"])
+            }
+        )
+
     """
 
     def create_io_manager(self, context) -> IOManager:
         return self
 
 
 PydanticShapeType: TypeAlias = int
```

### Comparing `dagster-1.3.1/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.2/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.2/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.2/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/snap.py` & `dagster-1.3.2/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/source.py` & `dagster-1.3.2/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/stack.py` & `dagster-1.3.2/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/traversal_context.py` & `dagster-1.3.2/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/type_printer.py` & `dagster-1.3.2/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_config/validate.py` & `dagster-1.3.2/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/assets.py` & `dagster-1.3.2/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/code_pointer.py` & `dagster-1.3.2/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/container_context/config.py` & `dagster-1.3.2/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/debug.py` & `dagster-1.3.2/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/decorator_utils.py` & `dagster-1.3.2/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/__init__.py` & `dagster-1.3.2/dagster/_core/definitions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     Output as Output,
     RetryRequested as RetryRequested,
     TypeCheck as TypeCheck,
 )
 from .executor_definition import (
     ExecutorDefinition as ExecutorDefinition,
     ExecutorRequirement as ExecutorRequirement,
-    default_executors as default_executors,
     executor as executor,
     in_process_executor as in_process_executor,
     multi_or_in_process_executor as multi_or_in_process_executor,
     multiple_process_executor_requirements as multiple_process_executor_requirements,
     multiprocess_executor as multiprocess_executor,
 )
 from .hook_definition import HookDefinition as HookDefinition
@@ -145,15 +144,14 @@
     load_assets_from_package_module as load_assets_from_package_module,
     load_assets_from_package_name as load_assets_from_package_name,
 )
 from .materialize import (
     materialize as materialize,
     materialize_to_memory as materialize_to_memory,
 )
-from .mode import ModeDefinition as ModeDefinition
 from .op_definition import OpDefinition as OpDefinition
 from .partition import (
     DynamicPartitionsDefinition as DynamicPartitionsDefinition,
     Partition as Partition,
     PartitionedConfig as PartitionedConfig,
     PartitionsDefinition as PartitionsDefinition,
     StaticPartitionsDefinition as StaticPartitionsDefinition,
@@ -169,16 +167,14 @@
     MultiPartitionMapping as MultiPartitionMapping,
     MultiToSingleDimensionPartitionMapping as MultiToSingleDimensionPartitionMapping,
     PartitionMapping as PartitionMapping,
 )
 from .partitioned_schedule import (
     build_schedule_from_partitioned_job as build_schedule_from_partitioned_job,
 )
-from .pipeline_definition import PipelineDefinition as PipelineDefinition
-from .preset import PresetDefinition as PresetDefinition
 from .run_status_sensor_definition import (
     RunFailureSensorContext as RunFailureSensorContext,
     RunStatusSensorContext as RunStatusSensorContext,
     RunStatusSensorDefinition as RunStatusSensorDefinition,
     run_failure_sensor as run_failure_sensor,
     run_status_sensor as run_status_sensor,
 )
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.2/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.2/dagster/_core/definitions/asset_graph_subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,18 +222,29 @@
             asset_graph, partitions_subsets_by_asset_key, non_partitioned_asset_keys
         )
 
     @classmethod
     def all(
         cls, asset_graph: AssetGraph, dynamic_partitions_store: DynamicPartitionsStore
     ) -> "AssetGraphSubset":
+        return cls.from_asset_keys(
+            asset_graph.non_source_asset_keys, asset_graph, dynamic_partitions_store
+        )
+
+    @classmethod
+    def from_asset_keys(
+        cls,
+        asset_keys: Iterable[AssetKey],
+        asset_graph: AssetGraph,
+        dynamic_partitions_store: DynamicPartitionsStore,
+    ) -> "AssetGraphSubset":
         partitions_subsets_by_asset_key: Dict[AssetKey, PartitionsSubset] = {}
         non_partitioned_asset_keys: Set[AssetKey] = set()
 
-        for asset_key in asset_graph.non_source_asset_keys:
+        for asset_key in asset_keys:
             partitions_def = asset_graph.get_partitions_def(asset_key)
             if partitions_def:
                 partitions_subsets_by_asset_key[
                     asset_key
                 ] = partitions_def.empty_subset().with_partition_keys(
                     partitions_def.get_partition_keys(
                         dynamic_partitions_store=dynamic_partitions_store
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_group.py` & `dagster-1.3.2/dagster/_core/definitions/asset_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,28 +92,30 @@
 
     """
 
     def __init__(
         self,
         assets: Sequence[AssetsDefinition],
         source_assets: Optional[Sequence[SourceAsset]] = None,
-        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+        resource_defs: Optional[Mapping[str, Any]] = None,
         executor_def: Optional[ExecutorDefinition] = None,
     ):
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
+
         check.sequence_param(assets, "assets", of_type=AssetsDefinition)
 
         source_assets = check.opt_sequence_param(
             source_assets, "source_assets", of_type=SourceAsset
         )
-        resource_defs = check.opt_mapping_param(
-            resource_defs, "resource_defs", key_type=str, value_type=ResourceDefinition
-        )
-        resource_defs = merge_dicts(
-            {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
-            resource_defs,
+        resource_defs = check.opt_mapping_param(resource_defs, "resource_defs", key_type=str)
+        resource_defs = wrap_resources_for_execution(
+            merge_dicts(
+                {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
+                resource_defs,
+            )
         )
         executor_def = check.opt_inst_param(executor_def, "executor_def", ExecutorDefinition)
 
         check_resources_satisfy_requirements(assets, source_assets, resource_defs)
 
         self._assets = assets
         self._source_assets = source_assets
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_in.py` & `dagster-1.3.2/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.2/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_out.py` & `dagster-1.3.2/dagster/_core/definitions/asset_out.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Mapping, NamedTuple, Optional, Sequence, Type, Union
 
 import dagster._check as check
 from dagster._annotations import PublicAttr
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.events import (
     AssetKey,
     CoercibleToAssetKey,
     CoercibleToAssetKeyPrefix,
 )
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.input import NoValueSentinel
@@ -25,14 +26,15 @@
             ("io_manager_key", PublicAttr[str]),
             ("description", PublicAttr[Optional[str]]),
             ("is_required", PublicAttr[bool]),
             ("dagster_type", PublicAttr[Union[DagsterType, Type[NoValueSentinel]]]),
             ("group_name", PublicAttr[Optional[str]]),
             ("code_version", PublicAttr[Optional[str]]),
             ("freshness_policy", PublicAttr[Optional[FreshnessPolicy]]),
+            ("auto_materialize_policy", PublicAttr[Optional[AutoMaterializePolicy]]),
         ],
     )
 ):
     """Defines one of the assets produced by a :py:func:`@multi_asset <multi_asset>`.
 
     Attributes:
         key_prefix (Optional[Union[str, Sequence[str]]]): If provided, the asset's key is the
@@ -53,28 +55,31 @@
             filesystem, or provide information of a database table when it is going to load the data
             into the table.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If
             not provided, the name "default" is used.
         code_version (Optional[str]): The version of the code that generates this asset.
         freshness_policy (Optional[FreshnessPolicy]): A policy which indicates how up to date this
             asset is intended to be.
+        auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply to
+            the specified asset.
     """
 
     def __new__(
         cls,
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         key: Optional[CoercibleToAssetKey] = None,
         dagster_type: Union[Type, DagsterType] = NoValueSentinel,
         description: Optional[str] = None,
         is_required: bool = True,
         io_manager_key: Optional[str] = None,
         metadata: Optional[MetadataUserInput] = None,
         group_name: Optional[str] = None,
         code_version: Optional[str] = None,
         freshness_policy: Optional[FreshnessPolicy] = None,
+        auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
     ):
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
 
         return super(AssetOut, cls).__new__(
             cls,
             key=AssetKey.from_coerceable(key) if key is not None else None,
@@ -89,14 +94,17 @@
             ),
             metadata=check.opt_mapping_param(metadata, "metadata", key_type=str),
             group_name=check.opt_str_param(group_name, "group_name"),
             code_version=check.opt_str_param(code_version, "code_version"),
             freshness_policy=check.opt_inst_param(
                 freshness_policy, "freshness_policy", FreshnessPolicy
             ),
+            auto_materialize_policy=check.opt_inst_param(
+                auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
+            ),
         )
 
     def to_out(self) -> Out:
         return Out(
             dagster_type=self.dagster_type,
             description=self.description,
             metadata=self.metadata,
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.2/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,32 @@
     Iterable,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Set,
     Tuple,
+    Union,
     cast,
 )
 
 import pendulum
 
 import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.asset_graph_subset import AssetGraphSubset
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
-from dagster._core.definitions.partition_mapping import IdentityPartitionMapping
+from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
+    has_one_dimension_time_window_partitioning,
 )
 from dagster._utils.backcompat import deprecation_warning
 from dagster._utils.schedules import cron_string_iterator
 
 from .asset_selection import AssetGraph, AssetSelection
 from .decorators.sensor_decorator import sensor
 from .partition import PartitionsDefinition, PartitionsSubset
@@ -60,20 +62,31 @@
             for_freshness=True,
             time_window_partition_scope_minutes=24 * 60,
         )
     return auto_materialize_policy
 
 
 def reconciliation_window_for_time_window_partitions(
-    partitions_def: TimeWindowPartitionsDefinition,
+    partitions_def: Union[TimeWindowPartitionsDefinition, MultiPartitionsDefinition],
     time_window_partition_scope: Optional[datetime.timedelta],
     current_time: datetime.datetime,
 ) -> Optional[TimeWindow]:
-    latest_partition_window = partitions_def.get_last_partition_window(current_time=current_time)
-    earliest_partition_window = partitions_def.get_first_partition_window(current_time=current_time)
+    if isinstance(partitions_def, MultiPartitionsDefinition):
+        time_partitions_def = cast(
+            TimeWindowPartitionsDefinition, partitions_def.time_window_dimension.partitions_def
+        )
+    else:
+        time_partitions_def = partitions_def
+
+    latest_partition_window = time_partitions_def.get_last_partition_window(
+        current_time=current_time
+    )
+    earliest_partition_window = time_partitions_def.get_first_partition_window(
+        current_time=current_time
+    )
     if latest_partition_window is None or earliest_partition_window is None:
         return None
 
     allowable_start_time = (
         max(
             earliest_partition_window.start,
             latest_partition_window.start
@@ -83,15 +96,15 @@
         if time_window_partition_scope is not None
         else earliest_partition_window.start
     )
     return TimeWindow(allowable_start_time, latest_partition_window.end)
 
 
 def can_reconcile_time_window_partition(
-    partitions_def: TimeWindowPartitionsDefinition,
+    partitions_def: Union[TimeWindowPartitionsDefinition, MultiPartitionsDefinition],
     partition_key: Optional[str],
     time_window_partition_scope: Optional[datetime.timedelta],
     current_time: datetime.datetime,
 ) -> bool:
     if partition_key is None:
         return False
     if time_window_partition_scope is None:
@@ -399,22 +412,24 @@
                         partition_mapping.get_downstream_partitions_for_partitions(
                             partitions_subset,
                             downstream_partitions_def=child_partitions_def,
                             dynamic_partitions_store=instance_queryer,
                         )
                     )
                     for child_partition in child_partitions_subset.get_partition_keys():
-                        # we need to see if the child was materialized in the same run, but this is
+                        # we need to see if the child is planned for the same run, but this is
                         # expensive, so we try to avoid doing so in as many situations as possible
                         child_asset_partition = AssetKeyPartitionKey(child, child_partition)
                         if not can_reconcile_fn(child_asset_partition):
                             continue
-                        # cannot materialize in the same run if different partitions defs
-                        elif child_partitions_def != partitions_def or not isinstance(
-                            partition_mapping, IdentityPartitionMapping
+                        # cannot materialize in the same run if different partitions defs or
+                        # different partition keys
+                        elif (
+                            child_partitions_def != partitions_def
+                            or child_partition not in materialized_partitions
                         ):
                             result_asset_partitions.add(child_asset_partition)
                         else:
                             latest_partition_record = check.not_none(
                                 instance_queryer.get_latest_materialization_record(
                                     AssetKeyPartitionKey(asset_key, child_partition),
                                     after_cursor=latest_storage_id,
@@ -518,21 +533,25 @@
         )
         partitions_def = asset_graph.get_partitions_def(candidate.asset_key)
 
         # no policy means no reconciliation
         if auto_materialize_policy is None:
             return False
         # the partition is too old to reconcile
-        elif isinstance(
-            partitions_def, TimeWindowPartitionsDefinition
-        ) and not can_reconcile_time_window_partition(
-            partitions_def=partitions_def,
-            partition_key=candidate.partition_key,
-            time_window_partition_scope=auto_materialize_policy.time_window_partition_scope,
-            current_time=current_time,
+        elif (
+            partitions_def
+            and has_one_dimension_time_window_partitioning(partitions_def)
+            and not can_reconcile_time_window_partition(
+                partitions_def=cast(
+                    Union[TimeWindowPartitionsDefinition, MultiPartitionsDefinition], partitions_def
+                ),
+                partition_key=candidate.partition_key,
+                time_window_partition_scope=auto_materialize_policy.time_window_partition_scope,
+                current_time=current_time,
+            )
         ):
             return False
         # the policy does not allow for materializing missing partitions and it's missing
         elif not auto_materialize_policy.on_missing and not instance_queryer.materialization_exists(
             candidate
         ):
             return False
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.2/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.2/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/assets.py` & `dagster-1.3.2/dagster/_core/definitions/assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,14 +283,17 @@
         partition_mappings: Optional[Mapping[str, PartitionMapping]] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         group_name: Optional[str] = None,
         group_names_by_output_name: Optional[Mapping[str, Optional[str]]] = None,
         descriptions_by_output_name: Optional[Mapping[str, str]] = None,
         metadata_by_output_name: Optional[Mapping[str, Optional[ArbitraryMetadataMapping]]] = None,
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
+        auto_materialize_policies_by_output_name: Optional[
+            Mapping[str, Optional[AutoMaterializePolicy]]
+        ] = None,
         can_subset: bool = False,
     ) -> "AssetsDefinition":
         """Constructs an AssetsDefinition from a GraphDefinition.
 
         Args:
             graph_def (GraphDefinition): The GraphDefinition that is an asset.
             keys_by_input_name (Optional[Mapping[str, AssetKey]]): A mapping of the input
@@ -331,14 +334,18 @@
                 be associated with each of the output assets for this node. Keys are names of the
                 outputs, and values are dictionaries of metadata to be associated with the related
                 asset.
             freshness_policies_by_output_name (Optional[Mapping[str, Optional[FreshnessPolicy]]]): Defines a
                 FreshnessPolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
+            auto_materialize_policies_by_output_name (Optional[Mapping[str, Optional[AutoMaterializePolicy]]]): Defines an
+                AutoMaterializePolicy to be associated with some or all of the output assets for this node.
+                Keys are the names of the outputs, and values are the AutoMaterializePolicies to be attached
+                to the associated asset.
         """
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "AssetsDefinition.from_graph")
         return AssetsDefinition._from_node(
             node_def=graph_def,
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
@@ -348,14 +355,15 @@
             partition_mappings=partition_mappings,
             resource_defs=resource_defs,
             group_name=group_name,
             group_names_by_output_name=group_names_by_output_name,
             descriptions_by_output_name=descriptions_by_output_name,
             metadata_by_output_name=metadata_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
+            auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
             can_subset=can_subset,
         )
 
     @public
     @staticmethod
     def from_op(
         op_def: OpDefinition,
@@ -367,14 +375,17 @@
         partitions_def: Optional[PartitionsDefinition] = None,
         partition_mappings: Optional[Mapping[str, PartitionMapping]] = None,
         group_name: Optional[str] = None,
         group_names_by_output_name: Optional[Mapping[str, Optional[str]]] = None,
         descriptions_by_output_name: Optional[Mapping[str, str]] = None,
         metadata_by_output_name: Optional[Mapping[str, Optional[ArbitraryMetadataMapping]]] = None,
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
+        auto_materialize_policies_by_output_name: Optional[
+            Mapping[str, Optional[AutoMaterializePolicy]]
+        ] = None,
         can_subset: bool = False,
     ) -> "AssetsDefinition":
         """Constructs an AssetsDefinition from an OpDefinition.
 
         Args:
             op_def (OpDefinition): The OpDefinition that is an asset.
             keys_by_input_name (Optional[Mapping[str, AssetKey]]): A mapping of the input
@@ -411,28 +422,33 @@
                 be associated with each of the output assets for this node. Keys are names of the
                 outputs, and values are dictionaries of metadata to be associated with the related
                 asset.
             freshness_policies_by_output_name (Optional[Mapping[str, Optional[FreshnessPolicy]]]): Defines a
                 FreshnessPolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
+            auto_materialize_policies_by_output_name (Optional[Mapping[str, Optional[AutoMaterializePolicy]]]): Defines an
+                AutoMaterializePolicy to be associated with some or all of the output assets for this node.
+                Keys are the names of the outputs, and values are the AutoMaterializePolicies to be attached
+                to the associated asset.
         """
         return AssetsDefinition._from_node(
             node_def=op_def,
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
             key_prefix=key_prefix,
             internal_asset_deps=internal_asset_deps,
             partitions_def=partitions_def,
             partition_mappings=partition_mappings,
             group_name=group_name,
             group_names_by_output_name=group_names_by_output_name,
             descriptions_by_output_name=descriptions_by_output_name,
             metadata_by_output_name=metadata_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
+            auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
             can_subset=can_subset,
         )
 
     @staticmethod
     def _from_node(
         node_def: Union[OpDefinition, "GraphDefinition"],
         *,
@@ -444,14 +460,17 @@
         partition_mappings: Optional[Mapping[str, PartitionMapping]] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         group_name: Optional[str] = None,
         group_names_by_output_name: Optional[Mapping[str, Optional[str]]] = None,
         descriptions_by_output_name: Optional[Mapping[str, str]] = None,
         metadata_by_output_name: Optional[Mapping[str, Optional[ArbitraryMetadataMapping]]] = None,
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
+        auto_materialize_policies_by_output_name: Optional[
+            Mapping[str, Optional[AutoMaterializePolicy]]
+        ] = None,
         can_subset: bool = False,
     ) -> "AssetsDefinition":
         node_def = check.inst_param(node_def, "node_def", NodeDefinition)
         keys_by_input_name = _infer_keys_by_input_names(
             node_def,
             check.opt_mapping_param(
                 keys_by_input_name, "keys_by_input_name", key_type=str, value_type=AssetKey
@@ -539,14 +558,21 @@
             freshness_policies_by_key={
                 keys_by_output_name_with_prefix[output_name]: freshness_policy
                 for output_name, freshness_policy in freshness_policies_by_output_name.items()
                 if freshness_policy is not None
             }
             if freshness_policies_by_output_name
             else None,
+            auto_materialize_policies_by_key={
+                keys_by_output_name_with_prefix[output_name]: auto_materialize_policy
+                for output_name, auto_materialize_policy in auto_materialize_policies_by_output_name.items()
+                if auto_materialize_policy is not None
+            }
+            if auto_materialize_policies_by_output_name
+            else None,
             descriptions_by_key={
                 keys_by_output_name_with_prefix[output_name]: description
                 for output_name, description in descriptions_by_output_name.items()
                 if description is not None
             }
             if descriptions_by_output_name
             else None,
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/assets_job.py` & `dagster-1.3.2/dagster/_core/definitions/assets_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             config=config,
             tags=tags,
             executor_def=executor_def,
             partitions_def=partitions_def,
             asset_layer=asset_layer,
             _asset_selection_data=_asset_selection_data,
             metadata=original_job.metadata,
-            logger_defs=original_job.get_mode_definition().loggers,
+            logger_defs=original_job.loggers,
             hooks=original_job.hook_defs,
             op_retry_policy=original_job._op_retry_policy,  # noqa: SLF001
             version_strategy=original_job.version_strategy,
         )
 
     return graph.to_job(
         resource_defs=all_resource_defs,
@@ -314,15 +314,15 @@
             config=config,
             tags=tags,
             executor_def=executor_def,
             partitions_def=partitions_def,
             asset_layer=asset_layer,
             _asset_selection_data=_asset_selection_data,
             metadata=original_job.metadata,
-            logger_defs=original_job.get_mode_definition().loggers,
+            logger_defs=original_job.loggers,
             hooks=original_job.hook_defs,
             op_retry_policy=original_job._op_retry_policy,  # noqa: SLF001
             version_strategy=original_job.version_strategy,
         )
 
     return graph.to_job(
         resource_defs=all_resource_defs,
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.2/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 import datetime
+from enum import Enum
 from typing import NamedTuple, Optional
 
+import dagster._check as check
 from dagster._annotations import experimental, public
 from dagster._serdes.serdes import whitelist_for_serdes
 
 
+class AutoMaterializePolicyType(Enum):
+    EAGER = "EAGER"
+    LAZY = "LAZY"
+
+
 @experimental
 @whitelist_for_serdes
-class AutoMaterializePolicy(NamedTuple):
+class AutoMaterializePolicy(
+    NamedTuple(
+        "_AutoMaterializePolicy",
+        [
+            ("on_missing", bool),
+            ("on_new_parent_data", bool),
+            ("for_freshness", bool),
+            ("time_window_partition_scope_minutes", Optional[float]),
+        ],
+    )
+):
     """An AutoMaterializePolicy specifies how Dagster should attempt to keep an asset up-to-date.
 
     There are two main modes of reconciliation: eager and lazy.
 
     Regardless of this selection an asset / partition will never be materialized if any of its
     parents are missing.
 
@@ -34,18 +51,33 @@
 
     **Warning:**
 
     Constructing an AutoMaterializePolicy directly is not recommended as the API is subject to change.
     AutoMaterializePolicy.eager() and AutoMaterializePolicy.lazy() are the recommended API.
     """
 
-    on_missing: bool
-    on_new_parent_data: bool
-    for_freshness: bool
-    time_window_partition_scope_minutes: Optional[float]
+    def __new__(
+        cls,
+        on_missing: bool,
+        on_new_parent_data: bool,
+        for_freshness: bool,
+        time_window_partition_scope_minutes: Optional[float],
+    ):
+        check.invariant(
+            on_new_parent_data or for_freshness,
+            "One of on_new_parent_data or for_freshness must be True",
+        )
+
+        return super(AutoMaterializePolicy, cls).__new__(
+            cls,
+            on_missing=on_missing,
+            on_new_parent_data=on_new_parent_data,
+            for_freshness=for_freshness,
+            time_window_partition_scope_minutes=time_window_partition_scope_minutes,
+        )
 
     @property
     def time_window_partition_scope(self) -> Optional[datetime.timedelta]:
         if self.time_window_partition_scope_minutes is None:
             return None
         return datetime.timedelta(minutes=self.time_window_partition_scope_minutes)
 
@@ -64,7 +96,13 @@
     def lazy() -> "AutoMaterializePolicy":
         return AutoMaterializePolicy(
             on_missing=True,
             on_new_parent_data=False,
             for_freshness=True,
             time_window_partition_scope_minutes=datetime.timedelta.resolution.total_seconds() / 60,
         )
+
+    @property
+    def policy_type(self) -> AutoMaterializePolicyType:
+        if self.on_new_parent_data is True:
+            return AutoMaterializePolicyType.EAGER
+        return AutoMaterializePolicyType.LAZY
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.2/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/composition.py` & `dagster-1.3.2/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/config.py` & `dagster-1.3.2/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/configurable.py` & `dagster-1.3.2/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/data_time.py` & `dagster-1.3.2/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/data_version.py` & `dagster-1.3.2/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -551,14 +551,19 @@
 
         # source freshness policies from the AssetOuts (if any)
         freshness_policies_by_key = {
             keys_by_output_name[output_name]: out.freshness_policy
             for output_name, out in outs.items()
             if isinstance(out, AssetOut) and out.freshness_policy is not None
         }
+        auto_materialize_policies_by_key = {
+            keys_by_output_name[output_name]: out.auto_materialize_policy
+            for output_name, out in outs.items()
+            if isinstance(out, AssetOut) and out.auto_materialize_policy is not None
+        }
         partition_mappings = {
             keys_by_input_name[input_name]: asset_in.partition_mapping
             for input_name, asset_in in (ins or {}).items()
             if asset_in.partition_mapping is not None
         }
 
         return AssetsDefinition(
@@ -568,14 +573,15 @@
             asset_deps={keys_by_output_name[name]: asset_deps[name] for name in asset_deps},
             partitions_def=partitions_def,
             partition_mappings=partition_mappings if partition_mappings else None,
             can_subset=can_subset,
             resource_defs=resource_defs,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
+            auto_materialize_policies_by_key=auto_materialize_policies_by_key,
         )
 
     return inner
 
 
 def build_asset_ins(
     fn: Callable,
@@ -661,14 +667,15 @@
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     description: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
     metadata: Optional[MetadataUserInput] = ...,
     freshness_policy: Optional[FreshnessPolicy] = ...,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = ...,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     ...
 
 
 def graph_asset(
     compose_fn: Optional[Callable] = None,
     *,
@@ -676,14 +683,16 @@
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     description: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
     metadata: Optional[MetadataUserInput] = None,
     freshness_policy: Optional[FreshnessPolicy] = None,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+    resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> Union[AssetsDefinition, Callable[[Callable[..., Any]], AssetsDefinition]]:
     """Creates a software-defined asset that's computed using a graph of ops.
 
     This decorator is meant to decorate a function that composes a set of ops or graphs to define
     the dependencies between them.
 
     Args:
@@ -698,16 +707,18 @@
             about the input.
         partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
             compose the asset.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If
             not provided, the name "default" is used.
         metadata (Optional[MetadataUserInput]): Dictionary of metadata to be associated with
             the asset.
-        freshness_policy (FreshnessPolicy): A constraint telling Dagster how often this asset is
+        freshness_policy (Optional[FreshnessPolicy]): A constraint telling Dagster how often this asset is
             intended to be updated with respect to its root data.
+        auto_materialize_policy (Optional[AutoMaterializePolicy]): The AutoMaterializePolicy to use
+            for this asset.
 
     Examples:
         .. code-block:: python
 
             @op
             def fetch_files_from_slack(context) -> pd.DataFrame:
                 ...
@@ -729,14 +740,16 @@
             key_prefix=key_prefix,
             ins=ins,
             description=description,
             partitions_def=partitions_def,
             group_name=group_name,
             metadata=metadata,
             freshness_policy=freshness_policy,
+            auto_materialize_policy=auto_materialize_policy,
+            resource_defs=resource_defs,
         )(fn)
 
     return inner
 
 
 class _GraphBackedAsset:
     def __init__(
@@ -745,26 +758,30 @@
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         ins: Optional[Mapping[str, AssetIn]] = None,
         description: Optional[str] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         group_name: Optional[str] = None,
         metadata: Optional[MetadataUserInput] = None,
         freshness_policy: Optional[FreshnessPolicy] = None,
+        auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     ):
         self.name = name
 
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
         self.key_prefix = key_prefix
         self.ins = ins or {}
         self.description = description
         self.partitions_def = partitions_def
         self.group_name = group_name
         self.metadata = metadata
         self.freshness_policy = freshness_policy
+        self.auto_materialize_policy = auto_materialize_policy
+        self.resource_defs = resource_defs
 
     def __call__(self, fn: Callable) -> AssetsDefinition:
         asset_name = self.name or fn.__name__
         asset_ins = build_asset_ins(fn, self.ins or {}, set())
         out_asset_key = AssetKey(list(filter(None, [*(self.key_prefix or []), asset_name])))
 
         keys_by_input_name = {
@@ -786,26 +803,31 @@
             partitions_def=self.partitions_def,
             partition_mappings=partition_mappings if partition_mappings else None,
             group_name=self.group_name,
             metadata_by_output_name={"result": self.metadata} if self.metadata else None,
             freshness_policies_by_output_name={"result": self.freshness_policy}
             if self.freshness_policy
             else None,
+            auto_materialize_policies_by_output_name={"result": self.auto_materialize_policy}
+            if self.auto_materialize_policy
+            else None,
             descriptions_by_output_name={"result": self.description} if self.description else None,
+            resource_defs=self.resource_defs,
         )
 
 
 def graph_multi_asset(
     *,
     outs: Mapping[str, AssetOut],
     name: Optional[str] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     partitions_def: Optional[PartitionsDefinition[object]] = None,
     group_name: Optional[str] = None,
     can_subset: bool = False,
+    resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Create a combined definition of multiple assets that are computed using the same graph of
     ops, and the same upstream assets.
 
     Each argument to the decorated function references an upstream asset that this asset depends on.
     The name of the argument designates the name of the upstream asset.
 
@@ -849,14 +871,21 @@
         # source freshness policies from the AssetOuts (if any)
         freshness_policies_by_output_name = {
             output_name: out.freshness_policy
             for output_name, out in outs.items()
             if isinstance(out, AssetOut) and out.freshness_policy is not None
         }
 
+        # source auto materialize policies from the AssetOuts (if any)
+        auto_materialize_policies_by_output_name = {
+            output_name: out.auto_materialize_policy
+            for output_name, out in outs.items()
+            if isinstance(out, AssetOut) and out.auto_materialize_policy is not None
+        }
+
         # source descriptions from the AssetOuts (if any)
         descriptions_by_output_name = {
             output_name: out.description
             for output_name, out in outs.items()
             if isinstance(out, AssetOut) and out.description is not None
         }
 
@@ -868,15 +897,17 @@
             },
             partitions_def=partitions_def,
             partition_mappings=partition_mappings if partition_mappings else None,
             group_name=group_name,
             can_subset=can_subset,
             metadata_by_output_name=metadata_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
+            auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
             descriptions_by_output_name=descriptions_by_output_name,
+            resource_defs=resource_defs,
         )
 
     return inner
 
 
 def build_asset_outs(asset_outs: Mapping[str, AssetOut]) -> Mapping[AssetKey, Tuple[str, Out]]:
     """Creates a mapping from AssetKey to (name of output, Out object)."""
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import dagster._check as check
 from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError
 
 from ..executor_definition import ExecutorDefinition
 from ..graph_definition import GraphDefinition
+from ..job_definition import JobDefinition
 from ..logger_definition import LoggerDefinition
 from ..partitioned_schedule import UnresolvedPartitionedAssetScheduleDefinition
-from ..pipeline_definition import PipelineDefinition
 from ..repository_definition import (
     VALID_REPOSITORY_DATA_DICT_KEYS,
     CachingRepositoryData,
     PendingRepositoryDefinition,
     PendingRepositoryListDefinition,
     RepositoryData,
     RepositoryDefinition,
@@ -117,15 +117,15 @@
             defer_repository_data = False
             for i, definition in enumerate(_flatten(repository_definitions)):
                 if isinstance(definition, CacheableAssetsDefinition):
                     defer_repository_data = True
                 elif not isinstance(
                     definition,
                     (
-                        PipelineDefinition,
+                        JobDefinition,
                         ScheduleDefinition,
                         UnresolvedPartitionedAssetScheduleDefinition,
                         SensorDefinition,
                         GraphDefinition,
                         AssetGroup,
                         AssetsDefinition,
                         SourceAsset,
@@ -138,15 +138,15 @@
 
             if bad_defns:
                 bad_definitions_str = ", ".join(
                     [f"value of type {type_} at index {i}" for i, type_ in bad_defns]
                 )
                 raise DagsterInvalidDefinitionError(
                     "Bad return value from repository construction function: all elements of list "
-                    "must be of type JobDefinition, GraphDefinition, PipelineDefinition, "
+                    "must be of type JobDefinition, GraphDefinition, "
                     "ScheduleDefinition, SensorDefinition, "
                     "AssetsDefinition, or SourceAsset."
                     f"Got {bad_definitions_str}."
                 )
 
             repository_data = (
                 None
@@ -160,15 +160,15 @@
                 )
             )
 
         elif isinstance(repository_definitions, dict):
             if not set(repository_definitions.keys()).issubset(VALID_REPOSITORY_DATA_DICT_KEYS):
                 raise DagsterInvalidDefinitionError(
                     "Bad return value from repository construction function: dict must not contain "
-                    "keys other than {{'pipelines', 'schedules', 'jobs'}}: found "
+                    "keys other than {{'schedules', 'sensors', 'jobs'}}: found "
                     "{bad_keys}".format(
                         bad_keys=", ".join(
                             [
                                 f"'{key}'"
                                 for key in repository_definitions.keys()
                                 if key not in VALID_REPOSITORY_DATA_DICT_KEYS
                             ]
@@ -250,15 +250,15 @@
     _resource_key_mapping: Optional[Mapping[int, str]] = None,
 ) -> Union[RepositoryDefinition, PendingRepositoryDefinition, _Repository]:
     """Create a repository from the decorated function.
 
     The decorated function should take no arguments and its return value should one of:
 
     1. ``List[Union[JobDefinition, ScheduleDefinition, SensorDefinition]]``.
-    Use this form when you have no need to lazy load pipelines or other definitions. This is the
+    Use this form when you have no need to lazy load jobs or other definitions. This is the
     typical use case.
 
     2. A dict of the form:
 
     .. code-block:: python
 
         {
@@ -355,15 +355,15 @@
             # of files in a bespoke YAML format
             ######################################################################
 
             class ComplexRepositoryData(RepositoryData):
                 def __init__(self, yaml_directory):
                     self._yaml_directory = yaml_directory
 
-                def get_all_pipelines(self):
+                def get_all_jobs(self):
                     return [
                         self._construct_job_def_from_yaml_file(
                           self._yaml_file_for_job_name(file_name)
                         )
                         for file_name in os.listdir(self._yaml_directory)
                     ]
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.2/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.2/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.2/dagster/_core/definitions/definitions_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,14 @@
     check.opt_iterable_param(
         schedules, "schedules", (ScheduleDefinition, UnresolvedPartitionedAssetScheduleDefinition)
     )
     check.opt_iterable_param(sensors, "sensors", SensorDefinition)
     check.opt_iterable_param(jobs, "jobs", (JobDefinition, UnresolvedAssetJobDefinition))
 
     check.opt_inst_param(executor, "executor", (ExecutorDefinition, Executor))
-
     executor_def = (
         executor
         if isinstance(executor, ExecutorDefinition) or executor is None
         else ExecutorDefinition.hardcoded_executor(executor)
     )
 
     # Generate a mapping from each top-level resource instance ID to its resource key
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/dependency.py` & `dagster-1.3.2/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/events.py` & `dagster-1.3.2/dagster/_core/definitions/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,19 +426,19 @@
 UNDEFINED_ASSET_KEY_PATH = ["__undefined__"]
 
 
 class AssetMaterializationSerializer(NamedTupleSerializer):
     # There are old `Materialization` objects in storage. We set the default value for asset key to
     # be `AssetKey(["__undefined__"])` to ensure that we can load these objects, without needing to
     # allow for the construction of new `AssetMaterialization` objects with no defined AssetKey.
-    def before_unpack(self, **raw_dict: Any) -> Any:
+    def before_unpack(self, context, unpacked_dict: Any) -> Any:
         # cover both the case where "asset_key" is not present at all and where it is None
-        if raw_dict.get("asset_key") is None:
-            raw_dict["asset_key"] = {"__class__": "AssetKey", "path": UNDEFINED_ASSET_KEY_PATH}
-        return raw_dict
+        if unpacked_dict.get("asset_key") is None:
+            unpacked_dict["asset_key"] = AssetKey(UNDEFINED_ASSET_KEY_PATH)
+        return unpacked_dict
 
 
 @whitelist_for_serdes(
     old_storage_names={"Materialization"},
     serializer=AssetMaterializationSerializer,
     storage_field_names={"metadata": "metadata_entries"},
     field_serializers={"metadata": MetadataFieldSerializer},
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.2/dagster/_core/definitions/executor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,17 +422,14 @@
     Execution priority can be configured using the ``dagster/priority`` tag via solid/op metadata,
     where the higher the number the higher the priority. 0 is the default and both positive
     and negative numbers can be used.
     """
     return _core_multiprocess_executor_creation(init_context.executor_config)
 
 
-default_executors: Sequence[ExecutorDefinition] = [in_process_executor, multiprocess_executor]
-
-
 def check_cross_process_constraints(init_context: "InitExecutorContext") -> None:
     from dagster._core.executor.init import InitExecutorContext
 
     check.inst_param(init_context, "init_context", InitExecutorContext)
     requirements_lst = init_context.executor_def.get_requirements(init_context.executor_config)
 
     if ExecutorRequirement.RECONSTRUCTABLE_JOB in requirements_lst:
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.2/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.2/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.2/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.2/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.2/dagster/_core/definitions/hook_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,17 @@
                 def a_job():
                     foo(bar())
 
         """
         from ..execution.context.hook import HookContext
         from .graph_definition import GraphDefinition
         from .hook_invocation import hook_invocation_result
-        from .pipeline_definition import PipelineDefinition
+        from .job_definition import JobDefinition
 
-        if len(args) > 0 and isinstance(args[0], (PipelineDefinition, GraphDefinition)):
+        if len(args) > 0 and isinstance(args[0], (JobDefinition, GraphDefinition)):
             # when it decorates a pipeline, we apply this hook to all the solid invocations within
             # the pipeline.
             return args[0].with_hooks({self})
         else:
             if not self.decorated_fn:
                 raise DagsterInvalidInvocationError(
                     "Only hook definitions created using one of the hook decorators can be invoked."
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.2/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/inference.py` & `dagster-1.3.2/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/input.py` & `dagster-1.3.2/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.2/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/job_definition.py` & `dagster-1.3.2/dagster/_core/definitions/job_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from datetime import datetime
 from functools import update_wrapper
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Dict,
+    Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
+    Set,
     Tuple,
     Type,
     Union,
     cast,
 )
 
 from typing_extensions import Self
@@ -34,61 +36,94 @@
     NodeHandle,
     NodeInputHandle,
     NodeInvocation,
     NodeOutput,
 )
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.node_definition import NodeDefinition
+from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition import DynamicPartitionsDefinition
 from dagster._core.definitions.policy import RetryPolicy
+from dagster._core.definitions.resource_requirement import (
+    ResourceRequirement,
+    ensure_requirements_satisfied,
+)
 from dagster._core.definitions.utils import check_valid_name
 from dagster._core.errors import (
     DagsterInvalidConfigError,
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidSubsetError,
+    DagsterInvariantViolationError,
 )
 from dagster._core.selector.subset_selector import (
     AssetSelectionData,
     OpSelectionData,
     SelectionTreeBranch,
     SelectionTreeLeaf,
     parse_op_selection,
 )
 from dagster._core.storage.io_manager import IOManagerDefinition, io_manager
+from dagster._core.storage.tags import MEMOIZED_RUN_TAG
+from dagster._core.types.dagster_type import DagsterType
 from dagster._core.utils import str_format_set
-from dagster._utils.backcompat import deprecation_warning
+from dagster._utils.backcompat import deprecation_warning, experimental_class_warning
 from dagster._utils.merger import merge_dicts
 
 from .asset_layer import AssetLayer, build_asset_selection_job
 from .config import ConfigMapping
-from .dependency import DependencyDefinition, GraphNode
+from .dependency import (
+    DependencyDefinition,
+    DependencyMapping,
+    DependencyStructure,
+    GraphNode,
+    OpNode,
+)
 from .executor_definition import ExecutorDefinition, multi_or_in_process_executor
 from .graph_definition import GraphDefinition, SubselectedGraphDefinition
 from .hook_definition import HookDefinition
 from .logger_definition import LoggerDefinition
-from .metadata import RawMetadataValue
-from .mode import ModeDefinition
+from .metadata import MetadataValue, RawMetadataValue, normalize_metadata
 from .partition import PartitionedConfig, PartitionsDefinition
-from .pipeline_definition import PipelineDefinition
-from .preset import PresetDefinition
 from .resource_definition import ResourceDefinition
 from .run_request import RunRequest
-from .utils import DEFAULT_IO_MANAGER_KEY
+from .utils import DEFAULT_IO_MANAGER_KEY, validate_tags
 from .version_strategy import VersionStrategy
 
 if TYPE_CHECKING:
+    from dagster._config.snap import ConfigSchemaSnapshot
     from dagster._core.definitions.run_config import RunConfig
     from dagster._core.execution.execute_in_process_result import ExecuteInProcessResult
     from dagster._core.execution.resources_init import InitResourceContext
+    from dagster._core.host_representation.pipeline_index import PipelineIndex
     from dagster._core.instance import DagsterInstance
     from dagster._core.snap import PipelineSnapshot
 
+    from .run_config_schema import RunConfigSchema
+
+DEFAULT_EXECUTOR_DEF = multi_or_in_process_executor
+
 
-class JobDefinition(PipelineDefinition):
+class JobDefinition:
+    """Defines a Dagster job."""
+
+    _name: str
+    _graph_def: GraphDefinition
+    _description: Optional[str]
+    _tags: Mapping[str, str]
+    _metadata: Mapping[str, MetadataValue]
+    _current_level_node_defs: Sequence[NodeDefinition]
+    _hook_defs: AbstractSet[HookDefinition]
+    _op_retry_policy: Optional[RetryPolicy]
+    _asset_layer: AssetLayer
+    _resource_requirements: Mapping[str, AbstractSet[str]]
+    _all_node_defs: Mapping[str, NodeDefinition]
+    _cached_run_config_schemas: Dict[str, "RunConfigSchema"]
+    _cached_external_pipeline: Any
+    _version_strategy: VersionStrategy
     _subset_selection_data: Optional[Union[OpSelectionData, AssetSelectionData]]
     input_values: Mapping[str, object]
 
     def __init__(
         self,
         *,
         graph_def: GraphDefinition,
@@ -105,201 +140,387 @@
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         hook_defs: Optional[AbstractSet[HookDefinition]] = None,
         op_retry_policy: Optional[RetryPolicy] = None,
         version_strategy: Optional[VersionStrategy] = None,
         _subset_selection_data: Optional[Union[OpSelectionData, AssetSelectionData]] = None,
         asset_layer: Optional[AssetLayer] = None,
         input_values: Optional[Mapping[str, object]] = None,
-        _executor_def_specified: Optional[bool] = None,
-        _logger_defs_specified: Optional[bool] = None,
-        _preset_defs: Optional[Sequence[PresetDefinition]] = None,
         _was_explicitly_provided_resources: Optional[bool] = None,
     ):
         from dagster._core.definitions.run_config import RunConfig, convert_config_input
-        from dagster._loggers import default_loggers
 
-        check.inst_param(graph_def, "graph_def", GraphDefinition)
-        resource_defs = check.opt_mapping_param(
-            resource_defs, "resource_defs", key_type=str, value_type=ResourceDefinition
-        )
-        # We need to check whether an actual executor/logger def was passed in
-        # before we set a default executor/logger defs. This is so we can
-        # determine if someone passed in the default executor vs the system set
-        # it directly. Once JobDefinition no longer subclasses
-        # PipelineDefinition, we can change the default executor to be set
-        # elsewhere to avoid the need for this check.
-        self._executor_def_specified = (
-            _executor_def_specified
-            if _executor_def_specified is not None
-            else executor_def is not None
-        )
-        self._logger_defs_specified = (
-            _logger_defs_specified
-            if _logger_defs_specified is not None
-            else logger_defs is not None
-        )
-        executor_def = check.opt_inst_param(
-            executor_def, "executor_def", ExecutorDefinition, default=multi_or_in_process_executor
-        )
-        check.opt_mapping_param(
+        self._graph_def = graph_def
+        self._current_level_node_defs = self._graph_def.node_defs
+        # Recursively explore all nodes in the this pipeline
+        self._all_node_defs = _build_all_node_defs(self._current_level_node_defs)
+        self._asset_layer = check.opt_inst_param(
+            asset_layer, "asset_layer", AssetLayer
+        ) or _infer_asset_layer_from_source_asset_deps(graph_def)
+
+        # validates
+        self._graph_def.get_inputs_must_be_resolved_top_level(self._asset_layer)
+
+        self._name = check_valid_name(check.str_param(name, "name")) if name else graph_def.name
+        self._executor_def = check.opt_inst_param(executor_def, "executor_def", ExecutorDefinition)
+        self._loggers = check.opt_nullable_mapping_param(
             logger_defs,
             "logger_defs",
             key_type=str,
             value_type=LoggerDefinition,
         )
-        logger_defs = logger_defs or default_loggers()
-        name = check_valid_name(check.opt_str_param(name, "name", default=graph_def.name))
 
         config = check.opt_inst_param(
             config, "config", (Mapping, ConfigMapping, PartitionedConfig, RunConfig)
         )
         config = convert_config_input(config)
 
-        description = check.opt_str_param(description, "description")
         partitions_def = check.opt_inst_param(
             partitions_def, "partitions_def", PartitionsDefinition
         )
-        tags = check.opt_mapping_param(tags, "tags", key_type=str)
-        metadata = check.opt_mapping_param(metadata, "metadata", key_type=str)
-        hook_defs = check.opt_set_param(hook_defs, "hook_defs")
-        op_retry_policy = check.opt_inst_param(op_retry_policy, "op_retry_policy", RetryPolicy)
-        version_strategy = check.opt_inst_param(
+        # tags and description can exist on graph as well, but since
+        # same graph may be in multiple pipelines/jobs, keep separate layer
+        self._description = check.opt_str_param(description, "description")
+        self._tags = validate_tags(tags)
+        self._metadata = normalize_metadata(
+            check.opt_mapping_param(metadata, "metadata", key_type=str)
+        )
+        self._hook_defs = check.opt_set_param(hook_defs, "hook_defs")
+        self._op_retry_policy = check.opt_inst_param(
+            op_retry_policy, "op_retry_policy", RetryPolicy
+        )
+        self.version_strategy = check.opt_inst_param(
             version_strategy, "version_strategy", VersionStrategy
         )
+        if self.version_strategy is not None:
+            experimental_class_warning("VersionStrategy")
+
         _subset_selection_data = check.opt_inst_param(
             _subset_selection_data, "_subset_selection_data", (OpSelectionData, AssetSelectionData)
         )
-        asset_layer = check.opt_inst_param(asset_layer, "asset_layer", AssetLayer)
         input_values = check.opt_mapping_param(input_values, "input_values", key_type=str)
-        _preset_defs = check.opt_sequence_param(
-            _preset_defs, "preset_defs", of_type=PresetDefinition
-        )
 
+        resource_defs = check.opt_mapping_param(
+            resource_defs, "resource_defs", key_type=str, value_type=ResourceDefinition
+        )
+        for key in resource_defs.keys():
+            if not key.isidentifier():
+                check.failed(f"Resource key '{key}' must be a valid Python identifier.")
         was_provided_resources = (
             bool(resource_defs)
             if _was_explicitly_provided_resources is None
             else _was_explicitly_provided_resources
         )
-        if resource_defs and DEFAULT_IO_MANAGER_KEY in resource_defs:
-            resource_defs_with_defaults = resource_defs
-        else:
-            resource_defs_with_defaults = merge_dicts(
-                {DEFAULT_IO_MANAGER_KEY: default_job_io_manager}, resource_defs or {}
-            )
+        self._resource_defs = {
+            DEFAULT_IO_MANAGER_KEY: default_job_io_manager,
+            **resource_defs,
+        }
+        self._required_resource_keys = self._get_required_resource_keys(was_provided_resources)
 
-        presets = []
-        config_mapping = None
-        partitioned_config = None
-        self._explicit_config = False
+        self._config_mapping = None
+        self._partitioned_config = None
+        self._run_config = None
+        self._run_config_schema = None
 
         if partitions_def:
-            partitioned_config = PartitionedConfig.from_flexible_config(config, partitions_def)
+            self._partitioned_config = PartitionedConfig.from_flexible_config(
+                config, partitions_def
+            )
         else:
             if isinstance(config, ConfigMapping):
-                config_mapping = config
+                self._config_mapping = config
             elif isinstance(config, PartitionedConfig):
-                partitioned_config = config
+                self._partitioned_config = config
             elif isinstance(config, dict):
-                check.invariant(
-                    len(_preset_defs) == 0,
-                    (
-                        "Bad state: attempted to pass preset definitions to job alongside config"
-                        " dictionary."
-                    ),
-                )
-                presets = [PresetDefinition(name="default", run_config=config)]
+                self._run_config = config
                 # Using config mapping here is a trick to make it so that the preset will be used even
                 # when no config is supplied for the job.
-                config_mapping = _config_mapping_with_default_value(
+                self._config_mapping = _config_mapping_with_default_value(
                     get_run_config_schema_for_job(
                         graph_def,
-                        resource_defs_with_defaults,
-                        executor_def,
-                        logger_defs,
+                        self.resource_defs,
+                        self.executor_def,
+                        self.loggers,
                         asset_layer,
                         was_explicitly_provided_resources=was_provided_resources,
                     ),
                     config,
-                    name,
+                    self.name,
                 )
-                self._explicit_config = True
             elif config is not None:
                 check.failed(
                     "config param must be a ConfigMapping, a PartitionedConfig, or a dictionary,"
                     f" but is an object of type {type(config)}"
                 )
 
-        # Exists for backcompat - JobDefinition is implemented as a single-mode pipeline.
-        mode_def = ModeDefinition(
-            resource_defs=resource_defs_with_defaults,
-            logger_defs=logger_defs,
-            executor_defs=[executor_def] if executor_def else None,
-            _config_mapping=config_mapping,
-            _partitioned_config=partitioned_config,
-        )
-
         self._subset_selection_data = _subset_selection_data
         self.input_values = input_values
         for input_name in sorted(list(self.input_values.keys())):
             if not graph_def.has_input(input_name):
                 raise DagsterInvalidDefinitionError(
-                    f"Error when constructing JobDefinition '{name}': Input value provided for key"
-                    f" '{input_name}', but job has no top-level input with that name."
+                    f"Error when constructing JobDefinition '{self.name}': Input value provided for"
+                    f" key '{input_name}', but job has no top-level input with that name."
                 )
 
-        super(JobDefinition, self).__init__(
-            name=name,
-            description=description,
-            mode_defs=[mode_def],
-            preset_defs=presets or _preset_defs,
-            tags=tags,
-            metadata=metadata,
-            hook_defs=hook_defs,
-            op_retry_policy=op_retry_policy,
-            graph_def=graph_def,
-            version_strategy=version_strategy,
-            asset_layer=asset_layer or _infer_asset_layer_from_source_asset_deps(graph_def),
-            _should_validate_resource_requirements=was_provided_resources,
-        )
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def tags(self) -> Mapping[str, str]:
+        return merge_dicts(self._graph_def.tags, self._tags)
 
     @property
-    def target_type(self) -> str:
-        return "job"
+    def metadata(self) -> Mapping[str, MetadataValue]:
+        return self._metadata
 
     @property
-    def is_job(self) -> bool:
-        return True
+    def description(self) -> Optional[str]:
+        return self._description
 
-    def describe_target(self):
-        return f"{self.target_type} '{self.name}'"
+    @property
+    def graph(self) -> GraphDefinition:
+        return self._graph_def
+
+    @property
+    def dependency_structure(self) -> DependencyStructure:
+        return self._graph_def.dependency_structure
+
+    @property
+    def dependencies(self) -> DependencyMapping[NodeInvocation]:
+        return self._graph_def.dependencies
 
     @public
     @property
     def executor_def(self) -> ExecutorDefinition:
-        return self.get_mode_definition().executor_defs[0]
+        return self._executor_def or DEFAULT_EXECUTOR_DEF
+
+    @public
+    @property
+    def has_specified_executor(self) -> bool:
+        return self._executor_def is not None
 
     @public
     @property
     def resource_defs(self) -> Mapping[str, ResourceDefinition]:
-        return self.get_mode_definition().resource_defs
+        return self._resource_defs
 
     @public
     @property
     def partitioned_config(self) -> Optional[PartitionedConfig]:
-        return self.get_mode_definition().partitioned_config
+        return self._partitioned_config
 
     @public
     @property
     def config_mapping(self) -> Optional[ConfigMapping]:
-        return self.get_mode_definition().config_mapping
+        return self._config_mapping
 
     @public
     @property
     def loggers(self) -> Mapping[str, LoggerDefinition]:
-        return self.get_mode_definition().loggers
+        from dagster._loggers import default_loggers
+
+        return self._loggers or default_loggers()
+
+    @public
+    @property
+    def has_specified_loggers(self) -> bool:
+        return self._loggers is not None
+
+    @property
+    def required_resource_keys(self) -> AbstractSet[str]:
+        return self._required_resource_keys
+
+    @property
+    def run_config(self) -> Optional[Mapping[str, Any]]:
+        return self._run_config
+
+    @property
+    def run_config_schema(self) -> "RunConfigSchema":
+        if self._run_config_schema is None:
+            self._run_config_schema = _create_run_config_schema(self, self.required_resource_keys)
+        return self._run_config_schema
+
+    @public
+    @property
+    def partitions_def(self) -> Optional[PartitionsDefinition]:
+        return None if not self.partitioned_config else self.partitioned_config.partitions_def
+
+    @property
+    def hook_defs(self) -> AbstractSet[HookDefinition]:
+        return self._hook_defs
+
+    @property
+    def asset_layer(self) -> AssetLayer:
+        return self._asset_layer
+
+    @property
+    def all_node_defs(self) -> Sequence[NodeDefinition]:
+        return list(self._all_node_defs.values())
+
+    @property
+    def top_level_node_defs(self) -> Sequence[NodeDefinition]:
+        return self._current_level_node_defs
+
+    def node_def_named(self, name: str) -> NodeDefinition:
+        check.str_param(name, "name")
+
+        check.invariant(name in self._all_node_defs, f"{name} not found")
+        return self._all_node_defs[name]
+
+    def has_node(self, name: str) -> bool:
+        check.str_param(name, "name")
+        return name in self._all_node_defs
+
+    def get_node(self, handle: NodeHandle) -> Node:
+        return self._graph_def.get_node(handle)
+
+    def get_op(self, handle: NodeHandle) -> OpNode:
+        node = self.get_node(handle)
+        assert isinstance(
+            node, OpNode
+        ), f"Tried to retrieve node {handle} as op, but it represents a nested graph."
+        return node
+
+    def has_node_named(self, name: str) -> bool:
+        return self._graph_def.has_node_named(name)
+
+    def get_node_named(self, name: str) -> Node:
+        return self._graph_def.node_named(name)
+
+    @property
+    def nodes(self) -> Sequence[Node]:
+        return self._graph_def.nodes
+
+    @property
+    def nodes_in_topological_order(self) -> Sequence[Node]:
+        return self._graph_def.nodes_in_topological_order
+
+    def all_dagster_types(self) -> Iterable[DagsterType]:
+        return self._graph_def.all_dagster_types()
+
+    def has_dagster_type(self, name: str) -> bool:
+        return self._graph_def.has_dagster_type(name)
+
+    def dagster_type_named(self, name: str) -> DagsterType:
+        return self._graph_def.dagster_type_named(name)
+
+    def describe_target(self) -> str:
+        return f"job '{self.name}'"
+
+    def is_using_memoization(self, run_tags: Mapping[str, str]) -> bool:
+        tags = merge_dicts(self.tags, run_tags)
+        # If someone provides a false value for memoized run tag, then they are intentionally
+        # switching off memoization.
+        if tags.get(MEMOIZED_RUN_TAG) == "false":
+            return False
+        return (
+            MEMOIZED_RUN_TAG in tags and tags.get(MEMOIZED_RUN_TAG) == "true"
+        ) or self.version_strategy is not None
+
+    def get_required_resource_defs(self) -> Mapping[str, ResourceDefinition]:
+        return {
+            resource_key: resource
+            for resource_key, resource in self.resource_defs.items()
+            if resource_key in self.required_resource_keys
+        }
+
+    def _get_required_resource_keys(self, validate_requirements: bool = False) -> AbstractSet[str]:
+        from ..execution.resources_init import get_transitive_required_resource_keys
+
+        requirements = self._get_resource_requirements()
+        if validate_requirements:
+            ensure_requirements_satisfied(self.resource_defs, requirements)
+        required_keys = {req.key for req in requirements}
+        if validate_requirements:
+            return required_keys.union(
+                get_transitive_required_resource_keys(required_keys, self.resource_defs)
+            )
+        else:
+            return required_keys
+
+    def _get_resource_requirements(self) -> Sequence[ResourceRequirement]:
+        return [
+            *self._graph_def.get_resource_requirements(self.asset_layer),
+            *[
+                req
+                for hook_def in self._hook_defs
+                for req in hook_def.get_resource_requirements(outer_context=f"job '{self._name}'")
+            ],
+        ]
+
+    def validate_resource_requirements_satisfied(self) -> None:
+        resource_requirements = self._get_resource_requirements()
+        ensure_requirements_satisfied(self.resource_defs, resource_requirements)
+
+    def is_missing_required_resources(self) -> bool:
+        requirements = self._get_resource_requirements()
+        for requirement in requirements:
+            if not requirement.resources_contain_key(self.resource_defs):
+                return True
+        return False
+
+    def get_all_hooks_for_handle(self, handle: NodeHandle) -> AbstractSet[HookDefinition]:
+        """Gather all the hooks for the given node from all places possibly attached with a hook.
+
+        A hook can be attached to any of the following objects
+        * Node (node invocation)
+        * JobDefinition
+
+        Args:
+            handle (NodeHandle): The node's handle
+
+        Returns:
+            FrozenSet[HookDefinition]
+        """
+        check.inst_param(handle, "handle", NodeHandle)
+        hook_defs: Set[HookDefinition] = set()
+
+        current = handle
+        lineage = []
+        while current:
+            lineage.append(current.name)
+            current = current.parent
+
+        # hooks on top-level node
+        name = lineage.pop()
+        node = self._graph_def.node_named(name)
+        hook_defs = hook_defs.union(node.hook_defs)
+
+        # hooks on non-top-level nodes
+        while lineage:
+            name = lineage.pop()
+            # While lineage is non-empty, definition is guaranteed to be a graph
+            definition = cast(GraphDefinition, node.definition)
+            node = definition.node_named(name)
+            hook_defs = hook_defs.union(node.hook_defs)
+
+        # hooks applied to a pipeline definition will run on every node
+        hook_defs = hook_defs.union(self.hook_defs)
+
+        return frozenset(hook_defs)
+
+    def get_retry_policy_for_handle(self, handle: NodeHandle) -> Optional[RetryPolicy]:
+        node = self.get_node(handle)
+        definition = node.definition
+
+        if node.retry_policy:
+            return node.retry_policy
+        elif isinstance(definition, OpDefinition) and definition.retry_policy:
+            return definition.retry_policy
+
+        # could be expanded to look in graph containers
+        else:
+            return self._op_retry_policy
+
+    # make Callable for decorator reference updates
+    def __call__(self, *args, **kwargs):
+        raise DagsterInvariantViolationError(
+            f"Attempted to call job '{self.name}' directly. Jobs should be invoked by "
+            "using an execution API function (e.g. `job.execute_in_process`)."
+        )
 
     @public
     def execute_in_process(
         self,
         run_config: Optional[Union[Mapping[str, Any], "RunConfig"]] = None,
         instance: Optional["DagsterInstance"] = None,
         partition_key: Optional[str] = None,
@@ -370,31 +591,27 @@
 
         # Combine provided input values at execute_in_process with input values
         # provided to the definition. Input values provided at
         # execute_in_process will override those provided on the definition.
         input_values = merge_dicts(self.input_values, input_values)
 
         bound_resource_defs = dict(self.resource_defs)
-        logger_defs = dict(self.loggers)
         ephemeral_job = JobDefinition(
             name=self._name,
             graph_def=self._graph_def,
             resource_defs={**_swap_default_io_man(bound_resource_defs, self), **resource_defs},
             executor_def=execute_in_process_executor,
-            logger_defs=logger_defs,
+            logger_defs=self._loggers,
             hook_defs=self.hook_defs,
-            config=self.config_mapping or self.partitioned_config,
+            config=self.config_mapping or self.partitioned_config or self.run_config,
             tags=self.tags,
             op_retry_policy=self._op_retry_policy,
             version_strategy=self.version_strategy,
             asset_layer=self.asset_layer,
             input_values=input_values,
-            _executor_def_specified=self._executor_def_specified,
-            _logger_defs_specified=self._logger_defs_specified,
-            _preset_defs=self._preset_defs,
         )
 
         ephemeral_job = ephemeral_job.get_job_def_for_subset_selection(
             op_selection, frozenset(asset_selection) if asset_selection else None
         )
 
         merged_tags = merge_dicts(self.tags, tags or {})
@@ -440,17 +657,15 @@
             self._subset_selection_data
             if isinstance(self._subset_selection_data, AssetSelectionData)
             else None
         )
 
     @property
     def is_subset_pipeline(self) -> bool:
-        if self._subset_selection_data:
-            return True
-        return False
+        return bool(self._subset_selection_data)
 
     def get_job_def_for_subset_selection(
         self,
         op_selection: Optional[Sequence[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ) -> Self:
         check.invariant(
@@ -509,88 +724,59 @@
             tags=self.tags,
             asset_selection=asset_selection,
             asset_selection_data=asset_selection_data,
             config=self.config_mapping or self.partitioned_config,
         )
         return new_job
 
-    def _get_job_def_for_op_selection(
-        self,
-        op_selection: Optional[Sequence[str]] = None,
-    ) -> Self:
-        if not op_selection:
-            return self
-
-        op_selection = check.opt_sequence_param(op_selection, "op_selection", str)
-
+    def _get_job_def_for_op_selection(self, op_selection: Sequence[str]) -> Self:
         resolved_op_selection_dict = parse_op_selection(self, op_selection)
 
         try:
             sub_graph = get_subselected_graph_definition(self.graph, resolved_op_selection_dict)
 
             # if explicit config was passed the config_mapping that resolves the defaults implicitly is
-            # very unlikely to work. The preset will still present the default config in dagit.
-            if self._explicit_config:
-                config_arg = None
-            else:
-                config_arg = self.config_mapping or self.partitioned_config
+            # very unlikely to work. The job will still present the default config in dagit.
+            config = (
+                None
+                if self.run_config is not None
+                else self.config_mapping or self.partitioned_config
+            )
 
-            return JobDefinition(
-                name=self.name,
-                description=self.description,
-                resource_defs=dict(self.resource_defs),
-                logger_defs=dict(self.loggers),
-                executor_def=self.executor_def,
-                config=config_arg,
-                tags=self.tags,
-                hook_defs=self.hook_defs,
-                op_retry_policy=self._op_retry_policy,
+            return self._copy(
+                config=config,
                 graph_def=sub_graph,
-                version_strategy=self.version_strategy,
-                _executor_def_specified=self._executor_def_specified,
-                _logger_defs_specified=self._logger_defs_specified,
                 _subset_selection_data=OpSelectionData(
                     op_selection=op_selection,
                     resolved_op_selection=set(
                         resolved_op_selection_dict.keys()
                     ),  # equivalent to solids_to_execute. currently only gets top level nodes.
                     parent_job_def=self,  # used by pipeline snapshot lineage
                 ),
                 # TODO: subset this structure.
                 # https://github.com/dagster-io/dagster/issues/7541
                 asset_layer=self.asset_layer,
-                _preset_defs=self._preset_defs,
             )
         except DagsterInvalidDefinitionError as exc:
             # This handles the case when you construct a subset such that an unsatisfied
             # input cannot be loaded from config. Instead of throwing a DagsterInvalidDefinitionError,
             # we re-raise a DagsterInvalidSubsetError.
             raise DagsterInvalidSubsetError(
                 f"The attempted subset {str_format_set(resolved_op_selection_dict)} for graph "
                 f"{self.graph.name} results in an invalid graph."
             ) from exc
 
     @public
-    @property
-    def partitions_def(self) -> Optional[PartitionsDefinition]:
-        mode = self.get_mode_definition()
-        if not mode.partitioned_config:
-            return None
-
-        return mode.partitioned_config.partitions_def
-
-    @public
     def run_request_for_partition(
         self,
         partition_key: str,
         run_key: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
         asset_selection: Optional[Sequence[AssetKey]] = None,
         run_config: Optional[Mapping[str, Any]] = None,
-        instance: Optional["DagsterInstance"] = None,
         current_time: Optional[datetime] = None,
     ) -> RunRequest:
         """Creates a RunRequest object for a run that processes the given partition.
 
         Args:
             partition_key: The key of the partition to request a run for.
             run_key (Optional[str]): A string key to identify this launched run. For sensors, ensures that
@@ -616,119 +802,68 @@
 
         if not (self.partitions_def and self.partitioned_config):
             check.failed("Called run_request_for_partition on a non-partitioned job")
 
         if (
             isinstance(self.partitions_def, DynamicPartitionsDefinition)
             and self.partitions_def.name
-            and not instance
         ):
+            # Do not support using run_request_for_partition with dynamic partitions,
+            # since this requires querying the instance once per run request for the
+            # existent dynamic partitions
             check.failed(
-                "Must provide a dagster instance when calling run_request_for_partition on a "
-                "dynamic partition set"
+                "run_request_for_partition is not supported for dynamic partitions. Instead, use"
+                " RunRequest(partition_key=...)"
             )
 
         partition = self.partitions_def.get_partition(
-            partition_key, dynamic_partitions_store=instance, current_time=current_time
+            partition_key, dynamic_partitions_store=None, current_time=current_time
         )
         run_config = (
             run_config
             if run_config is not None
             else self.partitioned_config.get_run_config_for_partition_key(
-                partition.name, dynamic_partitions_store=instance, current_time=current_time
+                partition.name, dynamic_partitions_store=None, current_time=current_time
             )
         )
         run_request_tags = {
             **(tags or {}),
             **self.partitioned_config.get_tags_for_partition_key(
                 partition_key,
-                dynamic_partitions_store=instance,
+                dynamic_partitions_store=None,
                 current_time=current_time,
                 job_name=self.name,
             ),
         }
 
         return RunRequest(
             run_key=run_key,
             run_config=run_config,
             tags=run_request_tags,
             job_name=self.name,
             asset_selection=asset_selection,
             partition_key=partition_key,
         )
 
-    @public
-    def with_hooks(self, hook_defs: AbstractSet[HookDefinition]) -> "JobDefinition":
-        """Apply a set of hooks to all op instances within the job."""
-        hook_defs = check.set_param(hook_defs, "hook_defs", of_type=HookDefinition)
+    def get_config_schema_snapshot(self) -> "ConfigSchemaSnapshot":
+        return self.get_pipeline_snapshot().config_schema_snapshot
 
-        job_def = JobDefinition(
-            name=self.name,
-            graph_def=self._graph_def,
-            resource_defs=dict(self.resource_defs),
-            logger_defs=dict(self.loggers),
-            executor_def=self.executor_def,
-            config=self.partitioned_config or self.config_mapping,
-            tags=self.tags,
-            hook_defs=hook_defs | self.hook_defs,
-            description=self._description,
-            op_retry_policy=self._op_retry_policy,
-            asset_layer=self.asset_layer,
-            _subset_selection_data=self._subset_selection_data,
-            _executor_def_specified=self._executor_def_specified,
-            _logger_defs_specified=self._logger_defs_specified,
-            _preset_defs=self._preset_defs,
-        )
-
-        update_wrapper(job_def, self, updated=())
+    def get_pipeline_snapshot(self) -> "PipelineSnapshot":
+        return self.get_pipeline_index().pipeline_snapshot
 
-        return job_def
+    def get_pipeline_index(self) -> "PipelineIndex":
+        from dagster._core.host_representation import PipelineIndex
+        from dagster._core.snap import PipelineSnapshot
 
-    @public
-    def with_top_level_resources(
-        self, resource_defs: Mapping[str, ResourceDefinition]
-    ) -> "JobDefinition":
-        """Apply a set of resources to all op instances within the job."""
-        resource_defs = check.dict_param(resource_defs, "resource_defs", key_type=str)
-
-        merged_resource_defs = {
-            **resource_defs,
-            **self.resource_defs,
-        }
-
-        # If we are using the default io_manager, we want to replace it with the one
-        # provided at the top level
-        if (
-            "io_manager" in resource_defs
-            and self.resource_defs.get("io_manager") == default_job_io_manager
-        ):
-            merged_resource_defs["io_manager"] = resource_defs["io_manager"]
-
-        job_def = JobDefinition(
-            name=self._name,
-            graph_def=self._graph_def,
-            resource_defs=merged_resource_defs,
-            logger_defs=dict(self.loggers),
-            executor_def=self.executor_def,
-            config=self.partitioned_config or self.config_mapping,
-            description=self._description,
-            tags=self._tags,
-            hook_defs=self._hook_defs,
-            version_strategy=self.version_strategy,
-            _subset_selection_data=self._subset_selection_data,
-            asset_layer=self._asset_layer,
-            metadata=self._metadata,
-            _executor_def_specified=self._executor_def_specified,
-            _logger_defs_specified=self._logger_defs_specified,
-            _preset_defs=self._preset_defs,
+        return PipelineIndex(
+            PipelineSnapshot.from_pipeline_def(self), self.get_parent_pipeline_snapshot()
         )
 
-        update_wrapper(job_def, self, updated=())
-
-        return job_def
+    def get_pipeline_snapshot_id(self) -> str:
+        return self.get_pipeline_index().pipeline_snapshot_id
 
     def get_parent_pipeline_snapshot(self) -> Optional["PipelineSnapshot"]:
         if self.op_selection_data:
             return self.op_selection_data.parent_job_def.get_pipeline_snapshot()
         elif self.asset_selection_data:
             return self.asset_selection_data.parent_job_def.get_pipeline_snapshot()
         else:
@@ -742,60 +877,60 @@
             raise DagsterInvalidInvocationError(
                 f"On job '{self.name}', attempted to retrieve input value for input named"
                 f" '{input_name}', but no value was provided. Provided input values:"
                 f" {sorted(list(self.input_values.keys()))}"
             )
         return self.input_values[input_name]
 
-    def with_executor_def(self, executor_def: ExecutorDefinition) -> "JobDefinition":
-        return JobDefinition(
+    def _copy(self, **kwargs: Any) -> "JobDefinition":
+        # dict() calls copy dict props
+        base_kwargs = dict(
             graph_def=self.graph,
             resource_defs=dict(self.resource_defs),
-            executor_def=executor_def,
-            logger_defs=dict(self.loggers),
-            config=self.config_mapping or self.partitioned_config,
-            name=self.name,
+            executor_def=self._executor_def,
+            logger_defs=self._loggers,
+            config=self._config_mapping or self._partitioned_config or self._run_config,
+            name=self._name,
             description=self.description,
             tags=self.tags,
             metadata=self._metadata,
             hook_defs=self.hook_defs,
             op_retry_policy=self._op_retry_policy,
             version_strategy=self.version_strategy,
             _subset_selection_data=self._subset_selection_data,
             asset_layer=self.asset_layer,
             input_values=self.input_values,
-            _executor_def_specified=False,
-            _logger_defs_specified=self._logger_defs_specified,
-            _preset_defs=self._preset_defs,
         )
+        resolved_kwargs = {**base_kwargs, **kwargs}  # base kwargs overwritten for conflicts
+        job_def = JobDefinition(**resolved_kwargs)
+        update_wrapper(job_def, self, updated=())
+        return job_def
+
+    @public
+    def with_top_level_resources(
+        self, resource_defs: Mapping[str, ResourceDefinition]
+    ) -> "JobDefinition":
+        """Apply a set of resources to all op instances within the job."""
+        resource_defs = check.mapping_param(resource_defs, "resource_defs", key_type=str)
+        return self._copy(resource_defs=resource_defs)
+
+    @public
+    def with_hooks(self, hook_defs: AbstractSet[HookDefinition]) -> "JobDefinition":
+        """Apply a set of hooks to all op instances within the job."""
+        hook_defs = check.set_param(hook_defs, "hook_defs", of_type=HookDefinition)
+        return self._copy(hook_defs=(hook_defs | self.hook_defs))
+
+    def with_executor_def(self, executor_def: ExecutorDefinition) -> "JobDefinition":
+        return self._copy(executor_def=executor_def)
 
     def with_logger_defs(self, logger_defs: Mapping[str, LoggerDefinition]) -> "JobDefinition":
-        return JobDefinition(
-            graph_def=self.graph,
-            resource_defs=dict(self.resource_defs),
-            executor_def=self.executor_def,
-            logger_defs=logger_defs,
-            config=self.config_mapping or self.partitioned_config,
-            name=self.name,
-            description=self.description,
-            tags=self.tags,
-            metadata=self._metadata,
-            hook_defs=self.hook_defs,
-            op_retry_policy=self._op_retry_policy,
-            version_strategy=self.version_strategy,
-            _subset_selection_data=self._subset_selection_data,
-            asset_layer=self.asset_layer,
-            input_values=self.input_values,
-            _executor_def_specified=self._executor_def_specified,
-            _logger_defs_specified=False,
-            _preset_defs=self._preset_defs,
-        )
+        return self._copy(logger_defs=logger_defs)
 
 
-def _swap_default_io_man(resources: Mapping[str, ResourceDefinition], job: PipelineDefinition):
+def _swap_default_io_man(resources: Mapping[str, ResourceDefinition], job: JobDefinition):
     """Used to create the user facing experience of the default io_manager
     switching to in-memory when using execute_in_process.
     """
     from dagster._core.storage.mem_io_manager import mem_io_manager
 
     if (
         resources.get(DEFAULT_IO_MANAGER_KEY) in [default_job_io_manager]
@@ -910,21 +1045,14 @@
         dependencies=deps,
         node_defs=[definition for _, definition in selected_nodes],
         input_mappings=new_input_mappings,
         output_mappings=new_output_mappings,
     )
 
 
-def get_direct_input_values_from_job(target: PipelineDefinition) -> Mapping[str, Any]:
-    if target.is_job:
-        return cast(JobDefinition, target).input_values
-    else:
-        return {}
-
-
 @io_manager(
     description="Built-in filesystem IO manager that stores and retrieves values using pickling."
 )
 def default_job_io_manager(init_context: "InitResourceContext"):
     # support overriding the default io manager via environment variables
     module_name = os.getenv("DAGSTER_DEFAULT_IO_MANAGER_MODULE")
     attribute_name = os.getenv("DAGSTER_DEFAULT_IO_MANAGER_ATTRIBUTE")
@@ -1059,27 +1187,23 @@
     graph_def: GraphDefinition,
     resource_defs: Mapping[str, ResourceDefinition],
     executor_def: "ExecutorDefinition",
     logger_defs: Mapping[str, LoggerDefinition],
     asset_layer: Optional[AssetLayer],
     was_explicitly_provided_resources: bool = False,
 ) -> ConfigType:
-    return (
-        JobDefinition(
-            name=graph_def.name,
-            graph_def=graph_def,
-            resource_defs=resource_defs,
-            executor_def=executor_def,
-            logger_defs=logger_defs,
-            asset_layer=asset_layer,
-            _was_explicitly_provided_resources=was_explicitly_provided_resources,
-        )
-        .get_run_config_schema("default")
-        .run_config_schema_type
-    )
+    return JobDefinition(
+        name=graph_def.name,
+        graph_def=graph_def,
+        resource_defs=resource_defs,
+        executor_def=executor_def,
+        logger_defs=logger_defs,
+        asset_layer=asset_layer,
+        _was_explicitly_provided_resources=was_explicitly_provided_resources,
+    ).run_config_schema.run_config_schema_type
 
 
 def _infer_asset_layer_from_source_asset_deps(job_graph_def: GraphDefinition) -> AssetLayer:
     """For non-asset jobs that have some inputs that are fed from SourceAssets, constructs an
     AssetLayer that includes those SourceAssets.
     """
     asset_keys_by_node_input_handle: Dict[NodeInputHandle, AssetKey] = {}
@@ -1121,7 +1245,90 @@
         dependency_node_handles_by_asset_key={},
         assets_defs=[],
         source_asset_defs=source_assets_list,
         io_manager_keys_by_asset_key=io_manager_keys_by_asset_key,
         node_output_handles_to_dep_asset_keys={},
         partition_mappings_by_asset_dep={},
     )
+
+
+def _build_all_node_defs(node_defs: Sequence[NodeDefinition]) -> Mapping[str, NodeDefinition]:
+    all_defs: Dict[str, NodeDefinition] = {}
+    for current_level_node_def in node_defs:
+        for node_def in current_level_node_def.iterate_node_defs():
+            if node_def.name in all_defs:
+                if all_defs[node_def.name] != node_def:
+                    raise DagsterInvalidDefinitionError(
+                        'Detected conflicting node definitions with the same name "{name}"'.format(
+                            name=node_def.name
+                        )
+                    )
+            else:
+                all_defs[node_def.name] = node_def
+
+    return all_defs
+
+
+def _create_run_config_schema(
+    job_def: JobDefinition,
+    required_resources: AbstractSet[str],
+) -> "RunConfigSchema":
+    from .run_config import (
+        RunConfigSchemaCreationData,
+        construct_config_type_dictionary,
+        define_run_config_schema_type,
+    )
+    from .run_config_schema import RunConfigSchema
+
+    # When executing with a subset pipeline, include the missing nodes
+    # from the original pipeline as ignored to allow execution with
+    # run config that is valid for the original
+    ignored_nodes: Sequence[Node] = []
+    if job_def.is_subset_pipeline:
+        if isinstance(job_def.graph, SubselectedGraphDefinition):  # op selection provided
+            ignored_nodes = job_def.graph.get_top_level_omitted_nodes()
+        elif job_def.asset_selection_data:
+            parent_job = job_def
+            while parent_job.asset_selection_data:
+                parent_job = parent_job.asset_selection_data.parent_job_def
+
+            ignored_nodes = [
+                node for node in parent_job.graph.nodes if not job_def.has_node_named(node.name)
+            ]
+    else:
+        ignored_nodes = []
+
+    run_config_schema_type = define_run_config_schema_type(
+        RunConfigSchemaCreationData(
+            pipeline_name=job_def.name,
+            nodes=job_def.graph.nodes,
+            graph_def=job_def.graph,
+            dependency_structure=job_def.graph.dependency_structure,
+            executor_def=job_def.executor_def,
+            resource_defs=job_def.resource_defs,
+            logger_defs=job_def.loggers,
+            ignored_nodes=ignored_nodes,
+            required_resources=required_resources,
+            direct_inputs=job_def.input_values,
+            asset_layer=job_def.asset_layer,
+        )
+    )
+
+    if job_def.config_mapping:
+        outer_config_type = job_def.config_mapping.config_schema.config_type
+    else:
+        outer_config_type = run_config_schema_type
+
+    if outer_config_type is None:
+        check.failed("Unexpected outer_config_type value of None")
+
+    config_type_dict_by_name, config_type_dict_by_key = construct_config_type_dictionary(
+        job_def.all_node_defs,
+        outer_config_type,
+    )
+
+    return RunConfigSchema(
+        run_config_schema_type=run_config_schema_type,
+        config_type_dict_by_name=config_type_dict_by_name,
+        config_type_dict_by_key=config_type_dict_by_key,
+        config_mapping=job_def.config_mapping,
+    )
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.2/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.2/dagster/_core/definitions/logger_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .configurable import AnonymousConfigurableDefinition
 from .definition_config_schema import (
     CoercableToConfigSchema,
     convert_user_facing_definition_config_schema,
 )
 
 if TYPE_CHECKING:
-    from dagster._core.definitions import JobDefinition, PipelineDefinition
+    from dagster._core.definitions import JobDefinition
     from dagster._core.execution.context.logger import InitLoggerContext, UnboundInitLoggerContext
 
     InitLoggerFunction = Callable[[InitLoggerContext], logging.Logger]
 
 
 class LoggerDefinition(AnonymousConfigurableDefinition):
     """Core class for defining loggers.
@@ -154,15 +154,15 @@
         )
 
     return _wrap
 
 
 def build_init_logger_context(
     logger_config: Any = None,
-    pipeline_def: Optional["PipelineDefinition"] = None,
+    pipeline_def: Optional["JobDefinition"] = None,
     job_def: Optional["JobDefinition"] = None,
 ) -> "UnboundInitLoggerContext":
     """Builds logger initialization context from provided parameters.
 
     This function can be used to provide the context argument to the invocation of a logger
     definition.
 
@@ -176,18 +176,18 @@
 
     Examples:
         .. code-block:: python
 
             context = build_init_logger_context()
             logger_to_init(context)
     """
-    from dagster._core.definitions import JobDefinition, PipelineDefinition
+    from dagster._core.definitions import JobDefinition
     from dagster._core.execution.context.logger import UnboundInitLoggerContext
 
-    check.opt_inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    check.opt_inst_param(pipeline_def, "pipeline_def", JobDefinition)
     check.opt_inst_param(job_def, "job_def", JobDefinition)
 
     check.invariant(
         not (pipeline_def and job_def),
         (
             "In build_init_logger_context, you may only specify one of the pipeline_def and job_def"
             " parameters, not both."
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.2/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/materialize.py` & `dagster-1.3.2/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.2/dagster/_core/definitions/metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 import dagster._seven as seven
 from dagster._annotations import PublicAttr, deprecated, experimental, public
 from dagster._core.errors import DagsterInvalidMetadata
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import (
     FieldSerializer,
     PackableValue,
+    UnpackContext,
     WhitelistMap,
     pack_value,
-    unpack_value,
 )
 from dagster._utils.backcompat import (
     canonicalize_backcompat_args,
     deprecation_warning,
 )
 
 from .table import (  # re-exported
@@ -939,29 +939,19 @@
                 "description": None,
             }
             for k, v in metadata_dict.items()
         ]
 
     def unpack(
         self,
-        metadata_entries: List[Mapping[str, Any]],
+        metadata_entries: List["MetadataEntry"],
         whitelist_map: WhitelistMap,
-        descent_path: str,
+        context: UnpackContext,
     ) -> Mapping[str, MetadataValue]:
-        return {
-            e["label"]: unpack_value(
-                e["entry_data"],
-                # MetadataValue itself can't inherit from NamedTuple and so isn't a PackableValue,
-                # but one of its subclasses will always be returned here.
-                as_type=MetadataValue,  # type: ignore
-                whitelist_map=whitelist_map,
-                descent_path=descent_path,
-            )
-            for e in metadata_entries
-        }
+        return {e.label: e.entry_data for e in metadata_entries}
 
 
 T_MetadataValue = TypeVar("T_MetadataValue", bound=MetadataValue, covariant=True)
 
 
 # NOTE: This currently stores value in the `entry_data` NamedTuple attribute. In the next release,
 # we will change the name of the NamedTuple property to `value`, and need to implement custom
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.2/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/mode.py` & `dagster-1.3.2/dagster/_core/execution/with_resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,107 @@
-from typing import TYPE_CHECKING, Mapping, NamedTuple, Optional, Sequence
+from typing import Any, Iterable, List, Mapping, Optional, Sequence, TypeVar, cast
 
-import dagster._check as check
-from dagster._core.definitions.executor_definition import ExecutorDefinition, default_executors
-from dagster._loggers import default_loggers
+from dagster import _check as check
+from dagster._core.execution.build_resources import wrap_resources_for_execution
 from dagster._utils.merger import merge_dicts
 
-from .config import ConfigMapping
-from .logger_definition import LoggerDefinition
-from .resource_definition import ResourceDefinition
-from .utils import DEFAULT_IO_MANAGER_KEY, check_valid_name
-
-DEFAULT_MODE_NAME = "default"
-
-if TYPE_CHECKING:
-    from .partition import PartitionedConfig
-
-
-class ModeDefinition(
-    NamedTuple(
-        "_ModeDefinition",
-        [
-            ("name", str),
-            ("resource_defs", Mapping[str, ResourceDefinition]),
-            ("loggers", Mapping[str, LoggerDefinition]),
-            ("executor_defs", Sequence[ExecutorDefinition]),
-            ("description", Optional[str]),
-            ("config_mapping", Optional[ConfigMapping]),
-            ("partitioned_config", Optional["PartitionedConfig"]),
-        ],
-    )
-):
-    """Define a mode in which a pipeline can operate.
-
-    A mode provides pipelines with a set of resource implementations, loggers, system storages,
-    and executors.
+from ..._config import Shape
+from ..definitions.resource_requirement import ResourceAddable
+from ..definitions.utils import DEFAULT_IO_MANAGER_KEY
+from ..errors import DagsterInvalidConfigError, DagsterInvalidInvocationError
+
+T = TypeVar("T", bound=ResourceAddable)
+
+
+def with_resources(
+    definitions: Iterable[T],
+    resource_defs: Mapping[str, object],
+    resource_config_by_key: Optional[Mapping[str, Any]] = None,
+) -> Sequence[T]:
+    """Adds dagster resources to copies of resource-requiring dagster definitions.
+
+    An error will be thrown if any provided definitions have a conflicting
+    resource definition provided for a key provided to resource_defs. Resource
+    config can be provided, with keys in the config dictionary corresponding to
+    the keys for each resource definition. If any definition has unsatisfied
+    resource keys after applying with_resources, an error will be thrown.
 
     Args:
-        name (Optional[str]): The name of the mode. Must be unique within the
-            :py:class:`PipelineDefinition` to which the mode is attached. (default: "default").
-        resource_defs (Optional[Mapping [str, ResourceDefinition]]): A dictionary of string resource
-            keys to their implementations. Individual solids may require resources to be present by
-            these keys.
-        logger_defs (Optional[Dict[str, LoggerDefinition]]): A dictionary of string logger
-            identifiers to their implementations.
-        executor_defs (Optional[List[ExecutorDefinition]]): The set of executors available when
-            executing in this mode. By default, this will be the 'in_process' and 'multiprocess'
-            executors (:py:data:`~dagster.default_executors`).
-        description (Optional[str]): A human-readable description of the mode.
-        _config_mapping (Optional[ConfigMapping]): Only for internal use.
-        _partitioned_config (Optional[PartitionedConfig]): Only for internal use.
+        definitions (Iterable[ResourceAddable]): Dagster definitions to provide resources to.
+        resource_defs (Mapping[str, object]):
+            Mapping of resource keys to objects to satisfy
+            resource requirements of provided dagster definitions.
+        resource_config_by_key (Optional[Mapping[str, Any]]):
+            Specifies config for provided resources. The key in this dictionary
+            corresponds to configuring the same key in the resource_defs
+            dictionary.
+
+    Examples:
+        .. code-block:: python
+
+            from dagster import asset, resource, with_resources
+
+            @resource(config_schema={"bar": str})
+            def foo_resource():
+                ...
+
+            @asset(required_resource_keys={"foo"})
+            def asset1(context):
+                foo = context.resources.foo
+                ...
+
+            @asset(required_resource_keys={"foo"})
+            def asset2(context):
+                foo = context.resources.foo
+                ...
+
+            asset1_with_foo, asset2_with_foo = with_resources(
+                [the_asset, other_asset],
+                resource_config_by_key={
+                    "foo": {
+                        "config": {"bar": ...}
+                    }
+                }
+            )
     """
+    from dagster._config import validate_config
+    from dagster._core.definitions.job_definition import (
+        default_job_io_manager_with_fs_io_manager_schema,
+    )
 
-    def __new__(
-        cls,
-        name: Optional[str] = None,
-        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
-        logger_defs: Optional[Mapping[str, LoggerDefinition]] = None,
-        executor_defs: Optional[Sequence[ExecutorDefinition]] = None,
-        description: Optional[str] = None,
-        _config_mapping: Optional[ConfigMapping] = None,
-        _partitioned_config: Optional["PartitionedConfig"] = None,
-    ):
-        from .partition import PartitionedConfig
+    check.mapping_param(resource_defs, "resource_defs")
+    resource_config_by_key = check.opt_mapping_param(
+        resource_config_by_key, "resource_config_by_key"
+    )
 
-        resource_defs = check.opt_mapping_param(
-            resource_defs, "resource_defs", key_type=str, value_type=ResourceDefinition
+    resource_defs = wrap_resources_for_execution(
+        merge_dicts(
+            {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
+            resource_defs,
         )
+    )
 
-        for key in resource_defs:
-            if not key.isidentifier():
-                check.failed(f"Resource key '{key}' must be a valid Python identifier.")
-
-        if resource_defs and DEFAULT_IO_MANAGER_KEY in resource_defs:
-            resource_defs_with_defaults = resource_defs
-        else:
-            from dagster._core.storage.mem_io_manager import mem_io_manager
-
-            resource_defs_with_defaults = merge_dicts(
-                {DEFAULT_IO_MANAGER_KEY: mem_io_manager}, resource_defs or {}
-            )
+    for key, resource_def in resource_defs.items():
+        if key in resource_config_by_key:
+            resource_config = resource_config_by_key[key]
+            if not isinstance(resource_config, dict) or "config" not in resource_config:
+                raise DagsterInvalidInvocationError(
+                    f"Error with config for resource key '{key}': Expected a "
+                    "dictionary of the form {'config': ...}, but received "
+                    f"{str(resource_config)}"
+                )
 
-        return super(ModeDefinition, cls).__new__(
-            cls,
-            name=check_valid_name(name) if name else DEFAULT_MODE_NAME,
-            resource_defs=resource_defs_with_defaults,
-            loggers=(
-                check.opt_mapping_param(
-                    logger_defs, "logger_defs", key_type=str, value_type=LoggerDefinition
+            outer_config_shape = Shape({"config": resource_def.get_config_field()})
+            config_evr = validate_config(outer_config_shape, resource_config)
+            if not config_evr.success:
+                raise DagsterInvalidConfigError(
+                    f"Error when applying config for resource with key '{key}' ",
+                    config_evr.errors,
+                    resource_config,
                 )
-                or default_loggers()
-            ),
-            executor_defs=check.list_param(
-                executor_defs if executor_defs else default_executors,
-                "executor_defs",
-                of_type=ExecutorDefinition,
-            ),
-            description=check.opt_str_param(description, "description"),
-            config_mapping=check.opt_inst_param(_config_mapping, "_config_mapping", ConfigMapping),
-            partitioned_config=check.opt_inst_param(
-                _partitioned_config, "_partitioned_config", PartitionedConfig
-            ),
-        )
+            resource_defs[key] = resource_defs[key].configured(resource_config["config"])
 
-    @property
-    def resource_key_set(self):
-        return frozenset(self.resource_defs.keys())
-
-    @staticmethod
-    def from_resources(resources, name=None):
-        check.dict_param(resources, "resources", key_type=str)
-
-        return ModeDefinition(
-            name=name,
-            resource_defs={
-                resource_name: ResourceDefinition.hardcoded_resource(resource)
-                for resource_name, resource in resources.items()
-            },
-        )
+    transformed_defs: List[T] = []
+    for definition in definitions:
+        transformed_defs.append(cast(T, definition.with_resources(resource_defs)))
+
+    return transformed_defs
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.2/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.2/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/node_container.py` & `dagster-1.3.2/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/node_definition.py` & `dagster-1.3.2/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/observe.py` & `dagster-1.3.2/dagster/_core/definitions/observe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import warnings
 from typing import TYPE_CHECKING, Any, Mapping, Optional, Sequence
 
 import dagster._check as check
 from dagster._core.definitions.assets_job import build_source_asset_observation_job
 from dagster._core.definitions.definitions_class import Definitions
 from dagster._utils.backcompat import ExperimentalWarning
-from dagster._utils.merger import merge_dicts
 
 from ..instance import DagsterInstance
-from .job_definition import default_job_io_manager_with_fs_io_manager_schema
 from .source_asset import SourceAsset
-from .utils import DEFAULT_IO_MANAGER_KEY
 
 if TYPE_CHECKING:
     from ..execution.execute_in_process_result import ExecuteInProcessResult
 
 
 def observe(
     source_assets: Sequence[SourceAsset],
@@ -41,37 +38,31 @@
             The string partition key that specifies the run config to execute. Can only be used
             to select run config for assets with partitioned config.
         tags (Optional[Mapping[str, str]]): Tags for the run.
 
     Returns:
         ExecuteInProcessResult: The result of the execution.
     """
-    from ..execution.build_resources import wrap_resources_for_execution
-
     source_assets = check.sequence_param(source_assets, "assets", of_type=(SourceAsset))
     instance = check.opt_inst_param(instance, "instance", DagsterInstance)
     partition_key = check.opt_str_param(partition_key, "partition_key")
     resources = check.opt_mapping_param(resources, "resources", key_type=str)
-    resource_defs = wrap_resources_for_execution(resources)
-    resource_defs = merge_dicts(
-        {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema}, resource_defs
-    )
 
     with warnings.catch_warnings():
         warnings.filterwarnings(
             "ignore", category=ExperimentalWarning, message=".*build_source_asset_observation_job.*"
         )
 
         observation_job = build_source_asset_observation_job(
             "in_process_observation_job", source_assets
         )
         defs = Definitions(
             assets=source_assets,
             jobs=[observation_job],
-            resources=resource_defs,
+            resources=resources,
         )
 
         return defs.get_job_def("in_process_observation_job").execute_in_process(
             run_config=run_config,
             instance=instance,
             partition_key=partition_key,
             raise_on_error=raise_on_error,
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/op_definition.py` & `dagster-1.3.2/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.2/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/output.py` & `dagster-1.3.2/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/partition.py` & `dagster-1.3.2/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.2/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.2/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/pipeline_base.py` & `dagster-1.3.2/dagster/_core/definitions/pipeline_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.errors import DagsterInvalidSubsetError
 from dagster._core.selector import parse_solid_selection
 
 if TYPE_CHECKING:
-    from .pipeline_definition import PipelineDefinition
+    from .job_definition import JobDefinition
 
 
 class IPipeline(ABC):
     """IPipeline is a wrapper interface for PipelineDefinitions to be used as parameters to Dagster's
     core execution APIs.  This enables these execution APIs to operate on both in memory pipeline
     definitions to be executed in the current process (InMemoryPipeline) as well as definitions that
     can be reconstructed and executed in a different process (ReconstructablePipeline).
     """
 
     @abstractmethod
-    def get_definition(self) -> "PipelineDefinition":
+    def get_definition(self) -> "JobDefinition":
         pass
 
     @abstractmethod
     def subset_for_execution(
         self,
         solid_selection: Optional[Sequence[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
@@ -49,64 +49,60 @@
     ) -> "IPipeline":
         pass
 
 
 class InMemoryPipeline(IPipeline, object):
     def __init__(
         self,
-        pipeline_def: "PipelineDefinition",
+        pipeline_def: "JobDefinition",
         solid_selection: Optional[Sequence[str]] = None,
         solids_to_execute: Optional[AbstractSet[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ):
         self._pipeline_def = pipeline_def
         self._solid_selection = solid_selection
         self._solids_to_execute = solids_to_execute
         self._asset_selection = asset_selection
 
-    def get_definition(self) -> "PipelineDefinition":
+    def get_definition(self) -> "JobDefinition":
         return self._pipeline_def
 
-    def _resolve_solid_selection(self, solid_selection: Sequence[str]) -> AbstractSet[str]:
-        # resolve a list of solid selection queries to a frozenset of qualified solid names
-        # e.g. ['foo_solid+'] to {'foo_solid', 'bar_solid'}
-        check.list_param(solid_selection, "solid_selection", of_type=str)
-        solids_to_execute = parse_solid_selection(self.get_definition(), solid_selection)
+    def _resolve_op_selection(self, op_selection: Sequence[str]) -> AbstractSet[str]:
+        # resolve a list of op selection queries to a frozenset of qualified op names
+        # e.g. ['foo_op+'] to {'foo_op', 'bar_op'}
+        check.list_param(op_selection, "op_selection", of_type=str)
+        solids_to_execute = parse_solid_selection(self.get_definition(), op_selection)
         if len(solids_to_execute) == 0:
-            node_type = "ops" if self._pipeline_def.is_job else "solids"
-            selection_type = "op_selection" if self._pipeline_def.is_job else "solid_selection"
             raise DagsterInvalidSubsetError(
-                "No qualified {node_type} to execute found for {selection_type}={requested}".format(
-                    node_type=node_type, requested=solid_selection, selection_type=selection_type
-                )
+                f"No qualified ops to execute found for op_selection={op_selection}"
             )
         return solids_to_execute
 
     def _subset_for_execution(
         self,
         solids_to_execute: Optional[AbstractSet[str]],
         solid_selection: Optional[Sequence[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ) -> Self:
         if asset_selection:
             return InMemoryPipeline(
-                self._pipeline_def.get_job_def_for_subset_selection(  # type: ignore  # (must be JobDefinition)
+                self._pipeline_def.get_job_def_for_subset_selection(
                     asset_selection=asset_selection
                 ),
                 asset_selection=asset_selection,
             )
         if self._pipeline_def.is_subset_pipeline:
             return InMemoryPipeline(
                 self._pipeline_def.parent_pipeline_def.get_pipeline_subset_def(solids_to_execute),  # type: ignore  # (possible none)
                 solid_selection=solid_selection,
                 solids_to_execute=solids_to_execute,
             )
 
         return InMemoryPipeline(
-            self._pipeline_def.get_pipeline_subset_def(solids_to_execute),
+            self._pipeline_def.get_pipeline_subset_def(solids_to_execute),  # type: ignore  # (possible none)
             solid_selection=solid_selection,
             solids_to_execute=solids_to_execute,
         )
 
     def subset_for_execution(
         self,
         solid_selection: Optional[Sequence[str]] = None,
@@ -117,17 +113,15 @@
         check.opt_set_param(asset_selection, "asset_selection", of_type=AssetKey)
 
         check.invariant(
             not (solid_selection and asset_selection),
             "solid_selection and asset_selection cannot both be provided as arguments",
         )
 
-        solids_to_execute = (
-            self._resolve_solid_selection(solid_selection) if solid_selection else None
-        )
+        solids_to_execute = self._resolve_op_selection(solid_selection) if solid_selection else None
         return self._subset_for_execution(solids_to_execute, solid_selection, asset_selection)
 
     def subset_for_execution_from_existing_pipeline(
         self,
         solids_to_execute: Optional[AbstractSet[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ) -> Self:
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/policy.py` & `dagster-1.3.2/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.2/dagster/_core/definitions/reconstruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     from dagster._core.definitions.repository_definition import (
         PendingRepositoryDefinition,
         RepositoryLoadData,
     )
 
     from .asset_group import AssetGroup
     from .graph_definition import GraphDefinition
-    from .pipeline_definition import PipelineDefinition
     from .repository_definition import RepositoryDefinition
 
 
 def get_ephemeral_repository_name(pipeline_name: str) -> str:
     check.str_param(pipeline_name, "pipeline_name")
     return f"__repository__{pipeline_name}"
 
@@ -230,15 +229,15 @@
     @property
     def solid_selection(self) -> Optional[Sequence[str]]:
         return seven.json.loads(self.solid_selection_str) if self.solid_selection_str else None
 
     # Keep the most recent 1 definition (globally since this is a NamedTuple method)
     # This allows repeated calls to get_definition in execution paths to not reload the job
     @lru_cache(maxsize=1)
-    def get_definition(self) -> Union[JobDefinition, "PipelineDefinition"]:
+    def get_definition(self) -> Union[JobDefinition, "JobDefinition"]:
         return self.repository.get_definition().get_maybe_subset_job_def(
             self.pipeline_name,
             self.solid_selection,
             self.asset_selection,
             self.solids_to_execute,
         )
 
@@ -254,15 +253,15 @@
         # no selection
         if solid_selection is None and solids_to_execute is None and asset_selection is None:
             return ReconstructablePipeline(
                 repository=self.repository,
                 pipeline_name=self.pipeline_name,
             )
 
-        from dagster._core.definitions import JobDefinition, PipelineDefinition
+        from dagster._core.definitions import JobDefinition
 
         pipeline_def = self.get_definition()
         if isinstance(pipeline_def, JobDefinition):
             # jobs use pre-resolved selection
             # when subselecting a job
             # * job subselection depend on solid_selection rather than solids_to_execute
             # * we'll resolve the op selection later in the stack
@@ -273,15 +272,15 @@
             return ReconstructablePipeline(
                 repository=self.repository,
                 pipeline_name=self.pipeline_name,
                 solid_selection_str=seven.json.dumps(solid_selection) if solid_selection else None,
                 solids_to_execute=None,
                 asset_selection=asset_selection,
             )
-        elif isinstance(pipeline_def, PipelineDefinition):
+        elif isinstance(pipeline_def, JobDefinition):
             # when subselecting a pipeline
             # * pipeline subselection depend on solids_to_excute rather than solid_selection
             # * we resolve a list of solid selection queries to a frozenset of qualified solid names
             #   e.g. ['foo_solid+'] to {'foo_solid', 'bar_solid'}
             if solid_selection and solids_to_execute is None:
                 # when post-resolution query is unavailable, resolve the query
                 solids_to_execute = parse_solid_selection(pipeline_def, solid_selection)
@@ -379,15 +378,15 @@
 
         return None
 
 
 ReconstructableJob = ReconstructablePipeline
 
 
-def reconstructable(target: Callable[..., "PipelineDefinition"]) -> ReconstructablePipeline:
+def reconstructable(target: Callable[..., "JobDefinition"]) -> ReconstructablePipeline:
     """Create a :py:class:`~dagster._core.definitions.reconstructable.ReconstructablePipeline` from a
     function that returns a :py:class:`~dagster.PipelineDefinition`/:py:class:`~dagster.JobDefinition`,
     or a function decorated with :py:func:`@job <dagster.job>`.
 
     When your pipeline/job must cross process boundaries, e.g., for execution on multiple nodes or
     in different systems (like ``dagstermill``), Dagster must know how to reconstruct the pipeline/job
     on the other side of the process boundary.
@@ -435,17 +434,17 @@
                 ...
 
             def make_bar_job():
                 return foo.to_job()
 
             reconstructable_bar_job = reconstructable(make_bar_job)
     """
-    from dagster._core.definitions import JobDefinition, PipelineDefinition
+    from dagster._core.definitions import JobDefinition
 
-    if not seven.is_function_or_decorator_instance_of(target, PipelineDefinition):
+    if not seven.is_function_or_decorator_instance_of(target, JobDefinition):
         if isinstance(target, JobDefinition):
             raise DagsterInvariantViolationError(
                 "Reconstructable target was not a function returning a job definition, or a job "
                 "definition produced by a decorated function. If your job was constructed using "
                 "``GraphDefinition.to_job``, you must wrap the ``to_job`` call in a function at "
                 "module scope, ie not within any other functions. "
                 "To learn more, check out the docs on ``reconstructable``: "
@@ -613,36 +612,36 @@
     return ReconstructablePipeline(
         repository=ReconstructableRepository(pointer),  # creates ephemeral repo
         pipeline_name=pipeline_def.name,
     )
 
 
 LoadableDefinition: TypeAlias = Union[
-    "PipelineDefinition",
+    "JobDefinition",
     "RepositoryDefinition",
     "PendingRepositoryDefinition",
     "GraphDefinition",
     "AssetGroup",
 ]
 
 T_LoadableDefinition = TypeVar("T_LoadableDefinition", bound=LoadableDefinition)
 
 
 def _check_is_loadable(definition: T_LoadableDefinition) -> T_LoadableDefinition:
     from dagster._core.definitions import AssetGroup
 
     from .definitions_class import Definitions
     from .graph_definition import GraphDefinition
-    from .pipeline_definition import PipelineDefinition
+    from .job_definition import JobDefinition
     from .repository_definition import PendingRepositoryDefinition, RepositoryDefinition
 
     if not isinstance(
         definition,
         (
-            PipelineDefinition,
+            JobDefinition,
             RepositoryDefinition,
             PendingRepositoryDefinition,
             GraphDefinition,
             AssetGroup,
             Definitions,
         ),
     ):
@@ -677,23 +676,23 @@
     pointer: CodePointer,
 ) -> LoadableDefinition:
     target = pointer.load_target()
 
     from dagster._core.definitions import AssetGroup
 
     from .graph_definition import GraphDefinition
-    from .pipeline_definition import PipelineDefinition
+    from .job_definition import JobDefinition
     from .repository_definition import PendingRepositoryDefinition, RepositoryDefinition
 
     if isinstance(
         target,
         (
             AssetGroup,
             GraphDefinition,
-            PipelineDefinition,
+            JobDefinition,
             PendingRepositoryDefinition,
             RepositoryDefinition,
         ),
     ) or not callable(target):
         return _check_is_loadable(target)  # type: ignore
 
     # if its a function invoke it - otherwise we are pointing to a
@@ -706,32 +705,32 @@
                 target=pointer.describe()
             )
         )
 
     return _check_is_loadable(target())
 
 
-def pipeline_def_from_pointer(pointer: CodePointer) -> "PipelineDefinition":
-    from .pipeline_definition import PipelineDefinition
+def pipeline_def_from_pointer(pointer: CodePointer) -> "JobDefinition":
+    from .job_definition import JobDefinition
 
     target = def_from_pointer(pointer)
 
-    if isinstance(target, PipelineDefinition):
+    if isinstance(target, JobDefinition):
         return target
 
     raise DagsterInvariantViolationError(
         "CodePointer ({str}) must resolve to a JobDefinition (or PipelineDefinition for legacy"
         " code). Received a {type}".format(str=pointer.describe(), type=type(target))
     )
 
 
 @overload
 # NOTE: mypy can't handle these overloads but pyright can
 def repository_def_from_target_def(
-    target: Union["RepositoryDefinition", "PipelineDefinition", "GraphDefinition", "AssetGroup"],
+    target: Union["RepositoryDefinition", "JobDefinition", "GraphDefinition", "AssetGroup"],
     repository_load_data: Optional["RepositoryLoadData"] = None,
 ) -> "RepositoryDefinition":
     ...
 
 
 @overload
 def repository_def_from_target_def(
@@ -743,28 +742,28 @@
 def repository_def_from_target_def(
     target: object, repository_load_data: Optional["RepositoryLoadData"] = None
 ) -> Optional["RepositoryDefinition"]:
     from dagster._core.definitions import AssetGroup
 
     from .definitions_class import Definitions
     from .graph_definition import GraphDefinition
-    from .pipeline_definition import PipelineDefinition
+    from .job_definition import JobDefinition
     from .repository_definition import (
         SINGLETON_REPOSITORY_NAME,
         CachingRepositoryData,
         PendingRepositoryDefinition,
         RepositoryDefinition,
     )
 
     if isinstance(target, Definitions):
         # reassign to handle both repository and pending repo case
         target = target.get_inner_repository_for_loading_process()
 
     # special case - we can wrap a single pipeline in a repository
-    if isinstance(target, (PipelineDefinition, GraphDefinition)):
+    if isinstance(target, (JobDefinition, GraphDefinition)):
         # consider including pipeline name in generated repo name
         return RepositoryDefinition(
             name=get_ephemeral_repository_name(target.name),
             repository_data=CachingRepositoryData.from_list([target]),
         )
     elif isinstance(target, AssetGroup):
         return RepositoryDefinition(
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.2/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.2/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.2/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 from types import FunctionType
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
     Dict,
-    List,
     Mapping,
     Optional,
     Sequence,
     TypeVar,
     Union,
-    cast,
 )
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.executor_definition import ExecutorDefinition
 from dagster._core.definitions.graph_definition import SubselectedGraphDefinition
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.logger_definition import LoggerDefinition
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.schedule_definition import ScheduleDefinition
 from dagster._core.definitions.sensor_definition import SensorDefinition
 from dagster._core.definitions.source_asset import SourceAsset
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvariantViolationError
 
 from .caching_index import CacheingDefinitionIndex
@@ -44,22 +41,14 @@
     """Users should usually rely on the :py:func:`@repository <repository>` decorator to create new
     repositories, which will in turn call the static constructors on this class. However, users may
     subclass :py:class:`RepositoryData` for fine-grained control over access to and lazy creation
     of repository members.
     """
 
     @abstractmethod
-    def get_all_pipelines(self) -> Sequence[PipelineDefinition]:
-        """Return all pipelines/jobs in the repository as a list.
-
-        Returns:
-            List[PipelineDefinition]: All pipelines/jobs in the repository.
-        """
-
-    @abstractmethod
     def get_resource_key_mapping(self) -> Mapping[int, str]:
         pass
 
     @abstractmethod
     def get_top_level_resources(self) -> Mapping[str, ResourceDefinition]:
         """Return all top-level resources in the repository as a list,
         such as those provided to the Definitions constructor.
@@ -68,81 +57,44 @@
             List[ResourceDefinition]: All top-level resources in the repository.
         """
 
     @abstractmethod
     def get_env_vars_by_top_level_resource(self) -> Mapping[str, AbstractSet[str]]:
         pass
 
+    @abstractmethod
     @public
     def get_all_jobs(self) -> Sequence[JobDefinition]:
         """Return all jobs in the repository as a list.
 
         Returns:
             List[JobDefinition]: All jobs in the repository.
         """
-        return [job for job in self.get_all_pipelines() if isinstance(job, JobDefinition)]
-
-    def get_pipeline_names(self) -> Sequence[str]:
-        """Get the names of all pipelines/jobs in the repository.
-
-        Returns:
-            List[str]
-        """
-        return [pipeline_def.name for pipeline_def in self.get_all_pipelines()]
 
     @public
     def get_job_names(self) -> Sequence[str]:
         """Get the names of all jobs in the repository.
 
         Returns:
             List[str]
         """
         return [job_def.name for job_def in self.get_all_jobs()]
 
-    def has_pipeline(self, pipeline_name: str) -> bool:
-        """Check if a pipeline/job with a given name is present in the repository.
-
-        Args:
-            pipeline_name (str): The name of the pipeline/job.
-
-        Returns:
-            bool
-        """
-        return pipeline_name in self.get_pipeline_names()
-
     @public
     def has_job(self, job_name: str) -> bool:
         """Check if a job with a given name is present in the repository.
 
         Args:
             job_name (str): The name of the job.
 
         Returns:
             bool
         """
         return job_name in self.get_job_names()
 
-    def get_pipeline(self, pipeline_name) -> PipelineDefinition:
-        """Get a pipeline/job by name.
-
-        Args:
-            pipeline_name (str): Name of the pipeline/job to retrieve.
-
-        Returns:
-            PipelineDefinition: The pipeline/job definition corresponding to the given name.
-        """
-        pipelines_with_name = [
-            pipeline for pipeline in self.get_all_pipelines() if pipeline.name == pipeline_name
-        ]
-        if not pipelines_with_name:
-            raise DagsterInvariantViolationError(
-                f"Could not find pipeline/job {pipeline_name} in repository"
-            )
-        return pipelines_with_name[0]
-
     @public
     def get_job(self, job_name: str) -> JobDefinition:
         """Get a job by name.
 
         Args:
             job_name (str): Name of the job to retrieve.
 
@@ -223,31 +175,29 @@
 
     @public
     def get_assets_defs_by_key(self) -> Mapping[AssetKey, "AssetsDefinition"]:
         return {}
 
     def load_all_definitions(self):
         # force load of all lazy constructed code artifacts
-        self.get_all_pipelines()
         self.get_all_jobs()
         self.get_all_schedules()
         self.get_all_sensors()
         self.get_source_assets_by_key()
 
 
 class CachingRepositoryData(RepositoryData):
     """Default implementation of RepositoryData used by the :py:func:`@repository <repository>` decorator.
     """
 
     _all_jobs: Optional[Sequence[JobDefinition]]
-    _all_pipelines: Optional[Sequence[PipelineDefinition]]
+    _all_pipelines: Optional[Sequence[JobDefinition]]
 
     def __init__(
         self,
-        pipelines: Mapping[str, Union[PipelineDefinition, Resolvable[PipelineDefinition]]],
         jobs: Mapping[str, Union[JobDefinition, Resolvable[JobDefinition]]],
         schedules: Mapping[str, Union[ScheduleDefinition, Resolvable[ScheduleDefinition]]],
         sensors: Mapping[str, Union[SensorDefinition, Resolvable[SensorDefinition]]],
         source_assets_by_key: Mapping[AssetKey, SourceAsset],
         assets_defs_by_key: Mapping[AssetKey, "AssetsDefinition"],
         top_level_resources: Mapping[str, ResourceDefinition],
         utilized_env_vars: Mapping[str, AbstractSet[str]],
@@ -261,33 +211,28 @@
         or when constructing the definitions is costly.
 
         Note that when lazily constructing a definition, the name of the definition must match its
         key in its dictionary index, or a :py:class:`DagsterInvariantViolationError` will be thrown
         at retrieval time.
 
         Args:
-            pipelines (Mapping[str, Union[PipelineDefinition, Callable[[], PipelineDefinition]]]):
-                The pipeline definitions belonging to the repository.
             jobs (Mapping[str, Union[JobDefinition, Callable[[], JobDefinition]]]):
                 The job definitions belonging to the repository.
             schedules (Mapping[str, Union[ScheduleDefinition, Callable[[], ScheduleDefinition]]]):
                 The schedules belonging to the repository.
             sensors (Mapping[str, Union[SensorDefinition, Callable[[], SensorDefinition]]]):
                 The sensors belonging to a repository.
             source_assets_by_key (Mapping[AssetKey, SourceAsset]): The source assets belonging to a repository.
             assets_defs_by_key (Mapping[AssetKey, AssetsDefinition]): The assets definitions
                 belonging to a repository.
             top_level_resources (Mapping[str, ResourceDefinition]): A dict of top-level
                 resource keys to defintions, for resources which should be displayed in the UI.
         """
         from dagster._core.definitions import AssetsDefinition
 
-        check.mapping_param(
-            pipelines, "pipelines", key_type=str, value_type=(PipelineDefinition, FunctionType)
-        )
         check.mapping_param(jobs, "jobs", key_type=str, value_type=(JobDefinition, FunctionType))
         check.mapping_param(
             schedules, "schedules", key_type=str, value_type=(ScheduleDefinition, FunctionType)
         )
         check.mapping_param(
             sensors, "sensors", key_type=str, value_type=(SensorDefinition, FunctionType)
         )
@@ -305,22 +250,14 @@
             "utilized_resources",
             key_type=str,
         )
         check.mapping_param(
             resource_key_mapping, "resource_key_mapping", key_type=int, value_type=str
         )
 
-        self._pipelines = CacheingDefinitionIndex(
-            PipelineDefinition,
-            "PipelineDefinition",
-            "pipeline",
-            pipelines,
-            self._validate_pipeline,
-        )
-
         self._jobs = CacheingDefinitionIndex(
             JobDefinition,
             "JobDefinition",
             "job",
             jobs,
             self._validate_job,
         )
@@ -347,26 +284,24 @@
             "sensor",
             sensors,
             self._validate_sensor,
         )
         # load all sensors to force validation
         self._sensors.get_all_definitions()
 
-        self._all_pipelines = None
         self._all_jobs = None
 
     @staticmethod
     def from_dict(repository_definitions: Dict[str, Dict[str, Any]]) -> "CachingRepositoryData":
         """Static constructor.
 
         Args:
             repository_definition (Dict[str, Dict[str, ...]]): A dict of the form:
 
                 {
-                    'pipelines': Dict[str, Callable[[], PipelineDefinition]],
                     'jobs': Dict[str, Callable[[], JobDefinition]],
                     'schedules': Dict[str, Callable[[], ScheduleDefinition]]
                 }
 
             This form is intended to allow definitions to be created lazily when accessed by name,
             which can be helpful for performance when there are many definitions in a repository, or
             when constructing the definitions is costly.
@@ -384,15 +319,15 @@
         top_level_resources: Optional[Mapping[str, ResourceDefinition]] = None,
         resource_key_mapping: Optional[Mapping[int, str]] = None,
     ) -> "CachingRepositoryData":
         """Static constructor.
 
         Args:
             repository_definitions (List[Union[PipelineDefinition, ScheduleDefinition, SensorDefinition, AssetGroup, GraphDefinition]]):
-                Use this constructor when you have no need to lazy load pipelines/jobs or other
+                Use this constructor when you have no need to lazy load jobs or other
                 definitions.
             top_level_resources (Optional[Mapping[str, ResourceDefinition]]): A dict of top-level
                 resource keys to defintions, for resources which should be displayed in the UI.
         """
         from .repository_data_builder import build_caching_repository_data_from_list
 
         return build_caching_repository_data_from_list(
@@ -402,48 +337,25 @@
             top_level_resources=top_level_resources,
             resource_key_mapping=resource_key_mapping,
         )
 
     def get_env_vars_by_top_level_resource(self) -> Mapping[str, AbstractSet[str]]:
         return self._utilized_env_vars
 
-    def get_pipeline_names(self) -> Sequence[str]:
-        """Get the names of all pipelines/jobs in the repository.
-
-        Returns:
-            List[str]
-        """
-        return [*self._pipelines.get_definition_names(), *self.get_job_names()]
-
     def get_resource_key_mapping(self) -> Mapping[int, str]:
         return self._resource_key_mapping
 
     def get_job_names(self) -> Sequence[str]:
         """Get the names of all jobs in the repository.
 
         Returns:
             List[str]
         """
         return self._jobs.get_definition_names()
 
-    def has_pipeline(self, pipeline_name: str) -> bool:
-        """Check if a pipeline/job with a given name is present in the repository.
-
-        Args:
-            pipeline_name (str): The name of the pipeline/job.
-
-        Returns:
-            bool
-        """
-        check.str_param(pipeline_name, "pipeline_name")
-
-        return self._pipelines.has_definition(pipeline_name) or self._jobs.has_definition(
-            pipeline_name
-        )
-
     def has_job(self, job_name: str) -> bool:
         """Check if a job with a given name is present in the repository.
 
         Args:
             job_name (str): The name of the job.
 
         Returns:
@@ -451,71 +363,28 @@
         """
         check.str_param(job_name, "job_name")
         return self._jobs.has_definition(job_name)
 
     def get_top_level_resources(self) -> Mapping[str, ResourceDefinition]:
         return self._top_level_resources
 
-    def get_all_pipelines(self) -> Sequence[PipelineDefinition]:
-        """Return all pipelines/jobs in the repository as a list.
-
-        Note that this will construct any pipeline/job that has not yet been constructed.
-
-        Returns:
-            List[PipelineDefinition]: All pipelines/jobs in the repository.
-        """
-        if self._all_pipelines is not None:
-            return self._all_pipelines
-
-        self._all_jobs = self._jobs.get_all_definitions()
-        pipelines: List[PipelineDefinition] = [
-            *self._pipelines.get_all_definitions(),
-            *self._all_jobs,
-        ]
-        self._check_solid_defs(pipelines)
-        self._all_pipelines = pipelines
-        return self._all_pipelines
-
     def get_all_jobs(self) -> Sequence[JobDefinition]:
         """Return all jobs in the repository as a list.
 
         Note that this will construct any job that has not yet been constructed.
 
         Returns:
-            List[JobDefinition]: All jobs in the repository.
+            List[PipelineDefinition]: All jobs in the repository.
         """
         if self._all_jobs is not None:
             return self._all_jobs
 
-        # _check_solid_defs enforces that pipeline and graph definition names are
-        # unique within a repository. Loads pipelines in the line below to enforce
-        # pipeline/job/graph uniqueness.
-        self.get_all_pipelines()
-
-        # The `get_all_pipelines` call ensures _all_jobs is set.
-        return cast(Sequence[JobDefinition], self._all_jobs)
-
-    def get_pipeline(self, pipeline_name: str) -> PipelineDefinition:
-        """Get a pipeline/job by name.
-
-        If this pipeline/job has not yet been constructed, only this pipeline/job is constructed, and will
-        be cached for future calls.
-
-        Args:
-            pipeline_name (str): Name of the pipeline/job to retrieve.
-
-        Returns:
-            PipelineDefinition: The pipeline/job definition corresponding to the given name.
-        """
-        check.str_param(pipeline_name, "pipeline_name")
-
-        if self._jobs.has_definition(pipeline_name):
-            return self._jobs.get_definition(pipeline_name)
-        else:
-            return self._pipelines.get_definition(pipeline_name)
+        self._all_jobs = self._jobs.get_all_definitions()
+        self._check_node_defs(self._all_jobs)
+        return self._all_jobs
 
     def get_job(self, job_name: str) -> JobDefinition:
         """Get a job by name.
 
         If this job has not yet been constructed, only this job is constructed, and will
         be cached for future calls.
 
@@ -581,63 +450,58 @@
 
     def get_source_assets_by_key(self) -> Mapping[AssetKey, SourceAsset]:
         return self._source_assets_by_key
 
     def get_assets_defs_by_key(self) -> Mapping[AssetKey, "AssetsDefinition"]:
         return self._assets_defs_by_key
 
-    def _check_solid_defs(self, pipelines: Sequence[PipelineDefinition]) -> None:
-        solid_defs = {}
-        solid_to_pipeline = {}
-        for pipeline in pipelines:
-            for solid_def in [*pipeline.all_node_defs, pipeline.graph]:
+    def _check_node_defs(self, job_defs: Sequence[JobDefinition]) -> None:
+        node_defs = {}
+        node_to_job = {}
+        for job_def in job_defs:
+            for node_def in [*job_def.all_node_defs, job_def.graph]:
                 # skip checks for subselected graphs because they don't have their own names
-                if isinstance(solid_def, SubselectedGraphDefinition):
+                if isinstance(node_def, SubselectedGraphDefinition):
                     break
 
-                if solid_def.name not in solid_defs:
-                    solid_defs[solid_def.name] = solid_def
-                    solid_to_pipeline[solid_def.name] = pipeline.name
-
-                if solid_defs[solid_def.name] is not solid_def:
-                    first_name, second_name = sorted(
-                        [solid_to_pipeline[solid_def.name], pipeline.name]
-                    )
+                if node_def.name not in node_defs:
+                    node_defs[node_def.name] = node_def
+                    node_to_job[node_def.name] = job_def.name
+
+                if node_defs[node_def.name] is not node_def:
+                    first_name, second_name = sorted([node_to_job[node_def.name], job_def.name])
                     raise DagsterInvalidDefinitionError(
-                        f"Conflicting definitions found in repository with name '{solid_def.name}'."
+                        f"Conflicting definitions found in repository with name '{node_def.name}'."
                         " Op/Graph definition names must be unique within a repository."
-                        f" {solid_def.__class__.__name__} is defined in"
-                        f" {pipeline.target_type} '{first_name}' and in"
-                        f" {pipeline.target_type} '{second_name}'."
+                        f" {node_def.__class__.__name__} is defined in"
+                        f" job '{first_name}' and in"
+                        f" job '{second_name}'."
                     )
 
-    def _validate_pipeline(self, pipeline: PipelineDefinition) -> PipelineDefinition:
-        return pipeline
-
     def _validate_job(self, job: JobDefinition) -> JobDefinition:
         return job
 
     def _validate_schedule(self, schedule: ScheduleDefinition) -> ScheduleDefinition:
-        pipelines = self.get_pipeline_names()
+        job_names = self.get_job_names()
 
-        if schedule.job_name not in pipelines:
+        if schedule.job_name not in job_names:
             raise DagsterInvalidDefinitionError(
-                f'ScheduleDefinition "{schedule.name}" targets job/pipeline "{schedule.job_name}" '
+                f'ScheduleDefinition "{schedule.name}" targets job "{schedule.job_name}" '
                 "which was not found in this repository."
             )
 
         return schedule
 
     def _validate_sensor(self, sensor: SensorDefinition) -> SensorDefinition:
-        pipelines = self.get_pipeline_names()
+        job_names = self.get_job_names()
         if len(sensor.targets) == 0:
-            # skip validation when the sensor does not target a pipeline
+            # skip validation when the sensor does not target a job
             return sensor
 
         for target in sensor.targets:
-            if target.pipeline_name not in pipelines:
+            if target.pipeline_name not in job_names:
                 raise DagsterInvalidDefinitionError(
-                    f'SensorDefinition "{sensor.name}" targets job/pipeline "{sensor.job_name}" '
+                    f'SensorDefinition "{sensor.name}" targets job "{sensor.job_name}" '
                     "which was not found in this repository."
                 )
 
         return sensor
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.2/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from dagster._core.definitions.executor_definition import ExecutorDefinition
 from dagster._core.definitions.graph_definition import GraphDefinition
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.logger_definition import LoggerDefinition
 from dagster._core.definitions.partitioned_schedule import (
     UnresolvedPartitionedAssetScheduleDefinition,
 )
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.schedule_definition import ScheduleDefinition
 from dagster._core.definitions.sensor_definition import SensorDefinition
 from dagster._core.definitions.source_asset import SourceAsset
 from dagster._core.definitions.unresolved_asset_job_definition import UnresolvedAssetJobDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError
 
@@ -102,42 +101,40 @@
 ) -> CachingRepositoryData:
     from dagster._core.definitions import AssetGroup, AssetsDefinition
     from dagster._core.definitions.partitioned_schedule import (
         UnresolvedPartitionedAssetScheduleDefinition,
     )
 
     schedule_and_sensor_names: Set[str] = set()
-    pipelines_or_jobs: Dict[str, Union[PipelineDefinition, JobDefinition]] = {}
+    jobs: Dict[str, JobDefinition] = {}
     coerced_graphs: Dict[str, JobDefinition] = {}
     unresolved_jobs: Dict[str, UnresolvedAssetJobDefinition] = {}
     schedules: Dict[str, ScheduleDefinition] = {}
     unresolved_partitioned_asset_schedules: Dict[
         str, UnresolvedPartitionedAssetScheduleDefinition
     ] = {}
     sensors: Dict[str, SensorDefinition] = {}
     assets_defs: List[AssetsDefinition] = []
     asset_keys: Set[AssetKey] = set()
     source_assets: List[SourceAsset] = []
     combined_asset_group = None
     for definition in repository_definitions:
-        if isinstance(definition, PipelineDefinition):
+        if isinstance(definition, JobDefinition):
             if (
-                definition.name in pipelines_or_jobs
-                and pipelines_or_jobs[definition.name] != definition
+                definition.name in jobs and jobs[definition.name] != definition
             ) or definition.name in unresolved_jobs:
                 raise DagsterInvalidDefinitionError(
-                    f"Duplicate {definition.target_type} definition found for"
-                    f" {definition.describe_target()}"
+                    f"Duplicate job definition found for {definition.describe_target()}"
                 )
             if is_base_asset_job_name(definition.name):
                 raise DagsterInvalidDefinitionError(
                     f"Attempted to provide job called {definition.name} to repository, which "
                     "is a reserved name. Please rename the job."
                 )
-            pipelines_or_jobs[definition.name] = definition
+            jobs[definition.name] = definition
         elif isinstance(definition, SensorDefinition):
             if definition.name in schedule_and_sensor_names:
                 raise DagsterInvalidDefinitionError(
                     f"Duplicate definition found for {definition.name}"
                 )
             schedule_and_sensor_names.add(definition.name)
             sensors[definition.name] = definition
@@ -156,22 +153,22 @@
                     f"Duplicate definition found for {definition.name}"
                 )
             schedule_and_sensor_names.add(definition.name)
 
             unresolved_partitioned_asset_schedules[definition.name] = definition
         elif isinstance(definition, GraphDefinition):
             coerced = definition.coerce_to_job()
-            if coerced.name in pipelines_or_jobs:
+            if coerced.name in jobs:
                 raise DagsterInvalidDefinitionError(
-                    f"Duplicate {coerced.target_type} definition found for graph '{coerced.name}'"
+                    f"Duplicate job definition found for graph '{coerced.name}'"
                 )
-            pipelines_or_jobs[coerced.name] = coerced
+            jobs[coerced.name] = coerced
             coerced_graphs[coerced.name] = coerced
         elif isinstance(definition, UnresolvedAssetJobDefinition):
-            if definition.name in pipelines_or_jobs or definition.name in unresolved_jobs:
+            if definition.name in jobs or definition.name in unresolved_jobs:
                 raise DagsterInvalidDefinitionError(
                     f"Duplicate definition found for unresolved job '{definition.name}'"
                 )
             # we can only resolve these once we have all assets
             unresolved_jobs[definition.name] = definition
         elif isinstance(definition, AssetGroup):
             if combined_asset_group:
@@ -204,15 +201,15 @@
     if combined_asset_group:
         for job_def in get_base_asset_jobs(
             assets=combined_asset_group.assets,
             source_assets=combined_asset_group.source_assets,
             executor_def=combined_asset_group.executor_def,
             resource_defs=combined_asset_group.resource_defs,
         ):
-            pipelines_or_jobs[job_def.name] = job_def
+            jobs[job_def.name] = job_def
 
         source_assets_by_key = {
             source_asset.key: source_asset for source_asset in combined_asset_group.source_assets
         }
         assets_defs_by_key = {
             key: asset for asset in combined_asset_group.assets for key in asset.keys
         }
@@ -221,22 +218,22 @@
         assets_defs_by_key = {}
 
     for name, sensor_def in sensors.items():
         if sensor_def.has_loadable_targets():
             targets = sensor_def.load_targets()
             for target in targets:
                 _process_and_validate_target(
-                    sensor_def, coerced_graphs, unresolved_jobs, pipelines_or_jobs, target
+                    sensor_def, coerced_graphs, unresolved_jobs, jobs, target
                 )
 
     for name, schedule_def in schedules.items():
         if schedule_def.has_loadable_target():
             target = schedule_def.load_target()
             _process_and_validate_target(
-                schedule_def, coerced_graphs, unresolved_jobs, pipelines_or_jobs, target
+                schedule_def, coerced_graphs, unresolved_jobs, jobs, target
             )
 
     asset_graph = AssetGraph.from_assets(
         [*combined_asset_group.assets, *combined_asset_group.source_assets]
         if combined_asset_group
         else []
     )
@@ -246,70 +243,61 @@
             name,
             unresolved_partitioned_asset_schedule,
         ) in unresolved_partitioned_asset_schedules.items():
             _process_and_validate_target(
                 unresolved_partitioned_asset_schedule,
                 coerced_graphs,
                 unresolved_jobs,
-                pipelines_or_jobs,
+                jobs,
                 unresolved_partitioned_asset_schedule.job,
             )
 
     # resolve all the UnresolvedAssetJobDefinitions using the full set of assets
     if unresolved_jobs:
         for name, unresolved_job_def in unresolved_jobs.items():
             resolved_job = unresolved_job_def.resolve(
                 asset_graph=asset_graph, default_executor_def=default_executor_def
             )
-            pipelines_or_jobs[name] = resolved_job
+            jobs[name] = resolved_job
 
     # resolve all the UnresolvedPartitionedAssetScheduleDefinitions using
     # the resolved job containing the partitions def
     if unresolved_partitioned_asset_schedules:
         for (
             name,
             unresolved_partitioned_asset_schedule,
         ) in unresolved_partitioned_asset_schedules.items():
-            resolved_job = pipelines_or_jobs[unresolved_partitioned_asset_schedule.job.name]
+            resolved_job = jobs[unresolved_partitioned_asset_schedule.job.name]
             schedules[name] = unresolved_partitioned_asset_schedule.resolve(
                 cast(JobDefinition, resolved_job)
             )
 
-    for pipeline_or_job in pipelines_or_jobs.values():
-        pipeline_or_job.validate_resource_requirements_satisfied()
-
-    pipelines: Dict[str, PipelineDefinition] = {}
-    jobs: Dict[str, JobDefinition] = {}
-    for name, pipeline_or_job in pipelines_or_jobs.items():
-        if isinstance(pipeline_or_job, JobDefinition):
-            jobs[name] = pipeline_or_job
-        else:
-            pipelines[name] = pipeline_or_job
+    for job_def in jobs.values():
+        job_def.validate_resource_requirements_satisfied()
 
     if default_executor_def:
         for name, job_def in jobs.items():
-            if not job_def._executor_def_specified:  # noqa: SLF001
+            if not job_def.has_specified_executor:
                 jobs[name] = job_def.with_executor_def(default_executor_def)
 
     if default_logger_defs:
         for name, job_def in jobs.items():
-            if not job_def._logger_defs_specified:  # noqa: SLF001
+            if not job_def.has_specified_loggers:
                 jobs[name] = job_def.with_logger_defs(default_logger_defs)
 
     top_level_resources = top_level_resources or {}
 
     utilized_env_vars: Dict[str, Set[str]] = defaultdict(set)
 
     for resource_key, resource_def in top_level_resources.items():
         used_env_vars = _env_vars_from_resource_defaults(resource_def)
         for env_var in used_env_vars:
             utilized_env_vars[env_var].add(resource_key)
 
     return CachingRepositoryData(
-        pipelines=pipelines,
         jobs=jobs,
         schedules=schedules,
         sensors=sensors,
         source_assets_by_key=source_assets_by_key,
         assets_defs_by_key=assets_defs_by_key,
         top_level_resources=top_level_resources or {},
         utilized_env_vars=utilized_env_vars,
@@ -344,40 +332,34 @@
     )
     if duplicate_keys:
         raise DagsterInvalidDefinitionError(
             "Duplicate definitions between schedules and sensors found for keys:"
             f" {', '.join(duplicate_keys)}"
         )
 
-    # merge jobs in to pipelines while they are just implemented as pipelines
-    for key, job in repository_definitions["jobs"].items():
-        if key in repository_definitions["pipelines"]:
-            raise DagsterInvalidDefinitionError(
-                f'Conflicting entries for name {key} in "jobs" and "pipelines".'
-            )
-
-        if isinstance(job, GraphDefinition):
-            repository_definitions["jobs"][key] = job.coerce_to_job()
-        elif isinstance(job, UnresolvedAssetJobDefinition):
-            repository_definitions["jobs"][key] = job.resolve(
+    for key, raw_job_def in repository_definitions["jobs"].items():
+        if isinstance(raw_job_def, GraphDefinition):
+            repository_definitions["jobs"][key] = raw_job_def.coerce_to_job()
+        elif isinstance(raw_job_def, UnresolvedAssetJobDefinition):
+            repository_definitions["jobs"][key] = raw_job_def.resolve(
                 # TODO: https://github.com/dagster-io/dagster/issues/8263
                 assets=[],
                 source_assets=[],
                 default_executor_def=None,
             )
-        elif not isinstance(job, JobDefinition) and not isfunction(job):
+        elif not isinstance(raw_job_def, JobDefinition) and not isfunction(raw_job_def):
             raise DagsterInvalidDefinitionError(
                 f"Object mapped to {key} is not an instance of JobDefinition or GraphDefinition."
             )
 
     # Late validate all jobs' resource requirements are satisfied, since
     # they may not be applied until now
-    for pipeline_or_job in repository_definitions["jobs"].values():
-        if isinstance(pipeline_or_job, PipelineDefinition):
-            pipeline_or_job.validate_resource_requirements_satisfied()
+    for job_def in repository_definitions["jobs"].values():
+        if isinstance(job_def, JobDefinition):
+            job_def.validate_resource_requirements_satisfied()
 
     return CachingRepositoryData(
         **repository_definitions,
         source_assets_by_key={},
         assets_defs_by_key={},
         top_level_resources={},
         utilized_env_vars={},
@@ -387,75 +369,68 @@
 
 def _process_and_validate_target(
     schedule_or_sensor_def: Union[
         SensorDefinition, ScheduleDefinition, UnresolvedPartitionedAssetScheduleDefinition
     ],
     coerced_graphs: Dict[str, JobDefinition],
     unresolved_jobs: Dict[str, UnresolvedAssetJobDefinition],
-    pipelines_or_jobs: Dict[str, PipelineDefinition],
-    target: Union[GraphDefinition, PipelineDefinition, UnresolvedAssetJobDefinition],
+    jobs: Dict[str, JobDefinition],
+    target: Union[GraphDefinition, JobDefinition, UnresolvedAssetJobDefinition],
 ):
-    """This function modifies the state of coerced_graphs, unresolved_jobs, and pipelines_or_jobs.
-    """
+    """This function modifies the state of coerced_graphs, unresolved_jobs, and jobs."""
     targeter = (
         f"schedule '{schedule_or_sensor_def.name}'"
         if isinstance(schedule_or_sensor_def, ScheduleDefinition)
         else f"sensor '{schedule_or_sensor_def.name}'"
     )
     if isinstance(target, GraphDefinition):
         if target.name not in coerced_graphs:
             # Since this is a graph we have to coerce, it is not possible to be
             # the same definition by reference equality
-            if target.name in pipelines_or_jobs:
-                dupe_target_type = pipelines_or_jobs[target.name].target_type
+            if target.name in jobs:
                 raise DagsterInvalidDefinitionError(
-                    _get_error_msg_for_target_conflict(
-                        targeter, "graph", target.name, dupe_target_type
-                    )
+                    _get_error_msg_for_target_conflict(targeter, "graph", target.name, "job")
                 )
         elif coerced_graphs[target.name].graph != target:
             raise DagsterInvalidDefinitionError(
                 _get_error_msg_for_target_conflict(targeter, "graph", target.name, "graph")
             )
         coerced_job = target.coerce_to_job()
         coerced_graphs[target.name] = coerced_job
-        pipelines_or_jobs[target.name] = coerced_job
+        jobs[target.name] = coerced_job
     elif isinstance(target, UnresolvedAssetJobDefinition):
         if target.name not in unresolved_jobs:
             # Since this is an unresolved job we have to resolve, it is not possible to
             # be the same definition by reference equality
-            if target.name in pipelines_or_jobs:
-                dupe_target_type = pipelines_or_jobs[target.name].target_type
+            if target.name in jobs:
                 raise DagsterInvalidDefinitionError(
                     _get_error_msg_for_target_conflict(
-                        targeter, "unresolved asset job", target.name, dupe_target_type
+                        targeter, "unresolved asset job", target.name, "job"
                     )
                 )
         elif unresolved_jobs[target.name].selection != target.selection:
             raise DagsterInvalidDefinitionError(
                 _get_error_msg_for_target_conflict(
                     targeter, "unresolved asset job", target.name, "unresolved asset job"
                 )
             )
         unresolved_jobs[target.name] = target
     else:
-        if target.name in pipelines_or_jobs and pipelines_or_jobs[target.name] != target:
+        if target.name in jobs and jobs[target.name] != target:
             dupe_target_type = (
                 "graph"
                 if target.name in coerced_graphs
                 else "unresolved asset job"
                 if target.name in unresolved_jobs
-                else pipelines_or_jobs[target.name].target_type
+                else "job"
             )
             raise DagsterInvalidDefinitionError(
-                _get_error_msg_for_target_conflict(
-                    targeter, target.target_type, target.name, dupe_target_type
-                )
+                _get_error_msg_for_target_conflict(targeter, "job", target.name, dupe_target_type)
             )
-        pipelines_or_jobs[target.name] = target
+        jobs[target.name] = target
 
 
 def _get_error_msg_for_target_conflict(targeter, target_type, target_name, dupe_target_type):
     return (
         f"{targeter} targets {target_type} '{target_name}', but a different {dupe_target_type} with"
         " the same name was provided. Disambiguate between these by providing a separate name to"
         " one of them."
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.2/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,21 @@
     ASSET_BASE_JOB_PREFIX,
 )
 from dagster._core.definitions.cacheable_assets import AssetsDefinitionCacheableData
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKey
 from dagster._core.definitions.executor_definition import ExecutorDefinition
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.logger_definition import LoggerDefinition
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.schedule_definition import ScheduleDefinition
 from dagster._core.definitions.sensor_definition import SensorDefinition
 from dagster._core.definitions.source_asset import SourceAsset
 from dagster._core.definitions.utils import check_valid_name
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.instance import DagsterInstance
-from dagster._core.selector import parse_solid_selection
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils import hash_collection
 
 from .repository_data import CachingRepositoryData, RepositoryData
 from .valid_definitions import (
     SINGLETON_REPOSITORY_NAME as SINGLETON_REPOSITORY_NAME,
     VALID_REPOSITORY_DATA_DICT_KEYS as VALID_REPOSITORY_DATA_DICT_KEYS,
@@ -128,58 +126,36 @@
     def load_all_definitions(self):
         # force load of all lazy constructed code artifacts
         self._repository_data.load_all_definitions()
 
     @property
     def pipeline_names(self) -> Sequence[str]:
         """List[str]: Names of all pipelines/jobs in the repository."""
-        return self._repository_data.get_pipeline_names()
+        return self._repository_data.get_job_names()
 
     @public
     @property
     def job_names(self) -> Sequence[str]:
         """List[str]: Names of all jobs in the repository."""
         return self._repository_data.get_job_names()
 
-    def has_pipeline(self, name: str) -> bool:
-        """Check if a pipeline/job with a given name is present in the repository.
-
-        Args:
-            name (str): The name of the pipeline/job.
-
-        Returns:
-            bool
-        """
-        return self._repository_data.has_pipeline(name)
-
-    def get_pipeline(self, name: str) -> PipelineDefinition:
+    def get_pipeline(self, name: str) -> JobDefinition:
         """Get a pipeline/job by name.
 
         If this pipeline/job is present in the lazily evaluated dictionary passed to the
         constructor, but has not yet been constructed, only this pipeline/job is constructed, and will
         be cached for future calls.
 
         Args:
             name (str): Name of the pipeline/job to retrieve.
 
         Returns:
             PipelineDefinition: The pipeline/job definition corresponding to the given name.
         """
-        return self._repository_data.get_pipeline(name)
-
-    def get_all_pipelines(self) -> Sequence[PipelineDefinition]:
-        """Return all pipelines/jobs in the repository as a list.
-
-        Note that this will construct any pipeline/job in the lazily evaluated dictionary that
-        has not yet been constructed.
-
-        Returns:
-            List[PipelineDefinition]: All pipelines/jobs in the repository.
-        """
-        return self._repository_data.get_all_pipelines()
+        return self._repository_data.get_job(name)
 
     def get_top_level_resources(self) -> Mapping[str, ResourceDefinition]:
         return self._repository_data.get_top_level_resources()
 
     def get_env_vars_by_top_level_resource(self) -> Mapping[str, AbstractSet[str]]:
         return self._repository_data.get_env_vars_by_top_level_resource()
 
@@ -315,27 +291,16 @@
         self,
         job_name: str,
         op_selection: Optional[Sequence[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         solids_to_execute: Optional[AbstractSet[str]] = None,
     ):
         # named job forward expecting pipeline distinction to be removed soon
-        defn = self.get_pipeline(job_name)
-        if isinstance(defn, JobDefinition):
-            return defn.get_job_def_for_subset_selection(op_selection, asset_selection)
-
-        check.invariant(
-            asset_selection is None,
-            f"Asset selection cannot be provided with a pipeline {asset_selection}",
-        )
-        # pipelines use post-resolved selection, should be removed soon
-        if op_selection and solids_to_execute is None:
-            solids_to_execute = parse_solid_selection(defn, op_selection)
-
-        return defn.get_pipeline_subset_def(solids_to_execute)
+        defn = self.get_job(job_name)
+        return defn.get_job_def_for_subset_selection(op_selection, asset_selection)
 
     @public
     def load_asset_value(
         self,
         asset_key: CoercibleToAssetKey,
         *,
         python_type: Optional[Type] = None,
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.2/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import TYPE_CHECKING, TypeVar, Union
 
 from typing_extensions import TypeAlias
 
 from dagster._core.definitions.graph_definition import GraphDefinition
 from dagster._core.definitions.job_definition import JobDefinition
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.definitions.schedule_definition import ScheduleDefinition
 from dagster._core.definitions.sensor_definition import SensorDefinition
 from dagster._core.definitions.source_asset import SourceAsset
 from dagster._core.definitions.unresolved_asset_job_definition import UnresolvedAssetJobDefinition
 
 if TYPE_CHECKING:
     from dagster._core.definitions import AssetGroup, AssetsDefinition
@@ -16,33 +15,31 @@
     from dagster._core.definitions.partitioned_schedule import (
         UnresolvedPartitionedAssetScheduleDefinition,
     )
 
 SINGLETON_REPOSITORY_NAME = "__repository__"
 
 VALID_REPOSITORY_DATA_DICT_KEYS = {
-    "pipelines",
     "schedules",
     "sensors",
     "jobs",
 }
 
 T_RepositoryLevelDefinition = TypeVar(
     "T_RepositoryLevelDefinition",
-    PipelineDefinition,
     JobDefinition,
     ScheduleDefinition,
     SensorDefinition,
 )
 
 RepositoryListDefinition: TypeAlias = Union[
     "AssetsDefinition",
     "AssetGroup",
     GraphDefinition,
-    PipelineDefinition,
+    JobDefinition,
     ScheduleDefinition,
     SensorDefinition,
     SourceAsset,
     UnresolvedAssetJobDefinition,
     "UnresolvedPartitionedAssetScheduleDefinition",
 ]
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.2/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.2/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.2/dagster/_core/definitions/resource_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ]
 
 
 class ResourceDefinition(AnonymousConfigurableDefinition, RequiresResources):
     """Core class for defining resources.
 
     Resources are scoped ways to make external resources (like database connections) available to
-    during job execution and to clean up after execution resolves.
+    ops and assets during job execution and to clean up after execution resolves.
 
     If resource_fn yields once rather than returning (in the manner of functions decorable with
     :py:func:`@contextlib.contextmanager <python:contextlib.contextmanager>`) then the body of the
     function after the yield will be run after execution resolves, allowing users to write their
     own teardown/cleanup logic.
 
     Depending on your executor, resources may be instantiated and cleaned up more than once in a
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.2/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.2/dagster/_core/definitions/resource_requirement.py`

 * *Files 12% similar despite different names*

```diff
@@ -198,41 +198,36 @@
     ) -> Iterator[ResourceRequirement]:
         raise NotImplementedError()
 
 
 def ensure_resources_of_expected_type(
     resource_defs: Mapping[str, "ResourceDefinition"],
     requirements: Sequence[ResourceRequirement],
-    mode_name: Optional[str] = None,
 ) -> None:
-    mode_descriptor = f" by mode '{mode_name}'" if mode_name and mode_name != "default" else ""
     for requirement in requirements:
         if requirement.resources_contain_key(
             resource_defs
         ) and not requirement.resource_is_expected_type(resource_defs):
             raise DagsterInvalidDefinitionError(
                 f"{requirement.describe_requirement()}, but received"
-                f" {type(resource_defs[requirement.key])}{mode_descriptor}."
+                f" {type(resource_defs[requirement.key])}."
             )
 
 
 def ensure_requirements_satisfied(
     resource_defs: Mapping[str, "ResourceDefinition"],
     requirements: Sequence[ResourceRequirement],
-    mode_name: Optional[str] = None,
 ) -> None:
-    ensure_resources_of_expected_type(resource_defs, requirements, mode_name)
-
-    mode_descriptor = f" by mode '{mode_name}'" if mode_name and mode_name != "default" else ""
+    ensure_resources_of_expected_type(resource_defs, requirements)
 
     # Error if resource defs don't provide the correct resource key
     for requirement in requirements:
         if not requirement.resources_contain_key(resource_defs):
             raise DagsterInvalidDefinitionError(
-                f"{requirement.describe_requirement()} was not provided{mode_descriptor}. Please"
+                f"{requirement.describe_requirement()} was not provided. Please"
                 f" provide a {str(requirement.expected_type)} to key '{requirement.key}', or change"
                 " the required key to one of the following keys which points to an"
                 f" {str(requirement.expected_type)}:"
                 f" {requirement.keys_of_expected_type(resource_defs)}"
             )
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/run_config.py` & `dagster-1.3.2/dagster/_core/definitions/run_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 from dagster._utils import check
 
 from .configurable import ConfigurableDefinition
 from .definition_config_schema import IDefinitionConfigSchema
 from .dependency import DependencyStructure, GraphNode, Node, NodeHandle, NodeInput, OpNode
 from .graph_definition import GraphDefinition
 from .logger_definition import LoggerDefinition
-from .mode import ModeDefinition
 from .op_definition import NodeDefinition, OpDefinition
 from .resource_definition import ResourceDefinition
 
 if TYPE_CHECKING:
     from .source_asset import SourceAsset
 
 
@@ -93,19 +92,19 @@
 
 
 class RunConfigSchemaCreationData(NamedTuple):
     pipeline_name: str
     nodes: Sequence[Node]
     graph_def: GraphDefinition
     dependency_structure: DependencyStructure
-    mode_definition: ModeDefinition
+    executor_def: ExecutorDefinition
+    resource_defs: Mapping[str, ResourceDefinition]
     logger_defs: Mapping[str, LoggerDefinition]
     ignored_nodes: Sequence[Node]
     required_resources: AbstractSet[str]
-    is_using_graph_job_op_apis: bool
     direct_inputs: Mapping[str, Any]
     asset_layer: AssetLayer
 
 
 def define_logger_dictionary_cls(creation_data: RunConfigSchemaCreationData) -> Shape:
     return Shape(
         {
@@ -136,24 +135,17 @@
 
 
 def define_single_execution_field(executor_def: ExecutorDefinition, description: str) -> Field:
     return def_config_field(executor_def, description=description)
 
 
 def define_run_config_schema_type(creation_data: RunConfigSchemaCreationData) -> ConfigType:
-    execution_field = (
-        define_execution_field(
-            creation_data.mode_definition.executor_defs,
-            "Configure how steps are executed within a run.",
-        )
-        if not creation_data.is_using_graph_job_op_apis
-        else define_single_execution_field(
-            creation_data.mode_definition.executor_defs[0],
-            "Configure how steps are executed within a run.",
-        )
+    execution_field = define_single_execution_field(
+        creation_data.executor_def,
+        "Configure how steps are executed within a run.",
     )
 
     top_level_node = GraphNode(
         name=creation_data.graph_def.name,
         definition=creation_data.graph_def,
         graph_definition=creation_data.graph_def,
     )
@@ -162,29 +154,28 @@
         "execution": execution_field,
         "loggers": Field(
             define_logger_dictionary_cls(creation_data),
             description="Configure how loggers emit messages within a run.",
         ),
         "resources": Field(
             define_resource_dictionary_cls(
-                creation_data.mode_definition.resource_defs,
+                creation_data.resource_defs,
                 creation_data.required_resources,
             ),
             description="Configure how shared resources are implemented within a run.",
         ),
         "inputs": get_inputs_field(
             node=top_level_node,
             handle=NodeHandle(top_level_node.name, parent=None),
             dependency_structure=creation_data.dependency_structure,
-            resource_defs=creation_data.mode_definition.resource_defs,
+            resource_defs=creation_data.resource_defs,
             node_ignored=False,
             direct_inputs=creation_data.direct_inputs,
             input_source_assets={},
             asset_layer=creation_data.asset_layer,
-            is_using_graph_job_op_apis=creation_data.is_using_graph_job_op_apis,
         ),
     }
 
     if creation_data.graph_def.has_config_mapping:
         config_schema = cast(IDefinitionConfigSchema, creation_data.graph_def.config_schema)
         nodes_field = Field(
             {"config": config_schema.as_field()},
@@ -192,28 +183,23 @@
         )
     else:
         nodes_field = Field(
             define_node_shape(
                 nodes=creation_data.nodes,
                 ignored_nodes=creation_data.ignored_nodes,
                 dependency_structure=creation_data.dependency_structure,
-                resource_defs=creation_data.mode_definition.resource_defs,
-                is_using_graph_job_op_apis=creation_data.is_using_graph_job_op_apis,
+                resource_defs=creation_data.resource_defs,
                 asset_layer=creation_data.asset_layer,
                 node_input_source_assets=creation_data.graph_def.node_input_source_assets,
             ),
             description="Configure runtime parameters for ops or assets.",
         )
 
-    if creation_data.is_using_graph_job_op_apis:
-        fields["ops"] = nodes_field
-        field_aliases = {"ops": "solids"}
-    else:
-        fields["solids"] = nodes_field
-        field_aliases = {"solids": "ops"}
+    fields["ops"] = nodes_field
+    field_aliases = {"ops": "solids"}
 
     return Shape(
         fields=remove_none_entries(fields),
         field_aliases=field_aliases,
     )
 
 
@@ -226,15 +212,14 @@
 def get_inputs_field(
     node: Node,
     handle: NodeHandle,
     dependency_structure: DependencyStructure,
     resource_defs: Mapping[str, ResourceDefinition],
     node_ignored: bool,
     asset_layer: AssetLayer,
-    is_using_graph_job_op_apis: bool,
     input_source_assets: Mapping[str, "SourceAsset"],
     direct_inputs: Optional[Mapping[str, Any]] = None,
 ) -> Optional[Field]:
     direct_inputs = check.opt_mapping_param(direct_inputs, "direct_inputs")
     inputs_field_fields = {}
     for name, inp in node.definition.input_dict.items():
         inp_handle = NodeInput(node, inp)
@@ -261,20 +246,19 @@
 
         if input_field:
             inputs_field_fields[name] = input_field
 
     if not inputs_field_fields:
         return None
     if node_ignored:
-        node_type = "op" if is_using_graph_job_op_apis else "solid"
         return Field(
             Shape(inputs_field_fields),
             is_required=False,
             description=(
-                f"This {node_type} is not present in the current {node_type} selection, "
+                "This op is not present in the current op selection, "
                 "the input config values are allowed but ignored."
             ),
         )
     else:
         return Field(Shape(inputs_field_fields))
 
 
@@ -383,27 +367,24 @@
         and output_manager_def.output_config_schema
     ):
         return output_manager_def.output_config_schema.as_field()
 
     return None
 
 
-def node_config_field(
-    fields: Mapping[str, Optional[Field]], ignored: bool, is_using_graph_job_op_apis: bool
-) -> Optional[Field]:
-    field_aliases = {"ops": "solids"} if is_using_graph_job_op_apis else {"solids": "ops"}
+def node_config_field(fields: Mapping[str, Optional[Field]], ignored: bool) -> Optional[Field]:
+    field_aliases = {"ops": "solids"}
     trimmed_fields = remove_none_entries(fields)
     if trimmed_fields:
         if ignored:
-            node_type = "op" if is_using_graph_job_op_apis else "solid"
             return Field(
                 Shape(trimmed_fields, field_aliases=field_aliases),
                 is_required=False,
                 description=(
-                    f"This {node_type} is not present in the current {node_type} selection, "
+                    "This op is not present in the current op selection, "
                     "the config values are allowed but ignored."
                 ),
             )
         else:
             return Field(Shape(trimmed_fields, field_aliases=field_aliases))
     else:
         return None
@@ -412,45 +393,41 @@
 def construct_leaf_node_config(
     node: Node,
     handle: NodeHandle,
     dependency_structure: DependencyStructure,
     config_schema: Optional[IDefinitionConfigSchema],
     resource_defs: Mapping[str, ResourceDefinition],
     ignored: bool,
-    is_using_graph_job_op_apis: bool,
     asset_layer: AssetLayer,
     input_source_assets: Mapping[str, "SourceAsset"],
 ) -> Optional[Field]:
     return node_config_field(
         {
             "inputs": get_inputs_field(
                 node,
                 handle,
                 dependency_structure,
                 resource_defs,
                 ignored,
                 asset_layer,
-                is_using_graph_job_op_apis,
                 input_source_assets,
             ),
             "outputs": get_outputs_field(node, resource_defs),
             "config": config_schema.as_field() if config_schema else None,
         },
         ignored=ignored,
-        is_using_graph_job_op_apis=is_using_graph_job_op_apis,
     )
 
 
 def define_node_field(
     node: Node,
     handle: NodeHandle,
     dependency_structure: DependencyStructure,
     resource_defs: Mapping[str, ResourceDefinition],
     ignored: bool,
-    is_using_graph_job_op_apis: bool,
     asset_layer: AssetLayer,
     input_source_assets: Mapping[str, "SourceAsset"],
 ) -> Optional[Field]:
     # All nodes regardless of compositing status get the same inputs and outputs
     # config. The only thing the varies is on extra element of configuration
     # 1) Vanilla op definition: a 'config' key with the config_schema as the value
     # 2) Graph with field mapping: a 'config' key with the config_schema of
@@ -466,15 +443,14 @@
         return construct_leaf_node_config(
             node,
             handle,
             dependency_structure,
             node.definition.config_schema,
             resource_defs,
             ignored,
-            is_using_graph_job_op_apis,
             asset_layer,
             input_source_assets,
         )
 
     graph_def = node.definition
 
     if graph_def.has_config_mapping:
@@ -484,62 +460,52 @@
             node,
             handle,
             dependency_structure,
             # ...and in both cases, the correct schema for 'config' key is exposed by this property:
             graph_def.config_schema,
             resource_defs,
             ignored,
-            is_using_graph_job_op_apis,
             asset_layer,
             input_source_assets,
         )
         # This case omits an 'ops' key, thus if a graph is `configured` or has a field
         # mapping, the user cannot stub any config, inputs, or outputs for inner (child) nodes.
     else:
         fields = {
             "inputs": get_inputs_field(
                 node,
                 handle,
                 dependency_structure,
                 resource_defs,
                 ignored,
                 asset_layer,
-                is_using_graph_job_op_apis,
                 input_source_assets,
             ),
             "outputs": get_outputs_field(node, resource_defs),
+            "ops": Field(
+                define_node_shape(
+                    nodes=graph_def.nodes,
+                    ignored_nodes=None,
+                    dependency_structure=graph_def.dependency_structure,
+                    parent_handle=handle,
+                    resource_defs=resource_defs,
+                    asset_layer=asset_layer,
+                    node_input_source_assets=graph_def.node_input_source_assets,
+                )
+            ),
         }
-        nodes_field = Field(
-            define_node_shape(
-                nodes=graph_def.nodes,
-                ignored_nodes=None,
-                dependency_structure=graph_def.dependency_structure,
-                parent_handle=handle,
-                resource_defs=resource_defs,
-                is_using_graph_job_op_apis=is_using_graph_job_op_apis,
-                asset_layer=asset_layer,
-                node_input_source_assets=graph_def.node_input_source_assets,
-            )
-        )
-        if is_using_graph_job_op_apis:
-            fields["ops"] = nodes_field
-        else:
-            fields["solids"] = nodes_field
 
-        return node_config_field(
-            fields, ignored=ignored, is_using_graph_job_op_apis=is_using_graph_job_op_apis
-        )
+        return node_config_field(fields, ignored=ignored)
 
 
 def define_node_shape(
     nodes: Sequence[Node],
     ignored_nodes: Optional[Sequence[Node]],
     dependency_structure: DependencyStructure,
     resource_defs: Mapping[str, ResourceDefinition],
-    is_using_graph_job_op_apis: bool,
     asset_layer: AssetLayer,
     node_input_source_assets: Mapping[str, Mapping[str, "SourceAsset"]],
     parent_handle: Optional[NodeHandle] = None,
 ) -> Shape:
     """Examples of what this method is used to generate the schema for:
     1.
         inputs: ...
@@ -564,38 +530,35 @@
     for node in nodes:
         node_field = define_node_field(
             node,
             NodeHandle(node.name, parent_handle),
             dependency_structure,
             resource_defs,
             ignored=False,
-            is_using_graph_job_op_apis=is_using_graph_job_op_apis,
             asset_layer=asset_layer,
             input_source_assets=node_input_source_assets.get(node.name, {}),
         )
 
         if node_field:
             fields[node.name] = node_field
 
     for node in ignored_nodes:
         node_field = define_node_field(
             node,
             NodeHandle(node.name, parent_handle),
             dependency_structure,
             resource_defs,
             ignored=True,
-            is_using_graph_job_op_apis=is_using_graph_job_op_apis,
             asset_layer=asset_layer,
             input_source_assets=node_input_source_assets.get(node.name, {}),
         )
         if node_field:
             fields[node.name] = node_field
 
-    field_aliases = {"ops": "solids"} if is_using_graph_job_op_apis else {"solids": "ops"}
-    return Shape(fields, field_aliases=field_aliases)
+    return Shape(fields, field_aliases={"ops": "solids"})
 
 
 def iterate_node_def_config_types(node_def: NodeDefinition) -> Iterator[ConfigType]:
     if isinstance(node_def, OpDefinition):
         if node_def.has_config_field:
             yield from node_def.get_config_field().config_type.type_iterator()
     elif isinstance(node_def, GraphDefinition):
@@ -660,15 +623,36 @@
             else v
         }
         for k, v in configs.items()
     }
 
 
 class RunConfig:
-    """RunConfig is a container for all the configuration that can be passed to a pipeline run."""
+    """Container for all the configuration that can be passed to a pipeline run. Accepts Pythonic definitions
+    for op and asset config and resources and converts them under the hood to the appropriate config dictionaries.
+
+    Example usage:
+
+    .. code-block:: python
+
+        class MyAssetConfig(Config):
+            a_str: str
+
+        @asset
+        def my_asset(config: MyAssetConfig):
+            assert config.a_str == "foo"
+
+        materialize(
+            [my_asset],
+            run_config=RunConfig(
+                ops={"my_asset": MyAssetConfig(a_str="foo")}
+            )
+        )
+
+    """
 
     def __init__(
         self,
         ops: Optional[Dict[str, Any]] = None,
         resources: Optional[Dict[str, Any]] = None,
         loggers: Optional[Dict[str, Any]] = None,
         execution: Optional[Dict[str, Any]] = None,
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.2/dagster/_core/definitions/run_config_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable, Mapping, NamedTuple, Optional
 
 import dagster._check as check
 from dagster._config import ConfigType
 
 from .config import ConfigMapping
-from .pipeline_definition import PipelineDefinition
+from .job_definition import JobDefinition
 
 
 class RunConfigSchema(NamedTuple):
     run_config_schema_type: ConfigType
     config_type_dict_by_name: Mapping[str, ConfigType]
     config_type_dict_by_key: Mapping[str, ConfigType]
     config_mapping: Optional[ConfigMapping]
@@ -36,13 +36,10 @@
                 check.failed("ConfigMapping config type unexpectedly None")
             return mapped_type
 
         return self.run_config_schema_type
 
 
 def create_run_config_schema(
-    pipeline_def: PipelineDefinition,
-    mode: Optional[str] = None,
+    pipeline_def: JobDefinition,
 ) -> RunConfigSchema:
-    mode = check.opt_str_param(mode, "mode", default=pipeline_def.get_default_mode_name())
-
-    return pipeline_def.get_run_config_schema(mode)
+    return pipeline_def.run_config_schema
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/run_request.py` & `dagster-1.3.2/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.2/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from dagster._serdes.serdes import deserialize_value
 from dagster._seven import JSONDecodeError
 from dagster._utils import utc_datetime_from_timestamp
 from dagster._utils.backcompat import deprecation_warning
 from dagster._utils.error import serializable_error_info_from_exc_info
 
 from .graph_definition import GraphDefinition
-from .pipeline_definition import PipelineDefinition
+from .job_definition import JobDefinition
 from .sensor_definition import (
     DefaultSensorStatus,
     PipelineRunReaction,
     RawSensorEvaluationFunctionReturn,
     RunRequest,
     SensorDefinition,
     SensorEvaluationContext,
@@ -129,35 +129,38 @@
         dagster_event,
         instance,
         context: Optional[
             SensorEvaluationContext
         ] = None,  # deprecated arg, but we need to keep it for backcompat
         resource_defs: Optional[Mapping[str, "ResourceDefinition"]] = None,
         logger: Optional[logging.Logger] = None,
+        partition_key: Optional[str] = None,
     ) -> None:
         self._exit_stack = ExitStack()
         self._sensor_name = check.str_param(sensor_name, "sensor_name")
         self._dagster_run = check.inst_param(dagster_run, "dagster_run", DagsterRun)
         self._dagster_event = check.inst_param(dagster_event, "dagster_event", DagsterEvent)
         self._instance = check.inst_param(instance, "instance", DagsterInstance)
         self._logger: Optional[logging.Logger] = logger or (context.log if context else None)
+        self._partition_key = check.opt_str_param(partition_key, "partition_key")
 
         # Wait to set resources unless they're accessed
         self._resource_defs = resource_defs
         self._resources = None
         self._cm_scope_entered = False
 
     def for_run_failure(self) -> "RunFailureSensorContext":
         """Converts RunStatusSensorContext to RunFailureSensorContext."""
         return RunFailureSensorContext(
             sensor_name=self._sensor_name,
             dagster_run=self._dagster_run,
             dagster_event=self._dagster_event,
             instance=self._instance,
             logger=self._logger,
+            partition_key=self._partition_key,
         )
 
     @property
     def resource_defs(self) -> Optional[Mapping[str, "ResourceDefinition"]]:
         return self._resource_defs
 
     @property
@@ -223,14 +226,19 @@
     @property
     def log(self) -> logging.Logger:
         if not self._logger:
             self._logger = InstigationLogger()
 
         return self._logger
 
+    @public
+    @property
+    def partition_key(self) -> Optional[str]:
+        return self._partition_key
+
     @property
     def pipeline_run(self) -> DagsterRun:
         warnings.warn(
             "`RunStatusSensorContext.pipeline_run` is deprecated as of 0.13.0; use "
             "`RunStatusSensorContext.dagster_run` instead."
         )
         return self.dagster_run
@@ -261,14 +269,15 @@
 def build_run_status_sensor_context(
     sensor_name: str,
     dagster_event: DagsterEvent,
     dagster_instance: DagsterInstance,
     dagster_run: DagsterRun,
     context: Optional[SensorEvaluationContext] = None,
     resources: Optional[Mapping[str, object]] = None,
+    partition_key: Optional[str] = None,
 ) -> RunStatusSensorContext:
     """Builds run status sensor context from provided parameters.
 
     This function can be used to provide the context argument when directly invoking a function
     decorated with `@run_status_sensor` or `@run_failure_sensor`, such as when writing unit tests.
 
     Args:
@@ -302,14 +311,15 @@
     return RunStatusSensorContext(
         sensor_name=sensor_name,
         instance=dagster_instance,
         dagster_run=dagster_run,
         dagster_event=dagster_event,
         resource_defs=wrap_resources_for_execution(resources),
         logger=context.log if context else None,
+        partition_key=partition_key,
     )
 
 
 @overload
 def run_failure_sensor(
     name: RunFailureSensorEvaluationFn,
 ) -> SensorDefinition:
@@ -320,27 +330,27 @@
 def run_failure_sensor(
     name: Optional[str] = None,
     minimum_interval_seconds: Optional[int] = None,
     description: Optional[str] = None,
     monitored_jobs: Optional[
         Sequence[
             Union[
-                PipelineDefinition,
+                JobDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 "RepositorySelector",
                 "JobSelector",
                 "CodeLocationSelector",
             ]
         ]
     ] = None,
     job_selection: Optional[
         Sequence[
             Union[
-                PipelineDefinition,
+                JobDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 "RepositorySelector",
                 "JobSelector",
                 "CodeLocationSelector",
             ]
         ]
@@ -356,27 +366,27 @@
 def run_failure_sensor(
     name: Optional[Union[RunFailureSensorEvaluationFn, str]] = None,
     minimum_interval_seconds: Optional[int] = None,
     description: Optional[str] = None,
     monitored_jobs: Optional[
         Sequence[
             Union[
-                PipelineDefinition,
+                JobDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 "RepositorySelector",
                 "JobSelector",
                 "CodeLocationSelector",
             ]
         ]
     ] = None,
     job_selection: Optional[
         Sequence[
             Union[
-                PipelineDefinition,
+                JobDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 "RepositorySelector",
                 "JobSelector",
                 "CodeLocationSelector",
             ]
         ]
@@ -485,15 +495,15 @@
         run_status: DagsterRunStatus,
         run_status_sensor_fn: RunStatusSensorEvaluationFunction,
         minimum_interval_seconds: Optional[int] = None,
         description: Optional[str] = None,
         monitored_jobs: Optional[
             Sequence[
                 Union[
-                    PipelineDefinition,
+                    JobDefinition,
                     GraphDefinition,
                     UnresolvedAssetJobDefinition,
                     "RepositorySelector",
                     "JobSelector",
                     "CodeLocationSelector",
                 ]
             ]
@@ -517,15 +527,15 @@
         check.callable_param(run_status_sensor_fn, "run_status_sensor_fn")
         check.opt_int_param(minimum_interval_seconds, "minimum_interval_seconds")
         check.opt_str_param(description, "description")
         check.opt_list_param(
             monitored_jobs,
             "monitored_jobs",
             (
-                PipelineDefinition,
+                JobDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 RepositorySelector,
                 JobSelector,
                 CodeLocationSelector,
             ),
         )
@@ -702,14 +712,15 @@
                     with RunStatusSensorContext(
                         sensor_name=name,
                         dagster_run=pipeline_run,
                         dagster_event=event_log_entry.dagster_event,
                         instance=context.instance,
                         resource_defs=context.resource_defs,
                         logger=context.log,
+                        partition_key=pipeline_run.tags.get("dagster/partition"),
                     ) as sensor_context, user_code_error_boundary(
                         RunStatusSensorExecutionError,
                         lambda: f'Error occurred during the execution sensor "{name}".',
                     ):
                         context_param_name = get_context_param_name(run_status_sensor_fn)
                         context_param = (
                             {context_param_name: sensor_context} if context_param_name else {}
@@ -803,27 +814,27 @@
     run_status: DagsterRunStatus,
     name: Optional[str] = None,
     minimum_interval_seconds: Optional[int] = None,
     description: Optional[str] = None,
     monitored_jobs: Optional[
         Sequence[
             Union[
-                PipelineDefinition,
+                JobDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 "RepositorySelector",
                 "JobSelector",
                 "CodeLocationSelector",
             ]
         ]
     ] = None,
     job_selection: Optional[
         Sequence[
             Union[
-                PipelineDefinition,
+                JobDefinition,
                 GraphDefinition,
                 UnresolvedAssetJobDefinition,
                 "RepositorySelector",
                 "JobSelector",
                 "CodeLocationSelector",
             ]
         ]
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.2/dagster/_core/definitions/schedule_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,15 @@
     ScheduleExecutionError,
     user_code_error_boundary,
 )
 from ..instance import DagsterInstance
 from ..instance.ref import InstanceRef
 from ..storage.pipeline_run import DagsterRun
 from .graph_definition import GraphDefinition
-from .mode import DEFAULT_MODE_NAME
-from .pipeline_definition import PipelineDefinition
+from .job_definition import JobDefinition
 from .run_request import RunRequest, SkipReason
 from .target import DirectTarget, ExecutableDefinition, RepoRelativeTarget
 from .unresolved_asset_job_definition import UnresolvedAssetJobDefinition
 from .utils import check_valid_name, validate_tags
 
 if TYPE_CHECKING:
     from dagster import ResourceDefinition
@@ -542,15 +541,14 @@
             )
 
         if job is not None:
             self._target: Union[DirectTarget, RepoRelativeTarget] = DirectTarget(job)
         else:
             self._target = RepoRelativeTarget(
                 pipeline_name=check.str_param(job_name, "job_name"),
-                mode=DEFAULT_MODE_NAME,
                 solid_selection=None,
             )
 
         if name:
             self._name = check_valid_name(name)
         elif job_name:
             self._name = job_name + "_schedule"
@@ -752,15 +750,15 @@
     @public
     @property
     def execution_timezone(self) -> Optional[str]:
         return self._execution_timezone
 
     @public
     @property
-    def job(self) -> Union[GraphDefinition, PipelineDefinition, UnresolvedAssetJobDefinition]:
+    def job(self) -> Union[GraphDefinition, JobDefinition, UnresolvedAssetJobDefinition]:
         if isinstance(self._target, DirectTarget):
             return self._target.target
         raise DagsterInvalidDefinitionError("No job was provided to ScheduleDefinition.")
 
     def evaluate_tick(self, context: "ScheduleEvaluationContext") -> ScheduleExecutionData:
         """Evaluate schedule using the provided context.
 
@@ -856,15 +854,15 @@
     def targets_unresolved_asset_job(self) -> bool:
         return self.has_loadable_target() and isinstance(
             self.load_target(), UnresolvedAssetJobDefinition
         )
 
     def load_target(
         self,
-    ) -> Union[GraphDefinition, PipelineDefinition, UnresolvedAssetJobDefinition]:
+    ) -> Union[GraphDefinition, JobDefinition, UnresolvedAssetJobDefinition]:
         if isinstance(self._target, DirectTarget):
             return self._target.load()
 
         check.failed("Target is not loadable")
 
     @public
     @property
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.2/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/selector.py` & `dagster-1.3.2/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.2/dagster/_core/definitions/sensor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,14 @@
 
 from ..decorator_utils import (
     get_function_params,
 )
 from .asset_selection import AssetSelection
 from .graph_definition import GraphDefinition
 from .job_definition import JobDefinition
-from .mode import DEFAULT_MODE_NAME
-from .pipeline_definition import PipelineDefinition
 from .run_request import (
     AddDynamicPartitionsRequest,
     DeleteDynamicPartitionsRequest,
     PipelineRunReaction,
     RunRequest,
     SensorResult,
     SkipReason,
@@ -528,15 +526,14 @@
         jobs = jobs if jobs else [job] if job else None
 
         targets: Optional[List[Union[RepoRelativeTarget, DirectTarget]]] = None
         if job_name:
             targets = [
                 RepoRelativeTarget(
                     pipeline_name=check.str_param(job_name, "job_name"),
-                    mode=DEFAULT_MODE_NAME,
                     solid_selection=None,
                 )
             ]
         elif job:
             targets = [DirectTarget(job)]
         elif jobs:
             targets = [DirectTarget(job) for job in jobs]
@@ -619,15 +616,15 @@
 
     @property
     def targets(self) -> Sequence[Union[DirectTarget, RepoRelativeTarget]]:
         return self._targets
 
     @public
     @property
-    def job(self) -> Union[PipelineDefinition, GraphDefinition, UnresolvedAssetJobDefinition]:
+    def job(self) -> Union[JobDefinition, GraphDefinition, UnresolvedAssetJobDefinition]:
         if self._targets:
             if len(self._targets) == 1 and isinstance(self._targets[0], DirectTarget):
                 return self._targets[0].target
             elif len(self._targets) > 1:
                 raise DagsterInvalidDefinitionError(
                     "Job property not available when SensorDefinition has multiple jobs."
                 )
@@ -749,15 +746,15 @@
         for target in self._targets:
             if isinstance(target, DirectTarget):
                 return True
         return False
 
     def load_targets(
         self,
-    ) -> Sequence[Union[PipelineDefinition, GraphDefinition, UnresolvedAssetJobDefinition]]:
+    ) -> Sequence[Union[JobDefinition, GraphDefinition, UnresolvedAssetJobDefinition]]:
         """Returns job/graph definitions that have been directly passed into the sensor definition.
         Any jobs or graphs that are referenced by name will not be loaded.
         """
         targets = []
         for target in self._targets:
             if isinstance(target, DirectTarget):
                 targets.append(target.load())
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/source_asset.py` & `dagster-1.3.2/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.2/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.2/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.2/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.2/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Mapping, NamedTuple, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._core.definitions import AssetKey
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.errors import DagsterInvalidDefinitionError
-from dagster._core.instance import DagsterInstance
 from dagster._utils.backcompat import deprecation_warning
 
 from .asset_layer import build_asset_selection_job
 from .config import ConfigMapping
 
 if TYPE_CHECKING:
     from dagster._core.definitions import (
@@ -79,15 +78,14 @@
     def run_request_for_partition(
         self,
         partition_key: str,
         run_key: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
         asset_selection: Optional[Sequence[AssetKey]] = None,
         run_config: Optional[Mapping[str, Any]] = None,
-        instance: Optional[DagsterInstance] = None,
         current_time: Optional[datetime] = None,
     ) -> RunRequest:
         """Creates a RunRequest object for a run that processes the given partition.
 
         Args:
             partition_key: The key of the partition to request a run for.
             run_key (Optional[str]): A string key to identify this launched run. For sensors, ensures that
@@ -122,35 +120,40 @@
         partitioned_config = PartitionedConfig.from_flexible_config(
             self.config, self.partitions_def
         )
 
         if (
             isinstance(self.partitions_def, DynamicPartitionsDefinition)
             and self.partitions_def.name
-            and not instance
         ):
+            # Do not support using run_request_for_partition with dynamic partitions,
+            # since this requires querying the instance once per run request for the
+            # existent dynamic partitions
             check.failed(
-                "Must provide a dagster instance when calling run_request_for_partition on a "
-                "dynamic partition set"
+                "run_request_for_partition is not supported for dynamic partitions. Instead, use"
+                " RunRequest(partition_key=...)"
             )
 
         partition = self.partitions_def.get_partition(
-            partition_key, dynamic_partitions_store=instance, current_time=current_time
+            partition_key, dynamic_partitions_store=None, current_time=current_time
         )
         run_config = (
             run_config
             if run_config is not None
             else partitioned_config.get_run_config_for_partition_key(
-                partition.name, dynamic_partitions_store=instance, current_time=current_time
+                partition.name, dynamic_partitions_store=None, current_time=current_time
             )
         )
         run_request_tags = {
             **(tags or {}),
             **partitioned_config.get_tags_for_partition_key(
-                partition_key, instance, current_time=current_time, job_name=self.name
+                partition_key,
+                dynamic_partitions_store=None,
+                current_time=current_time,
+                job_name=self.name,
             ),
         }
 
         return RunRequest(
             job_name=self.name,
             run_key=run_key,
             run_config=run_config,
```

### Comparing `dagster-1.3.1/dagster/_core/definitions/utils.py` & `dagster-1.3.2/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.2/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/errors.py` & `dagster-1.3.2/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/event_api.py` & `dagster-1.3.2/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/events/__init__.py` & `dagster-1.3.2/dagster/_core/events/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from dagster._core.log_manager import DagsterLogManager
 from dagster._core.storage.captured_log_manager import CapturedLogContext
 from dagster._core.storage.pipeline_run import DagsterRunStatus
 from dagster._serdes import (
     NamedTupleSerializer,
     whitelist_for_serdes,
 )
+from dagster._serdes.serdes import UnpackContext
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.timing import format_duration
 
 if TYPE_CHECKING:
     from dagster._core.definitions.events import ObjectStoreOperation
     from dagster._core.execution.plan.plan import ExecutionPlan
     from dagster._core.execution.plan.step import StepKind
@@ -310,24 +311,29 @@
     event_specific_data = cast(EngineEventData, event.event_specific_data)
 
     log_level = logging.ERROR if event_specific_data.error else logging.DEBUG
     log_manager.log_dagster_event(level=log_level, msg=event.message or "", dagster_event=event)
 
 
 class DagsterEventSerializer(NamedTupleSerializer["DagsterEvent"]):
-    def before_unpack(self, **storage_dict: Any) -> Dict[str, Any]:
+    def before_unpack(self, context, unpacked_dict: Any) -> Dict[str, Any]:
         event_type_value, event_specific_data = _handle_back_compat(
-            storage_dict["event_type_value"], storage_dict.get("event_specific_data")
+            unpacked_dict["event_type_value"], unpacked_dict.get("event_specific_data")
         )
-        storage_dict["event_type_value"] = event_type_value
-        storage_dict["event_specific_data"] = event_specific_data
+        unpacked_dict["event_type_value"] = event_type_value
+        unpacked_dict["event_specific_data"] = event_specific_data
 
-        return storage_dict
+        return unpacked_dict
 
-    def handle_unpack_error(self, exc: Exception, **storage_dict: Any) -> "DagsterEvent":
+    def handle_unpack_error(
+        self,
+        exc: Exception,
+        context: UnpackContext,
+        storage_dict: Dict[str, Any],
+    ) -> "DagsterEvent":
         event_type_value, _ = _handle_back_compat(
             storage_dict["event_type_value"], storage_dict.get("event_specific_data")
         )
         step_key = storage_dict.get("step_key")
         orig_message = storage_dict.get("message")
         new_message = (
             f"Could not deserialize event of type {event_type_value}. This event may have been"
@@ -1729,15 +1735,16 @@
 #
 #
 # class PipelineInitFailureData(NamedTuple):
 #     error: SerializableErrorInfo
 
 
 def _handle_back_compat(
-    event_type_value: str, event_specific_data: Optional[Dict[str, Any]]
+    event_type_value: str,
+    event_specific_data: Optional[Dict[str, Any]],
 ) -> Tuple[str, Optional[Dict[str, Any]]]:
     # transform old specific process events in to engine events
     if event_type_value in [
         "PIPELINE_PROCESS_START",
         "PIPELINE_PROCESS_STARTED",
         "PIPELINE_PROCESS_EXITED",
     ]:
```

### Comparing `dagster-1.3.1/dagster/_core/events/log.py` & `dagster-1.3.2/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/events/utils.py` & `dagster-1.3.2/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/api.py` & `dagster-1.3.2/dagster/_core/execution/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,17 @@
     Tuple,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._annotations import experimental
-from dagster._core.definitions import IPipeline, JobDefinition, PipelineDefinition
+from dagster._core.definitions import IPipeline, JobDefinition
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.pipeline_base import InMemoryPipeline
-from dagster._core.definitions.pipeline_definition import PipelineSubsetDefinition
 from dagster._core.definitions.reconstruct import ReconstructableJob, ReconstructablePipeline
 from dagster._core.definitions.repository_definition import RepositoryLoadData
 from dagster._core.errors import DagsterExecutionInterruptedError, DagsterInvariantViolationError
 from dagster._core.events import DagsterEvent, EngineEventData
 from dagster._core.execution.context.system import PlanOrchestrationContext
 from dagster._core.execution.plan.execute_plan import inner_plan_execution_iterator
 from dagster._core.execution.plan.outputs import StepOutputHandle
@@ -32,15 +31,14 @@
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.execution.retries import RetryMode
 from dagster._core.instance import DagsterInstance, InstanceRef
 from dagster._core.selector import parse_step_selection
 from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus
 from dagster._core.system_config.objects import ResolvedRunConfig
 from dagster._core.telemetry import log_dagster_event, log_repo_stats, telemetry_wrapper
-from dagster._core.utils import str_format_set
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.interrupts import capture_interrupts
 from dagster._utils.merger import merge_dicts
 
 from .context_creation_pipeline import (
     ExecutionContextManager,
     PlanExecutionContextManager,
@@ -137,32 +135,21 @@
                 "resuming from a run worker failure".format(
                     dagster_run.pipeline_name, dagster_run.run_id, dagster_run.status
                 )
             ),
         )
 
     if dagster_run.solids_to_execute or dagster_run.asset_selection:
-        pipeline_def = pipeline.get_definition()
-        if isinstance(pipeline_def, PipelineSubsetDefinition):
-            check.invariant(
-                dagster_run.solids_to_execute == pipeline.solids_to_execute,
-                "Cannot execute DagsterRun with solids_to_execute {solids_to_execute} that"
-                " conflicts with pipeline subset {pipeline_solids_to_execute}.".format(
-                    pipeline_solids_to_execute=str_format_set(pipeline.solids_to_execute),  # type: ignore  # (possible none)
-                    solids_to_execute=str_format_set(dagster_run.solids_to_execute),  # type: ignore  # (possible none)
-                ),
-            )
-        else:
-            # when `execute_run_iterator` is directly called, the sub pipeline hasn't been created
-            # note that when we receive the solids to execute via DagsterRun, it won't support
-            # solid selection query syntax
-            pipeline = pipeline.subset_for_execution_from_existing_pipeline(
-                frozenset(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None,
-                asset_selection=dagster_run.asset_selection,
-            )
+        # when `execute_run_iterator` is directly called, the sub pipeline hasn't been created
+        # note that when we receive the solids to execute via DagsterRun, it won't support
+        # solid selection query syntax
+        pipeline = pipeline.subset_for_execution_from_existing_pipeline(
+            frozenset(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None,
+            asset_selection=dagster_run.asset_selection,
+        )
 
     execution_plan = _get_execution_plan_from_run(pipeline, dagster_run, instance)
     if isinstance(pipeline, ReconstructablePipeline):
         pipeline = pipeline.with_repository_load_data(execution_plan.repository_load_data)
 
     return iter(
         ExecuteRunWithPlanIterable(
@@ -200,27 +187,18 @@
         instance (DagsterInstance): The instance in which the run has been created.
         raise_on_error (Optional[bool]): Whether or not to raise exceptions when they occur.
             Defaults to ``False``.
 
     Returns:
         PipelineExecutionResult: The result of the execution.
     """
-    if isinstance(pipeline, PipelineDefinition):
-        if isinstance(pipeline, JobDefinition):
-            error = (
-                "execute_run requires a reconstructable job but received job definition directly"
-                " instead."
-            )
-        else:
-            error = (
-                "execute_run requires a reconstructable pipeline but received pipeline definition "
-                "directly instead."
-            )
+    if isinstance(pipeline, JobDefinition):
         raise DagsterInvariantViolationError(
-            f"{error} To support hand-off to other processes please wrap your definition in a call"
+            "execute_run requires a reconstructable job but received job definition directly"
+            " instead. To support hand-off to other processes please wrap your definition in a call"
             " to reconstructable(). Learn more about reconstructable here:"
             " https://docs.dagster.io/_apidocs/execution#dagster.reconstructable"
         )
 
     check.inst_param(pipeline, "pipeline", IPipeline)
     check.inst_param(dagster_run, "dagster_run", DagsterRun)
     check.inst_param(instance, "instance", DagsterInstance)
@@ -236,33 +214,22 @@
     check.invariant(
         dagster_run.status == DagsterRunStatus.NOT_STARTED
         or dagster_run.status == DagsterRunStatus.STARTING,
         desc="Run {} ({}) in state {}, expected NOT_STARTED or STARTING".format(
             dagster_run.pipeline_name, dagster_run.run_id, dagster_run.status
         ),
     )
-    pipeline_def = pipeline.get_definition()
     if dagster_run.solids_to_execute or dagster_run.asset_selection:
-        if isinstance(pipeline_def, PipelineSubsetDefinition):
-            check.invariant(
-                dagster_run.solids_to_execute == pipeline.solids_to_execute,
-                "Cannot execute DagsterRun with solids_to_execute {solids_to_execute} that "
-                "conflicts with pipeline subset {pipeline_solids_to_execute}.".format(
-                    pipeline_solids_to_execute=str_format_set(pipeline.solids_to_execute),  # type: ignore  # (possible none)
-                    solids_to_execute=str_format_set(dagster_run.solids_to_execute),  # type: ignore  # (possible none)
-                ),
-            )
-        else:
-            # when `execute_run` is directly called, the sub pipeline hasn't been created
-            # note that when we receive the solids to execute via DagsterRun, it won't support
-            # solid selection query syntax
-            pipeline = pipeline.subset_for_execution_from_existing_pipeline(
-                frozenset(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None,
-                dagster_run.asset_selection,
-            )
+        # when `execute_run` is directly called, the sub pipeline hasn't been created
+        # note that when we receive the solids to execute via DagsterRun, it won't support
+        # solid selection query syntax
+        pipeline = pipeline.subset_for_execution_from_existing_pipeline(
+            frozenset(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None,
+            dagster_run.asset_selection,
+        )
 
     execution_plan = _get_execution_plan_from_run(pipeline, dagster_run, instance)
     if isinstance(pipeline, ReconstructablePipeline):
         pipeline = pipeline.with_repository_load_data(execution_plan.repository_load_data)
 
     output_capture: Optional[Dict[StepOutputHandle, Any]] = {}
 
@@ -501,30 +468,29 @@
         event_list=result.event_list,
         dagster_run=instance.get_run_by_id(result.run_id),
     )
 
 
 @telemetry_wrapper
 def _logged_execute_job(
-    job_arg: Union[IPipeline, PipelineDefinition],
+    job_arg: Union[IPipeline, JobDefinition],
     instance: DagsterInstance,
     run_config: Optional[Mapping[str, object]] = None,
     tags: Optional[Mapping[str, str]] = None,
     op_selection: Optional[Sequence[str]] = None,
     raise_on_error: bool = True,
     asset_selection: Optional[Sequence[AssetKey]] = None,
 ) -> PipelineExecutionResult:
     check.inst_param(instance, "instance", DagsterInstance)
 
     job_arg, repository_load_data = _job_with_repository_load_data(job_arg)
 
     (
         job_arg,
         run_config,
-        mode,
         tags,
         solids_to_execute,
         op_selection,
     ) = _check_execute_job_args(
         job_arg=job_arg,
         run_config=run_config,
         tags=tags,
@@ -532,15 +498,14 @@
     )
 
     log_repo_stats(instance=instance, pipeline=job_arg, source="execute_pipeline")
 
     dagster_run = instance.create_run_for_pipeline(
         pipeline_def=job_arg.get_definition(),
         run_config=run_config,
-        mode=mode,
         solid_selection=op_selection,
         solids_to_execute=solids_to_execute,
         tags=tags,
         pipeline_code_origin=(
             job_arg.get_python_origin() if isinstance(job_arg, ReconstructableJob) else None
         ),
         repository_load_data=repository_load_data,
@@ -552,15 +517,15 @@
         dagster_run,
         instance,
         raise_on_error=raise_on_error,
     )
 
 
 def _reexecute_job(
-    job_arg: Union[IPipeline, PipelineDefinition],
+    job_arg: Union[IPipeline, JobDefinition],
     parent_run_id: str,
     run_config: Optional[Mapping[str, object]] = None,
     step_selection: Optional[Sequence[str]] = None,
     tags: Optional[Mapping[str, str]] = None,
     instance: Optional[DagsterInstance] = None,
     raise_on_error: bool = True,
 ) -> PipelineExecutionResult:
@@ -568,15 +533,15 @@
     check.opt_sequence_param(step_selection, "step_selection", of_type=str)
 
     check.str_param(parent_run_id, "parent_run_id")
 
     with ephemeral_instance_if_missing(instance) as execute_instance:
         job_arg, repository_load_data = _job_with_repository_load_data(job_arg)
 
-        (job_arg, run_config, mode, tags, _, _) = _check_execute_job_args(
+        (job_arg, run_config, tags, _, _) = _check_execute_job_args(
             job_arg=job_arg,
             run_config=run_config,
             tags=tags,
         )
 
         parent_dagster_run = execute_instance.get_run_by_id(parent_run_id)
         if parent_dagster_run is None:
@@ -588,30 +553,28 @@
 
         execution_plan: Optional[ExecutionPlan] = None
         # resolve step selection DSL queries using parent execution information
         if step_selection:
             execution_plan = _resolve_reexecute_step_selection(
                 execute_instance,
                 job_arg,
-                mode,
                 run_config,
                 cast(DagsterRun, parent_dagster_run),
                 step_selection,
             )
 
         if parent_dagster_run.asset_selection:
             job_arg = job_arg.subset_for_execution(
                 solid_selection=None, asset_selection=parent_dagster_run.asset_selection
             )
 
         dagster_run = execute_instance.create_run_for_pipeline(
             pipeline_def=job_arg.get_definition(),
             execution_plan=execution_plan,
             run_config=run_config,
-            mode=mode,
             tags=tags,
             solid_selection=parent_dagster_run.solid_selection,
             asset_selection=parent_dagster_run.asset_selection,
             solids_to_execute=parent_dagster_run.solids_to_execute,
             root_run_id=parent_dagster_run.root_run_id or parent_dagster_run.run_id,
             parent_run_id=parent_dagster_run.run_id,
             pipeline_code_origin=(
@@ -689,17 +652,17 @@
             dagster_run=dagster_run,
             instance=instance,
             retry_mode=retry_mode,
         )
     )
 
 
-def _check_pipeline(job_arg: Union[PipelineDefinition, IPipeline]) -> IPipeline:
+def _check_pipeline(job_arg: Union[JobDefinition, IPipeline]) -> IPipeline:
     # backcompat
-    if isinstance(job_arg, PipelineDefinition):
+    if isinstance(job_arg, JobDefinition):
         job_arg = InMemoryPipeline(job_arg)
 
     check.inst_param(job_arg, "job_arg", IPipeline)
     return job_arg
 
 
 def _get_execution_plan_from_run(
@@ -724,60 +687,57 @@
             dagster_run.pipeline_name,
             execution_plan_snapshot,
         )
 
     return create_execution_plan(
         pipeline,
         run_config=dagster_run.run_config,
-        mode=dagster_run.mode,
         step_keys_to_execute=dagster_run.step_keys_to_execute,
         instance_ref=instance.get_ref() if instance.is_persistent else None,
         repository_load_data=execution_plan_snapshot.repository_load_data
         if execution_plan_snapshot
         else None,
         known_state=execution_plan_snapshot.initial_known_state
         if execution_plan_snapshot
         else None,
     )
 
 
 def create_execution_plan(
-    pipeline: Union[IPipeline, PipelineDefinition],
+    pipeline: Union[IPipeline, JobDefinition],
     run_config: Optional[Mapping[str, object]] = None,
-    mode: Optional[str] = None,
     step_keys_to_execute: Optional[Sequence[str]] = None,
     known_state: Optional[KnownExecutionState] = None,
     instance_ref: Optional[InstanceRef] = None,
     tags: Optional[Mapping[str, str]] = None,
     repository_load_data: Optional[RepositoryLoadData] = None,
 ) -> ExecutionPlan:
     pipeline = _check_pipeline(pipeline)
 
     # If you have repository_load_data, make sure to use it when building plan
     if isinstance(pipeline, ReconstructablePipeline) and repository_load_data is not None:
         pipeline = pipeline.with_repository_load_data(repository_load_data)
 
     pipeline_def = pipeline.get_definition()
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
     run_config = check.opt_mapping_param(run_config, "run_config", key_type=str)
-    mode = check.opt_str_param(mode, "mode", default=pipeline_def.get_default_mode_name())
     check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
     check.opt_inst_param(instance_ref, "instance_ref", InstanceRef)
     tags = check.opt_mapping_param(tags, "tags", key_type=str, value_type=str)
     known_state = check.opt_inst_param(
         known_state,
         "known_state",
         KnownExecutionState,
         default=KnownExecutionState(),
     )
     repository_load_data = check.opt_inst_param(
         repository_load_data, "repository_load_data", RepositoryLoadData
     )
 
-    resolved_run_config = ResolvedRunConfig.build(pipeline_def, run_config, mode=mode)
+    resolved_run_config = ResolvedRunConfig.build(pipeline_def, run_config)
 
     return ExecutionPlan.build(
         pipeline,
         resolved_run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
         instance_ref=instance_ref,
@@ -934,87 +894,80 @@
             finally:
                 for event in self.execution_context_manager.shutdown_context():
                     if not generator_closed:
                         yield event
 
 
 def _check_execute_job_args(
-    job_arg: Union[PipelineDefinition, IPipeline],
+    job_arg: Union[JobDefinition, IPipeline],
     run_config: Optional[Mapping[str, object]],
     tags: Optional[Mapping[str, str]],
     op_selection: Optional[Sequence[str]] = None,
 ) -> Tuple[
     IPipeline,
     Optional[Mapping],
-    Optional[str],
     Mapping[str, str],
     Optional[AbstractSet[str]],
     Optional[Sequence[str]],
 ]:
     job_arg = _check_pipeline(job_arg)
     job_def = job_arg.get_definition()
     check.inst_param(job_def, "job_def", JobDefinition)
 
     run_config = check.opt_mapping_param(run_config, "run_config")
 
     tags = check.opt_mapping_param(tags, "tags", key_type=str)
     check.opt_sequence_param(op_selection, "solid_selection", of_type=str)
 
-    mode = job_def.get_default_mode_name()
-
     tags = merge_dicts(job_def.tags, tags)
 
     # generate pipeline subset from the given solid_selection
     if op_selection:
         job_arg = job_arg.subset_for_execution(op_selection)
 
     return (
         job_arg,
         run_config,
-        mode,
         tags,
         job_arg.solids_to_execute,
         op_selection,
     )
 
 
 def _resolve_reexecute_step_selection(
     instance: DagsterInstance,
     pipeline: IPipeline,
-    mode: Optional[str],
     run_config: Optional[Mapping],
     parent_dagster_run: DagsterRun,
     step_selection: Sequence[str],
 ) -> ExecutionPlan:
     if parent_dagster_run.solid_selection:
         pipeline = pipeline.subset_for_execution(parent_dagster_run.solid_selection, None)
 
     state = KnownExecutionState.build_for_reexecution(instance, parent_dagster_run)
 
     parent_plan = create_execution_plan(
         pipeline,
         parent_dagster_run.run_config,
-        mode,
         known_state=state,
     )
     step_keys_to_execute = parse_step_selection(parent_plan.get_all_step_deps(), step_selection)
     execution_plan = create_execution_plan(
         pipeline,
         run_config,
-        mode,
         step_keys_to_execute=list(step_keys_to_execute),
         known_state=state.update_for_step_selection(step_keys_to_execute),
         tags=parent_dagster_run.tags,
     )
     return execution_plan
 
 
 def _job_with_repository_load_data(
-    job_arg: Union[PipelineDefinition, IPipeline],
-) -> Tuple[Union[PipelineDefinition, IPipeline], Optional[RepositoryLoadData]]:
+    job_arg: Union[JobDefinition, IPipeline],
+) -> Tuple[Union[JobDefinition, IPipeline], Optional[RepositoryLoadData]]:
     """For ReconstructablePipeline, generate and return any required RepositoryLoadData, alongside
     a ReconstructablePipeline with this repository load data baked in.
     """
     if isinstance(job_arg, ReconstructablePipeline):
         # Unless this ReconstructablePipeline alread has repository_load_data attached, this will
         # force the repository_load_data to be computed from scratch.
         repository_load_data = job_arg.repository.get_definition().repository_load_data
```

### Comparing `dagster-1.3.1/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.2/dagster/_core/execution/asset_backfill.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     build_run_requests,
     find_parent_materialized_asset_partitions,
 )
 from dagster._core.definitions.asset_selection import AssetSelection
 from dagster._core.definitions.assets_job import is_base_asset_job_name
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
-from dagster._core.definitions.mode import DEFAULT_MODE_NAME
 from dagster._core.definitions.partition import PartitionsSubset
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.selector import PipelineSelector
 from dagster._core.errors import DagsterBackfillFailedError
 from dagster._core.events import DagsterEventType
 from dagster._core.host_representation import (
     ExternalExecutionPlan,
@@ -125,14 +124,32 @@
 
     def get_num_targeted_partitions_by_asset_key(self) -> Mapping[AssetKey, int]:
         return {
             asset_key: len(subset)
             for asset_key, subset in self.target_subset.partitions_subsets_by_asset_key.items()
         }
 
+    def get_targeted_partitioned_asset_keys_topological_order(self) -> Sequence[AssetKey]:
+        """Returns a topological ordering of partitioned asset keys targeted by the backfill.
+
+        Orders keys in the same topological level alphabetically.
+        """
+        toposorted_keys = self.target_subset.asset_graph.toposort_asset_keys()
+
+        targeted_toposorted_keys = []
+        for level_keys in toposorted_keys:
+            for key in sorted(level_keys):
+                if (
+                    key in self.target_subset.asset_keys
+                    and self.target_subset.asset_graph.get_partitions_def(key) is not None
+                ):
+                    targeted_toposorted_keys.append(key)
+
+        return targeted_toposorted_keys
+
     def get_partitions_status_counts_by_asset_key(
         self,
     ) -> Mapping[AssetKey, Mapping[BackfillPartitionsStatus, int]]:
         """Returns a mapping from asset key to a mapping from status to count of partitions in that
         status.
 
         Only includes assets that are partitioned.
@@ -212,55 +229,71 @@
             latest_storage_id=storage_dict["latest_storage_id"],
         )
 
     @classmethod
     def from_asset_partitions(
         cls,
         asset_graph: AssetGraph,
-        partition_names: Sequence[str],
+        partition_names: Optional[Sequence[str]],
         asset_selection: Sequence[AssetKey],
         dynamic_partitions_store: DynamicPartitionsStore,
+        all_partitions: bool,
     ) -> "AssetBackfillData":
-        partitioned_asset_keys = {
-            asset_key
-            for asset_key in asset_selection
-            if asset_graph.get_partitions_def(asset_key) is not None
-        }
-
-        root_partitioned_asset_keys = (
-            AssetSelection.keys(*partitioned_asset_keys).sources().resolve(asset_graph)
+        check.invariant(
+            partition_names is None or all_partitions is False,
+            "Can't provide both a set of partitions and all_partitions=True",
         )
-        root_partitions_defs = {
-            asset_graph.get_partitions_def(asset_key) for asset_key in root_partitioned_asset_keys
-        }
-        if len(root_partitions_defs) > 1:
-            raise DagsterBackfillFailedError(
-                "All the assets at the root of the backfill must have the same PartitionsDefinition"
+
+        if all_partitions:
+            target_subset = AssetGraphSubset.from_asset_keys(
+                asset_selection, asset_graph, dynamic_partitions_store
             )
+        elif partition_names is not None:
+            partitioned_asset_keys = {
+                asset_key
+                for asset_key in asset_selection
+                if asset_graph.get_partitions_def(asset_key) is not None
+            }
 
-        root_partitions_def = next(iter(root_partitions_defs))
-        if not root_partitions_def:
-            raise DagsterBackfillFailedError(
-                "If assets within the backfill have different partitionings, then root assets"
-                " must be partitioned"
+            root_partitioned_asset_keys = (
+                AssetSelection.keys(*partitioned_asset_keys).sources().resolve(asset_graph)
             )
+            root_partitions_defs = {
+                asset_graph.get_partitions_def(asset_key)
+                for asset_key in root_partitioned_asset_keys
+            }
+            if len(root_partitions_defs) > 1:
+                raise DagsterBackfillFailedError(
+                    "All the assets at the root of the backfill must have the same"
+                    " PartitionsDefinition"
+                )
 
-        root_partitions_subset = root_partitions_def.subset_with_partition_keys(partition_names)
-        target_subset = AssetGraphSubset(
-            asset_graph, non_partitioned_asset_keys=set(asset_selection) - partitioned_asset_keys
-        )
-        for root_asset_key in root_partitioned_asset_keys:
-            target_subset |= asset_graph.bfs_filter_subsets(
-                dynamic_partitions_store,
-                lambda asset_key, _: asset_key in partitioned_asset_keys,
-                AssetGraphSubset(
-                    asset_graph,
-                    partitions_subsets_by_asset_key={root_asset_key: root_partitions_subset},
-                ),
+            root_partitions_def = next(iter(root_partitions_defs))
+            if not root_partitions_def:
+                raise DagsterBackfillFailedError(
+                    "If assets within the backfill have different partitionings, then root assets"
+                    " must be partitioned"
+                )
+
+            root_partitions_subset = root_partitions_def.subset_with_partition_keys(partition_names)
+            target_subset = AssetGraphSubset(
+                asset_graph,
+                non_partitioned_asset_keys=set(asset_selection) - partitioned_asset_keys,
             )
+            for root_asset_key in root_partitioned_asset_keys:
+                target_subset |= asset_graph.bfs_filter_subsets(
+                    dynamic_partitions_store,
+                    lambda asset_key, _: asset_key in partitioned_asset_keys,
+                    AssetGraphSubset(
+                        asset_graph,
+                        partitions_subsets_by_asset_key={root_asset_key: root_partitions_subset},
+                    ),
+                )
+        else:
+            check.failed("Either partition_names must not be None or all_partitions must be True")
 
         return cls.empty(target_subset)
 
     def serialize(self, dynamic_partitions_store: DynamicPartitionsStore) -> str:
         storage_dict = {
             "requested_runs_for_target_roots": self.requested_runs_for_target_roots,
             "serialized_target_subset": self.target_subset.to_storage_dict(
@@ -386,15 +419,14 @@
         code_location = workspace.get_code_location(repo_handle.code_location_origin.location_name)
 
         external_pipeline = code_location.get_external_pipeline(pipeline_selector)
 
         external_execution_plan = code_location.get_external_execution_plan(
             external_pipeline,
             {},
-            DEFAULT_MODE_NAME,
             step_keys_to_execute=None,
             known_state=None,
             instance=instance,
         )
         pipeline_and_execution_plan_cache[selector_id] = (
             external_pipeline,
             external_execution_plan,
@@ -407,15 +439,14 @@
         execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
         parent_pipeline_snapshot=external_pipeline.parent_pipeline_snapshot,
         pipeline_name=external_pipeline.name,
         run_id=None,
         solids_to_execute=None,
         solid_selection=None,
         run_config={},
-        mode=DEFAULT_MODE_NAME,
         step_keys_to_execute=None,
         tags=run_request.tags,
         root_run_id=None,
         parent_run_id=None,
         status=DagsterRunStatus.NOT_STARTED,
         external_pipeline_origin=external_pipeline.get_external_origin(),
         pipeline_code_origin=external_pipeline.get_python_origin(),
```

### Comparing `dagster-1.3.1/dagster/_core/execution/backfill.py` & `dagster-1.3.2/dagster/_core/execution/backfill.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dagster._core.definitions.partition import PartitionsSubset
 from dagster._core.errors import (
     DagsterDefinitionChangedDeserializationError,
 )
 from dagster._core.execution.bulk_actions import BulkActionType
 from dagster._core.host_representation.origin import ExternalPartitionSetOrigin
 from dagster._core.instance import DynamicPartitionsStore
+from dagster._core.storage.tags import USER_TAG
 from dagster._core.workspace.workspace import IWorkspace
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo
 
 from .asset_backfill import AssetBackfillData, BackfillPartitionsStatus
 
 
@@ -115,25 +116,34 @@
     @property
     def partition_set_name(self) -> Optional[str]:
         if self.partition_set_origin is None:
             return None
 
         return self.partition_set_origin.partition_set_name
 
+    @property
+    def user(self) -> Optional[str]:
+        if self.tags:
+            return self.tags.get(USER_TAG)
+        return None
+
     def is_valid_serialization(self, workspace: IWorkspace) -> bool:
         if self.serialized_asset_backfill_data is not None:
             return AssetBackfillData.is_valid_serialization(
                 self.serialized_asset_backfill_data, ExternalAssetGraph.from_workspace(workspace)
             )
         else:
             return True
 
     def get_partitions_status_counts_and_totals_by_asset(
         self, workspace: IWorkspace
     ) -> Mapping[AssetKey, Tuple[Mapping[BackfillPartitionsStatus, int], int]]:
+        """Returns a list of tuples of the form (asset_key, partitions_status_counts, total_partitions)
+        in topological order of the asset graph. Includes only partitioned assets.
+        """
         if not self.is_valid_serialization(workspace):
             return {}
 
         if self.serialized_asset_backfill_data is not None:
             try:
                 asset_backfill_data = AssetBackfillData.from_serialized(
                     self.serialized_asset_backfill_data,
@@ -144,26 +154,32 @@
 
             partitions_status_counts_by_asset_key = (
                 asset_backfill_data.get_partitions_status_counts_by_asset_key()
             )
             num_targeted_partitions_by_asset_key = (
                 asset_backfill_data.get_num_targeted_partitions_by_asset_key()
             )
+            topological_order = (
+                asset_backfill_data.get_targeted_partitioned_asset_keys_topological_order()
+            )
 
             check.invariant(
                 partitions_status_counts_by_asset_key.keys()
                 == num_targeted_partitions_by_asset_key.keys()
             )
+            check.invariant(
+                set(partitions_status_counts_by_asset_key.keys()) == set(topological_order)
+            )
 
             return {
                 asset_key: (
                     partitions_status_counts_by_asset_key[asset_key],
                     num_targeted_partitions_by_asset_key[asset_key],
                 )
-                for asset_key in partitions_status_counts_by_asset_key
+                for asset_key in topological_order
             }
 
         else:
             return {}
 
     def get_target_root_partitions_subset(
         self, workspace: IWorkspace
@@ -317,19 +333,20 @@
         )
 
     @classmethod
     def from_asset_partitions(
         cls,
         backfill_id: str,
         asset_graph: AssetGraph,
-        partition_names: Sequence[str],
+        partition_names: Optional[Sequence[str]],
         asset_selection: Sequence[AssetKey],
         backfill_timestamp: float,
         tags: Mapping[str, str],
         dynamic_partitions_store: DynamicPartitionsStore,
+        all_partitions: bool,
     ) -> "PartitionBackfill":
         """If all the selected assets that have PartitionsDefinitions have the same partitioning, then
         the backfill will target the provided partition_names for all those assets.
 
         Otherwise, the backfill must consist of a partitioned "anchor" asset and a set of other
         assets that descend from it. In that case, the backfill will target the partition_names of
         the anchor asset, as well as all partitions of other selected assets that are downstream
@@ -343,9 +360,10 @@
             backfill_timestamp=backfill_timestamp,
             asset_selection=asset_selection,
             serialized_asset_backfill_data=AssetBackfillData.from_asset_partitions(
                 asset_graph=asset_graph,
                 partition_names=partition_names,
                 asset_selection=asset_selection,
                 dynamic_partitions_store=dynamic_partitions_store,
+                all_partitions=all_partitions,
             ).serialize(dynamic_partitions_store=dynamic_partitions_store),
         )
```

### Comparing `dagster-1.3.1/dagster/_core/execution/build_resources.py` & `dagster-1.3.2/dagster/_core/execution/build_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,9 +126,8 @@
             resource_defs[resource_key] = resource.get_resource_definition()
         elif isinstance(resource, ResourceDefinition):
             resource_defs[resource_key] = resource
         elif isinstance(resource, IOManager):
             resource_defs[resource_key] = IOManagerDefinition.hardcoded_io_manager(resource)
         else:
             resource_defs[resource_key] = ResourceDefinition.hardcoded_resource(resource)
-
     return resource_defs
```

### Comparing `dagster-1.3.1/dagster/_core/execution/compute_logs.py` & `dagster-1.3.2/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/context/compute.py` & `dagster-1.3.2/dagster/_core/execution/context/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,17 @@
     AssetKey,
     AssetMaterialization,
     AssetObservation,
     ExpectationResult,
     UserEvent,
 )
 from dagster._core.definitions.job_definition import JobDefinition
-from dagster._core.definitions.mode import ModeDefinition
 from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.definitions.step_launcher import StepLauncher
 from dagster._core.definitions.time_window_partitions import TimeWindow
 from dagster._core.errors import (
     DagsterInvalidPropertyError,
     DagsterInvariantViolationError,
 )
 from dagster._core.events import DagsterEvent
@@ -188,15 +186,15 @@
     @public
     @property
     def run_config(self) -> Mapping[str, object]:
         """dict: The run config for the current execution."""
         return self._step_execution_context.run_config
 
     @property
-    def pipeline_def(self) -> PipelineDefinition:
+    def pipeline_def(self) -> JobDefinition:
         """PipelineDefinition: The currently executing pipeline."""
         return self._step_execution_context.pipeline_def
 
     @public
     @property
     def job_def(self) -> JobDefinition:
         """JobDefinition: The currently executing job."""
@@ -216,19 +214,14 @@
 
     @public
     @property
     def job_name(self) -> str:
         """str: The name of the currently executing job."""
         return self.pipeline_name
 
-    @property
-    def mode_def(self) -> ModeDefinition:
-        """ModeDefinition: The mode of the current execution."""
-        return self._step_execution_context.mode_def
-
     @public
     @property
     def log(self) -> DagsterLogManager:
         """DagsterLogManager: The log manager available in the execution context."""
         return self._step_execution_context.log
 
     @property
```

### Comparing `dagster-1.3.1/dagster/_core/execution/context/hook.py` & `dagster-1.3.2/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/context/init.py` & `dagster-1.3.2/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/context/input.py` & `dagster-1.3.2/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/context/invocation.py` & `dagster-1.3.2/dagster/_core/execution/context/invocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 from dagster._core.definitions.events import (
     AssetMaterialization,
     AssetObservation,
     ExpectationResult,
     UserEvent,
 )
 from dagster._core.definitions.hook_definition import HookDefinition
-from dagster._core.definitions.mode import ModeDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.op_definition import OpDefinition
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.definitions.resource_definition import (
     IContainsGenerator,
     ResourceDefinition,
     Resources,
     ScopedResourcesBuilder,
 )
 from dagster._core.definitions.resource_requirement import ensure_requirements_satisfied
@@ -183,26 +182,22 @@
         return "EPHEMERAL"
 
     @property
     def run_config(self) -> dict:
         raise DagsterInvalidPropertyError(_property_msg("run_config", "property"))
 
     @property
-    def pipeline_def(self) -> PipelineDefinition:
+    def pipeline_def(self) -> JobDefinition:
         raise DagsterInvalidPropertyError(_property_msg("pipeline_def", "property"))
 
     @property
     def pipeline_name(self) -> str:
         raise DagsterInvalidPropertyError(_property_msg("pipeline_name", "property"))
 
     @property
-    def mode_def(self) -> ModeDefinition:
-        raise DagsterInvalidPropertyError(_property_msg("mode_def", "property"))
-
-    @property
     def log(self) -> DagsterLogManager:
         """DagsterLogManager: A console manager constructed for this context."""
         return self._log
 
     @property
     def node_handle(self) -> NodeHandle:
         raise DagsterInvalidPropertyError(_property_msg("solid_handle", "property"))
@@ -472,26 +467,22 @@
         run_config: Dict[str, object] = {}
         if self._op_config:
             run_config["ops"] = {self._op_def.name: {"config": self._op_config}}
         run_config["resources"] = self._resources_config
         return run_config
 
     @property
-    def pipeline_def(self) -> PipelineDefinition:
+    def pipeline_def(self) -> JobDefinition:
         raise DagsterInvalidPropertyError(_property_msg("pipeline_def", "property"))
 
     @property
     def pipeline_name(self) -> str:
         raise DagsterInvalidPropertyError(_property_msg("pipeline_name", "property"))
 
     @property
-    def mode_def(self) -> ModeDefinition:
-        raise DagsterInvalidPropertyError(_property_msg("mode_def", "property"))
-
-    @property
     def log(self) -> DagsterLogManager:
         """DagsterLogManager: A console manager constructed for this context."""
         return self._log
 
     @property
     def node_handle(self) -> NodeHandle:
         raise DagsterInvalidPropertyError(_property_msg("solid_handle", "property"))
```

### Comparing `dagster-1.3.1/dagster/_core/execution/context/logger.py` & `dagster-1.3.2/dagster/_core/execution/context/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any, Optional
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.logger_definition import LoggerDefinition
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.errors import DagsterInvariantViolationError
 
 from .output import RUN_ID_PLACEHOLDER
 
 
 class InitLoggerContext:
     """The context object available as the argument to the initialization function of a :py:class:`dagster.LoggerDefinition`.
@@ -35,29 +34,29 @@
 
     """
 
     def __init__(
         self,
         logger_config: Any,
         logger_def: Optional[LoggerDefinition] = None,
-        pipeline_def: Optional[PipelineDefinition] = None,
+        pipeline_def: Optional[JobDefinition] = None,
         run_id: Optional[str] = None,
     ):
         self._logger_config = logger_config
-        self._pipeline_def = check.opt_inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+        self._pipeline_def = check.opt_inst_param(pipeline_def, "pipeline_def", JobDefinition)
         self._logger_def = check.opt_inst_param(logger_def, "logger_def", LoggerDefinition)
         self._run_id = check.opt_str_param(run_id, "run_id")
 
     @public
     @property
     def logger_config(self) -> Any:
         return self._logger_config
 
     @property
-    def pipeline_def(self) -> Optional[PipelineDefinition]:
+    def pipeline_def(self) -> Optional[JobDefinition]:
         return self._pipeline_def
 
     @public
     @property
     def job_def(self) -> Optional[JobDefinition]:
         if not self._pipeline_def:
             return None
@@ -84,15 +83,15 @@
 
     Represents a context whose config has not yet been validated against a logger definition, hence
     the inability to access the `logger_def` attribute. When an instance of
     ``UnboundInitLoggerContext`` is passed to ``LoggerDefinition.initialize``, config is validated,
     and it is subsumed into an `InitLoggerContext`, which contains the logger_def validated against.
     """
 
-    def __init__(self, logger_config: Any, pipeline_def: Optional[PipelineDefinition]):
+    def __init__(self, logger_config: Any, pipeline_def: Optional[JobDefinition]):
         super(UnboundInitLoggerContext, self).__init__(
             logger_config, logger_def=None, pipeline_def=pipeline_def, run_id=None
         )
 
     @property
     def logger_def(self) -> LoggerDefinition:
         raise DagsterInvariantViolationError(
```

### Comparing `dagster-1.3.1/dagster/_core/execution/context/output.py` & `dagster-1.3.2/dagster/_core/execution/context/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 )
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
 from dagster._core.definitions.time_window_partitions import TimeWindow
 from dagster._core.errors import DagsterInvalidMetadata, DagsterInvariantViolationError
 from dagster._core.execution.plan.utils import build_resources_for_manager
 
 if TYPE_CHECKING:
-    from dagster._core.definitions import PartitionsDefinition, PipelineDefinition
+    from dagster._core.definitions import JobDefinition, PartitionsDefinition
     from dagster._core.definitions.op_definition import OpDefinition
     from dagster._core.definitions.resource_definition import Resources
     from dagster._core.events import DagsterEvent
     from dagster._core.execution.context.system import StepExecutionContext
     from dagster._core.execution.plan.outputs import StepOutputHandle
     from dagster._core.execution.plan.plan import ExecutionPlan
     from dagster._core.log_manager import DagsterLogManager
@@ -706,15 +706,15 @@
         result = self._user_generated_metadata
         self._user_generated_metadata = {}
         return result or {}
 
 
 def get_output_context(
     execution_plan: "ExecutionPlan",
-    pipeline_def: "PipelineDefinition",
+    pipeline_def: "JobDefinition",
     resolved_run_config: "ResolvedRunConfig",
     step_output_handle: "StepOutputHandle",
     run_id: Optional[str],
     log_manager: Optional["DagsterLogManager"],
     step_context: Optional["StepExecutionContext"],
     resources: Optional["Resources"],
     version: Optional[str],
@@ -773,15 +773,15 @@
         resources=resources,
         asset_info=asset_info,
         warn_on_step_context_use=warn_on_step_context_use,
     )
 
 
 def step_output_version(
-    pipeline_def: "PipelineDefinition",
+    pipeline_def: "JobDefinition",
     execution_plan: "ExecutionPlan",
     resolved_run_config: "ResolvedRunConfig",
     step_output_handle: "StepOutputHandle",
 ) -> Optional[str]:
     from dagster._core.execution.resolve_versions import resolve_step_output_versions
 
     step_output_versions = resolve_step_output_versions(
```

### Comparing `dagster-1.3.1/dagster/_core/execution/context/system.py` & `dagster-1.3.2/dagster/_core/execution/context/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,21 @@
 )
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.dependency import OpNode
 from dagster._core.definitions.events import AssetKey, AssetLineageInfo
 from dagster._core.definitions.hook_definition import HookDefinition
-from dagster._core.definitions.mode import ModeDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition import PartitionsDefinition, PartitionsSubset
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
 from dagster._core.definitions.partition_mapping import infer_partition_mapping
 from dagster._core.definitions.pipeline_base import IPipeline
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.definitions.policy import RetryPolicy
 from dagster._core.definitions.reconstruct import ReconstructablePipeline
 from dagster._core.definitions.resource_definition import ScopedResourcesBuilder
 from dagster._core.definitions.step_launcher import StepLauncher
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
@@ -63,15 +62,14 @@
 from .output import OutputContext, get_output_context
 
 if TYPE_CHECKING:
     from dagster._core.definitions.data_version import (
         DataVersion,
     )
     from dagster._core.definitions.dependency import NodeHandle
-    from dagster._core.definitions.job_definition import JobDefinition
     from dagster._core.definitions.resource_definition import Resources
     from dagster._core.event_api import EventLogRecord
     from dagster._core.execution.plan.plan import ExecutionPlan
     from dagster._core.execution.plan.state import KnownExecutionState
     from dagster._core.instance import DagsterInstance
 
     from .hook import HookContext
@@ -182,16 +180,15 @@
 
     This object contains information that requires access to user code, such as the pipeline
     definition and resources.
     """
 
     scoped_resources_builder: ScopedResourcesBuilder
     resolved_run_config: ResolvedRunConfig
-    pipeline_def: PipelineDefinition
-    mode_def: ModeDefinition
+    pipeline_def: JobDefinition
 
 
 class IStepContext(IPlanContext):
     """Interface to represent data to be available during either step orchestration or execution."""
 
     @property
     @abstractmethod
@@ -329,15 +326,15 @@
             log_manager=self._log_manager.with_tags(**step.logging_tags),
             step=step,
             output_capture=self.output_capture,
             known_state=known_state,
         )
 
     @property
-    def pipeline_def(self) -> PipelineDefinition:
+    def pipeline_def(self) -> JobDefinition:
         return self._execution_data.pipeline_def
 
     @property
     def resolved_run_config(self) -> ResolvedRunConfig:
         return self._execution_data.resolved_run_config
 
     @property
@@ -554,28 +551,20 @@
         return self._step_launcher
 
     @property
     def op_def(self) -> OpDefinition:
         return self.solid.definition
 
     @property
-    def pipeline_def(self) -> PipelineDefinition:
+    def pipeline_def(self) -> JobDefinition:
         return self._execution_data.pipeline_def
 
     @property
     def job_def(self) -> "JobDefinition":
-        check.invariant(
-            self._execution_data.pipeline_def.is_job,
-            "Attempted to call job_def property for a pipeline definition.",
-        )
-        return cast("JobDefinition", self._execution_data.pipeline_def)
-
-    @property
-    def mode_def(self) -> ModeDefinition:
-        return self._execution_data.mode_def
+        return self._execution_data.pipeline_def
 
     @property
     def solid(self) -> OpNode:
         return self.pipeline_def.get_op(self._step.node_handle)
 
     @property
     def solid_retry_policy(self) -> Optional[RetryPolicy]:
@@ -795,15 +784,15 @@
         # computations. for example, in backfills, with fixed path io manager, we allow users to
         # "re-execute" runs with steps where the outputs weren't previously stored by dagster.
 
         # Warn about this special case because it will also reach here when all previous runs have
         # skipped yielding this output. From the logs, we have no easy way to differentiate the fixed
         # path case and the skipping case, until we record the skipping info in KnownExecutionState,
         # i.e. resolve https://github.com/dagster-io/dagster/issues/3511
-        self.log.warn(
+        self.log.warning(
             f"No previously stored outputs found for source {step_output_handle}. "
             "This is either because you are using an IO Manager that does not depend on run ID, "
             "or because all the previous runs have skipped the output in conditional execution."
         )
         return None
 
     def _should_load_from_previous_runs(self, step_output_handle: StepOutputHandle) -> bool:
```

### Comparing `dagster-1.3.1/dagster/_core/execution/context_creation_pipeline.py` & `dagster-1.3.2/dagster/_core/execution/context_creation_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import dagster._check as check
-from dagster._core.definitions import ExecutorDefinition, ModeDefinition, PipelineDefinition
+from dagster._core.definitions import ExecutorDefinition, JobDefinition
 from dagster._core.definitions.executor_definition import check_cross_process_constraints
 from dagster._core.definitions.pipeline_base import IPipeline
 from dagster._core.definitions.resource_definition import ScopedResourcesBuilder
 from dagster._core.errors import DagsterError, DagsterUserCodeExecutionError
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.memoization import validate_reexecution_memoization
 from dagster._core.execution.plan.plan import ExecutionPlan
@@ -71,76 +71,50 @@
                     logger_config, logger_def, run_id=dagster_run.run_id if dagster_run else None
                 )
             )
         )
     return DagsterLogManager.create(loggers=loggers, dagster_run=dagster_run, instance=instance)
 
 
-def executor_def_from_config(
-    mode_definition: ModeDefinition, resolved_run_config: ResolvedRunConfig
-) -> ExecutorDefinition:
-    selected_executor = resolved_run_config.execution.execution_engine_name
-    if selected_executor is None:
-        if len(mode_definition.executor_defs) == 1:
-            return mode_definition.executor_defs[0]
-
-        check.failed(
-            f"No executor selected but there are {len(mode_definition.executor_defs)} options."
-        )
-
-    else:
-        for executor_def in mode_definition.executor_defs:
-            if executor_def.name == selected_executor:
-                return executor_def
-
-        check.failed(
-            f'Could not find executor "{selected_executor}". This should have been caught at config'
-            " validation time."
-        )
-
-
 # This represents all the data that is passed *into* context creation process.
 # The remainder of the objects generated (e.g. loggers, resources) are created
 # using user-defined code that may fail at runtime and result in the emission
 # of a pipeline init failure events. The data in this object are passed all
 # over the place during the context creation process so grouping here for
 # ease of argument passing etc.
 class ContextCreationData(NamedTuple):
     pipeline: IPipeline
     resolved_run_config: ResolvedRunConfig
     dagster_run: DagsterRun
-    mode_def: ModeDefinition
     executor_def: ExecutorDefinition
     instance: DagsterInstance
     resource_keys_to_init: AbstractSet[str]
     execution_plan: ExecutionPlan
 
     @property
-    def pipeline_def(self) -> PipelineDefinition:
+    def pipeline_def(self) -> JobDefinition:
         return self.pipeline.get_definition()
 
 
 def create_context_creation_data(
     pipeline: IPipeline,
     execution_plan: ExecutionPlan,
     run_config: Mapping[str, object],
     dagster_run: DagsterRun,
     instance: DagsterInstance,
 ) -> "ContextCreationData":
     pipeline_def = pipeline.get_definition()
-    resolved_run_config = ResolvedRunConfig.build(pipeline_def, run_config, mode=dagster_run.mode)
+    resolved_run_config = ResolvedRunConfig.build(pipeline_def, run_config)
 
-    mode_def = pipeline_def.get_mode_definition(dagster_run.mode)
-    executor_def = executor_def_from_config(mode_def, resolved_run_config)
+    executor_def = pipeline_def.executor_def
 
     return ContextCreationData(
         pipeline=pipeline,
         resolved_run_config=resolved_run_config,
         dagster_run=dagster_run,
-        mode_def=mode_def,
         executor_def=executor_def,
         instance=instance,
         resource_keys_to_init=get_required_resource_keys_to_init(
             execution_plan, pipeline_def, resolved_run_config
         ),
         execution_plan=execution_plan,
     )
@@ -163,17 +137,14 @@
     context_creation_data: "ContextCreationData",
     scoped_resources_builder: ScopedResourcesBuilder,
 ) -> ExecutionData:
     return ExecutionData(
         scoped_resources_builder=scoped_resources_builder,
         resolved_run_config=context_creation_data.resolved_run_config,
         pipeline_def=context_creation_data.pipeline_def,
-        mode_def=context_creation_data.pipeline_def.get_mode_definition(
-            context_creation_data.resolved_run_config.mode
-        ),
     )
 
 
 TContextType = TypeVar("TContextType", bound=IPlanContext)
 
 
 class ExecutionContextManager(Generic[TContextType], ABC):
@@ -240,17 +211,15 @@
         execution_plan,
         run_config,
         dagster_run,
         instance,
     )
 
     log_manager = create_log_manager(context_creation_data)
-    resource_defs = pipeline_def.get_required_resource_defs_for_mode(
-        check.not_none(context_creation_data.resolved_run_config.mode)
-    )
+    resource_defs = pipeline_def.get_required_resource_defs()
 
     resources_manager = scoped_resources_builder_cm(
         resource_defs=resource_defs,
         resource_configs=context_creation_data.resolved_run_config.resources,
         log_manager=log_manager,
         execution_plan=execution_plan,
         dagster_run=context_creation_data.dagster_run,
@@ -474,28 +443,27 @@
 
 
 def create_log_manager(
     context_creation_data: ContextCreationData,
 ) -> DagsterLogManager:
     check.inst_param(context_creation_data, "context_creation_data", ContextCreationData)
 
-    pipeline_def, mode_def, resolved_run_config, dagster_run = (
+    pipeline_def, resolved_run_config, dagster_run = (
         context_creation_data.pipeline_def,
-        context_creation_data.mode_def,
         context_creation_data.resolved_run_config,
         context_creation_data.dagster_run,
     )
 
     # The following logic is tightly coupled to the processing of logger config in
     # python_modules/dagster/dagster/_core/system_config/objects.py#config_map_loggers
     # Changes here should be accompanied checked against that function, which applies config mapping
     # via ConfigurableDefinition (@configured) to incoming logger configs. See docstring for more details.
 
     loggers = []
-    for logger_key, logger_def in mode_def.loggers.items() or default_loggers().items():
+    for logger_key, logger_def in pipeline_def.loggers.items() or default_loggers().items():
         if logger_key in resolved_run_config.loggers:
             loggers.append(
                 logger_def.logger_fn(
                     InitLoggerContext(
                         resolved_run_config.loggers.get(logger_key, {}).get("config"),
                         logger_def,
                         pipeline_def=pipeline_def,
```

### Comparing `dagster-1.3.1/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.2/dagster/_core/execution/execute_in_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,33 +29,30 @@
     output_capturing_enabled: bool,
     raise_on_error: bool,
     run_tags: Optional[Mapping[str, str]] = None,
     run_id: Optional[str] = None,
     asset_selection: Optional[FrozenSet[AssetKey]] = None,
 ) -> ExecuteInProcessResult:
     job_def = ephemeral_pipeline
-    mode_def = job_def.get_mode_definition()
     pipeline = InMemoryPipeline(job_def)
 
     _check_top_level_inputs(job_def)
 
     execution_plan = create_execution_plan(
         pipeline,
         run_config=run_config,
-        mode=mode_def.name,
         instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
     )
 
     output_capture: Dict[StepOutputHandle, Any] = {}
 
     with ephemeral_instance_if_missing(instance) as execute_instance:
         run = execute_instance.create_run_for_pipeline(
             pipeline_def=job_def,
             run_config=run_config,
-            mode=mode_def.name,
             tags={**job_def.tags, **(run_tags or {})},
             run_id=run_id,
             asset_selection=asset_selection,
             execution_plan=execution_plan,
         )
         run_id = run.run_id
```

### Comparing `dagster-1.3.1/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.2/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/execute_job_result.py` & `dagster-1.3.2/dagster/_core/execution/execute_job_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/execution_result.py` & `dagster-1.3.2/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/host_mode.py` & `dagster-1.3.2/dagster/_core/execution/host_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Iterator, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._config import Field, process_config
 from dagster._core.definitions.executor_definition import (
     ExecutorDefinition,
     check_cross_process_constraints,
-    default_executors,
+    multi_or_in_process_executor,
 )
 from dagster._core.definitions.reconstruct import ReconstructablePipeline
 from dagster._core.definitions.run_config import selector_for_named_defs
 from dagster._core.errors import (
     DagsterError,
     DagsterInvalidConfigError,
     DagsterInvariantViolationError,
@@ -167,15 +167,15 @@
     executor_defs: Optional[Sequence[ExecutorDefinition]] = None,
     raise_on_error: bool = False,
 ) -> Sequence[DagsterEvent]:
     check.inst_param(pipeline, "pipeline", ReconstructablePipeline)
     check.inst_param(pipeline_run, "pipeline_run", DagsterRun)
     check.inst_param(instance, "instance", DagsterInstance)
     check.opt_sequence_param(executor_defs, "executor_defs", of_type=ExecutorDefinition)
-    executor_defs = executor_defs if executor_defs is not None else default_executors
+    executor_defs = executor_defs if executor_defs is not None else [multi_or_in_process_executor]
 
     if pipeline_run.status == DagsterRunStatus.CANCELED:
         message = "Not starting execution since the run was canceled before execution could start"
         instance.report_engine_event(
             message,
             pipeline_run,
         )
```

### Comparing `dagster-1.3.1/dagster/_core/execution/job_backfill.py` & `dagster-1.3.2/dagster/_core/execution/job_backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,14 @@
         return instance.create_reexecuted_run(
             parent_run=last_run,
             code_location=code_location,
             external_pipeline=external_pipeline,
             strategy=ReexecutionStrategy.FROM_FAILURE,
             extra_tags=tags,
             run_config=partition_data.run_config,
-            mode=external_partition_set.mode,
             use_parent_run_tags=False,  # don't inherit tags from the previous run
         )
 
     else:  # backfill_job.reexecution_steps
         last_run = _fetch_last_run(instance, external_partition_set, partition_data.name)
         parent_run_id = last_run.run_id if last_run else None
         root_run_id = (last_run.root_run_id or last_run.run_id) if last_run else None
@@ -309,29 +308,27 @@
         if external_partition_set.solid_selection:
             solids_to_execute = frozenset(external_partition_set.solid_selection)
             solid_selection = external_partition_set.solid_selection
 
     external_execution_plan = code_location.get_external_execution_plan(
         external_pipeline,
         partition_data.run_config,
-        check.not_none(external_partition_set.mode),
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
         instance=instance,
     )
 
     return instance.create_run(
         pipeline_snapshot=external_pipeline.pipeline_snapshot,
         execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
         parent_pipeline_snapshot=external_pipeline.parent_pipeline_snapshot,
         pipeline_name=external_pipeline.name,
         run_id=make_new_run_id(),
         solids_to_execute=solids_to_execute,
         run_config=partition_data.run_config,
-        mode=external_partition_set.mode,
         step_keys_to_execute=step_keys_to_execute,
         tags=tags,
         root_run_id=root_run_id,
         parent_run_id=parent_run_id,
         status=DagsterRunStatus.NOT_STARTED,
         external_pipeline_origin=external_pipeline.get_external_origin(),
         pipeline_code_origin=external_pipeline.get_python_origin(),
```

### Comparing `dagster-1.3.1/dagster/_core/execution/memoization.py` & `dagster-1.3.2/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/active.py` & `dagster-1.3.2/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/compute.py` & `dagster-1.3.2/dagster/_core/execution/plan/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,19 +113,25 @@
             )
         )
 
     return event
 
 
 def gen_from_async_gen(async_gen: AsyncIterator[T]) -> Iterator[T]:
-    while True:
-        try:
-            yield asyncio.run(async_gen.__anext__())  # type: ignore # subtle awaitable vs coroutine issue
-        except StopAsyncIteration:
-            return
+    # prime use for asyncio.Runner, but new in 3.11 and did not find appealing backport
+    loop = asyncio.new_event_loop()
+    try:
+        while True:
+            try:
+                yield loop.run_until_complete(async_gen.__anext__())
+            except StopAsyncIteration:
+                return
+    finally:
+        loop.run_until_complete(loop.shutdown_asyncgens())
+        loop.close()
 
 
 def _yield_compute_results(
     step_context: StepExecutionContext, inputs: Mapping[str, Any], compute_fn: Callable
 ) -> Iterator[OpOutputUnion]:
     check.inst_param(step_context, "step_context", StepExecutionContext)
```

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.2/dagster/_core/execution/plan/compute_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
                     raise DagsterInvariantViolationError(
                         f"Error with output for {context.describe_op()}: output "
                         f"'{output_def.name}' has generic output annotation, "
                         "but did not receive an Output object for this output. "
                         f"Received instead an object of type {type(element)}."
                     )
                 if result is None and output_def.is_required is False:
-                    context.log.warn(
+                    context.log.warning(
                         'Value "None" returned for non-required output '
                         f'"{output_def.name}" of {context.describe_op()}. '
                         "This value will be passed to downstream "
                         f"{context.op_def.node_type_str}s. For conditional "
                         "execution, results must be yielded: "
                         "https://docs.dagster.io/concepts/ops-jobs-graphs/graphs#with-conditional-branching"
                     )
```

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.2/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.2/dagster/_core/execution/plan/execute_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,17 @@
 def _asset_key_and_partitions_for_output(
     output_context: OutputContext,
 ) -> Tuple[Optional[AssetKey], AbstractSet[str]]:
     output_asset_info = output_context.asset_info
 
     if output_asset_info:
         if not output_asset_info.is_required:
-            output_context.log.warn(f"Materializing unexpected asset key: {output_asset_info.key}.")
+            output_context.log.warning(
+                f"Materializing unexpected asset key: {output_asset_info.key}."
+            )
         return (
             output_asset_info.key,
             output_asset_info.partitions_fn(output_context) or set(),
         )
 
     return None, set()
```

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.2/dagster/_core/execution/plan/external_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,14 @@
             frozenset(solids_to_execute) if solids_to_execute else None,
             asset_selection=step_run_ref.dagster_run.asset_selection,
         )
 
     execution_plan = create_execution_plan(
         pipeline,
         step_run_ref.run_config,
-        mode=step_run_ref.dagster_run.mode,
         step_keys_to_execute=[step_run_ref.step_key],
         known_state=step_run_ref.known_state,
         # we packaged repository_load_data onto the reconstructable pipeline when creating the
         # StepRunRef, rather than putting it in a separate field
         repository_load_data=pipeline.repository.repository_load_data,
     )
```

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/handle.py` & `dagster-1.3.2/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.2/dagster/_core/execution/plan/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     Union,
     cast,
 )
 
 from typing_extensions import TypeAlias
 
 import dagster._check as check
-from dagster._core.definitions import InputDefinition, NodeHandle, PipelineDefinition
-from dagster._core.definitions.job_definition import JobDefinition
+from dagster._core.definitions import InputDefinition, JobDefinition, NodeHandle
 from dagster._core.definitions.version_strategy import ResourceVersionContext
 from dagster._core.errors import (
     DagsterExecutionLoadInputError,
     DagsterInvariantViolationError,
     DagsterTypeLoadingError,
     user_code_error_boundary,
 )
@@ -105,22 +104,22 @@
 
     @abstractmethod
     def load_input_object(
         self, step_context: "StepExecutionContext", input_def: InputDefinition
     ) -> Iterator[object]:
         ...
 
-    def required_resource_keys(self, _pipeline_def: PipelineDefinition) -> AbstractSet[str]:
+    def required_resource_keys(self, _pipeline_def: JobDefinition) -> AbstractSet[str]:
         return set()
 
     @abstractmethod
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         """See resolve_step_versions in resolve_versions.py for explanation of step_versions."""
         raise NotImplementedError()
 
 
 @whitelist_for_serdes(storage_field_names={"node_handle": "solid_handle"})
@@ -195,24 +194,22 @@
             manager_key=input_manager_key,
             metadata=metadata,
         )
 
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         from ..resolve_versions import check_valid_version, resolve_config_version
 
         op = pipeline_def.get_node(self.node_handle)
         input_manager_key = check.not_none(op.input_def_named(self.input_name).input_manager_key)
-        io_manager_def = pipeline_def.get_mode_definition(resolved_run_config.mode).resource_defs[
-            input_manager_key
-        ]
+        io_manager_def = pipeline_def.resource_defs[input_manager_key]
 
         op_config = check.not_none(resolved_run_config.ops.get(op.name))
         input_config = op_config.inputs.get(self.input_name)
         resource_entry = check.not_none(resolved_run_config.resources.get(input_manager_key))
         resource_config = resource_entry.config
 
         version_context = ResourceVersionContext(
@@ -237,15 +234,15 @@
         check_valid_version(io_manager_def_version)
         return join_and_hash(
             resolve_config_version(input_config),
             resolve_config_version(resource_config),
             io_manager_def_version,
         )
 
-    def required_resource_keys(self, pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, pipeline_def: JobDefinition) -> Set[str]:
         input_asset_key = pipeline_def.asset_layer.asset_key_for_input(
             self.node_handle, self.input_name
         )
         if input_asset_key is None:
             check.failed(
                 (
                     f"Must have an asset key associated with input {self.input_name} to load it"
@@ -328,28 +325,26 @@
             manager_key=input_manager_key,
             metadata=metadata,
         )
 
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         from ..resolve_versions import check_valid_version, resolve_config_version
 
         solid = pipeline_def.get_node(self.node_handle)
         input_manager_key: str = check.not_none(
             solid.input_def_named(self.input_name).root_manager_key
             if solid.input_def_named(self.input_name).root_manager_key
             else solid.input_def_named(self.input_name).input_manager_key
         )
-        input_manager_def = pipeline_def.get_mode_definition(
-            resolved_run_config.mode
-        ).resource_defs[input_manager_key]
+        input_manager_def = pipeline_def.resource_defs[input_manager_key]
 
         solid_config = resolved_run_config.ops[solid.name]
         input_config = solid_config.inputs.get(self.input_name)
         resource_config = check.not_none(
             resolved_run_config.resources.get(input_manager_key)
         ).config
 
@@ -375,15 +370,15 @@
         check_valid_version(root_manager_def_version)
         return join_and_hash(
             resolve_config_version(input_config),
             resolve_config_version(resource_config),
             root_manager_def_version,
         )
 
-    def required_resource_keys(self, pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, pipeline_def: JobDefinition) -> Set[str]:
         input_def = pipeline_def.get_node(self.node_handle).input_def_named(self.input_name)
 
         input_manager_key: str = check.not_none(
             input_def.root_manager_key
             if input_def.root_manager_key
             else input_def.input_manager_key
         )
@@ -520,28 +515,28 @@
             upstream_step_key=source_handle.step_key,
             metadata=metadata,
         )
 
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         if (
             self.step_output_handle.step_key not in step_versions
             or not step_versions[self.step_output_handle.step_key]
         ):
             return None
         else:
             return join_and_hash(
                 step_versions[self.step_output_handle.step_key], self.step_output_handle.output_name
             )
 
-    def required_resource_keys(self, _pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, _pipeline_def: JobDefinition) -> Set[str]:
         return set()
 
 
 @whitelist_for_serdes(storage_field_names={"node_handle": "solid_handle"})
 class FromConfig(
     NamedTuple(
         "_FromConfig",
@@ -560,15 +555,15 @@
     def __new__(cls, node_handle: Optional[NodeHandle], input_name: str):
         return super(FromConfig, cls).__new__(
             cls,
             node_handle=node_handle,
             input_name=input_name,
         )
 
-    def get_associated_input_def(self, pipeline_def: PipelineDefinition) -> InputDefinition:
+    def get_associated_input_def(self, pipeline_def: JobDefinition) -> InputDefinition:
         """Returns the InputDefinition along the potential composition InputMapping chain
         that the config was provided at.
         """
         if self.node_handle:
             return pipeline_def.get_node(self.node_handle).input_def_named(self.input_name)
         else:
             return pipeline_def.graph.input_def_named(self.input_name)
@@ -597,22 +592,22 @@
             dagster_type = self.get_associated_input_def(step_context.pipeline_def).dagster_type
             config_data = self.get_associated_config(step_context.resolved_run_config)
             loader = check.not_none(dagster_type.loader)
             yield loader.construct_from_config_value(
                 step_context.get_type_loader_context(), config_data
             )
 
-    def required_resource_keys(self, pipeline_def: PipelineDefinition) -> AbstractSet[str]:
+    def required_resource_keys(self, pipeline_def: JobDefinition) -> AbstractSet[str]:
         dagster_type = self.get_associated_input_def(pipeline_def).dagster_type
         return dagster_type.loader.required_resource_keys() if dagster_type.loader else set()
 
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         config_data = self.get_associated_config(resolved_run_config)
         input_def = self.get_associated_input_def(pipeline_def)
         dagster_type = input_def.dagster_type
         loader = check.not_none(dagster_type.loader)
 
@@ -634,30 +629,24 @@
             cls,
             input_name=input_name,
         )
 
     def load_input_object(
         self, step_context: "StepExecutionContext", input_def: InputDefinition
     ) -> Iterator[object]:
-        pipeline_def = step_context.pipeline_def
-        if not pipeline_def.is_job:
-            raise DagsterInvariantViolationError(
-                "Using input values with pipeline API, which is unsupported."
-            )
-
-        job_def = cast(JobDefinition, pipeline_def)
+        job_def = step_context.pipeline_def
         yield job_def.get_direct_input_value(self.input_name)
 
-    def required_resource_keys(self, _pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, _pipeline_def: JobDefinition) -> Set[str]:
         return set()
 
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         return str(self.input_name)
 
 
 @whitelist_for_serdes(storage_field_names={"node_handle": "solid_handle"})
 class FromDefaultValue(
@@ -671,30 +660,30 @@
     StepInputSource,
 ):
     """This step input source is the default value declared on an InputDefinition."""
 
     def __new__(cls, node_handle: NodeHandle, input_name: str):
         return super(FromDefaultValue, cls).__new__(cls, node_handle, input_name)
 
-    def _load_value(self, pipeline_def: PipelineDefinition):
+    def _load_value(self, pipeline_def: JobDefinition):
         return pipeline_def.get_node(self.node_handle).definition.default_value_for_input(
             self.input_name
         )
 
     def load_input_object(
         self,
         step_context: "StepExecutionContext",
         input_def: InputDefinition,
     ) -> Iterator[object]:
         yield self._load_value(step_context.pipeline_def)
 
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         return join_and_hash(repr(self._load_value(pipeline_def)))
 
 
 @whitelist_for_serdes(storage_field_names={"node_handle": "solid_handle"})
 class FromMultipleSources(
@@ -779,24 +768,24 @@
                 if isinstance(event_or_input_value, DagsterEvent):
                     yield event_or_input_value
                 else:
                     values.append(event_or_input_value)
 
         yield values
 
-    def required_resource_keys(self, pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, pipeline_def: JobDefinition) -> Set[str]:
         resource_keys: Set[str] = set()
         for source in self.sources:
             resource_keys = resource_keys.union(source.required_resource_keys(pipeline_def))
         return resource_keys
 
     def compute_version(
         self,
         step_versions: Mapping[str, Optional[str]],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
     ) -> Optional[str]:
         return join_and_hash(
             *[
                 inner_source.compute_version(step_versions, pipeline_def, resolved_run_config)
                 for inner_source in self.sources
             ]
@@ -881,15 +870,15 @@
             fan_in=False,
         )
 
     def get_step_output_handle_dep_with_placeholder(self) -> StepOutputHandle:
         # None mapping_key on StepOutputHandle acts as placeholder
         return self.step_output_handle
 
-    def required_resource_keys(self, _pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, _pipeline_def: JobDefinition) -> Set[str]:
         return set()
 
 
 @whitelist_for_serdes(storage_field_names={"node_handle": "solid_handle"})
 class FromUnresolvedStepOutput(
     NamedTuple(
         "_FromUnresolvedStepOutput",
@@ -940,15 +929,15 @@
             step_output_handle=self.unresolved_step_output_handle.resolve(mapping_key),
             fan_in=False,
         )
 
     def get_step_output_handle_dep_with_placeholder(self) -> StepOutputHandle:
         return self.unresolved_step_output_handle.get_step_output_handle_with_placeholder()
 
-    def required_resource_keys(self, _pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, _pipeline_def: JobDefinition) -> Set[str]:
         return set()
 
 
 @whitelist_for_serdes(storage_field_names={"node_handle": "solid_handle"})
 class FromDynamicCollect(
     NamedTuple(
         "_FromDynamicCollect",
@@ -984,15 +973,15 @@
     @property
     def resolved_by_output_name(self) -> str:
         return self.source.resolved_by_output_name
 
     def get_step_output_handle_dep_with_placeholder(self) -> StepOutputHandle:
         return self.source.get_step_output_handle_dep_with_placeholder()
 
-    def required_resource_keys(self, _pipeline_def: PipelineDefinition) -> Set[str]:
+    def required_resource_keys(self, _pipeline_def: JobDefinition) -> Set[str]:
         return set()
 
     def resolve(self, mapping_keys: Optional[Sequence[str]]):
         if mapping_keys is None:
             # None means that the dynamic output was skipped, so create
             # a dependency on the dynamic output that will continue cascading the skip
             return FromStepOutput(
```

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.2/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/objects.py` & `dagster-1.3.2/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.2/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/plan.py` & `dagster-1.3.2/dagster/_core/execution/plan/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 )
 
 import dagster._check as check
 from dagster._core.definitions import (
     GraphDefinition,
     InputDefinition,
     IPipeline,
-    JobDefinition,
     Node,
     NodeHandle,
     NodeOutput,
     OpDefinition,
 )
 from dagster._core.definitions.composition import MappedInputPlaceholder
 from dagster._core.definitions.dependency import DependencyStructure
 from dagster._core.definitions.executor_definition import ExecutorRequirement
-from dagster._core.definitions.mode import ModeDefinition
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.reconstruct import ReconstructablePipeline
 from dagster._core.definitions.repository_definition import RepositoryLoadData
 from dagster._core.errors import (
     DagsterExecutionStepNotFoundError,
     DagsterInvariantViolationError,
     DagsterUnmetExecutorRequirementsError,
 )
@@ -121,19 +119,14 @@
             )
         self.pipeline = check.inst_param(pipeline, "pipeline", IPipeline)
         self.resolved_run_config = check.inst_param(
             resolved_run_config, "resolved_run_config", ResolvedRunConfig
         )
         check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", str)
         self.step_keys_to_execute = step_keys_to_execute
-        self.mode_definition = (
-            pipeline.get_definition().get_mode_definition(resolved_run_config.mode)
-            if resolved_run_config.mode is not None
-            else pipeline.get_definition().get_default_mode()
-        )
         self._steps: Dict[str, IExecutionStep] = {}
         self.step_output_map: Dict[
             NodeOutput, Union[StepOutputHandle, UnresolvedStepOutputHandle]
         ] = {}
         self.known_state = check.inst_param(known_state, "known_state", KnownExecutionState)
         self._instance_ref = instance_ref
         self._seen_handles: Set[StepHandleUnion] = set()
@@ -162,15 +155,14 @@
         check.inst_param(handle, "handle", NodeHandle)
         return self._steps[handle.to_string()]
 
     def build(self) -> "ExecutionPlan":
         """Builds the execution plan."""
         _check_persistent_storage_requirement(
             self.pipeline,
-            self.mode_definition,
             self.resolved_run_config,
         )
 
         pipeline_def = self.pipeline.get_definition()
         root_inputs: List[
             Union[StepInput, UnresolvedMappedStepInput, UnresolvedCollectStepInput]
         ] = []
@@ -413,19 +405,17 @@
                 step_output_map[node_output] = step_output_handle
 
 
 def get_root_graph_input_source(
     plan_builder: _PlanBuilder,
     input_name: str,
     input_def: InputDefinition,
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
 ) -> Optional[Union[FromConfig, FromDirectInputValue]]:
-    from dagster._core.definitions.job_definition import get_direct_input_values_from_job
-
-    input_values = get_direct_input_values_from_job(pipeline_def)
+    input_values = pipeline_def.input_values
     if input_values and input_name in input_values:
         return FromDirectInputValue(input_name=input_name)
 
     input_config = plan_builder.resolved_run_config.inputs
 
     if input_config and input_name in input_config:
         return FromConfig(input_name=input_name, node_handle=None)
@@ -442,15 +432,15 @@
             described_target=plan_builder.pipeline.get_definition().describe_target(),
             input_name=input_name,
         )
     )
 
 
 def get_step_input_source(
-    job_def: PipelineDefinition,
+    job_def: JobDefinition,
     node: Node,
     input_name: str,
     input_def: InputDefinition,
     dependency_structure: DependencyStructure,
     handle: NodeHandle,
     node_config: Any,
     step_output_map: Dict[NodeOutput, Union[StepOutputHandle, UnresolvedStepOutputHandle]],
@@ -671,15 +661,15 @@
     def get_step_output(self, step_output_handle: StepOutputHandle) -> StepOutput:
         check.inst_param(step_output_handle, "step_output_handle", StepOutputHandle)
         return _get_step_output(self.step_dict_by_key, step_output_handle)
 
     def get_manager_key(
         self,
         step_output_handle: StepOutputHandle,
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
     ) -> str:
         return _get_manager_key(self.step_dict_by_key, step_output_handle, pipeline_def)
 
     def has_step(self, handle: StepHandleUnion) -> bool:
         check.inst_param(handle, "handle", StepHandleTypes)
         return handle in self.step_dict
 
@@ -750,15 +740,15 @@
         after = self.get_executable_step_deps()
 
         return {key: deps for key, deps in after.items() if key not in previous}
 
     def build_subset_plan(
         self,
         step_keys_to_execute: Sequence[str],
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
         step_output_versions: Optional[Mapping[StepOutputHandle, Optional[str]]] = None,
     ) -> "ExecutionPlan":
         check.sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
         step_output_versions = check.opt_mapping_param(
             step_output_versions, "step_output_versions", key_type=StepOutputHandle, value_type=str
         )
@@ -844,29 +834,26 @@
     def get_version_for_step_output_handle(
         self, step_output_handle: StepOutputHandle
     ) -> Optional[str]:
         return self.step_output_versions.get(step_output_handle)
 
     def build_memoized_plan(
         self,
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
         instance: DagsterInstance,
         selected_step_keys: Optional[Sequence[str]],
     ) -> "ExecutionPlan":
         """Returns:
         ExecutionPlan: Execution plan that runs only unmemoized steps.
         """
         from ...storage.memoizable_io_manager import MemoizableIOManager
         from ..build_resources import build_resources, initialize_console_manager
         from ..resources_init import get_dependencies, resolve_resource_dependencies
 
-        mode = resolved_run_config.mode
-        mode_def = pipeline_def.get_mode_definition(mode)
-
         # Memoization cannot be used with dynamic orchestration yet.
         # Tracking: https://github.com/dagster-io/dagster/issues/4451
         for node_def in pipeline_def.all_node_defs:
             if pipeline_def.dependency_structure.is_dynamic_mapped(
                 node_def.name
             ) or pipeline_def.dependency_structure.has_dynamic_downstreams(node_def.name):
                 raise DagsterInvariantViolationError(
@@ -886,18 +873,18 @@
         for step in self.steps:
             for output_name in cast(ExecutionStepUnion, step).step_output_dict.keys():
                 step_output_handle = StepOutputHandle(step.key, output_name)
 
                 io_manager_key = self.get_manager_key(step_output_handle, pipeline_def)
                 io_manager_keys[step_output_handle] = io_manager_key
 
-                resource_deps = resolve_resource_dependencies(mode_def.resource_defs)
+                resource_deps = resolve_resource_dependencies(pipeline_def.resource_defs)
                 resource_keys_to_init = get_dependencies(io_manager_key, resource_deps)
                 for resource_key in resource_keys_to_init:
-                    resource_defs_to_init[resource_key] = mode_def.resource_defs[resource_key]
+                    resource_defs_to_init[resource_key] = pipeline_def.resource_defs[resource_key]
 
         all_resources_config = resolved_run_config.to_dict().get("resources", {})
         resource_config = {
             resource_key: config_val
             for resource_key, config_val in all_resources_config.items()
             if resource_key in resource_defs_to_init
         }
@@ -1189,62 +1176,49 @@
         executable_map[step.key] = step.handle
         step_dict_by_key[step.key] = step
 
     for key_set in key_sets_to_clear:
         del resolvable_map[key_set]
 
 
-def can_isolate_steps(pipeline_def: PipelineDefinition, mode_def: ModeDefinition) -> bool:
+def can_isolate_steps(pipeline_def: JobDefinition) -> bool:
     """Returns true if every output definition in the pipeline uses an IO manager that's not
     the mem_io_manager.
 
     If true, this indicates that it's OK to execute steps in their own processes, because their
     outputs will be available to other processes.
     """
     output_defs = [
         output_def for node_def in pipeline_def.all_node_defs for output_def in node_def.output_defs
     ]
     for output_def in output_defs:
-        if mode_def.resource_defs[output_def.io_manager_key] == mem_io_manager:
+        if pipeline_def.resource_defs[output_def.io_manager_key] == mem_io_manager:
             return False
 
     return True
 
 
 def _check_persistent_storage_requirement(
     pipeline: IPipeline,
-    mode_def: ModeDefinition,
     resolved_run_config: ResolvedRunConfig,
 ) -> None:
-    from dagster._core.execution.context_creation_pipeline import executor_def_from_config
-
     pipeline_def = pipeline.get_definition()
-    executor_def = executor_def_from_config(mode_def, resolved_run_config)
+    executor_def = pipeline_def.executor_def
     requirements_lst = executor_def.get_requirements(
         resolved_run_config.execution.execution_engine_config
     )
     if ExecutorRequirement.PERSISTENT_OUTPUTS not in requirements_lst:
         return
 
-    if not can_isolate_steps(pipeline_def, mode_def):
-        if isinstance(pipeline_def, JobDefinition):
-            target = "job"
-            node = "op"
-            suggestion = 'the_graph.to_job(resource_defs={"io_manager": fs_io_manager})'
-        else:
-            target = "pipeline"
-            node = "solid"
-            suggestion = (
-                '@pipeline(mode_defs=[ModeDefinition(resource_defs={"io_manager": fs_io_manager})])'
-            )
+    if not can_isolate_steps(pipeline_def):
         raise DagsterUnmetExecutorRequirementsError(
             "You have attempted to use an executor that uses multiple processes, but your"
-            f" {target} includes {node} outputs that will not be stored somewhere where other"
+            " job includes op outputs that will not be stored somewhere where other"
             " processes can retrieve them. Please use a persistent IO manager for these outputs."
-            f" E.g. with\n    {suggestion}"
+            ' E.g. with\n   the_graph.to_job(resource_defs={"io_manager": fs_io_manager})'
         )
 
 
 def should_skip_step(execution_plan: ExecutionPlan, instance: DagsterInstance, run_id: str) -> bool:
     """[INTERNAL] Check if it should skip executing the plan. Primarily used by execution without
     run-level plan process, e.g. Airflow step execution. Note: this only checks one step at a time.
 
@@ -1300,24 +1274,22 @@
     return False
 
 
 def _compute_artifacts_persisted(
     step_dict: Dict[StepHandleUnion, IExecutionStep],
     step_dict_by_key: Dict[str, IExecutionStep],
     step_handles_to_execute: Sequence[StepHandleUnion],
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     resolved_run_config: ResolvedRunConfig,
     executable_map: Mapping[str, Union[StepHandle, ResolvedFromDynamicStepHandle]],
 ) -> bool:
     """Check if all the border steps of the current run have non-in-memory IO managers for reexecution.
 
     Border steps: all the steps that don't have upstream steps to execute, i.e. indegree is 0).
     """
-    mode_def = pipeline_def.get_mode_definition(resolved_run_config.mode)
-
     if len(step_dict) == 0:
         return False
 
     steps_by_level = _get_steps_to_execute_by_level(
         step_dict, step_dict_by_key, step_handles_to_execute, executable_map
     )
 
@@ -1327,15 +1299,15 @@
     for step in steps_by_level[0]:
         # check if all its inputs' upstream step outputs have non-in-memory IO manager configured
         for step_input in step.step_inputs:
             for step_output_handle in step_input.get_step_output_handle_dependencies():
                 io_manager_key = _get_manager_key(
                     step_dict_by_key, step_output_handle, pipeline_def
                 )
-                manager_def = mode_def.resource_defs.get(io_manager_key)
+                manager_def = pipeline_def.resource_defs.get(io_manager_key)
                 if (
                     # no IO manager is configured
                     not manager_def
                     # IO manager is non persistent
                     or manager_def == mem_io_manager
                 ):
                     return False
@@ -1398,15 +1370,15 @@
     step = step_dict_by_key[step_output_handle.step_key]
     return step.step_output_named(step_output_handle.output_name)
 
 
 def _get_manager_key(
     step_dict_by_key: Mapping[str, IExecutionStep],
     step_output_handle: StepOutputHandle,
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
 ) -> str:
     step_output = _get_step_output(step_dict_by_key, step_output_handle)
     node_handle = step_output.node_handle
     output_def = pipeline_def.get_node(node_handle).output_def_named(step_output.name)
     return output_def.io_manager_key
```

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/state.py` & `dagster-1.3.2/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/step.py` & `dagster-1.3.2/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/plan/utils.py` & `dagster-1.3.2/dagster/_core/execution/plan/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     from dagster._core.definitions.resource_definition import Resources
     from dagster._core.execution.context.system import StepExecutionContext
 
 
 def build_resources_for_manager(
     io_manager_key: str, step_context: "StepExecutionContext"
 ) -> "Resources":
-    required_resource_keys = step_context.mode_def.resource_defs[
+    required_resource_keys = step_context.job_def.resource_defs[
         io_manager_key
     ].required_resource_keys
     return step_context.scoped_resources_builder.build(required_resource_keys)
 
 
 class RetryRequestedFromPolicy(RetryRequested):
     """Subclass to indicate origin of retry request is policy."""
```

### Comparing `dagster-1.3.1/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.2/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.2/dagster/_core/execution/resolve_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import TYPE_CHECKING, Dict, Mapping, Optional
 
 import dagster._check as check
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.version_strategy import OpVersionContext, ResourceVersionContext
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.execution.plan.outputs import StepOutputHandle
 from dagster._core.execution.plan.step import is_executable_step
 from dagster._core.system_config.objects import ResolvedRunConfig
 
 from .plan.inputs import join_and_hash
@@ -47,15 +47,15 @@
         config_value = check.dict_param(config_value, "config_value")
         return join_and_hash(
             *[key + resolve_config_version(val) for key, val in config_value.items()]
         )
 
 
 def resolve_step_versions(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     execution_plan: "ExecutionPlan",
     resolved_run_config: ResolvedRunConfig,
 ) -> Mapping[str, Optional[str]]:
     """Resolves the version of each step in an execution plan.
 
     Execution plan provides execution steps for analysis. It returns dict[str, str] where each key
     is a step key, and each value is the associated version for that step.
@@ -76,15 +76,15 @@
                 and the solid's version definition.
 
     Returns:
         Dict[str, Optional[str]]: A dictionary that maps the key of an execution step to a version.
             If a step has no computed version, then the step key maps to None.
     """
     resource_versions = {}
-    resource_defs = pipeline_def.get_mode_definition(resolved_run_config.mode).resource_defs
+    resource_defs = pipeline_def.resource_defs
 
     step_versions: Dict[str, Optional[str]] = {}  # step_key (str) -> version (str)
 
     for step in execution_plan.get_all_steps_in_topo_order():
         # do not compute versions for steps that are not executable
         if not is_executable_step(step):  # type: ignore
             continue
@@ -166,15 +166,15 @@
 
         step_versions[step.key] = step_version
 
     return step_versions
 
 
 def resolve_step_output_versions(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     execution_plan: "ExecutionPlan",
     resolved_run_config: ResolvedRunConfig,
 ):
     step_versions = resolve_step_versions(pipeline_def, execution_plan, resolved_run_config)
     return {
         StepOutputHandle(step.key, output_name): join_and_hash(output_name, step_versions[step.key])
         for step in execution_plan.steps
```

### Comparing `dagster-1.3.1/dagster/_core/execution/resources_init.py` & `dagster-1.3.2/dagster/_core/execution/resources_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Optional,
     Set,
     Union,
     cast,
 )
 
 import dagster._check as check
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.resource_definition import (
     ResourceDefinition,
     ScopedResourcesBuilder,
     has_at_least_one_parameter,
 )
 from dagster._core.errors import (
     DagsterInvariantViolationError,
@@ -156,15 +156,14 @@
                 pipeline_name,
                 cast(ExecutionPlan, execution_plan),
                 resource_log_manager,
                 resource_keys_to_init,
             )
 
         resource_dependencies = resolve_resource_dependencies(resource_defs)
-
         for level in toposort(resource_dependencies):
             for resource_name in level:
                 resource_def = resource_defs[resource_name]
                 if resource_name not in resource_keys_to_init:
                     continue
 
                 resource_fn = cast(Callable[[InitResourceContext], Any], resource_def.resource_fn)
@@ -356,15 +355,15 @@
             pass
         else:
             check.failed(f"Resource generator {resource_name} yielded more than one item.")
 
 
 def get_required_resource_keys_to_init(
     execution_plan: ExecutionPlan,
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     resolved_run_config: ResolvedRunConfig,
 ) -> AbstractSet[str]:
     resource_keys: Set[str] = set()
 
     for step_handle, step in execution_plan.step_dict.items():
         if step_handle not in execution_plan.step_handles_to_execute:
             continue
@@ -373,16 +372,17 @@
         for hook_def in hook_defs:
             resource_keys = resource_keys.union(hook_def.required_resource_keys)
 
         resource_keys = resource_keys.union(
             get_required_resource_keys_for_step(pipeline_def, step, execution_plan)
         )
 
-    resource_defs = pipeline_def.get_mode_definition(resolved_run_config.mode).resource_defs
-    return frozenset(get_transitive_required_resource_keys(resource_keys, resource_defs))
+    return frozenset(
+        get_transitive_required_resource_keys(resource_keys, pipeline_def.resource_defs)
+    )
 
 
 def get_transitive_required_resource_keys(
     required_resource_keys: AbstractSet[str], resource_defs: Mapping[str, ResourceDefinition]
 ) -> AbstractSet[str]:
     resource_dependencies = resolve_resource_dependencies(resource_defs)
     ensure_resource_deps_satisfiable(resource_dependencies)
@@ -394,15 +394,15 @@
             set(get_dependencies(resource_key, resource_dependencies))
         )
 
     return transitive_required_resource_keys
 
 
 def get_required_resource_keys_for_step(
-    pipeline_def: PipelineDefinition, execution_step: IExecutionStep, execution_plan: ExecutionPlan
+    pipeline_def: JobDefinition, execution_step: IExecutionStep, execution_plan: ExecutionPlan
 ) -> AbstractSet[str]:
     resource_keys: Set[str] = set()
 
     # add all the solid compute resource keys
     solid_def = pipeline_def.get_node(execution_step.node_handle).definition
     resource_keys = resource_keys.union(solid_def.required_resource_keys)  # type: ignore  # (should be OpDefinition)
```

### Comparing `dagster-1.3.1/dagster/_core/execution/results.py` & `dagster-1.3.2/dagster/_core/execution/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Union,
     cast,
 )
 
 from typing_extensions import TypeAlias
 
 import dagster._check as check
-from dagster._core.definitions import GraphDefinition, Node, NodeHandle, PipelineDefinition
+from dagster._core.definitions import GraphDefinition, JobDefinition, Node, NodeHandle
 from dagster._core.definitions.dependency import GraphNode, OpNode
 from dagster._core.definitions.events import (
     AssetMaterialization,
     ExpectationResult,
 )
 from dagster._core.definitions.utils import DEFAULT_OUTPUT
 from dagster._core.errors import DagsterInvariantViolationError
@@ -51,25 +51,25 @@
 
 class GraphExecutionResult:
     def __init__(
         self,
         container: GraphDefinition,
         event_list: Sequence[DagsterEvent],
         reconstruct_context: ReconstructContextFn,
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         handle: Optional[NodeHandle] = None,
         output_capture: Optional[Dict[StepOutputHandle, object]] = None,
     ):
         self.container = check.inst_param(container, "container", GraphDefinition)
         self.event_list = check.sequence_param(event_list, "step_event_list", of_type=DagsterEvent)
         self.reconstruct_context = check.callable_param(
             reconstruct_context,
             "reconstruct_context",
         )
-        self.pipeline_def = check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+        self.pipeline_def = check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
         self.handle = check.opt_inst_param(handle, "handle", NodeHandle)
         self.output_capture = check.opt_dict_param(
             output_capture, "output_capture", key_type=StepOutputHandle
         )
         self._events_by_step_key = _construct_events_by_step_key(event_list)
 
     @property
@@ -205,22 +205,22 @@
     """The result of executing a pipeline.
 
     Returned by :py:func:`execute_pipeline`. Users should not instantiate this class directly.
     """
 
     def __init__(
         self,
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         run_id: str,
         event_list: Sequence[DagsterEvent],
         reconstruct_context: ReconstructContextFn,
         output_capture: Optional[Dict[StepOutputHandle, object]] = None,
     ):
         self.run_id = check.str_param(run_id, "run_id")
-        check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+        check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
 
         super(PipelineExecutionResult, self).__init__(
             container=pipeline_def.graph,
             event_list=event_list,
             reconstruct_context=reconstruct_context,
             pipeline_def=pipeline_def,
             output_capture=output_capture,
@@ -235,15 +235,15 @@
 
     def __init__(
         self,
         node: GraphNode,
         event_list: Sequence[DagsterEvent],
         step_events_by_kind: Mapping[StepKind, Sequence[DagsterEvent]],
         reconstruct_context: ReconstructContextFn,
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         handle: Optional[NodeHandle] = None,
         output_capture: Optional[Dict[StepOutputHandle, object]] = None,
     ):
         check.inst_param(node, "node", GraphNode)
         self.node = node
         self.step_events_by_kind = check.dict_param(
             step_events_by_kind, "step_events_by_kind", key_type=StepKind, value_type=list
@@ -332,28 +332,28 @@
     """
 
     def __init__(
         self,
         node: OpNode,
         step_events_by_kind: Mapping[StepKind, Sequence[DagsterEvent]],
         reconstruct_context: ReconstructContextFn,
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         output_capture: Optional[Dict[StepOutputHandle, object]] = None,
     ):
         check.inst_param(node, "node", OpNode)
         self.node = node
         self.step_events_by_kind = check.dict_param(
             step_events_by_kind, "step_events_by_kind", key_type=StepKind, value_type=list
         )
         self.reconstruct_context = check.callable_param(
             reconstruct_context,
             "reconstruct_context",
         )
         self.output_capture = check.opt_dict_param(output_capture, "output_capture")
-        self.pipeline_def = check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+        self.pipeline_def = check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
 
     @property
     def compute_input_event_dict(self) -> Mapping[str, DagsterEvent]:
         """Dict[str, DagsterEvent]: All events of type ``STEP_INPUT``, keyed by input name."""
         return {
             cast(StepInputData, se.event_specific_data).input_name: se
             for se in self.input_events_during_compute
```

### Comparing `dagster-1.3.1/dagster/_core/execution/retries.py` & `dagster-1.3.2/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.2/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/stats.py` & `dagster-1.3.2/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/tags.py` & `dagster-1.3.2/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.2/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.2/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/executor/base.py` & `dagster-1.3.2/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.2/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/executor/in_process.py` & `dagster-1.3.2/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/executor/init.py` & `dagster-1.3.2/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/executor/multiprocess.py` & `dagster-1.3.2/dagster/_core/executor/multiprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     def execute(self) -> Iterator[DagsterEvent]:
         pipeline = self.recon_pipeline
         with DagsterInstance.from_ref(self.instance_ref) as instance:
             start_termination_thread(self.term_event)
             execution_plan = create_execution_plan(
                 pipeline=pipeline,
                 run_config=self.run_config,
-                mode=self.pipeline_run.mode,
                 step_keys_to_execute=[self.step_key],
                 known_state=self.known_state,
                 repository_load_data=self.repository_load_data,
             )
 
             log_manager = create_context_free_log_manager(instance, self.pipeline_run)
```

### Comparing `dagster-1.3.1/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.2/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.2/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/__init__.py` & `dagster-1.3.2/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/code_location.py` & `dagster-1.3.2/dagster/_core/host_representation/code_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,14 @@
         return self.origin.location_name
 
     @abstractmethod
     def get_external_execution_plan(
         self,
         external_pipeline: ExternalPipeline,
         run_config: Mapping[str, object],
-        mode: str,
         step_keys_to_execute: Optional[Sequence[str]],
         known_state: Optional[KnownExecutionState],
         instance: Optional[DagsterInstance] = None,
     ) -> ExternalExecutionPlan:
         pass
 
     def get_external_pipeline(self, selector: PipelineSelector) -> ExternalPipeline:
@@ -374,37 +373,34 @@
             selector.asset_selection,
         )
 
     def get_external_execution_plan(
         self,
         external_pipeline: ExternalPipeline,
         run_config: Mapping[str, object],
-        mode: str,
         step_keys_to_execute: Optional[Sequence[str]],
         known_state: Optional[KnownExecutionState],
         instance: Optional[DagsterInstance] = None,
     ) -> ExternalExecutionPlan:
         check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
         check.mapping_param(run_config, "run_config")
-        check.str_param(mode, "mode")
         step_keys_to_execute = check.opt_nullable_sequence_param(
             step_keys_to_execute, "step_keys_to_execute", of_type=str
         )
         check.opt_inst_param(known_state, "known_state", KnownExecutionState)
         check.opt_inst_param(instance, "instance", DagsterInstance)
 
         execution_plan = create_execution_plan(
             pipeline=self.get_reconstructable_pipeline(
                 external_pipeline.repository_handle.repository_name, external_pipeline.name
             ).subset_for_execution_from_existing_pipeline(
                 external_pipeline.solids_to_execute,
                 external_pipeline.asset_selection,
             ),
             run_config=run_config,
-            mode=mode,
             step_keys_to_execute=step_keys_to_execute,
             known_state=known_state,
             instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
         )
         return ExternalExecutionPlan(
             execution_plan_snapshot=snapshot_from_execution_plan(
                 execution_plan,
@@ -718,37 +714,34 @@
     def get_repositories(self) -> Mapping[str, ExternalRepository]:
         return self.external_repositories
 
     def get_external_execution_plan(
         self,
         external_pipeline: ExternalPipeline,
         run_config: Mapping[str, Any],
-        mode: str,
         step_keys_to_execute: Optional[Sequence[str]],
         known_state: Optional[KnownExecutionState],
         instance: Optional[DagsterInstance] = None,
     ) -> ExternalExecutionPlan:
         check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
         run_config = check.mapping_param(run_config, "run_config")
-        check.str_param(mode, "mode")
         check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
         check.opt_inst_param(known_state, "known_state", KnownExecutionState)
         check.opt_inst_param(instance, "instance", DagsterInstance)
 
         asset_selection = (
             frozenset(check.opt_set_param(external_pipeline.asset_selection, "asset_selection"))
             if external_pipeline.asset_selection is not None
             else None
         )
 
         execution_plan_snapshot_or_error = sync_get_external_execution_plan_grpc(
             api_client=self.client,
             pipeline_origin=external_pipeline.get_external_origin(),
             run_config=run_config,
-            mode=mode,
             pipeline_snapshot_id=external_pipeline.identifying_pipeline_snapshot_id,
             asset_selection=asset_selection,
             solid_selection=external_pipeline.solid_selection,
             step_keys_to_execute=step_keys_to_execute,
             known_state=known_state,
             instance=instance,
         )
```

### Comparing `dagster-1.3.1/dagster/_core/host_representation/external.py` & `dagster-1.3.2/dagster/_core/host_representation/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from dagster._core.snap.execution_plan_snapshot import ExecutionStepSnap
 from dagster._core.utils import toposort
 from dagster._serdes import create_snapshot_id
 from dagster._utils.cached_method import cached_method
 from dagster._utils.schedules import schedule_execution_time_iterator
 
 from .external_data import (
+    DEFAULT_MODE_NAME,
     EnvVarConsumer,
     ExternalAssetNode,
     ExternalJobRef,
     ExternalPartitionSetData,
     ExternalPipelineData,
     ExternalPresetData,
     ExternalRepositoryData,
@@ -309,21 +310,19 @@
         self._data = external_pipeline_data
         self._ref = external_job_ref
         self._ref_to_data_fn = ref_to_data_fn
 
         if external_pipeline_data:
             self._active_preset_dict = {ap.name: ap for ap in external_pipeline_data.active_presets}
             self._name = external_pipeline_data.name
-            self._is_job = external_pipeline_data.is_job
             self._snapshot_id = self._pipeline_index.pipeline_snapshot_id
 
         elif external_job_ref:
             self._active_preset_dict = {ap.name: ap for ap in external_job_ref.active_presets}
             self._name = external_job_ref.name
-            self._is_job = not external_job_ref.is_legacy_pipeline
             if ref_to_data_fn is None:
                 check.failed("ref_to_data_fn must be passed when using deferred snapshots")
             self._snapshot_id = external_job_ref.snapshot_id
         else:
             check.failed("Expected either job data or ref, got neither")
 
         self._handle = JobHandle(self._name, repository_handle)
@@ -405,29 +404,16 @@
         return preset_name in self._active_preset_dict
 
     def get_preset(self, preset_name: str) -> ExternalPresetData:
         check.str_param(preset_name, "preset_name")
         return self._active_preset_dict[preset_name]
 
     @property
-    def available_modes(self) -> Sequence[str]:
-        return self._pipeline_index.available_modes
-
-    def has_mode(self, mode_name: str) -> bool:
-        check.str_param(mode_name, "mode_name")
-        return self._pipeline_index.has_mode_def(mode_name)
-
-    def root_config_key_for_mode(self, mode_name: Optional[str]) -> Optional[str]:
-        check.opt_str_param(mode_name, "mode_name")
-        return self.get_mode_def_snap(
-            mode_name if mode_name else self.get_default_mode_name()
-        ).root_config_key
-
-    def get_default_mode_name(self) -> str:
-        return self._pipeline_index.get_default_mode_name()
+    def root_config_key(self) -> Optional[str]:
+        return self.get_mode_def_snap(DEFAULT_MODE_NAME).root_config_key
 
     @property
     def tags(self) -> Mapping[str, object]:
         return self._pipeline_index.pipeline_snapshot.tags
 
     @property
     def metadata(self) -> Mapping[str, MetadataValue]:
@@ -451,18 +437,14 @@
 
     def get_external_origin(self) -> ExternalPipelineOrigin:
         return self.handle.get_external_origin()
 
     def get_external_origin_id(self) -> str:
         return self.get_external_origin().get_id()
 
-    @property
-    def is_job(self) -> bool:
-        return self._is_job
-
 
 class ExternalExecutionPlan:
     """ExternalExecution is a object that represents an execution plan that
     was compiled in another process or persisted in an instance.
     """
 
     def __init__(self, execution_plan_snapshot: ExecutionPlanSnapshot):
```

### Comparing `dagster-1.3.1/dagster/_core/host_representation/external_data.py` & `dagster-1.3.2/dagster/_core/host_representation/external_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     ConfigFieldSnap,
     ConfigSchemaSnapshot,
     snap_from_config_type,
 )
 from dagster._core.definitions import (
     JobDefinition,
     PartitionsDefinition,
-    PipelineDefinition,
-    PresetDefinition,
     RepositoryDefinition,
     ScheduleDefinition,
     SourceAsset,
 )
 from dagster._core.definitions.asset_layer import AssetOutputInfo
 from dagster._core.definitions.asset_sensor_definition import AssetSensorDefinition
 from dagster._core.definitions.assets_job import is_base_asset_job_name
@@ -64,15 +62,14 @@
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import (
     MetadataFieldSerializer,
     MetadataUserInput,
     MetadataValue,
     normalize_metadata,
 )
-from dagster._core.definitions.mode import DEFAULT_MODE_NAME
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition import (
     DynamicPartitionsDefinition,
     ScheduleType,
 )
 from dagster._core.definitions.partition_mapping import (
@@ -90,14 +87,17 @@
 from dagster._core.definitions.utils import DEFAULT_GROUP_NAME
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.snap import PipelineSnapshot
 from dagster._core.snap.mode import ResourceDefSnap, build_resource_def_snap
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo
 
+DEFAULT_MODE_NAME = "default"
+DEFAULT_PRESET_NAME = "default"
+
 
 @whitelist_for_serdes
 class ExternalRepositoryData(
     NamedTuple(
         "_ExternalRepositoryData",
         [
             ("name", str),
@@ -247,48 +247,45 @@
             error=check.opt_inst_param(error, "error", SerializableErrorInfo),
             external_pipeline_data=check.opt_inst_param(
                 external_pipeline_data, "external_pipeline_data", ExternalPipelineData
             ),
         )
 
 
-@whitelist_for_serdes
+@whitelist_for_serdes(old_fields={"is_job": True})
 class ExternalPipelineData(
     NamedTuple(
         "_ExternalPipelineData",
         [
             ("name", str),
             ("pipeline_snapshot", PipelineSnapshot),
             ("active_presets", Sequence["ExternalPresetData"]),
             ("parent_pipeline_snapshot", Optional[PipelineSnapshot]),
-            ("is_job", bool),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         pipeline_snapshot: PipelineSnapshot,
         active_presets: Sequence["ExternalPresetData"],
         parent_pipeline_snapshot: Optional[PipelineSnapshot],
-        is_job: bool = False,
     ):
         return super(ExternalPipelineData, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             pipeline_snapshot=check.inst_param(
                 pipeline_snapshot, "pipeline_snapshot", PipelineSnapshot
             ),
             parent_pipeline_snapshot=check.opt_inst_param(
                 parent_pipeline_snapshot, "parent_pipeline_snapshot", PipelineSnapshot
             ),
             active_presets=check.sequence_param(
                 active_presets, "active_presets", of_type=ExternalPresetData
             ),
-            is_job=check.bool_param(is_job, "is_job"),
         )
 
 
 @whitelist_for_serdes
 class EnvVarConsumerType(Enum):
     RESOURCE = "RESOURCE"
 
@@ -307,44 +304,41 @@
 
 @whitelist_for_serdes
 class NestedResource(NamedTuple):
     type: NestedResourceType
     name: str
 
 
-@whitelist_for_serdes
+@whitelist_for_serdes(old_fields={"is_legacy_pipeline": False})
 class ExternalJobRef(
     NamedTuple(
         "_ExternalJobRef",
         [
             ("name", str),
             ("snapshot_id", str),
             ("active_presets", Sequence["ExternalPresetData"]),
             ("parent_snapshot_id", Optional[str]),
-            ("is_legacy_pipeline", bool),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         snapshot_id: str,
         active_presets: Sequence["ExternalPresetData"],
         parent_snapshot_id: Optional[str],
-        is_legacy_pipeline: bool = False,
     ):
         return super(ExternalJobRef, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             snapshot_id=check.str_param(snapshot_id, "snapshot_id"),
             active_presets=check.sequence_param(
                 active_presets, "active_presets", of_type=ExternalPresetData
             ),
             parent_snapshot_id=check.opt_str_param(parent_snapshot_id, "parent_snapshot_id"),
-            is_legacy_pipeline=check.bool_param(is_legacy_pipeline, "is_legacy"),
         )
 
 
 @whitelist_for_serdes
 class ExternalPresetData(
     NamedTuple(
         "_ExternalPresetData",
@@ -448,15 +442,15 @@
         [("pipeline_name", str), ("mode", str), ("solid_selection", Optional[Sequence[str]])],
     )
 ):
     def __new__(cls, pipeline_name: str, mode: str, solid_selection: Optional[Sequence[str]]):
         return super(ExternalTargetData, cls).__new__(
             cls,
             pipeline_name=check.str_param(pipeline_name, "pipeline_name"),
-            mode=check.str_param(mode, "mode"),
+            mode=mode,
             solid_selection=check.opt_nullable_sequence_param(
                 solid_selection, "solid_selection", str
             ),
         )
 
 
 @whitelist_for_serdes
@@ -1156,28 +1150,28 @@
 
 class NodeHandleResourceUse(NamedTuple):
     resource_key: str
     node_handle: NodeHandle
 
 
 def _get_resource_usage_from_node(
-    pipeline: PipelineDefinition,
+    pipeline: JobDefinition,
     node: Node,
     parent_handle: Optional[NodeHandle] = None,
 ) -> Iterable[NodeHandleResourceUse]:
     handle = NodeHandle(node.name, parent_handle)
     if isinstance(node, OpNode):
         for resource_req in node.get_resource_requirements(pipeline.graph):
             yield NodeHandleResourceUse(resource_req.key, handle)
     elif isinstance(node, GraphNode):
         for nested_node in node.definition.nodes:
             yield from _get_resource_usage_from_node(pipeline, nested_node, handle)
 
 
-def _get_resource_job_usage(pipelines: Sequence[PipelineDefinition]) -> ResourceJobUsageMap:
+def _get_resource_job_usage(pipelines: Sequence[JobDefinition]) -> ResourceJobUsageMap:
     resource_job_usage_map: Dict[str, List[ResourceJobUsageEntry]] = defaultdict(list)
 
     for pipeline in pipelines:
         pipeline_name = pipeline.name
         if is_base_asset_job_name(pipeline_name):
             continue
 
@@ -1197,15 +1191,15 @@
 
 def external_repository_data_from_def(
     repository_def: RepositoryDefinition,
     defer_snapshots: bool = False,
 ) -> ExternalRepositoryData:
     check.inst_param(repository_def, "repository_def", RepositoryDefinition)
 
-    pipelines = repository_def.get_all_pipelines()
+    pipelines = repository_def.get_all_jobs()
     if defer_snapshots:
         pipeline_datas = None
         job_refs = sorted(
             list(map(external_job_ref_from_def, pipelines)),
             key=lambda pd: pd.name,
         )
     else:
@@ -1288,19 +1282,19 @@
             ]
             for env_var, res_names in repository_def.get_env_vars_by_top_level_resource().items()
         },
     )
 
 
 def external_asset_graph_from_defs(
-    pipelines: Sequence[PipelineDefinition],
+    pipelines: Sequence[JobDefinition],
     source_assets_by_key: Mapping[AssetKey, SourceAsset],
 ) -> Sequence[ExternalAssetNode]:
     node_defs_by_asset_key: Dict[
-        AssetKey, List[Tuple[NodeOutputHandle, PipelineDefinition]]
+        AssetKey, List[Tuple[NodeOutputHandle, JobDefinition]]
     ] = defaultdict(list)
     asset_info_by_asset_key: Dict[AssetKey, AssetOutputInfo] = dict()
     freshness_policy_by_asset_key: Dict[AssetKey, FreshnessPolicy] = dict()
     metadata_by_asset_key: Dict[AssetKey, MetadataUserInput] = dict()
     auto_materialize_policy_by_asset_key: Dict[AssetKey, AutoMaterializePolicy] = dict()
 
     deps: Dict[AssetKey, Dict[AssetKey, ExternalAssetDependency]] = defaultdict(dict)
@@ -1381,15 +1375,15 @@
         if source_asset.key not in node_defs_by_asset_key:
             job_names = (
                 [
                     job_def.name
                     for job_def in pipelines
                     if source_asset.key in job_def.asset_layer.source_assets_by_key
                     and source_asset.partitions_def is None
-                    or source_asset.partitions_def == job_def.partitions_def  # type: ignore
+                    or source_asset.partitions_def == job_def.partitions_def
                 ]
                 if source_asset.node_def is not None
                 else []
             )
             asset_nodes.append(
                 ExternalAssetNode(
                     asset_key=source_asset.key,
@@ -1474,46 +1468,32 @@
                 required_top_level_resources=required_top_level_resources,
             )
         )
 
     return asset_nodes
 
 
-def external_pipeline_data_from_def(pipeline_def: PipelineDefinition) -> ExternalPipelineData:
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+def external_pipeline_data_from_def(pipeline_def: JobDefinition) -> ExternalPipelineData:
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
     return ExternalPipelineData(
         name=pipeline_def.name,
         pipeline_snapshot=pipeline_def.get_pipeline_snapshot(),
         parent_pipeline_snapshot=pipeline_def.get_parent_pipeline_snapshot(),
-        active_presets=sorted(
-            list(map(external_preset_data_from_def, pipeline_def.preset_defs)),
-            key=lambda pd: pd.name,
-        ),
-        is_job=isinstance(pipeline_def, JobDefinition),
+        active_presets=active_presets_from_job_def(pipeline_def),
     )
 
 
-def external_job_ref_from_def(pipeline_def: PipelineDefinition) -> ExternalJobRef:
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
-
-    parent = pipeline_def.parent_pipeline_def
-    if parent:
-        parent_snapshot_id = parent.get_pipeline_snapshot_id()
-    else:
-        parent_snapshot_id = None
+def external_job_ref_from_def(pipeline_def: JobDefinition) -> ExternalJobRef:
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
 
     return ExternalJobRef(
         name=pipeline_def.name,
         snapshot_id=pipeline_def.get_pipeline_snapshot_id(),
-        parent_snapshot_id=parent_snapshot_id,
-        active_presets=sorted(
-            list(map(external_preset_data_from_def, pipeline_def.preset_defs)),
-            key=lambda pd: pd.name,
-        ),
-        is_legacy_pipeline=not isinstance(pipeline_def, JobDefinition),
+        parent_snapshot_id=None,
+        active_presets=active_presets_from_job_def(pipeline_def),
     )
 
 
 def external_resource_value_from_raw(v: Any) -> ExternalResourceValue:
     if isinstance(v, dict) and set(v.keys()) == {"env"}:
         return ExternalResourceConfigEnvVar(name=v["env"])
     return json.dumps(v)
@@ -1622,15 +1602,15 @@
 def external_schedule_data_from_def(schedule_def: ScheduleDefinition) -> ExternalScheduleData:
     check.inst_param(schedule_def, "schedule_def", ScheduleDefinition)
     return ExternalScheduleData(
         name=schedule_def.name,
         cron_schedule=schedule_def.cron_schedule,
         pipeline_name=schedule_def.job_name,
         solid_selection=schedule_def._target.solid_selection,  # noqa: SLF001
-        mode=schedule_def._target.mode,  # noqa: SLF001
+        mode=DEFAULT_MODE_NAME,
         environment_vars=schedule_def.environment_vars,
         partition_set_name=None,
         execution_timezone=schedule_def.execution_timezone,
         description=schedule_def.description,
         default_status=schedule_def.default_status,
     )
 
@@ -1725,15 +1705,15 @@
     else:
         partitions_def_data = None
 
     return ExternalPartitionSetData(
         name=external_partition_set_name_for_job_name(job_def.name),
         pipeline_name=job_def.name,
         solid_selection=None,
-        mode=job_def.get_mode_definition().name,
+        mode=DEFAULT_MODE_NAME,
         external_partitions_data=partitions_def_data,
     )
 
 
 EXTERNAL_PARTITION_SET_NAME_SUFFIX: Final = "_partition_set"
 
 
@@ -1762,36 +1742,41 @@
             )
             for base_asset_job_name in repository_def.get_implicit_asset_job_names()
         }
     else:
         target_dict = {
             target.pipeline_name: ExternalTargetData(
                 pipeline_name=target.pipeline_name,
-                mode=target.mode,
+                mode=DEFAULT_MODE_NAME,
                 solid_selection=target.solid_selection,
             )
             for target in sensor_def.targets
         }
 
     return ExternalSensorData(
         name=sensor_def.name,
         pipeline_name=first_target.pipeline_name if first_target else None,
-        mode=first_target.mode if first_target else None,
+        mode=None,
         solid_selection=first_target.solid_selection if first_target else None,
         target_dict=target_dict,
         min_interval=sensor_def.minimum_interval_seconds,
         description=sensor_def.description,
         metadata=ExternalSensorMetadata(asset_keys=asset_keys),
         default_status=sensor_def.default_status,
         sensor_type=sensor_def.sensor_type,
     )
 
 
-def external_preset_data_from_def(preset_def: PresetDefinition) -> ExternalPresetData:
-    check.inst_param(preset_def, "preset_def", PresetDefinition)
-    return ExternalPresetData(
-        name=preset_def.name,
-        run_config=preset_def.run_config,
-        solid_selection=preset_def.solid_selection,
-        mode=preset_def.mode,
-        tags=preset_def.tags,
-    )
+def active_presets_from_job_def(job_def: JobDefinition) -> Sequence[ExternalPresetData]:
+    check.inst_param(job_def, "job_def", JobDefinition)
+    if job_def.run_config is None:
+        return []
+    else:
+        return [
+            ExternalPresetData(
+                name=DEFAULT_PRESET_NAME,
+                run_config=job_def.run_config,
+                solid_selection=None,
+                mode=DEFAULT_MODE_NAME,
+                tags={},
+            )
+        ]
```

### Comparing `dagster-1.3.1/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.2/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.2/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/handle.py` & `dagster-1.3.2/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/historical.py` & `dagster-1.3.2/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/origin.py` & `dagster-1.3.2/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/pipeline_index.py` & `dagster-1.3.2/dagster/_core/host_representation/pipeline_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/host_representation/represented.py` & `dagster-1.3.2/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/instance/__init__.py` & `dagster-1.3.2/dagster/_core/instance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 import yaml
 from typing_extensions import Protocol, Self, TypeAlias, TypeVar, runtime_checkable
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.pipeline_base import InMemoryPipeline
-from dagster._core.definitions.pipeline_definition import (
-    PipelineDefinition,
-    PipelineSubsetDefinition,
-)
 from dagster._core.errors import (
     DagsterHomeNotSetError,
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
     DagsterRunAlreadyExists,
     DagsterRunConflict,
 )
@@ -63,15 +59,14 @@
     ASSET_PARTITION_RANGE_END_TAG,
     ASSET_PARTITION_RANGE_START_TAG,
     PARENT_RUN_ID_TAG,
     PARTITION_NAME_TAG,
     RESUME_RETRY_TAG,
     ROOT_RUN_ID_TAG,
 )
-from dagster._core.utils import str_format_list
 from dagster._serdes import ConfigurableClass
 from dagster._seven import get_current_datetime_in_utc
 from dagster._utils import PrintFn, traced
 from dagster._utils.backcompat import deprecation_warning, experimental_functionality_warning
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.merger import merge_dicts
 
@@ -89,14 +84,17 @@
 # whether 'airflow_execution_date' is needed.
 # https://github.com/dagster-io/dagster/issues/2403
 AIRFLOW_EXECUTION_DATE_STR = "airflow_execution_date"
 IS_AIRFLOW_INGEST_PIPELINE_STR = "is_airflow_ingest_pipeline"
 
 if TYPE_CHECKING:
     from dagster._core.debug import DebugRunPayload
+    from dagster._core.definitions.job_definition import (
+        JobDefinition,
+    )
     from dagster._core.definitions.repository_definition.repository_definition import (
         RepositoryLoadData,
     )
     from dagster._core.definitions.run_request import InstigatorType
     from dagster._core.event_api import EventHandlerFn
     from dagster._core.events import DagsterEvent, DagsterEventType, EngineEventData
     from dagster._core.events.log import EventLogEntry
@@ -949,89 +947,71 @@
 
     @traced
     def get_run_group(self, run_id: str) -> Optional[Tuple[str, Sequence[DagsterRun]]]:
         return self._run_storage.get_run_group(run_id)
 
     def create_run_for_pipeline(
         self,
-        pipeline_def: PipelineDefinition,
+        pipeline_def: "JobDefinition",
         execution_plan: Optional["ExecutionPlan"] = None,
         run_id: Optional[str] = None,
         run_config: Optional[Mapping[str, object]] = None,
-        mode: Optional[str] = None,
         solids_to_execute: Optional[AbstractSet[str]] = None,
-        status: Optional[str] = None,
+        status: Optional[Union[DagsterRunStatus, str]] = None,
         tags: Optional[Mapping[str, str]] = None,
         root_run_id: Optional[str] = None,
         parent_run_id: Optional[str] = None,
         solid_selection: Optional[Sequence[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         external_pipeline_origin: Optional["ExternalPipelineOrigin"] = None,
         pipeline_code_origin: Optional[PipelinePythonOrigin] = None,
         repository_load_data: Optional["RepositoryLoadData"] = None,
     ) -> DagsterRun:
         from dagster._core.definitions.job_definition import JobDefinition
         from dagster._core.execution.api import create_execution_plan
         from dagster._core.execution.plan.plan import ExecutionPlan
         from dagster._core.snap import snapshot_from_execution_plan
 
-        check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+        check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
         check.opt_inst_param(execution_plan, "execution_plan", ExecutionPlan)
 
         # note that solids_to_execute is required to execute the solid subset, which is the
         # frozenset version of the previous solid_subset.
         # solid_selection is not required and will not be converted to solids_to_execute here.
         # i.e. this function doesn't handle solid queries.
         # solid_selection is only used to pass the user queries further down.
         check.opt_set_param(solids_to_execute, "solids_to_execute", of_type=str)
         check.opt_list_param(solid_selection, "solid_selection", of_type=str)
         check.opt_set_param(asset_selection, "asset_selection", of_type=AssetKey)
 
-        if solids_to_execute:
-            if isinstance(pipeline_def, PipelineSubsetDefinition):
-                # for the case when pipeline_def is created by IPipeline or ExternalPipeline
-                check.invariant(
-                    solids_to_execute == pipeline_def.nodes_to_execute,
-                    "Cannot create a PipelineRun from pipeline subset {pipeline_solids_to_execute} "
-                    "that conflicts with solids_to_execute arg {solids_to_execute}".format(
-                        pipeline_solids_to_execute=str_format_list(pipeline_def.nodes_to_execute),
-                        solids_to_execute=str_format_list(solids_to_execute),
-                    ),
-                )
-            else:
-                # for cases when `create_run_for_pipeline` is directly called
-                pipeline_def = pipeline_def.get_pipeline_subset_def(
-                    nodes_to_execute=solids_to_execute
-                )
-        if isinstance(pipeline_def, JobDefinition) and (asset_selection or solid_selection):
+        # solids_to_execute never provided
+        if asset_selection or solid_selection:
             # for cases when `create_run_for_pipeline` is directly called
             pipeline_def = pipeline_def.get_job_def_for_subset_selection(
                 asset_selection=asset_selection,
                 op_selection=solid_selection,
             )
         step_keys_to_execute = None
 
         if execution_plan:
             step_keys_to_execute = execution_plan.step_keys_to_execute
 
         else:
             execution_plan = create_execution_plan(
                 pipeline=InMemoryPipeline(pipeline_def),
                 run_config=run_config,
-                mode=mode,
                 instance_ref=self.get_ref() if self.is_persistent else None,
                 tags=tags,
                 repository_load_data=repository_load_data,
             )
 
         return self.create_run(
             pipeline_name=pipeline_def.name,
             run_id=run_id,
             run_config=run_config,
-            mode=check.opt_str_param(mode, "mode", default=pipeline_def.get_default_mode_name()),
             solid_selection=solid_selection,
             asset_selection=asset_selection,
             solids_to_execute=solids_to_execute,
             step_keys_to_execute=step_keys_to_execute,
             status=DagsterRunStatus(status) if status else None,
             tags=tags,
             root_run_id=root_run_id,
@@ -1047,15 +1027,14 @@
         )
 
     def _construct_run_with_snapshots(
         self,
         pipeline_name: str,
         run_id: str,
         run_config: Optional[Mapping[str, object]],
-        mode: Optional[str],
         solids_to_execute: Optional[AbstractSet[str]],
         step_keys_to_execute: Optional[Sequence[str]],
         status: Optional[DagsterRunStatus],
         tags: Mapping[str, str],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
         pipeline_snapshot: Optional[PipelineSnapshot],
@@ -1097,15 +1076,14 @@
             else None
         )
 
         return DagsterRun(
             pipeline_name=pipeline_name,
             run_id=run_id,
             run_config=run_config,
-            mode=mode,
             asset_selection=asset_selection,
             solid_selection=solid_selection,
             solids_to_execute=solids_to_execute,
             step_keys_to_execute=step_keys_to_execute,
             status=status,
             tags=tags,
             root_run_id=root_run_id,
@@ -1247,15 +1225,14 @@
 
     def create_run(
         self,
         *,
         pipeline_name: str,
         run_id: Optional[str],
         run_config: Optional[Mapping[str, object]],
-        mode: Optional[str],
         status: Optional[DagsterRunStatus],
         tags: Optional[Mapping[str, Any]],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
         step_keys_to_execute: Optional[Sequence[str]],
         execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
         pipeline_snapshot: Optional[PipelineSnapshot],
@@ -1271,15 +1248,14 @@
         from dagster._core.snap import ExecutionPlanSnapshot, PipelineSnapshot
 
         check.str_param(pipeline_name, "pipeline_name")
         check.opt_str_param(
             run_id, "run_id"
         )  # will be assigned to make_new_run_id() lower in callstack
         check.opt_mapping_param(run_config, "run_config", key_type=str)
-        check.opt_str_param(mode, "mode")
 
         check.opt_inst_param(status, "status", DagsterRunStatus)
         check.opt_mapping_param(tags, "tags", key_type=str)
 
         validated_tags = validate_tags(tags)
 
         check.opt_str_param(root_run_id, "root_run_id")
@@ -1365,15 +1341,14 @@
         )
         check.opt_inst_param(pipeline_code_origin, "pipeline_code_origin", PipelinePythonOrigin)
 
         pipeline_run = self._construct_run_with_snapshots(
             pipeline_name=pipeline_name,
             run_id=run_id,  # type: ignore  # (possible none)
             run_config=run_config,
-            mode=mode,
             asset_selection=asset_selection,
             solid_selection=solid_selection,
             solids_to_execute=solids_to_execute,
             step_keys_to_execute=step_keys_to_execute,
             status=status,
             tags=validated_tags,
             root_run_id=root_run_id,
@@ -1397,30 +1372,28 @@
         *,
         parent_run: DagsterRun,
         code_location: "CodeLocation",
         external_pipeline: "ExternalPipeline",
         strategy: "ReexecutionStrategy",
         extra_tags: Optional[Mapping[str, Any]] = None,
         run_config: Optional[Mapping[str, Any]] = None,
-        mode: Optional[str] = None,
         use_parent_run_tags: bool = False,
     ) -> DagsterRun:
         from dagster._core.execution.plan.resume_retry import (
             ReexecutionStrategy,
         )
         from dagster._core.execution.plan.state import KnownExecutionState
         from dagster._core.host_representation import CodeLocation, ExternalPipeline
 
         check.inst_param(parent_run, "parent_run", DagsterRun)
         check.inst_param(code_location, "code_location", CodeLocation)
         check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
         check.inst_param(strategy, "strategy", ReexecutionStrategy)
         check.opt_mapping_param(extra_tags, "extra_tags", key_type=str)
         check.opt_mapping_param(run_config, "run_config", key_type=str)
-        check.opt_str_param(mode, "mode")
 
         check.bool_param(use_parent_run_tags, "use_parent_run_tags")
 
         root_run_id = parent_run.root_run_id or parent_run.run_id
         parent_run_id = parent_run.run_id
 
         tags = merge_dicts(
@@ -1430,15 +1403,14 @@
             extra_tags or {},
             {
                 PARENT_RUN_ID_TAG: parent_run_id,
                 ROOT_RUN_ID_TAG: root_run_id,
             },
         )
 
-        mode = cast(str, mode if mode is not None else parent_run.mode)
         run_config = run_config if run_config is not None else parent_run.run_config
 
         if strategy == ReexecutionStrategy.FROM_FAILURE:
             check.invariant(
                 parent_run.status == DagsterRunStatus.FAILURE,
                 "Cannot reexecute from failure a run that is not failed",
             )
@@ -1456,25 +1428,23 @@
             known_state = None
         else:
             raise DagsterInvariantViolationError(f"Unknown reexecution strategy: {strategy}")
 
         external_execution_plan = code_location.get_external_execution_plan(
             external_pipeline,
             run_config,
-            mode=mode,
             step_keys_to_execute=step_keys_to_execute,
             known_state=known_state,
             instance=self,
         )
 
         return self.create_run(
             pipeline_name=parent_run.pipeline_name,
             run_id=None,
             run_config=run_config,
-            mode=mode,
             solids_to_execute=parent_run.solids_to_execute,
             step_keys_to_execute=step_keys_to_execute,
             status=DagsterRunStatus.NOT_STARTED,
             tags=tags,
             root_run_id=root_run_id,
             parent_run_id=parent_run_id,
             pipeline_snapshot=external_pipeline.pipeline_snapshot,
@@ -1487,15 +1457,14 @@
         )
 
     def register_managed_run(
         self,
         pipeline_name: str,
         run_id: str,
         run_config: Optional[Mapping[str, object]],
-        mode: Optional[str],
         solids_to_execute: Optional[AbstractSet[str]],
         step_keys_to_execute: Optional[Sequence[str]],
         tags: Mapping[str, str],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
         pipeline_snapshot: Optional[PipelineSnapshot],
         execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
@@ -1514,15 +1483,14 @@
         # error; at this point, the failed tasks try again to fetch the existing run.
         # https://github.com/dagster-io/dagster/issues/2412
 
         pipeline_run = self._construct_run_with_snapshots(
             pipeline_name=pipeline_name,
             run_id=run_id,
             run_config=run_config,
-            mode=mode,
             solid_selection=solid_selection,
             solids_to_execute=solids_to_execute,
             step_keys_to_execute=step_keys_to_execute,
             status=DagsterRunStatus.MANAGED,
             tags=tags,
             root_run_id=root_run_id,
             parent_run_id=parent_run_id,
```

### Comparing `dagster-1.3.1/dagster/_core/instance/config.py` & `dagster-1.3.2/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/instance/ref.py` & `dagster-1.3.2/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/instance_for_test.py` & `dagster-1.3.2/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/launcher/base.py` & `dagster-1.3.2/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.2/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.2/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/log_manager.py` & `dagster-1.3.2/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/nux.py` & `dagster-1.3.2/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/origin.py` & `dagster-1.3.2/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/run_coordinator/base.py` & `dagster-1.3.2/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.2/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.2/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/scheduler/__init__.py` & `dagster-1.3.2/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/scheduler/execution.py` & `dagster-1.3.2/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/scheduler/instigation.py` & `dagster-1.3.2/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.2/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/secrets/env_file.py` & `dagster-1.3.2/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/selector/subset_selector.py` & `dagster-1.3.2/dagster/_core/selector/subset_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from dagster._core.definitions.events import AssetKey
 from dagster._core.errors import DagsterExecutionStepNotFoundError, DagsterInvalidSubsetError
 from dagster._utils import check
 
 if TYPE_CHECKING:
     from dagster._core.definitions.assets import AssetsDefinition
     from dagster._core.definitions.job_definition import JobDefinition
-    from dagster._core.definitions.pipeline_definition import PipelineDefinition
     from dagster._core.definitions.source_asset import SourceAsset
 
 MAX_NUM = sys.maxsize
 
 T = TypeVar("T")
 T_Hashable = TypeVar("T_Hashable", bound=Hashable)
 Direction: TypeAlias = Literal["downstream", "upstream"]
@@ -127,15 +126,15 @@
             )
             for upstream_key in upstream_asset_keys:
                 upstream[asset_key].add(upstream_key)
                 downstream[upstream_key] = downstream.get(upstream_key, set()) | {asset_key}
     return {"upstream": upstream, "downstream": downstream}
 
 
-def generate_dep_graph(pipeline_def: "PipelineDefinition") -> DependencyGraph[str]:
+def generate_dep_graph(pipeline_def: "JobDefinition") -> DependencyGraph[str]:
     """Pipeline to dependency graph. It currently only supports top-level solids.
 
     Args:
         pipeline (PipelineDefinition): The pipeline to execute.
 
     Returns:
         graph (Dict[str, Dict[str, Set[str]]]): the input and output dependency graph. e.g.
@@ -405,15 +404,15 @@
     return {
         top_level_op: SELECTION_TREE_LEAF_NODE
         for top_level_op in parse_solid_selection(job_def, op_selection)
     }
 
 
 def parse_solid_selection(
-    pipeline_def: "PipelineDefinition",
+    pipeline_def: "JobDefinition",
     solid_selection: Sequence[str],
 ) -> FrozenSet[str]:
     """Take pipeline definition and a list of solid selection queries (inlcuding names of solid
         invocations. See syntax examples below) and return a set of the qualified solid names.
 
     It currently only supports top-level solids.
 
@@ -448,19 +447,15 @@
     solids_set: Set[str] = set()
 
     # loop over clauses
     for clause in solid_selection:
         subset = clause_to_subset(graph, clause, lambda x: x)
         if len(subset) == 0:
             raise DagsterInvalidSubsetError(
-                "No qualified {node_type} to execute found for {selection_type}={requested}".format(
-                    requested=solid_selection,
-                    node_type="ops" if pipeline_def.is_job else "solids",
-                    selection_type="op_selection" if pipeline_def.is_job else "solid_selection",
-                )
+                f"No qualified ops to execute found for op_selection={solid_selection}"
             )
         solids_set.update(subset)
 
     return frozenset(solids_set)
 
 
 def parse_step_selection(
```

### Comparing `dagster-1.3.1/dagster/_core/snap/__init__.py` & `dagster-1.3.2/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/snap/dagster_types.py` & `dagster-1.3.2/dagster/_core/snap/dagster_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Mapping, NamedTuple, Optional, Sequence
 
 import dagster._check as check
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.metadata import (
     MetadataFieldSerializer,
     MetadataValue,
     normalize_metadata,
 )
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.types.dagster_type import DagsterType, DagsterTypeKind
 from dagster._serdes import whitelist_for_serdes
 
 
 def build_dagster_type_namespace_snapshot(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
 ) -> "DagsterTypeNamespaceSnapshot":
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
     return DagsterTypeNamespaceSnapshot(
         {dt.key: build_dagster_type_snap(dt) for dt in pipeline_def.all_dagster_types()}
     )
 
 
 def build_dagster_type_snap(dagster_type: DagsterType) -> "DagsterTypeSnap":
     check.inst_param(dagster_type, "dagster_type", DagsterType)
```

### Comparing `dagster-1.3.1/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.2/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.2/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/snap/mode.py` & `dagster-1.3.2/dagster/_core/snap/mode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # Contains mode, resources, loggers
 from typing import NamedTuple, Optional, Sequence
 
 import dagster._check as check
 from dagster._config import ConfigFieldSnap, snap_from_field
-from dagster._core.definitions import LoggerDefinition, ModeDefinition, ResourceDefinition
+from dagster._core.definitions import LoggerDefinition, ResourceDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._serdes import whitelist_for_serdes
 
 
-def build_mode_def_snap(mode_def, root_config_key):
-    check.inst_param(mode_def, "mode_def", ModeDefinition)
-    check.str_param(root_config_key, "root_config_key")
+def build_mode_def_snap(job_def: JobDefinition) -> "ModeDefSnap":
+    from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 
+    check.inst_param(job_def, "job_def", JobDefinition)
+
+    root_config_key = job_def.run_config_schema.config_type.key
     return ModeDefSnap(
-        name=mode_def.name,
-        description=mode_def.description,
+        name=DEFAULT_MODE_NAME,
+        description=None,
         resource_def_snaps=sorted(
-            [build_resource_def_snap(name, rd) for name, rd in mode_def.resource_defs.items()],
+            [build_resource_def_snap(name, rd) for name, rd in job_def.resource_defs.items()],
             key=lambda item: item.name,
         ),
         logger_def_snaps=sorted(
-            [build_logger_def_snap(name, ld) for name, ld in mode_def.loggers.items()],
+            [build_logger_def_snap(name, ld) for name, ld in job_def.loggers.items()],
             key=lambda item: item.name,
         ),
         root_config_key=root_config_key,
     )
 
 
 @whitelist_for_serdes
```

### Comparing `dagster-1.3.1/dagster/_core/snap/node.py` & `dagster-1.3.2/dagster/_core/snap/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import dagster._check as check
 from dagster._config import ConfigFieldSnap, snap_from_field
 from dagster._core.definitions import (
     GraphDefinition,
     InputDefinition,
     InputMapping,
+    JobDefinition,
     OpDefinition,
     OutputDefinition,
     OutputMapping,
-    PipelineDefinition,
 )
 from dagster._core.definitions.metadata import (
     MetadataFieldSerializer,
     MetadataValue,
     normalize_metadata,
 )
 from dagster._serdes import whitelist_for_serdes
@@ -342,16 +342,16 @@
                     of_type=GraphDefSnap,
                 ),
                 key=lambda graph_def: graph_def.name,
             ),
         )
 
 
-def build_node_defs_snapshot(pipeline_def: PipelineDefinition) -> NodeDefsSnapshot:
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+def build_node_defs_snapshot(pipeline_def: JobDefinition) -> NodeDefsSnapshot:
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
     op_def_snaps = []
     graph_def_snaps = []
     for node_def in pipeline_def.all_node_defs:
         if isinstance(node_def, OpDefinition):
             op_def_snaps.append(build_op_def_snap(node_def))
         elif isinstance(node_def, GraphDefinition):
             graph_def_snaps.append(build_graph_def_snap(node_def))
```

### Comparing `dagster-1.3.1/dagster/_core/snap/pipeline_snapshot.py` & `dagster-1.3.2/dagster/_core/snap/pipeline_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,23 @@
     Permissive,
     ScalarUnion,
     Selector,
     Shape,
     get_builtin_scalar_by_name,
 )
 from dagster._core.definitions.events import AssetKey
-from dagster._core.definitions.job_definition import JobDefinition
+from dagster._core.definitions.job_definition import (
+    JobDefinition,
+)
 from dagster._core.definitions.metadata import (
     MetadataFieldSerializer,
     MetadataValue,
     RawMetadataValue,
     normalize_metadata,
 )
-from dagster._core.definitions.pipeline_definition import (
-    PipelineDefinition,
-    PipelineSubsetDefinition,
-)
 from dagster._core.utils import toposort_flatten
 from dagster._serdes import (
     create_snapshot_id,
     deserialize_value,
     whitelist_for_serdes,
 )
 from dagster._serdes.serdes import NamedTupleSerializer
@@ -71,23 +69,24 @@
     #     - metadata added
     # v4:
     #     - add kwargs so that if future versions add new args, this version of deserialization will
     #     be able to ignore them. previously, new args would be passed to old versions and cause
     #     deserialization errors.
     def before_unpack(
         self,
-        **packed: Any,
+        context,
+        unpacked_dict: Any,
     ) -> Dict[str, Any]:
-        if packed.get("graph_def_name") is None:
-            packed["graph_def_name"] = packed["name"]
-        if packed.get("metadata") is None:
-            packed["metadata"] = {}
-        if packed.get("lineage_snapshot") is None:
-            packed["lineage_snapshot"] = None
-        return packed
+        if unpacked_dict.get("graph_def_name") is None:
+            unpacked_dict["graph_def_name"] = unpacked_dict["name"]
+        if unpacked_dict.get("metadata") is None:
+            unpacked_dict["metadata"] = []
+        if unpacked_dict.get("lineage_snapshot") is None:
+            unpacked_dict["lineage_snapshot"] = None
+        return unpacked_dict
 
 
 # Note that unlike other serdes-whitelisted objects that hold metadata, the field here has always
 # been called `metadata` instead of `metadata_entries`, so we don't need to rename the field for
 # serialization.
 @whitelist_for_serdes(
     serializer=PipelineSnapshotSerializer,
@@ -155,34 +154,26 @@
             graph_def_name=check.str_param(graph_def_name, "graph_def_name"),
             metadata=normalize_metadata(
                 check.opt_mapping_param(metadata, "metadata", key_type=str)
             ),
         )
 
     @classmethod
-    def from_pipeline_def(cls, pipeline_def: PipelineDefinition) -> "PipelineSnapshot":
-        check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    def from_pipeline_def(cls, pipeline_def: JobDefinition) -> "PipelineSnapshot":
+        check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
         lineage = None
-        if isinstance(pipeline_def, PipelineSubsetDefinition):
-            lineage = PipelineSnapshotLineage(
-                parent_snapshot_id=create_pipeline_snapshot_id(
-                    cls.from_pipeline_def(pipeline_def.parent_pipeline_def)
-                ),
-                node_selection=sorted(pipeline_def.node_selection),
-                nodes_to_execute=pipeline_def.nodes_to_execute,
-            )
-        if isinstance(pipeline_def, JobDefinition) and pipeline_def.op_selection_data:
+        if pipeline_def.op_selection_data:
             lineage = PipelineSnapshotLineage(
                 parent_snapshot_id=create_pipeline_snapshot_id(
                     cls.from_pipeline_def(pipeline_def.op_selection_data.parent_job_def)
                 ),
                 node_selection=sorted(pipeline_def.op_selection_data.op_selection),
                 nodes_to_execute=pipeline_def.op_selection_data.resolved_op_selection,
             )
-        if isinstance(pipeline_def, JobDefinition) and pipeline_def.asset_selection_data:
+        if pipeline_def.asset_selection_data:
             lineage = PipelineSnapshotLineage(
                 parent_snapshot_id=create_pipeline_snapshot_id(
                     cls.from_pipeline_def(pipeline_def.asset_selection_data.parent_job_def)
                 ),
                 asset_selection=pipeline_def.asset_selection_data.asset_selection,
             )
 
@@ -191,18 +182,15 @@
             description=pipeline_def.description,
             tags=pipeline_def.tags,
             metadata=pipeline_def.metadata,
             config_schema_snapshot=build_config_schema_snapshot(pipeline_def),
             dagster_type_namespace_snapshot=build_dagster_type_namespace_snapshot(pipeline_def),
             node_defs_snapshot=build_node_defs_snapshot(pipeline_def),
             dep_structure_snapshot=build_dep_structure_snapshot_from_graph_def(pipeline_def.graph),
-            mode_def_snaps=[
-                build_mode_def_snap(md, pipeline_def.get_run_config_schema(md.name).config_type.key)
-                for md in pipeline_def.mode_definitions
-            ],
+            mode_def_snaps=[build_mode_def_snap(pipeline_def)],
             lineage_snapshot=lineage,
             graph_def_name=pipeline_def.graph.name,
         )
 
     def get_node_def_snap(self, node_def_name: str) -> Union[OpDefSnap, GraphDefSnap]:
         check.str_param(node_def_name, "node_def_name")
         for node_def_snap in self.node_defs_snapshot.op_def_snaps:
```

### Comparing `dagster-1.3.1/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.2/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/README.md` & `dagster-1.3.2/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/env.py` & `dagster-1.3.2/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.2/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.2/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/base_storage.py` & `dagster-1.3.2/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.2/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.2/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.2/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.2/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/config.py` & `dagster-1.3.2/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.2/dagster/_core/storage/db_io_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,17 +192,17 @@
             else:
                 schema = "public"
             if context.has_asset_partitions:
                 partition_expr = output_context_metadata.get("partition_expr")
                 if partition_expr is None:
                     raise ValueError(
                         f"Asset '{context.asset_key}' has partitions, but no 'partition_expr'"
-                        " metadata value, so we don't know what column to filter it on. Specify"
-                        " which column(s) of the database contains partitioned data as the"
-                        " 'partition_expr' metadata."
+                        " metadata value, so we don't know what column it's partitioned on. To"
+                        " specify a column, set this metadata value. E.g."
+                        ' @asset(metadata={"partition_expr": "your_partition_column"}).'
                     )
 
                 if isinstance(context.asset_partitions_def, MultiPartitionsDefinition):
                     multi_partition_key_mapping = cast(
                         MultiPartitionKey, context.asset_partition_key
                     ).keys_by_dimension
                     for part in context.asset_partitions_def.partitions_defs:
```

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.2/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/base.py` & `dagster-1.3.2/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.2/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.2/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.2/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.2/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.2/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.2/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.2/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,16 @@
             for filename in all_filenames
             if os.path.splitext(os.path.basename(filename))[0] != INDEX_SHARD_NAME
         ]
 
     def has_table(self, table_name: str) -> bool:
         conn_string = self.conn_string_for_shard(INDEX_SHARD_NAME)
         engine = create_engine(conn_string, poolclass=NullPool)
-        return bool(engine.dialect.has_table(engine.connect(), table_name))
+        with engine.connect() as conn:
+            return bool(engine.dialect.has_table(conn, table_name))
 
     def path_for_shard(self, run_id: str) -> str:
         return os.path.join(self._base_dir, f"{run_id}.db")
 
     def conn_string_for_shard(self, shard_name: str) -> str:
         check.str_param(shard_name, "shard_name")
         return create_db_conn_string(self._base_dir, shard_name)
@@ -163,15 +164,15 @@
         while True:
             try:
                 with engine.connect() as connection:
                     db_revision, head_revision = check_alembic_revision(alembic_config, connection)
 
                     if not (db_revision and head_revision):
                         SqlEventLogStorageMetadata.create_all(engine)
-                        engine.execute("PRAGMA journal_mode=WAL;")
+                        connection.execute("PRAGMA journal_mode=WAL;")
                         stamp_alembic_rev(alembic_config, connection)
 
                 break
             except (db_exc.DatabaseError, sqlite3.DatabaseError, sqlite3.OperationalError) as exc:
                 # This is SQLite-specific handling for concurrency issues that can arise when
                 # multiple processes (e.g. the dagit process and user code process) contend with
                 # each other to init the db. When we hit the following errors, we know that another
```

### Comparing `dagster-1.3.1/dagster/_core/storage/file_manager.py` & `dagster-1.3.2/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.2/dagster/_core/storage/fs_io_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,136 @@
 import os
 import pickle
 from typing import Any, Optional
 
+from pydantic import Field
 from upath import UPath
 
 import dagster._check as check
-from dagster import DagsterInvariantViolationError
+from dagster import (
+    DagsterInvariantViolationError,
+    Field as DagsterField,
+)
 from dagster._annotations import experimental
-from dagster._config import Field, StringSource
+from dagster._config import StringSource
+from dagster._config.pythonic_config import ConfigurableIOManagerFactory
 from dagster._core.definitions.events import AssetKey, AssetMaterialization
 from dagster._core.definitions.metadata import MetadataValue
 from dagster._core.execution.context.init import InitResourceContext
 from dagster._core.execution.context.input import InputContext
 from dagster._core.execution.context.output import OutputContext
 from dagster._core.storage.io_manager import IOManager, io_manager
 from dagster._core.storage.upath_io_manager import UPathIOManager
 from dagster._utils import PICKLE_PROTOCOL, mkdir_p
 
 
+class FilesystemIOManager(ConfigurableIOManagerFactory["PickledObjectFilesystemIOManager"]):
+    """Built-in filesystem IO manager that stores and retrieves values using pickling.
+
+    The base directory that the pickle files live inside is determined by:
+
+    * The IO manager's "base_dir" configuration value, if specified. Otherwise...
+    * A "storage/" directory underneath the value for "local_artifact_storage" in your dagster.yaml
+      file, if specified. Otherwise...
+    * A "storage/" directory underneath the directory that the DAGSTER_HOME environment variable
+      points to, if that environment variable is specified. Otherwise...
+    * A temporary directory.
+
+    Assigns each op output to a unique filepath containing run ID, step key, and output name.
+    Assigns each asset to a single filesystem path, at "<base_dir>/<asset_key>". If the asset key
+    has multiple components, the final component is used as the name of the file, and the preceding
+    components as parent directories under the base_dir.
+
+    Subsequent materializations of an asset will overwrite previous materializations of that asset.
+    So, with a base directory of "/my/base/path", an asset with key
+    `AssetKey(["one", "two", "three"])` would be stored in a file called "three" in a directory
+    with path "/my/base/path/one/two/".
+
+    Example usage:
+
+
+    1. Attach an IO manager to a set of assets using the reserved resource key ``"io_manager"``.
+
+    .. code-block:: python
+
+        from dagster import Definitions, asset, FilesystemIOManager
+
+        @asset
+        def asset1():
+            # create df ...
+            return df
+
+        @asset
+        def asset2(asset1):
+            return asset1[:5]
+
+        defs = Definitions(
+            assets=[asset1, asset2],
+            resources={
+                "io_manager": FilesystemIOManager(base_dir="/my/base/path")
+            },
+        )
+
+
+    2. Specify a job-level IO manager using the reserved resource key ``"io_manager"``,
+    which will set the given IO manager on all ops in a job.
+
+    .. code-block:: python
+
+        from dagster import FilesystemIOManager, job, op
+
+        @op
+        def op_a():
+            # create df ...
+            return df
+
+        @op
+        def op_b(df):
+            return df[:5]
+
+        @job(
+            resource_defs={
+                "io_manager": FilesystemIOManager(base_dir="/my/base/path")
+            }
+        )
+        def job():
+            op_b(op_a())
+
+
+    3. Specify IO manager on :py:class:`Out`, which allows you to set different IO managers on
+    different step outputs.
+
+    .. code-block:: python
+
+        from dagster import FilesystemIOManager, job, op, Out
+
+        @op(out=Out(io_manager_key="my_io_manager"))
+        def op_a():
+            # create df ...
+            return df
+
+        @op
+        def op_b(df):
+            return df[:5]
+
+        @job(resource_defs={"my_io_manager": FilesystemIOManager()})
+        def job():
+            op_b(op_a())
+
+    """
+
+    base_dir: Optional[str] = Field(default=None, description="Base directory for storing files.")
+
+    def create_io_manager(self, context: InitResourceContext) -> "PickledObjectFilesystemIOManager":
+        base_dir = self.base_dir or check.not_none(context.instance).storage_directory()
+        return PickledObjectFilesystemIOManager(base_dir=base_dir)
+
+
 @io_manager(
-    config_schema={"base_dir": Field(StringSource, is_required=False)},
+    config_schema=FilesystemIOManager.to_config_schema(),
     description="Built-in filesystem IO manager that stores and retrieves values using pickling.",
 )
 def fs_io_manager(init_context: InitResourceContext) -> "PickledObjectFilesystemIOManager":
     """Built-in filesystem IO manager that stores and retrieves values using pickling.
 
     The base directory that the pickle files live inside is determined by:
 
@@ -47,33 +154,31 @@
     Example usage:
 
 
     1. Attach an IO manager to a set of assets using the reserved resource key ``"io_manager"``.
 
     .. code-block:: python
 
-        from dagster import asset, fs_io_manager, repository, with_resources
+        from dagster import Definitions, asset, fs_io_manager
 
         @asset
         def asset1():
             # create df ...
             return df
 
         @asset
         def asset2(asset1):
             return asset1[:5]
 
-        @repository
-        def repo():
-            return with_resources(
-                [asset1, asset2],
-                resource_defs={
-                    "io_manager": fs_io_manager.configured({"base_dir": "/my/base/path"})
-                },
-            )
+        defs = Definitions(
+            assets=[asset1, asset2],
+            resources={
+                "io_manager": fs_io_manager.configured({"base_dir": "/my/base/path"})
+            },
+        )
 
 
     2. Specify a job-level IO manager using the reserved resource key ``"io_manager"``,
     which will set the given IO manager on all ops in a job.
 
     .. code-block:: python
 
@@ -114,19 +219,15 @@
             return df[:5]
 
         @job(resource_defs={"my_io_manager": fs_io_manager})
         def job():
             op_b(op_a())
 
     """
-    base_dir = init_context.resource_config.get(
-        "base_dir", init_context.instance.storage_directory()  # type: ignore
-    )
-
-    return PickledObjectFilesystemIOManager(base_dir=base_dir)
+    return FilesystemIOManager.from_resource_context(init_context)
 
 
 class PickledObjectFilesystemIOManager(UPathIOManager):
     """Built-in filesystem IO manager that stores and retrieves values using pickling.
     Is compatible with local and remote filesystems via `universal-pathlib` and `fsspec`.
     Learn more about how to use remote filesystems here: https://github.com/fsspec/universal_pathlib.
 
@@ -144,15 +245,15 @@
         super().__init__(base_path=UPath(base_dir, **kwargs))
 
     def dump_to_path(self, context: OutputContext, obj: Any, path: UPath):
         try:
             with path.open("wb") as file:
                 pickle.dump(obj, file, PICKLE_PROTOCOL)
         except (AttributeError, RecursionError, ImportError, pickle.PicklingError) as e:
-            executor = context.step_context.pipeline_def.mode_definitions[0].executor_defs[0]
+            executor = context.step_context.pipeline_def.executor_def
 
             if isinstance(e, RecursionError):
                 # if obj can't be pickled because of RecursionError then __str__() will also
                 # throw a RecursionError
                 obj_repr = f"{obj.__class__} exceeds recursion limit and"
             else:
                 obj_repr = obj.__str__()
@@ -222,15 +323,15 @@
         filepath = self._get_path(path)
         context.log.debug(f"Loading file from: {filepath}")
 
         with open(filepath, self.read_mode) as read_obj:
             return pickle.load(read_obj)
 
 
-@io_manager(config_schema={"base_dir": Field(StringSource, is_required=True)})
+@io_manager(config_schema={"base_dir": DagsterField(StringSource, is_required=True)})
 @experimental
 def custom_path_fs_io_manager(
     init_context: InitResourceContext,
 ) -> CustomPathPickledObjectFilesystemIOManager:
     """Built-in IO manager that allows users to custom output file path per output definition.
 
     It requires users to specify a base directory where all the step output will be stored in. It
```

### Comparing `dagster-1.3.1/dagster/_core/storage/input_manager.py` & `dagster-1.3.2/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/io_manager.py` & `dagster-1.3.2/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.2/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.2/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.2/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.2/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/migration/utils.py` & `dagster-1.3.2/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.2/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/output_manager.py` & `dagster-1.3.2/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.2/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/pipeline_run.py` & `dagster-1.3.2/dagster/_core/storage/pipeline_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from dagster._annotations import public
 from dagster._core.definitions.events import AssetKey
 from dagster._core.origin import PipelinePythonOrigin
 from dagster._core.storage.tags import PARENT_RUN_ID_TAG, ROOT_RUN_ID_TAG
 from dagster._core.utils import make_new_run_id
 from dagster._serdes.serdes import (
     NamedTupleSerializer,
-    copy_packed_set,
     whitelist_for_serdes,
 )
 
 from .tags import (
     BACKFILL_ID_TAG,
     REPOSITORY_LABEL_TAG,
     RESUME_RETRY_TAG,
@@ -148,87 +147,87 @@
     # * added execution_plan_snapshot_id
     # * removed selector
     # * added solid_subset
     # * renamed solid_subset -> solid_selection, added solids_to_execute
     # * renamed environment_dict -> run_config
     # * added asset_selection
     # * added has_repository_load_data
-    def before_unpack(self, **unpacked: Any) -> Dict[str, Any]:
+    def before_unpack(self, context, unpacked_dict: Dict[str, Any]) -> Dict[str, Any]:
         # back compat for environment dict => run_config
-        if "environment_dict" in unpacked:
+        if "environment_dict" in unpacked_dict:
             check.invariant(
-                unpacked.get("run_config") is None,
+                unpacked_dict.get("run_config") is None,
                 "Cannot set both run_config and environment_dict. Use run_config parameter.",
             )
-            unpacked["run_config"] = unpacked["environment_dict"]
-            del unpacked["environment_dict"]
+            unpacked_dict["run_config"] = unpacked_dict["environment_dict"]
+            del unpacked_dict["environment_dict"]
 
         # back compat for previous_run_id => parent_run_id, root_run_id
-        if "previous_run_id" in unpacked and not (
-            "parent_run_id" in unpacked and "root_run_id" in unpacked
+        if "previous_run_id" in unpacked_dict and not (
+            "parent_run_id" in unpacked_dict and "root_run_id" in unpacked_dict
         ):
-            unpacked["parent_run_id"] = unpacked["previous_run_id"]
-            unpacked["root_run_id"] = unpacked["previous_run_id"]
-            del unpacked["previous_run_id"]
+            unpacked_dict["parent_run_id"] = unpacked_dict["previous_run_id"]
+            unpacked_dict["root_run_id"] = unpacked_dict["previous_run_id"]
+            del unpacked_dict["previous_run_id"]
 
         # back compat for selector => pipeline_name, solids_to_execute
-        if "selector" in unpacked:
-            selector = unpacked["selector"]
+        if "selector" in unpacked_dict:
+            selector = unpacked_dict["selector"]
 
-            pipeline_name = unpacked.get("pipeline_name")
+            if not isinstance(selector, ExecutionSelector):
+                check.failed(f"unexpected entry for 'select', {selector}")
+            selector_name = selector.name
+            selector_subset = selector.solid_subset
+
+            pipeline_name = unpacked_dict.get("pipeline_name")
             check.invariant(
-                pipeline_name is None or selector.get("name") == pipeline_name,
+                pipeline_name is None or selector_name == pipeline_name,
                 (
                     f"Conflicting pipeline name {pipeline_name} in arguments to PipelineRun: "
-                    f"selector was passed with pipeline {selector.get('name')}"
+                    f"selector was passed with pipeline {selector_name}"
                 ),
             )
             if pipeline_name is None:
-                unpacked["pipeline_name"] = selector.get("name")
+                unpacked_dict["pipeline_name"] = selector_name
 
-            solids_to_execute = unpacked.get("solids_to_execute")
+            solids_to_execute = unpacked_dict.get("solids_to_execute")
             check.invariant(
-                solids_to_execute is None or set(selector.get("solid_subset")) == solids_to_execute,
+                solids_to_execute is None
+                or (selector_subset and set(selector_subset) == solids_to_execute),
                 (
                     f"Conflicting solids_to_execute {solids_to_execute} in arguments to"
-                    f" PipelineRun: selector was passed with subset {selector.get('solid_subset')}"
+                    f" PipelineRun: selector was passed with subset {selector_subset}"
                 ),
             )
             # for old runs that only have selector but no solids_to_execute
             if solids_to_execute is None:
-                solids_to_execute = (
-                    copy_packed_set(selector["solid_subset"], "__frozenset__")
-                    if selector.get("solid_subset")
-                    else None
-                )
+                solids_to_execute = frozenset(selector_subset) if selector_subset else None
 
         # back compat for solid_subset => solids_to_execute
-        if "solid_subset" in unpacked:
-            unpacked["solids_to_execute"] = copy_packed_set(
-                unpacked["solid_subset"], "__frozenset__"
-            )
-            del unpacked["solid_subset"]
+        if "solid_subset" in unpacked_dict:
+            unpacked_dict["solids_to_execute"] = unpacked_dict["solid_subset"]
+            del unpacked_dict["solid_subset"]
 
-        return unpacked
+        return unpacked_dict
 
 
 @whitelist_for_serdes(
     serializer=DagsterRunSerializer,
     # DagsterRun is serialized as PipelineRun so that it can be read by older (pre 0.13.x) version
     # of Dagster, but is read back in as a DagsterRun.
     storage_name="PipelineRun",
+    old_fields={"mode": None},
 )
 class DagsterRun(
     NamedTuple(
         "_DagsterRun",
         [
             ("pipeline_name", str),
             ("run_id", str),
             ("run_config", Mapping[str, object]),
-            ("mode", Optional[str]),
             ("asset_selection", Optional[AbstractSet[AssetKey]]),
             ("solid_selection", Optional[Sequence[str]]),
             ("solids_to_execute", Optional[AbstractSet[str]]),
             ("step_keys_to_execute", Optional[Sequence[str]]),
             ("status", DagsterRunStatus),
             ("tags", Mapping[str, str]),
             ("root_run_id", Optional[str]),
@@ -246,15 +245,14 @@
     """
 
     def __new__(
         cls,
         pipeline_name: str,
         run_id: Optional[str] = None,
         run_config: Optional[Mapping[str, object]] = None,
-        mode: Optional[str] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         solid_selection: Optional[Sequence[str]] = None,
         solids_to_execute: Optional[AbstractSet[str]] = None,
         step_keys_to_execute: Optional[Sequence[str]] = None,
         status: Optional[DagsterRunStatus] = None,
         tags: Optional[Mapping[str, str]] = None,
         root_run_id: Optional[str] = None,
@@ -304,15 +302,14 @@
             run_id = make_new_run_id()
 
         return super(DagsterRun, cls).__new__(
             cls,
             pipeline_name=check.str_param(pipeline_name, "pipeline_name"),
             run_id=check.str_param(run_id, "run_id"),
             run_config=check.opt_mapping_param(run_config, "run_config", key_type=str),
-            mode=check.opt_str_param(mode, "mode"),
             solid_selection=solid_selection,
             asset_selection=asset_selection,
             solids_to_execute=solids_to_execute,
             step_keys_to_execute=step_keys_to_execute,
             status=check.opt_inst_param(
                 status, "status", DagsterRunStatus, DagsterRunStatus.NOT_STARTED
             ),
@@ -350,17 +347,14 @@
 
     def with_job_origin(self, origin: "ExternalPipelineOrigin") -> Self:
         from dagster._core.host_representation.origin import ExternalPipelineOrigin
 
         check.inst_param(origin, "origin", ExternalPipelineOrigin)
         return self._replace(external_pipeline_origin=origin)
 
-    def with_mode(self, mode: str) -> Self:
-        return self._replace(mode=mode)
-
     def with_tags(self, tags: Mapping[str, str]) -> Self:
         return self._replace(tags=tags)
 
     def get_root_run_id(self) -> Optional[str]:
         return self.tags.get(ROOT_RUN_ID_TAG)
 
     def get_parent_run_id(self) -> Optional[str]:
@@ -427,15 +421,16 @@
     def tags_for_backfill_id(backfill_id: str) -> Mapping[str, str]:
         return {BACKFILL_ID_TAG: backfill_id}
 
 
 class RunsFilterSerializer(NamedTupleSerializer["RunsFilter"]):
     def before_unpack(
         self,
-        **unpacked_dict: Any,
+        context,
+        unpacked_dict: Dict[str, Any],
     ) -> Dict[str, Any]:
         # We store empty run ids as [] but only accept None
         if "run_ids" in unpacked_dict and unpacked_dict["run_ids"] == []:
             unpacked_dict["run_ids"] = None
         return unpacked_dict
 
 
@@ -451,15 +446,14 @@
             ("run_ids", Sequence[str]),
             ("job_name", Optional[str]),
             ("statuses", Sequence[DagsterRunStatus]),
             ("tags", Mapping[str, Union[str, Sequence[str]]]),
             ("snapshot_id", Optional[str]),
             ("updated_after", Optional[datetime]),
             ("updated_before", Optional[datetime]),
-            ("mode", Optional[str]),
             ("created_after", Optional[datetime]),
             ("created_before", Optional[datetime]),
         ],
     )
 ):
     """Defines a filter across job runs, for use when querying storage directly.
 
@@ -475,29 +469,27 @@
         statuses (Optional[List[DagsterRunStatus]]):
             A list of run statuses to filter by. If blank, all run statuses will be allowed.
         tags (Optional[Dict[str, Union[str, List[str]]]]):
             A dictionary of run tags to query by. All tags specified here must be present for a given run to pass the filter.
         snapshot_id (Optional[str]): The ID of the job snapshot to query for. Intended for internal use.
         updated_after (Optional[DateTime]): Filter by runs that were last updated before this datetime.
         created_before (Optional[DateTime]): Filter by runs that were created before this datetime.
-        mode (Optional[str]): (deprecated)
         pipeline_name (Optional[str]): (deprecated)
 
     """
 
     def __new__(
         cls,
         run_ids: Optional[Sequence[str]] = None,
         job_name: Optional[str] = None,
         statuses: Optional[Sequence[DagsterRunStatus]] = None,
         tags: Optional[Mapping[str, Union[str, Sequence[str]]]] = None,
         snapshot_id: Optional[str] = None,
         updated_after: Optional[datetime] = None,
         updated_before: Optional[datetime] = None,
-        mode: Optional[str] = None,
         created_after: Optional[datetime] = None,
         created_before: Optional[datetime] = None,
         pipeline_name: Optional[str] = None,  # for backcompat purposes
     ):
         job_name = job_name or pipeline_name
 
         check.invariant(run_ids != [], "When filtering on run ids, a non-empty list must be used.")
@@ -507,15 +499,14 @@
             run_ids=check.opt_sequence_param(run_ids, "run_ids", of_type=str),
             job_name=check.opt_str_param(job_name, "job_name"),
             statuses=check.opt_sequence_param(statuses, "statuses", of_type=DagsterRunStatus),
             tags=check.opt_mapping_param(tags, "tags", key_type=str),
             snapshot_id=check.opt_str_param(snapshot_id, "snapshot_id"),
             updated_after=check.opt_inst_param(updated_after, "updated_after", datetime),
             updated_before=check.opt_inst_param(updated_before, "updated_before", datetime),
-            mode=check.opt_str_param(mode, "mode"),
             created_after=check.opt_inst_param(created_after, "created_after", datetime),
             created_before=check.opt_inst_param(created_before, "created_before", datetime),
         )
 
     @property
     def pipeline_name(self) -> Optional[str]:
         return self.job_name
```

### Comparing `dagster-1.3.1/dagster/_core/storage/root.py` & `dagster-1.3.2/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.2/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/runs/base.py` & `dagster-1.3.2/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.2/dagster/_core/storage/runs/in_memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import uuid
 from contextlib import contextmanager
 from typing import Iterator, Optional, Sequence
 
 import sqlalchemy as db
 from sqlalchemy.engine import Connection
 from sqlalchemy.pool import NullPool
 
@@ -16,55 +17,48 @@
 class InMemoryRunStorage(SqlRunStorage):
     """In memory only run storage. Used by ephemeral DagsterInstance or for testing purposes.
 
     WARNING: Dagit and other core functionality will not work if this is used on a real DagsterInstance
     """
 
     def __init__(self, preload: Optional[Sequence[DebugRunPayload]] = None):
-        self._engine = None
-        self._conn = None
+        self._engine = create_engine(
+            create_in_memory_conn_string(f"runs-{uuid.uuid4()}"),
+            poolclass=NullPool,
+        )
+
+        # hold one connection for life of instance, but vend new ones for specific calls
+        self._held_conn = self._engine.connect()
+
+        RunStorageSqlMetadata.create_all(self._held_conn)
+        alembic_config = get_alembic_config(__file__, "sqlite/alembic/alembic.ini")
+        stamp_alembic_rev(alembic_config, self._held_conn)
+        table_names = db.inspect(self._held_conn).get_table_names()
+        if "instance_info" not in table_names:
+            InstanceInfo.create(self._held_conn)
+        self.migrate()
+        self.optimize()
+
         if preload:
             for payload in preload:
                 self.add_pipeline_snapshot(
                     payload.pipeline_snapshot, payload.pipeline_run.pipeline_snapshot_id
                 )
                 self.add_execution_plan_snapshot(
                     payload.execution_plan_snapshot, payload.pipeline_run.execution_plan_snapshot_id
                 )
                 self.add_run(payload.pipeline_run)
 
-    def _create_connection(self) -> None:
-        engine = create_engine(create_in_memory_conn_string("runs"), poolclass=NullPool)
-        conn = engine.connect()
-
-        conn.execute("PRAGMA journal_mode=WAL;")
-        conn.execute("PRAGMA foreign_keys=ON;")
-        RunStorageSqlMetadata.create_all(conn)
-        alembic_config = get_alembic_config(__file__, "sqlite/alembic/alembic.ini")
-        stamp_alembic_rev(alembic_config, conn)
-        table_names = db.inspect(conn).get_table_names()
-        if "instance_info" not in table_names:
-            InstanceInfo.create(conn)
-
-        self._engine = engine
-        self._conn = conn
-
-        self.migrate()
-        self.optimize()
-
     @contextmanager
     def connect(self) -> Iterator[Connection]:
-        if not self._conn:
-            self._create_connection()
+        with self._engine.connect() as conn:
+            conn.execute("PRAGMA journal_mode=WAL;")
+            conn.execute("PRAGMA foreign_keys=ON;")
 
-        yield self._conn  # type: ignore
+            yield conn
 
     def upgrade(self) -> None:
         pass
 
     def dispose(self) -> None:
-        if self._conn:
-            self._conn.close()
-            self._conn = None
-
-        if self._engine:
-            self._engine.dispose()
+        self._held_conn.close()
+        self._engine.dispose()
```

### Comparing `dagster-1.3.1/dagster/_core/storage/runs/migration.py` & `dagster-1.3.2/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/runs/schema.py` & `dagster-1.3.2/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.2/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,17 +250,14 @@
 
         if filters.run_ids:
             query = query.where(RunsTable.c.run_id.in_(filters.run_ids))
 
         if filters.job_name:
             query = query.where(RunsTable.c.pipeline_name == filters.job_name)
 
-        if filters.mode:
-            query = query.where(RunsTable.c.mode == filters.mode)
-
         if filters.statuses:
             query = query.where(
                 RunsTable.c.status.in_([status.value for status in filters.statuses])
             )
 
         if filters.snapshot_id:
             query = query.where(RunsTable.c.snapshot_id == filters.snapshot_id)
```

### Comparing `dagster-1.3.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.2/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.2/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         alembic_config = get_alembic_config(__file__)
 
         should_mark_indexes = False
         with engine.connect() as connection:
             db_revision, head_revision = check_alembic_revision(alembic_config, connection)
             if not (db_revision and head_revision):
                 RunStorageSqlMetadata.create_all(engine)
-                engine.execute("PRAGMA journal_mode=WAL;")
+                connection.execute("PRAGMA journal_mode=WAL;")
                 stamp_alembic_rev(alembic_config, connection)
                 should_mark_indexes = True
 
             table_names = db.inspect(engine).get_table_names()
             if "instance_info" not in table_names:
                 InstanceInfo.create(engine)
```

### Comparing `dagster-1.3.1/dagster/_core/storage/schedules/base.py` & `dagster-1.3.2/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.2/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.2/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.2/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.2/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.2/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         alembic_config = get_alembic_config(__file__)
 
         should_migrate_data = False
         with engine.connect() as connection:
             db_revision, head_revision = check_alembic_revision(alembic_config, connection)
             if not (db_revision and head_revision):
                 ScheduleStorageSqlMetadata.create_all(engine)
-                engine.execute("PRAGMA journal_mode=WAL;")
+                connection.execute("PRAGMA journal_mode=WAL;")
                 stamp_alembic_rev(alembic_config, connection)
                 should_migrate_data = True
 
         schedule_storage = cls(conn_string, inst_data)
         if should_migrate_data:
             schedule_storage.migrate()
             schedule_storage.optimize()
```

### Comparing `dagster-1.3.1/dagster/_core/storage/sql.py` & `dagster-1.3.2/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/sqlite.py` & `dagster-1.3.2/dagster/_core/storage/sqlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
 
 def create_in_memory_conn_string(db_name: str) -> str:
     # Uses a named file-based URL for the in-memory connection (as opposed to the :memory: url) so
     # that multiple instances can share the same logical DB across connections, while maintaining
     # separate DBs for different db names.  The latter is required to have both the run / event_log
     # in-memory implementations within the same process
-    return f"sqlite:///file:{db_name}?mode=memory&uri=true&check_same_thread=false"
+    return f"sqlite:///file:{db_name}?mode=memory&uri=true&cache=shared"
 
 
 def get_sqlite_version() -> str:
     return str(sqlite3.sqlite_version)
```

### Comparing `dagster-1.3.1/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.2/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/tags.py` & `dagster-1.3.2/dagster/_core/storage/tags.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,14 +64,18 @@
 USER_EDITABLE_SYSTEM_TAGS = [
     PRIORITY_TAG,
     MAX_RETRIES_TAG,
     RETRY_STRATEGY_TAG,
     MAX_RUNTIME_SECONDS_TAG,
 ]
 
+# In cloud, we tag runs with the email of the user who triggered the run
+# This is used to display the user in the UI
+USER_TAG = "user"
+
 
 class TagType(Enum):
     # Custom tag provided by a user
     USER_PROVIDED = "USER_PROVIDED"
 
     # Tags used by Dagster to manage execution that should be surfaced to users.
     SYSTEM = "SYSTEM"
```

### Comparing `dagster-1.3.1/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.2/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.2/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.2/dagster/_core/system_config/composite_descent.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing_extensions import TypeAlias
 
 import dagster._check as check
 from dagster._config import EvaluateValueResult, process_config
 from dagster._core.definitions.asset_layer import AssetLayer
 from dagster._core.definitions.dependency import GraphNode, Node, NodeHandle, OpNode
 from dagster._core.definitions.graph_definition import GraphDefinition, SubselectedGraphDefinition
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.run_config import define_node_shape
 from dagster._core.errors import (
     DagsterConfigMappingFunctionError,
     DagsterInvalidConfigError,
     user_code_error_boundary,
 )
@@ -34,20 +34,20 @@
 
 # This is a dummy handle used to simplify the code, corresponding to the root container (graph). It
 # doesn't actually represent a node during execution.
 _ROOT_HANDLE = NodeHandle("root", None)
 
 
 class DescentStack(
-    NamedTuple("_DescentStack", [("pipeline_def", PipelineDefinition), ("handle", NodeHandle)])
+    NamedTuple("_DescentStack", [("pipeline_def", JobDefinition), ("handle", NodeHandle)])
 ):
-    def __new__(cls, pipeline_def: PipelineDefinition, handle: NodeHandle):
+    def __new__(cls, pipeline_def: JobDefinition, handle: NodeHandle):
         return super(DescentStack, cls).__new__(
             cls,
-            pipeline_def=check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition),
+            pipeline_def=check.inst_param(pipeline_def, "pipeline_def", JobDefinition),
             handle=check.inst_param(handle, "handle", NodeHandle),
         )
 
     @property
     def current_container(self) -> GraphDefinition:
         if self.handle == _ROOT_HANDLE:
             return self.pipeline_def.graph
@@ -66,15 +66,15 @@
 
     def descend(self, node: Node) -> "DescentStack":
         parent = self.handle if self.handle != _ROOT_HANDLE else None
         return self._replace(handle=NodeHandle(node.name, parent=parent))
 
 
 def composite_descent(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     ops_config: Mapping[str, RawNodeConfig],
     resource_defs: Mapping[str, ResourceDefinition],
 ) -> Mapping[str, OpConfig]:
     """This function is responsible for constructing the dictionary of OpConfig (indexed by handle)
     that will be passed into the ResolvedRunConfig. Critically this is the codepath that manages
     config mapping, where the runtime calls into user-defined config mapping functions to produce
     config for child solids of composites.
@@ -85,44 +85,41 @@
             of the run_config. Assumed to have already been validated.
 
     Returns:
         Dict[str, OpConfig]: A dictionary mapping string representations of NodeHandles to
             OpConfig objects. It includes an entry for ops at every level of the
             composite tree - i.e. not just leaf ops, but composite ops as well
     """
-    check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+    check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
     check.dict_param(ops_config, "solids_config")
     check.dict_param(resource_defs, "resource_defs", key_type=str, value_type=ResourceDefinition)
 
     # If top-level graph has config mapping, apply that config mapping before descending.
     if pipeline_def.graph.has_config_mapping:
         ops_config = _apply_top_level_config_mapping(
             pipeline_def,
             ops_config,
             resource_defs,
-            pipeline_def.is_job,
         )
 
     return {
         handle.to_string(): op_config
         for handle, op_config in _composite_descent(
             parent_stack=DescentStack(pipeline_def, _ROOT_HANDLE),
             ops_config_dict=ops_config,
             resource_defs=resource_defs,
-            is_using_graph_job_op_apis=pipeline_def.is_job,
             asset_layer=pipeline_def.asset_layer,
         )
     }
 
 
 def _composite_descent(
     parent_stack: DescentStack,
     ops_config_dict: Mapping[str, RawNodeConfig],
     resource_defs: Mapping[str, ResourceDefinition],
-    is_using_graph_job_op_apis: bool,
     asset_layer: AssetLayer,
 ) -> Iterator[OpConfigEntry]:
     """The core implementation of composite_descent. This yields a stream of OpConfigEntry. This is
     used by composite_descent to construct a dictionary.
 
     It descends over the entire node hierarchy, constructing an entry for every handle. If it
     encounters a graph instance with a config mapping, it will invoke that config mapping fn,
@@ -160,47 +157,43 @@
                 OpConfig.from_dict(
                     {
                         "inputs": current_op_config.get("inputs"),
                         "outputs": current_op_config.get("outputs"),
                     }
                 ),
             )
-            node_key = "ops" if is_using_graph_job_op_apis else "solids"
 
             # If there is a config mapping, invoke it and get the descendent solids
             # config that way. Else just grabs the solids entry of the current config
             mapped_nodes_config = (
                 _apply_config_mapping(
                     node,
                     current_stack,
                     current_op_config,
                     resource_defs,
-                    is_using_graph_job_op_apis,
                     asset_layer,
                 )
                 if node.definition.has_config_mapping
-                else cast(Mapping[str, RawNodeConfig], current_op_config.get(node_key, {}))
+                else cast(Mapping[str, RawNodeConfig], current_op_config.get("ops", {}))
             )
 
             yield from _composite_descent(
                 current_stack,
                 mapped_nodes_config,
                 resource_defs,
-                is_using_graph_job_op_apis,
                 asset_layer,
             )
         else:
             check.failed(f"Unexpected node type {type(node)}")
 
 
 def _apply_top_level_config_mapping(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     outer_config: Mapping[str, Mapping[str, object]],
     resource_defs: Mapping[str, ResourceDefinition],
-    is_using_graph_job_op_apis: bool,
 ) -> Mapping[str, RawNodeConfig]:
     graph_def = pipeline_def.graph
     config_mapping = graph_def.config_mapping
     if config_mapping is None:
         return outer_config
 
     else:
@@ -223,15 +216,14 @@
         # be evaluated against
 
         type_to_evaluate_against = define_node_shape(
             nodes=graph_def.nodes,
             ignored_nodes=None,
             dependency_structure=graph_def.dependency_structure,
             resource_defs=resource_defs,
-            is_using_graph_job_op_apis=is_using_graph_job_op_apis,
             asset_layer=pipeline_def.asset_layer,
             node_input_source_assets=graph_def.node_input_source_assets,
         )
 
         # process against that new type
 
         evr = process_config(type_to_evaluate_against, mapped_graph_config)
@@ -243,15 +235,14 @@
 
 
 def _apply_config_mapping(
     graph_node: GraphNode,
     current_stack: DescentStack,
     current_node_config: RawNodeConfig,
     resource_defs: Mapping[str, ResourceDefinition],
-    is_using_graph_job_op_apis: bool,
     asset_layer: AssetLayer,
 ) -> Mapping[str, RawNodeConfig]:
     # the spec of the config mapping function is that it takes the dictionary at:
     # solid_name:
     #    config: {dict_passed_to_user}
 
     # and it returns the dictionary rooted at solids
@@ -293,15 +284,14 @@
 
     type_to_evaluate_against = define_node_shape(
         nodes=graph_def.nodes,
         ignored_nodes=ignored_solids,
         dependency_structure=graph_def.dependency_structure,
         parent_handle=current_stack.handle,
         resource_defs=resource_defs,
-        is_using_graph_job_op_apis=is_using_graph_job_op_apis,
         asset_layer=asset_layer,
         node_input_source_assets=graph_def.node_input_source_assets,
     )
 
     # process against that new type
 
     evr = process_config(type_to_evaluate_against, mapped_solids_config)
@@ -320,22 +310,22 @@
     ).format(
         described_node=current_stack.current_node.describe_node(),
         described_target=current_stack.pipeline_def.describe_target(),
         stack_str=":".join(current_stack.handle.path),
     )
 
 
-def _get_top_level_error_lambda(pipeline_def: PipelineDefinition) -> Callable[[], str]:
+def _get_top_level_error_lambda(pipeline_def: JobDefinition) -> Callable[[], str]:
     return (
         lambda: f"The config mapping function on top-level graph {pipeline_def.graph.name} in job {pipeline_def.name} has thrown an unexpected error during its execution."
     )
 
 
 def raise_top_level_config_error(
-    pipeline_def: PipelineDefinition, failed_config_value: object, evr: EvaluateValueResult
+    pipeline_def: JobDefinition, failed_config_value: object, evr: EvaluateValueResult
 ) -> NoReturn:
     message = (
         f"In job '{pipeline_def.name}', top level graph '{pipeline_def.graph.name}' has a "
         "configuration error."
     )
 
     raise DagsterInvalidConfigError(message, evr.errors, failed_config_value)
```

### Comparing `dagster-1.3.1/dagster/_core/system_config/objects.py` & `dagster-1.3.2/dagster/_core/system_config/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import dagster._check as check
 from dagster._core.definitions.configurable import ConfigurableDefinition
 from dagster._core.definitions.executor_definition import (
     ExecutorDefinition,
     execute_in_process_executor,
 )
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
+from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.errors import DagsterInvalidConfigError
 from dagster._utils import ensure_single_item
 
 
 class OpConfig(
     NamedTuple(
@@ -92,129 +92,106 @@
         "_ResolvedRunConfig",
         [
             ("ops", Mapping[str, OpConfig]),
             ("execution", "ExecutionConfig"),
             ("resources", Mapping[str, ResourceConfig]),
             ("loggers", Mapping[str, Mapping[str, object]]),
             ("original_config_dict", Any),
-            ("mode", Optional[str]),
             ("inputs", Mapping[str, Any]),
         ],
     )
 ):
     def __new__(
         cls,
         ops: Optional[Mapping[str, OpConfig]] = None,
         execution: Optional["ExecutionConfig"] = None,
         resources: Optional[Mapping[str, ResourceConfig]] = None,
         loggers: Optional[Mapping[str, Mapping[str, object]]] = None,
         original_config_dict: Optional[Mapping[str, object]] = None,
-        mode: Optional[str] = None,
         inputs: Optional[Mapping[str, object]] = None,
     ):
         check.opt_inst_param(execution, "execution", ExecutionConfig)
         check.opt_mapping_param(original_config_dict, "original_config_dict")
         resources = check.opt_mapping_param(resources, "resources", key_type=str)
-        check.opt_str_param(mode, "mode")
         inputs = check.opt_mapping_param(inputs, "inputs", key_type=str)
 
         if execution is None:
             execution = ExecutionConfig(None, None)
 
         return super(ResolvedRunConfig, cls).__new__(
             cls,
             ops=check.opt_mapping_param(ops, "ops", key_type=str, value_type=OpConfig),
             execution=execution,
             resources=resources,
             loggers=check.opt_mapping_param(loggers, "loggers", key_type=str, value_type=Mapping),
             original_config_dict=original_config_dict,
-            mode=mode,
             inputs=inputs,
         )
 
     @staticmethod
     def build(
-        pipeline_def: PipelineDefinition,
+        pipeline_def: JobDefinition,
         run_config: Optional[Mapping[str, object]] = None,
-        mode: Optional[str] = None,
     ) -> "ResolvedRunConfig":
         """This method validates a given run config against the pipeline config schema. If
         successful, we instantiate an ResolvedRunConfig object.
 
         In case the run_config is invalid, this method raises a DagsterInvalidConfigError
         """
         from dagster._config import process_config
 
         from .composite_descent import composite_descent
 
-        check.inst_param(pipeline_def, "pipeline_def", PipelineDefinition)
+        check.inst_param(pipeline_def, "pipeline_def", JobDefinition)
         run_config = check.opt_mapping_param(run_config, "run_config")
-        check.opt_str_param(mode, "mode")
 
-        mode = mode or pipeline_def.get_default_mode_name()
-        run_config_schema = pipeline_def.get_run_config_schema(mode)
+        run_config_schema = pipeline_def.run_config_schema
         if run_config_schema.config_mapping:
             # add user code boundary
             run_config = run_config_schema.config_mapping.resolve_from_unvalidated_config(
                 run_config
             )
 
         config_evr = process_config(
             run_config_schema.run_config_schema_type, check.not_none(run_config)
         )
         if not config_evr.success:
             raise DagsterInvalidConfigError(
-                f"Error in config for {pipeline_def.target_type}".format(pipeline_def.name),
+                f"Error in config for job {pipeline_def.name}",
                 config_evr.errors,
                 run_config,
             )
 
         config_value = cast(Dict[str, Any], config_evr.value)
 
-        mode_def = pipeline_def.get_mode_definition(mode)
-
         # If using the `execute_in_process` executor, we ignore the execution config value, since it
         # may be pointing to the executor for the job rather than the `execute_in_process` executor.
-        if (
-            len(mode_def.executor_defs) == 1
-            and mode_def.executor_defs[0] == execute_in_process_executor
-        ):
+        if pipeline_def.executor_def == execute_in_process_executor:
             config_mapped_execution_configs: Optional[Mapping[str, Any]] = {}
         else:
-            if pipeline_def.is_job:
-                executor_config = config_value.get("execution", {})
-                config_mapped_execution_configs = config_map_executor(
-                    executor_config, mode_def.executor_defs[0]
-                )
-            else:
-                config_mapped_execution_configs = config_map_objects(
-                    config_value,
-                    mode_def.executor_defs,
-                    "execution",
-                    ExecutorDefinition,
-                    "executor",
-                )
+            executor_config = config_value.get("execution", {})
+            config_mapped_execution_configs = config_map_executor(
+                executor_config, pipeline_def.executor_def
+            )
 
-        resource_defs = pipeline_def.get_required_resource_defs_for_mode(mode)
+        resource_defs = pipeline_def.get_required_resource_defs()
         resource_configs = config_value.get("resources", {})
         config_mapped_resource_configs = config_map_resources(resource_defs, resource_configs)
-        config_mapped_logger_configs = config_map_loggers(pipeline_def, config_value, mode)
+        config_mapped_logger_configs = config_map_loggers(pipeline_def, config_value)
 
-        node_key = "ops" if pipeline_def.is_job else "solids"
-        solid_config_dict = composite_descent(
-            pipeline_def, config_value.get(node_key, {}), mode_def.resource_defs
+        op_config_dict = composite_descent(
+            pipeline_def, config_value.get("ops", {}), pipeline_def.resource_defs
         )
         input_configs = config_value.get("inputs", {})
         return ResolvedRunConfig(
-            ops=solid_config_dict,
+            ops=op_config_dict,
             execution=ExecutionConfig.from_dict(config_mapped_execution_configs),
             loggers=config_mapped_logger_configs,
             original_config_dict=run_config,
             resources=config_mapped_resource_configs,
-            mode=mode,
             inputs=input_configs,
         )
 
     def to_dict(self) -> Mapping[str, Mapping[str, object]]:
         env_dict: Dict[str, Mapping[str, object]] = {}
 
         op_configs: Dict[str, object] = {}
@@ -281,17 +258,16 @@
                 resource_config_evr.value
             )
 
     return config_mapped_resource_configs
 
 
 def config_map_loggers(
-    pipeline_def: PipelineDefinition,
+    pipeline_def: JobDefinition,
     config_value: Mapping[str, Any],
-    mode: str,
 ) -> Mapping[str, Any]:
     """This function executes the config mappings for loggers with respect to ConfigurableDefinition.
     It uses the `loggers` key on the run_config to determine which loggers will be initialized (and
     thus which ones need config mapping) and then iterates over each, looking up the corresponding
     LoggerDefinition in `mode_def.loggers`.
 
     The following are the cases of run_config and loggers on mode_def that could emerge
@@ -304,21 +280,20 @@
 
     The behavior of `run_config.loggers` as a source of truth for logger selection comes from:
     python_modules/dagster/dagster/_core/execution/context_creation_pipeline.py#create_log_manager
     See that codepath for more info on how the behavior in the above table is implemented. The logic
     in that function is tightly coupled to this one and changes in either path should be confirmed
     in the other.
     """
-    mode_def = pipeline_def.get_mode_definition(mode)
     logger_configs = config_value.get("loggers", {})
 
     config_mapped_logger_configs = {}
 
     for logger_key, logger_config in logger_configs.items():
-        logger_def = mode_def.loggers.get(logger_key)
+        logger_def = pipeline_def.loggers.get(logger_key)
         if logger_def is None:
             check.failed(f"No logger found for key {logger_key}")
 
         logger_config_evr = logger_def.apply_config_mapping(logger_config)
         if not logger_config_evr.success:
             raise DagsterInvalidConfigError(
                 f"Error in config for logger {logger_key}",
```

### Comparing `dagster-1.3.1/dagster/_core/telemetry.py` & `dagster-1.3.2/dagster/_core/telemetry.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 )
 
 import click
 import yaml
 from typing_extensions import ParamSpec
 
 import dagster._check as check
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicyType
 from dagster._core.definitions.pipeline_base import IPipeline
 from dagster._core.definitions.reconstruct import (
     ReconstructablePipeline,
     ReconstructableRepository,
     get_ephemeral_repository_name,
 )
 from dagster._core.errors import DagsterInvariantViolationError
@@ -465,14 +466,16 @@
     external_asset_nodes = external_repo.get_external_asset_nodes()
     num_assets_in_repo = len(external_asset_nodes)
 
     num_partitioned_assets_in_repo = 0
     num_multi_partitioned_assets_in_repo = 0
     num_dynamic_partitioned_assets_in_repo = 0
     num_assets_with_freshness_policies_in_repo = 0
+    num_assets_with_eager_auto_materialize_policies_in_repo = 0
+    num_assets_with_lazy_auto_materialize_policies_in_repo = 0
     num_source_assets_in_repo = 0
     num_observable_source_assets_in_repo = 0
     num_dbt_assets_in_repo = 0
     num_assets_with_code_versions_in_repo = 0
     for asset in external_asset_nodes:
         if asset.partitions_def_data:
             num_partitioned_assets_in_repo += 1
@@ -482,14 +485,20 @@
 
             if isinstance(asset.partitions_def_data, ExternalMultiPartitionsDefinitionData):
                 num_multi_partitioned_assets_in_repo += 1
 
         if asset.freshness_policy is not None:
             num_assets_with_freshness_policies_in_repo += 1
 
+        if asset.auto_materialize_policy is not None:
+            if asset.auto_materialize_policy.policy_type == AutoMaterializePolicyType.EAGER:
+                num_assets_with_eager_auto_materialize_policies_in_repo += 1
+            else:
+                num_assets_with_lazy_auto_materialize_policies_in_repo += 1
+
         if asset.is_source:
             num_source_assets_in_repo += 1
 
             if asset.is_observable:
                 num_observable_source_assets_in_repo += 1
 
         if asset.code_version is not None:
@@ -512,14 +521,20 @@
         "num_source_assets_in_repo": str(num_source_assets_in_repo),
         "num_partitioned_assets_in_repo": str(num_partitioned_assets_in_repo),
         "num_dynamic_partitioned_assets_in_repo": str(num_dynamic_partitioned_assets_in_repo),
         "num_multi_partitioned_assets_in_repo": str(num_multi_partitioned_assets_in_repo),
         "num_assets_with_freshness_policies_in_repo": str(
             num_assets_with_freshness_policies_in_repo
         ),
+        "num_assets_with_eager_auto_materialize_policies_in_repo": str(
+            num_assets_with_eager_auto_materialize_policies_in_repo
+        ),
+        "num_assets_with_lazy_auto_materialize_policies_in_repo": str(
+            num_assets_with_lazy_auto_materialize_policies_in_repo
+        ),
         "num_observable_source_assets_in_repo": str(num_observable_source_assets_in_repo),
         "num_dbt_assets_in_repo": str(num_dbt_assets_in_repo),
         "num_assets_with_code_versions_in_repo": str(num_assets_with_code_versions_in_repo),
         "num_asset_reconciliation_sensors_in_repo": str(num_asset_reconciliation_sensors_in_repo),
     }
```

### Comparing `dagster-1.3.1/dagster/_core/telemetry_upload.py` & `dagster-1.3.2/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/test_utils.py` & `dagster-1.3.2/dagster/_core/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 from dagster._core.launcher import RunLauncher
 from dagster._core.run_coordinator import RunCoordinator, SubmitRunContext
 from dagster._core.secrets import SecretsLoader
 from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus, RunsFilter
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
 from dagster._core.workspace.context import WorkspaceProcessContext, WorkspaceRequestContext
 from dagster._core.workspace.load_target import WorkspaceLoadTarget
-from dagster._legacy import ModeDefinition
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
 from dagster._seven.compat.pendulum import create_pendulum_time, mock_pendulum_timezone
 from dagster._utils import Counter, get_terminate_signal, traced, traced_counter
 from dagster._utils.log import configure_loggers
 
 # test utils from separate light weight file since are exported top level
@@ -131,15 +130,14 @@
 
 
 def create_run_for_test(
     instance: DagsterInstance,
     pipeline_name: str = TEST_PIPELINE_NAME,
     run_id=None,
     run_config=None,
-    mode=None,
     solids_to_execute=None,
     step_keys_to_execute=None,
     status=None,
     tags=None,
     root_run_id=None,
     parent_run_id=None,
     pipeline_snapshot=None,
@@ -150,15 +148,14 @@
     asset_selection=None,
     solid_selection=None,
 ):
     return instance.create_run(
         pipeline_name=pipeline_name,
         run_id=run_id,
         run_config=run_config,
-        mode=mode,
         solids_to_execute=solids_to_execute,
         step_keys_to_execute=step_keys_to_execute,
         status=status,
         tags=tags,
         root_run_id=root_run_id,
         parent_run_id=parent_run_id,
         pipeline_snapshot=pipeline_snapshot,
@@ -172,29 +169,27 @@
 
 
 def register_managed_run_for_test(
     instance,
     pipeline_name=TEST_PIPELINE_NAME,
     run_id=None,
     run_config=None,
-    mode=None,
     solids_to_execute=None,
     step_keys_to_execute=None,
     tags=None,
     root_run_id=None,
     parent_run_id=None,
     pipeline_snapshot=None,
     execution_plan_snapshot=None,
     parent_pipeline_snapshot=None,
 ):
     return instance.register_managed_run(
         pipeline_name,
         run_id,
         run_config,
-        mode,
         solids_to_execute,
         step_keys_to_execute,
         tags,
         root_run_id,
         parent_run_id,
         pipeline_snapshot,
         execution_plan_snapshot,
@@ -534,15 +529,14 @@
             for k, v in obj.items()
             if k is not None and v is not None
         )
     else:
         return obj
 
 
-default_mode_def_for_test = ModeDefinition(resource_defs={"io_manager": fs_io_manager})
 default_resources_for_test = {"io_manager": fs_io_manager}
 
 
 def strip_ansi(input_str: str) -> str:
     ansi_escape = re.compile(r"(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]")
     return ansi_escape.sub("", input_str)
```

### Comparing `dagster-1.3.1/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.2/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/config_schema.py` & `dagster-1.3.2/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/dagster_type.py` & `dagster-1.3.2/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/decorator.py` & `dagster-1.3.2/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.2/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.2/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/python_dict.py` & `dagster-1.3.2/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/python_set.py` & `dagster-1.3.2/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/python_tuple.py` & `dagster-1.3.2/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/types/transform_typing.py` & `dagster-1.3.2/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/utility_solids.py` & `dagster-1.3.2/dagster/_core/utility_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/utils.py` & `dagster-1.3.2/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.2/dagster/_core/workspace/autodiscovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 from types import ModuleType
 from typing import Callable, NamedTuple, Optional, Sequence, Tuple, Type, Union
 
 from dagster import (
     DagsterInvariantViolationError,
     GraphDefinition,
-    JobDefinition,
     RepositoryDefinition,
 )
 from dagster._core.code_pointer import load_python_file, load_python_module
 from dagster._core.definitions import AssetGroup
 from dagster._core.definitions.definitions_class import Definitions
 from dagster._core.definitions.repository_definition import PendingRepositoryDefinition
 
@@ -49,15 +48,15 @@
     module = load_python_module(
         package_name, working_directory, remove_from_path_fn=remove_from_path_fn
     )
     return loadable_targets_from_loaded_module(module)
 
 
 def loadable_targets_from_loaded_module(module: ModuleType) -> Sequence[LoadableTarget]:
-    from dagster._legacy import PipelineDefinition
+    from dagster._core.definitions import JobDefinition
 
     loadable_defs = _loadable_targets_of_type(module, Definitions)
 
     if loadable_defs:
         if len(loadable_defs) > 1:
             raise DagsterInvariantViolationError(
                 "Cannot have more than one Definitions object defined at module scope"
@@ -67,15 +66,15 @@
 
     loadable_repos = _loadable_targets_of_type(
         module, (RepositoryDefinition, PendingRepositoryDefinition)
     )
     if loadable_repos:
         return loadable_repos
 
-    loadable_pipelines = _loadable_targets_of_type(module, PipelineDefinition)
+    loadable_pipelines = _loadable_targets_of_type(module, JobDefinition)
     loadable_jobs = _loadable_targets_of_type(module, JobDefinition)
 
     if len(loadable_pipelines) == 1:
         return loadable_pipelines
 
     elif len(loadable_pipelines) > 1:
         target_type = "job" if len(loadable_jobs) > 1 else "pipeline"
```

### Comparing `dagster-1.3.1/dagster/_core/workspace/config_schema.py` & `dagster-1.3.2/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/workspace/context.py` & `dagster-1.3.2/dagster/_core/workspace/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,24 +222,22 @@
             .get_full_external_job(selector.pipeline_name)
         )
 
     def get_external_execution_plan(
         self,
         external_pipeline: ExternalPipeline,
         run_config: Mapping[str, object],
-        mode: str,
         step_keys_to_execute: Optional[Sequence[str]],
         known_state: Optional[KnownExecutionState],
     ) -> ExternalExecutionPlan:
         return self.get_code_location(
             external_pipeline.handle.location_name
         ).get_external_execution_plan(
             external_pipeline=external_pipeline,
             run_config=run_config,
-            mode=mode,
             step_keys_to_execute=step_keys_to_execute,
             known_state=known_state,
             instance=self.instance,
         )
 
     def get_external_partition_config(
         self,
```

### Comparing `dagster-1.3.1/dagster/_core/workspace/load.py` & `dagster-1.3.2/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/workspace/load_target.py` & `dagster-1.3.2/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/workspace/permissions.py` & `dagster-1.3.2/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_core/workspace/workspace.py` & `dagster-1.3.2/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/__init__.py` & `dagster-1.3.2/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/asset_daemon.py` & `dagster-1.3.2/dagster/_daemon/asset_daemon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import dagster._check as check
 from dagster._core.definitions.asset_reconciliation_sensor import (
     AssetReconciliationCursor,
     reconcile,
 )
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
-from dagster._core.definitions.mode import DEFAULT_MODE_NAME
 from dagster._core.definitions.selector import PipelineSelector
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.pipeline_run import DagsterRunStatus
 from dagster._core.storage.tags import CREATED_BY_TAG
 from dagster._core.workspace.context import IWorkspaceProcessContext
 from dagster._daemon.daemon import DaemonIterator, IntervalDaemon
 
@@ -111,26 +110,24 @@
                 CREATED_BY_TAG: "auto_materialize",
                 **instance.auto_materialize_run_tags,
             }
 
             external_execution_plan = code_location.get_external_execution_plan(
                 external_pipeline,
                 run_request.run_config,
-                DEFAULT_MODE_NAME,
                 step_keys_to_execute=None,
                 known_state=None,
                 instance=instance,
             )
             execution_plan_snapshot = external_execution_plan.execution_plan_snapshot
 
             run = instance.create_run(
                 pipeline_name=external_pipeline.name,
                 run_id=None,
                 run_config=None,
-                mode=DEFAULT_MODE_NAME,
                 solids_to_execute=None,
                 step_keys_to_execute=None,
                 status=DagsterRunStatus.NOT_STARTED,
                 solid_selection=None,
                 root_run_id=None,
                 parent_run_id=None,
                 tags=tags,
```

### Comparing `dagster-1.3.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.2/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.2/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/backfill.py` & `dagster-1.3.2/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/cli/__init__.py` & `dagster-1.3.2/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/controller.py` & `dagster-1.3.2/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/daemon.py` & `dagster-1.3.2/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.2/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.2/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_daemon/sensor.py` & `dagster-1.3.2/dagster/_daemon/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -857,15 +857,14 @@
     target_data: ExternalTargetData,
 ) -> DagsterRun:
     from dagster._daemon.daemon import get_telemetry_daemon_session_id
 
     external_execution_plan = code_location.get_external_execution_plan(
         external_pipeline,
         run_request.run_config,
-        target_data.mode,
         step_keys_to_execute=None,
         known_state=None,
         instance=instance,
     )
     execution_plan_snapshot = external_execution_plan.execution_plan_snapshot
 
     pipeline_tags = validate_tags(external_pipeline.tags or {}, allow_reserved_tags=False)
@@ -887,15 +886,14 @@
         },
     )
 
     return instance.create_run(
         pipeline_name=target_data.pipeline_name,
         run_id=None,
         run_config=run_request.run_config,
-        mode=target_data.mode,
         solids_to_execute=external_pipeline.solids_to_execute,
         step_keys_to_execute=None,
         status=DagsterRunStatus.NOT_STARTED,
         solid_selection=target_data.solid_selection,
         root_run_id=None,
         parent_run_id=None,
         tags=tags,
```

### Comparing `dagster-1.3.1/dagster/_daemon/types.py` & `dagster-1.3.2/dagster/_daemon/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from typing import Any, NamedTuple, Optional, Sequence
+from typing import NamedTuple, Optional, Sequence
 
 import dagster._check as check
 from dagster._serdes import whitelist_for_serdes
-from dagster._serdes.serdes import NamedTupleSerializer, is_packed_enum
+from dagster._serdes.serdes import NamedTupleSerializer, UnknownSerdesValue
 from dagster._utils.error import SerializableErrorInfo
 
 
 class DaemonHeartbeatSerializer(NamedTupleSerializer["DaemonHeartbeat"]):
-    def before_unpack(self, **packed_dict: Any):
+    def before_unpack(self, context, unpacked_dict):
         # Previously daemon types were enums, now they are strings. If we find a packed enum,
         # just extract the name, which is the string we want.
-        if is_packed_enum(packed_dict.get("daemon_type")):
-            packed_dict["daemon_type"] = packed_dict["daemon_type"]["__enum__"].split(".")[-1]
-        if packed_dict.get("error"):
-            packed_dict["errors"] = [packed_dict["error"]]
-            del packed_dict["error"]
-        return packed_dict
+        if isinstance(unpacked_dict.get("daemon_type"), UnknownSerdesValue):
+            unknown = unpacked_dict["daemon_type"]
+            unpacked_dict["daemon_type"] = unknown.value["__enum__"].split(".")[-1]
+            context.clear_ignored_unknown_values(unknown)
+        if unpacked_dict.get("error"):
+            unpacked_dict["errors"] = [unpacked_dict["error"]]
+            del unpacked_dict["error"]
+        return unpacked_dict
 
 
 @whitelist_for_serdes(serializer=DaemonHeartbeatSerializer)
 class DaemonHeartbeat(
     NamedTuple(
         "_DaemonHeartbeat",
         [
```

### Comparing `dagster-1.3.1/dagster/_daemon/workspace.py` & `dagster-1.3.2/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_generate/download.py` & `dagster-1.3.2/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_generate/generate.py` & `dagster-1.3.2/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.2/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.2/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/__init__.py` & `dagster-1.3.2/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/client.py` & `dagster-1.3.2/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/compile.py` & `dagster-1.3.2/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/impl.py` & `dagster-1.3.2/dagster/_grpc/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,15 +497,14 @@
             asset_selection=args.asset_selection,
         )
 
         return snapshot_from_execution_plan(
             create_execution_plan(
                 job_def,
                 run_config=args.run_config,
-                mode=args.mode,
                 step_keys_to_execute=args.step_keys_to_execute,
                 known_state=args.known_state,
                 instance_ref=args.instance_ref,
                 repository_load_data=repo_def.repository_load_data,
             ),
             args.pipeline_snapshot_id,
         )
```

### Comparing `dagster-1.3.1/dagster/_grpc/protos/api.proto` & `dagster-1.3.2/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/server.py` & `dagster-1.3.2/dagster/_grpc/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
     def ExternalJob(self, request, _context) -> api_pb2.ExternalJobReply:  # type: ignore
         try:
             repository_origin = deserialize_value(
                 request.serialized_repository_origin,
                 ExternalRepositoryOrigin,
             )
 
-            job_def = self._get_repo_for_origin(repository_origin).get_pipeline(request.job_name)
+            job_def = self._get_repo_for_origin(repository_origin).get_job(request.job_name)
             ser_job_data = serialize_value(external_pipeline_data_from_def(job_def))
             return api_pb2.ExternalJobReply(serialized_job_data=ser_job_data)  # type: ignore
         except Exception:
             return api_pb2.ExternalJobReply(  # type: ignore
                 serialized_error=serialize_value(
                     serializable_error_info_from_exc_info(sys.exc_info())
                 )
```

### Comparing `dagster-1.3.1/dagster/_grpc/server_watcher.py` & `dagster-1.3.2/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_grpc/types.py` & `dagster-1.3.2/dagster/_grpc/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import AbstractSet, Any, Mapping, NamedTuple, Optional, Sequence
 
 import dagster._check as check
 from dagster._core.code_pointer import CodePointer
 from dagster._core.definitions.events import AssetKey
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.execution.retries import RetryMode
+from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 from dagster._core.host_representation.origin import (
     CodeLocationOrigin,
     ExternalPipelineOrigin,
     ExternalRepositoryOrigin,
 )
 from dagster._core.instance.ref import InstanceRef
 from dagster._core.origin import PipelinePythonOrigin, get_python_environment_entry_point
@@ -22,34 +23,34 @@
 class ExecutionPlanSnapshotArgs(
     NamedTuple(
         "_ExecutionPlanSnapshotArgs",
         [
             ("pipeline_origin", ExternalPipelineOrigin),
             ("solid_selection", Sequence[str]),
             ("run_config", Mapping[str, object]),
-            ("mode", str),
             ("step_keys_to_execute", Optional[Sequence[str]]),
             ("pipeline_snapshot_id", str),
             ("known_state", Optional[KnownExecutionState]),
             ("instance_ref", Optional[InstanceRef]),
             ("asset_selection", Optional[AbstractSet[AssetKey]]),
+            ("mode", str),
         ],
     )
 ):
     def __new__(
         cls,
         pipeline_origin: ExternalPipelineOrigin,
         solid_selection: Sequence[str],
         run_config: Mapping[str, object],
-        mode: str,
         step_keys_to_execute: Optional[Sequence[str]],
         pipeline_snapshot_id: str,
         known_state: Optional[KnownExecutionState] = None,
         instance_ref: Optional[InstanceRef] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
+        mode: str = DEFAULT_MODE_NAME,
     ):
         return super(ExecutionPlanSnapshotArgs, cls).__new__(
             cls,
             pipeline_origin=check.inst_param(
                 pipeline_origin, "pipeline_origin", ExternalPipelineOrigin
             ),
             solid_selection=check.opt_sequence_param(
```

### Comparing `dagster-1.3.1/dagster/_grpc/utils.py` & `dagster-1.3.2/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_loggers/__init__.py` & `dagster-1.3.2/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_module_alias_map.py` & `dagster-1.3.2/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_scheduler/scheduler.py` & `dagster-1.3.2/dagster/_scheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -733,15 +733,14 @@
 
     run_config = run_request.run_config
     schedule_tags = run_request.tags
 
     external_execution_plan = code_location.get_external_execution_plan(
         external_pipeline,
         run_config,
-        check.not_none(external_schedule.mode),
         step_keys_to_execute=None,
         known_state=None,
     )
     execution_plan_snapshot = external_execution_plan.execution_plan_snapshot
 
     tags = merge_dicts(
         validate_tags(external_pipeline.tags, allow_reserved_tags=False) or {},
@@ -763,15 +762,14 @@
         },
     )
 
     return instance.create_run(
         pipeline_name=external_schedule.pipeline_name,
         run_id=None,
         run_config=run_config,
-        mode=external_schedule.mode,
         solids_to_execute=external_pipeline.solids_to_execute,
         step_keys_to_execute=None,
         solid_selection=external_pipeline.solid_selection,
         status=DagsterRunStatus.NOT_STARTED,
         root_run_id=None,
         parent_run_id=None,
         tags=tags,
```

### Comparing `dagster-1.3.1/dagster/_scheduler/stale.py` & `dagster-1.3.2/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_serdes/__init__.py` & `dagster-1.3.2/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_serdes/config_class.py` & `dagster-1.3.2/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_serdes/ipc.py` & `dagster-1.3.2/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_serdes/serdes.py` & `dagster-1.3.2/dagster/_serdes/serdes.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,42 +8,41 @@
   serialization boundary the types we expect to.
 
 Why not pickle?
 
 * This isn't meant to replace pickle in the conditions that pickle is reasonable to use
   (in memory, not human readable, etc) just handle the json case effectively.
 """
-
 import collections.abc
 import warnings
 from abc import ABC, abstractmethod
 from enum import Enum
+from functools import partial
 from inspect import Parameter, signature
 from typing import (
     AbstractSet,
     Any,
     Callable,
     Dict,
     FrozenSet,
     Generic,
     List,
     Mapping,
     NamedTuple,
-    NoReturn,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     Union,
     cast,
     overload,
 )
 
-from typing_extensions import Final, Literal, Self, TypeAlias, TypeGuard, TypeVar
+from typing_extensions import Final, Self, TypeAlias, TypeVar
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._utils import is_named_tuple_instance, is_named_tuple_subclass
 from dagster._utils.cached_method import cached_method
 
 from .errors import DeserializationError, SerdesUsageError, SerializationError
@@ -72,22 +71,38 @@
     None,
     NamedTuple,
     Set["PackableValue"],
     FrozenSet["PackableValue"],
     Enum,
 ]
 
+UnpackedValue: TypeAlias = Union[
+    Sequence["UnpackedValue"],
+    Mapping[str, "UnpackedValue"],
+    str,
+    int,
+    float,
+    bool,
+    None,
+    NamedTuple,
+    Set["PackableValue"],
+    FrozenSet["PackableValue"],
+    Enum,
+    "UnknownSerdesValue",
+]
+
 
 ###################################################################################################
 # Whitelisting
 ###################################################################################################
 
 
 class WhitelistMap(NamedTuple):
-    tuples: Dict[str, "NamedTupleSerializer"]
+    tuple_serializers: Dict[str, "NamedTupleSerializer"]
+    tuple_deserializers: Dict[str, "NamedTupleSerializer"]
     enums: Dict[str, "EnumSerializer"]
 
     def register_tuple(
         self,
         name: str,
         named_tuple_class: Type[NamedTuple],
         serializer_class: Optional[Type["NamedTupleSerializer"]] = None,
@@ -113,26 +128,32 @@
             storage_field_names=storage_field_names,
             old_fields=old_fields,
             skip_when_empty_fields=skip_when_empty_fields,
             field_serializers={k: klass.get_instance() for k, klass in field_serializers.items()}
             if field_serializers
             else None,
         )
-        self.tuples[name] = serializer
-        if storage_name:
-            self.tuples[storage_name] = serializer
+        self.tuple_serializers[name] = serializer
+        deserializer_name = storage_name or name
+        self.tuple_deserializers[deserializer_name] = serializer
         if old_storage_names:
             for old_storage_name in old_storage_names:
-                self.tuples[old_storage_name] = serializer
+                self.tuple_deserializers[old_storage_name] = serializer
+
+    def has_tuple_serializer(self, name: str) -> bool:
+        return name in self.tuple_serializers
 
-    def has_tuple_entry(self, name: str) -> bool:
-        return name in self.tuples
+    def has_tuple_deserializer(self, name: str) -> bool:
+        return name in self.tuple_deserializers
 
-    def get_tuple_entry(self, name: str) -> "NamedTupleSerializer":
-        return self.tuples[name]
+    def get_tuple_serializer(self, name: str) -> "NamedTupleSerializer":
+        return self.tuple_serializers[name]
+
+    def get_tuple_deserializer(self, name: str) -> "NamedTupleSerializer":
+        return self.tuple_deserializers[name]
 
     def register_enum(
         self,
         name: str,
         enum_class: Type[Enum],
         serializer_class: Optional[Type["EnumSerializer"]] = None,
         storage_name: Optional[str] = None,
@@ -154,15 +175,15 @@
         return name in self.enums
 
     def get_enum_entry(self, name: str) -> "EnumSerializer":
         return self.enums[name]
 
     @staticmethod
     def create() -> "WhitelistMap":
-        return WhitelistMap(tuples={}, enums={})
+        return WhitelistMap(tuple_serializers={}, tuple_deserializers={}, enums={})
 
 
 _WHITELIST_MAP: Final[WhitelistMap] = WhitelistMap.create()
 
 T = TypeVar("T")
 U = TypeVar("U")
 T_Type = TypeVar("T_Type", bound=Type[object])
@@ -310,14 +331,66 @@
             return klass  # type: ignore  # (NamedTuple quirk)
         else:
             raise SerdesUsageError(f"Can not whitelist class {klass} for serializer {serializer}")
 
     return __whitelist_for_serdes
 
 
+###################################################################################################
+# Serializers
+###################################################################################################
+
+
+class UnpackContext:
+    """values are unpacked bottom up."""
+
+    def __init__(self):
+        self.observed_unknown_serdes_values: Set[UnknownSerdesValue] = set()
+
+    def assert_no_unknown_values(self, obj: UnpackedValue) -> PackableValue:
+        if isinstance(obj, UnknownSerdesValue):
+            raise DeserializationError(
+                f"{obj.message}\nThis error can occur due to version skew, verify processes are"
+                " running expected versions."
+            )
+        elif isinstance(obj, (list, set, frozenset)):
+            for inner in obj:
+                self.assert_no_unknown_values(inner)
+        elif isinstance(obj, dict):
+            for v in obj.values():
+                self.assert_no_unknown_values(v)
+
+        return cast(PackableValue, obj)
+
+    def observe_unknown_value(self, val: "UnknownSerdesValue") -> "UnknownSerdesValue":
+        self.observed_unknown_serdes_values.add(val)
+        return val
+
+    def clear_ignored_unknown_values(self, obj: T) -> T:
+        if isinstance(obj, UnknownSerdesValue):
+            self.observed_unknown_serdes_values.discard(obj)
+        elif isinstance(obj, (list, set, frozenset)):
+            for inner in obj:
+                self.clear_ignored_unknown_values(inner)
+        elif isinstance(obj, dict):
+            for k, v in obj.items():
+                self.clear_ignored_unknown_values(v)
+
+        return obj
+
+    def finalize_unpack(self, unpacked: UnpackedValue) -> PackableValue:
+        if self.observed_unknown_serdes_values:
+            message = ",".join(v.message for v in self.observed_unknown_serdes_values)
+            raise DeserializationError(
+                f"{message}\nThis error can occur due to version skew, verify processes are"
+                " running expected versions."
+            )
+        return cast(PackableValue, unpacked)
+
+
 class Serializer(ABC):
     pass
 
 
 T_Enum = TypeVar("T_Enum", bound=Enum, default=Enum)
 
 
@@ -325,15 +398,20 @@
     def __init__(self, *, klass: Type[T_Enum], storage_name: Optional[str] = None):
         self.klass = klass
         self.storage_name = storage_name
 
     def unpack(self, value: str) -> T_Enum:
         return self.klass[value]
 
-    def pack(self, value: Enum, whitelist_map: WhitelistMap, descent_path: str) -> str:
+    def pack(
+        self,
+        value: Enum,
+        whitelist_map: WhitelistMap,
+        descent_path: str,
+    ) -> str:
         return f"{self.get_storage_name()}.{value.name}"
 
     def get_storage_name(self) -> str:
         return self.storage_name or self.klass.__name__
 
 
 T_NamedTuple = TypeVar("T_NamedTuple", bound=NamedTuple, default=NamedTuple)
@@ -352,72 +430,106 @@
         old_fields: Optional[Mapping[str, JsonSerializableValue]] = None,
         skip_when_empty_fields: Optional[AbstractSet[str]] = None,
         field_serializers: Optional[Mapping[str, "FieldSerializer"]] = None,
     ):
         self.klass = klass
         self.storage_name = storage_name
         self.storage_field_names = storage_field_names or {}
+        self.loaded_field_names = {v: k for k, v in self.storage_field_names.items()}
         self.old_fields = old_fields or {}
         self.skip_when_empty_fields = skip_when_empty_fields or set()
         self.field_serializers = field_serializers or {}
 
     def unpack(
         self,
-        storage_dict: Dict[str, Any],
+        unpacked_dict: Dict[str, UnpackedValue],
         whitelist_map: WhitelistMap,
-        descent_path: str,
+        context: UnpackContext,
     ) -> T_NamedTuple:
         try:
-            storage_dict = self.before_unpack(**storage_dict)
+            unpacked_dict = self.before_unpack(context, unpacked_dict)
             unpacked: Dict[str, PackableValue] = {}
-            for key, value in storage_dict.items():
-                loaded_name = self.get_loaded_field_name(field=key)
+            for key, value in unpacked_dict.items():
+                loaded_name = self.loaded_field_names.get(key, key)
                 # Naively implements backwards compatibility by filtering arguments that aren't present in
                 # the constructor. If a property is present in the serialized object, but doesn't exist in
                 # the version of the class loaded into memory, that property will be completely ignored.
                 if loaded_name in self.constructor_param_names:
-                    unpack_fn = self.get_field_unpack_fn(field=loaded_name)
-                    unpacked[loaded_name] = unpack_fn(
-                        value, whitelist_map=whitelist_map, descent_path=descent_path
-                    )
+                    # custom unpack regardless of hook vs recursive descent
+                    custom = self.field_serializers.get(loaded_name)
+                    if custom:
+                        unpacked[loaded_name] = custom.unpack(
+                            value,
+                            whitelist_map=whitelist_map,
+                            context=context,
+                        )
+                    elif context.observed_unknown_serdes_values:
+                        unpacked[loaded_name] = context.assert_no_unknown_values(value)
+                    else:
+                        unpacked[loaded_name] = cast(PackableValue, value)
+
+                else:
+                    context.clear_ignored_unknown_values(value)
 
             # False positive type error here due to an eccentricity of `NamedTuple`-- calling `NamedTuple`
             # directly acts as a class factory, which is not true for `NamedTuple` subclasses (which act
             # like normal constructors). Because we have no subclass info here, the type checker thinks
             # we are invoking the class factory and complains about arguments.
             return self.klass(**unpacked)  # type: ignore
         except Exception as exc:
-            return self.handle_unpack_error(exc, **storage_dict)
+            value = self.handle_unpack_error(exc, context, unpacked_dict)
+            if isinstance(context, UnpackContext):
+                context.assert_no_unknown_values(value)
+                context.clear_ignored_unknown_values(unpacked_dict)
+            return value
 
-    # Hook: Modify the contents of the loaded dict before it is unpacked into domain objects during
+    # Hook: Modify the contents of the unpacked dict before domain object construction during
     # deserialization.
-    def before_unpack(self, **raw_dict: JsonSerializableValue) -> Dict[str, JsonSerializableValue]:
-        return raw_dict
+    def before_unpack(
+        self,
+        context: UnpackContext,
+        unpacked_dict: Dict[str, UnpackedValue],
+    ) -> Dict[str, UnpackedValue]:
+        return unpacked_dict
 
     # Hook: Handle an error that occurs when unpacking a NamedTuple. Can be used to return a default
     # value.
-    def handle_unpack_error(self, exc: Exception, **storage_dict: Any) -> NoReturn:
+    def handle_unpack_error(
+        self,
+        exc: Exception,
+        context: UnpackContext,
+        storage_dict: Dict[str, Any],
+    ) -> Any:
         raise exc
 
     def pack(
         self,
         value: T_NamedTuple,
         whitelist_map: WhitelistMap,
         descent_path: str,
     ) -> Dict[str, JsonSerializableValue]:
         packed: Dict[str, JsonSerializableValue] = {}
         packed["__class__"] = self.get_storage_name()
         for key, inner_value in value._asdict().items():
             if key in self.skip_when_empty_fields and inner_value in EMPTY_VALUES_TO_SKIP:
                 continue
-            storage_key = self.get_storage_field_name(field=key)
-            pack_fn = self.get_field_pack_fn(field=key)
-            packed[storage_key] = pack_fn(
-                inner_value, whitelist_map=whitelist_map, descent_path=f"{descent_path}.{key}"
-            )
+            storage_key = self.storage_field_names.get(key, key)
+            custom = self.field_serializers.get(key)
+            if custom:
+                packed[storage_key] = custom.pack(
+                    inner_value,
+                    whitelist_map=whitelist_map,
+                    descent_path=f"{descent_path}.{key}",
+                )
+            else:
+                packed[storage_key] = _pack_value(
+                    inner_value,
+                    whitelist_map=whitelist_map,
+                    descent_path=f"{descent_path}.{key}",
+                )
         for key, default in self.old_fields.items():
             packed[key] = default
         packed = self.after_pack(**packed)
         return packed
 
     # Hook: Modify the contents of the packed, json-serializable dict before it is converted to a
     # string.
@@ -428,31 +540,14 @@
     @cached_method
     def constructor_param_names(self) -> Sequence[str]:
         return list(signature(self.klass.__new__).parameters.keys())
 
     def get_storage_name(self) -> str:
         return self.storage_name or self.klass.__name__
 
-    def get_field_unpack_fn(self, field: str) -> Callable[..., PackableValue]:
-        field_serializer = self.field_serializers.get(field)
-        return field_serializer.unpack if field_serializer else unpack_value
-
-    def get_field_pack_fn(self, field: str) -> Callable[..., JsonSerializableValue]:
-        field_serializer = self.field_serializers.get(field)
-        return field_serializer.pack if field_serializer else pack_value
-
-    def get_storage_field_name(self, field: str) -> str:
-        return self.storage_field_names.get(field, field)
-
-    def get_loaded_field_name(self, field: str) -> str:
-        for k, v in self.storage_field_names.items():
-            if v == field:
-                return k
-        return field
-
 
 class FieldSerializer(Serializer):
     _instance = None
 
     # Because `FieldSerializer` is not currently parameterizable (all variation is contained in the
     # logic of pack/unpack), we store references to a singleton instance in the whitelist map to
     # save memory.
@@ -461,17 +556,17 @@
         if cls._instance is None:
             cls._instance = cls()
         return cls._instance
 
     @abstractmethod
     def unpack(
         self,
-        __packed_value: Any,
+        __unpacked_value: UnpackedValue,
         whitelist_map: WhitelistMap,
-        descent_path: str,
+        context: UnpackContext,
     ) -> PackableValue:
         ...
 
     @abstractmethod
     def pack(
         self,
         __unpacked_value: Any,
@@ -483,27 +578,31 @@
 
 ###################################################################################################
 # Serialize / Pack
 ###################################################################################################
 
 
 def serialize_value(
-    val: PackableValue, whitelist_map: WhitelistMap = _WHITELIST_MAP, **json_kwargs: object
+    val: PackableValue,
+    whitelist_map: WhitelistMap = _WHITELIST_MAP,
+    **json_kwargs: object,
 ) -> str:
     """Serialize an object to a JSON string.
 
     Objects are first converted to a JSON-serializable form with `pack_value`.
     """
     packed_value = pack_value(val, whitelist_map=whitelist_map)
     return seven.json.dumps(packed_value, **json_kwargs)
 
 
 @overload
 def pack_value(
-    val: T_Scalar, whitelist_map: WhitelistMap = ..., descent_path: Optional[str] = ...
+    val: T_Scalar,
+    whitelist_map: WhitelistMap = ...,
+    descent_path: Optional[str] = ...,
 ) -> T_Scalar:
     ...
 
 
 @overload
 def pack_value(
     val: Union[
@@ -534,49 +633,60 @@
     The following types are transformed in to dicts with special marker keys:
         * whitelisted named tuples
         * whitelisted enums
         * set
         * frozenset
     """
     descent_path = _root(val) if descent_path is None else descent_path
-    return _pack_value(val, whitelist_map=whitelist_map, descent_path=_root(val))
+    return _pack_value(val, whitelist_map=whitelist_map, descent_path=descent_path)
 
 
 def _pack_value(
-    val: PackableValue, whitelist_map: WhitelistMap, descent_path: str
+    val: PackableValue,
+    whitelist_map: WhitelistMap,
+    descent_path: str,
 ) -> JsonSerializableValue:
-    if is_named_tuple_instance(val):
+    # this is a hot code path so we handle the common base cases without isinstance
+    tval = type(val)
+    if tval in (int, float, str, bool) or val is None:
+        return cast(JsonSerializableValue, val)
+    if tval is list:
+        return [
+            _pack_value(item, whitelist_map, f"{descent_path}[{idx}]")
+            for idx, item in enumerate(cast(list, val))
+        ]
+    if tval is dict:
+        return {
+            key: _pack_value(value, whitelist_map, f"{descent_path}.{key}")
+            for key, value in cast(dict, val).items()
+        }
+
+    # inlined is_named_tuple_instance
+    if isinstance(val, tuple) and hasattr(val, "_fields"):
         klass_name = val.__class__.__name__
-        if not whitelist_map.has_tuple_entry(klass_name):
+        if not whitelist_map.has_tuple_serializer(klass_name):
             raise SerializationError(
                 (
                     "Can only serialize whitelisted namedtuples, received"
-                    f" {val}.{_path_msg(descent_path)}"
+                    f" {val}.\nDescent path: {descent_path}"
                 ),
             )
-        serializer = whitelist_map.get_tuple_entry(klass_name)
-        return serializer.pack(val, whitelist_map, descent_path)
+        serializer = whitelist_map.get_tuple_serializer(klass_name)
+        return serializer.pack(cast(NamedTuple, val), whitelist_map, descent_path)
     if isinstance(val, Enum):
         klass_name = val.__class__.__name__
         if not whitelist_map.has_enum_entry(klass_name):
             raise SerializationError(
                 (
                     "Can only serialize whitelisted Enums, received"
-                    f" {klass_name}.{_path_msg(descent_path)}"
+                    f" {klass_name}.\nDescent path: {descent_path}"
                 ),
             )
         enum_serializer = whitelist_map.get_enum_entry(klass_name)
         return {"__enum__": enum_serializer.pack(val, whitelist_map, descent_path)}
-    if isinstance(val, (int, float, str, bool)) or val is None:
-        return val
-    if isinstance(val, collections.abc.Sequence):
-        return [
-            _pack_value(item, whitelist_map, f"{descent_path}[{idx}]")
-            for idx, item in enumerate(val)
-        ]
     if isinstance(val, set):
         set_path = descent_path + "{}"
         return {
             "__set__": [
                 _pack_value(item, whitelist_map, set_path) for item in sorted(list(val), key=str)
             ]
         }
@@ -584,21 +694,31 @@
         frz_set_path = descent_path + "{}"
         return {
             "__frozenset__": [
                 _pack_value(item, whitelist_map, frz_set_path)
                 for item in sorted(list(val), key=str)
             ]
         }
+
+    # custom string subclasses
+    if isinstance(val, str):
+        return val
+
+    # handle more expensive and uncommon abc instance checks last
     if isinstance(val, collections.abc.Mapping):
         return {
             key: _pack_value(value, whitelist_map, f"{descent_path}.{key}")
             for key, value in val.items()
         }
+    if isinstance(val, collections.abc.Sequence):
+        return [
+            _pack_value(item, whitelist_map, f"{descent_path}[{idx}]")
+            for idx, item in enumerate(val)
+        ]
 
-    # list/dict checks above don't fully cover Sequence/Mapping
     return val
 
 
 ###################################################################################################
 # Deserialize / Unpack
 ###################################################################################################
 
@@ -650,134 +770,152 @@
     - Optionally, check that the resulting object is of the expected type.
     """
     check.str_param(val, "val")
 
     # Never issue warnings when deserializing deprecated objects.
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", DeprecationWarning)
-
-        packed_value = seven.json.loads(val)
-        unpacked_value = unpack_value(packed_value, whitelist_map=whitelist_map)
+        context = UnpackContext()
+        unpacked_value = seven.json.loads(
+            val, object_hook=partial(_unpack_object, whitelist_map=whitelist_map, context=context)
+        )
+        unpacked_value = context.finalize_unpack(unpacked_value)
         if as_type and not (
             is_named_tuple_instance(unpacked_value)
             if as_type is NamedTuple
             else isinstance(unpacked_value, as_type)
         ):
             raise DeserializationError(
                 f"Deserialized object was not expected type {as_type}, got {type(unpacked_value)}"
             )
-        return unpacked_value
+
+    return unpacked_value
+
+
+class UnknownSerdesValue:
+    def __init__(self, message: str, value: Mapping[str, UnpackedValue]):
+        self.message = message
+        self.value = value
+
+
+def _unpack_object(val: dict, whitelist_map: WhitelistMap, context: UnpackContext):
+    if "__class__" in val:
+        klass_name = cast(str, val["__class__"])
+        if not whitelist_map.has_tuple_deserializer(klass_name):
+            return context.observe_unknown_value(
+                UnknownSerdesValue(
+                    f'Attempted to deserialize class "{klass_name}" which is not in the whitelist.',
+                    val,
+                )
+            )
+
+        val.pop("__class__")
+        deserializer = whitelist_map.get_tuple_deserializer(klass_name)
+        return deserializer.unpack(val, whitelist_map, context)
+
+    if "__enum__" in val:
+        enum = cast(str, val["__enum__"])
+        name, member = enum.split(".")
+        if not whitelist_map.has_enum_entry(name):
+            return context.observe_unknown_value(
+                UnknownSerdesValue(
+                    f"Attempted to deserialize enum {name} which was not in the whitelist.",
+                    val,
+                )
+            )
+
+        enum_serializer = whitelist_map.get_enum_entry(name)
+        return enum_serializer.unpack(member)
+
+    if "__set__" in val:
+        items = cast(List[JsonSerializableValue], val["__set__"])
+        return set(items)
+
+    if "__frozenset__" in val:
+        items = cast(List[JsonSerializableValue], val["__frozenset__"])
+        return frozenset(items)
+
+    return val
 
 
 @overload
 def unpack_value(
     val: JsonSerializableValue,
     as_type: Tuple[Type[T_PackableValue], Type[U_PackableValue]],
     whitelist_map: WhitelistMap = ...,
-    descent_path: str = ...,
+    context: Optional[UnpackContext] = ...,
 ) -> Union[T_PackableValue, U_PackableValue]:
     ...
 
 
 @overload
 def unpack_value(
     val: JsonSerializableValue,
     as_type: Type[T_PackableValue],
     whitelist_map: WhitelistMap = ...,
-    descent_path: str = ...,
+    context: Optional[UnpackContext] = ...,
 ) -> T_PackableValue:
     ...
 
 
 @overload
 def unpack_value(
     val: JsonSerializableValue,
     as_type: None = ...,
     whitelist_map: WhitelistMap = ...,
-    descent_path: str = ...,
+    context: Optional[UnpackContext] = ...,
 ) -> PackableValue:
     ...
 
 
 def unpack_value(
     val: JsonSerializableValue,
     as_type: Optional[
         Union[Type[T_PackableValue], Tuple[Type[T_PackableValue], Type[U_PackableValue]]]
     ] = None,
     whitelist_map: WhitelistMap = _WHITELIST_MAP,
-    descent_path: Optional[str] = None,
+    context: Optional[UnpackContext] = None,
 ) -> Union[PackableValue, T_PackableValue, Union[T_PackableValue, U_PackableValue]]:
     """Convert a JSON-serializable complex of dicts, lists, and scalars into domain objects.
 
     Dicts with special keys are processed specially:
     - {"__set__": [...]}: becomes a set()
     - {"__frozenset__": [...]}: becomes a frozenset()
     - {"__enum__": "<class>.<name>"}: becomes an Enum class[name], where `class` is an Enum descendant
     - {"__class__": "<class>", ...}: becomes a NamedTuple, where `class` is a NamedTuple descendant
     """
-    descent_path = _root(val) if descent_path is None else descent_path
+    context = UnpackContext() if context is None else context
     unpacked_value = _unpack_value(
         val,
         whitelist_map,
-        descent_path,
+        context,
     )
+    unpacked_value = context.finalize_unpack(unpacked_value)
     if as_type and not (
         is_named_tuple_instance(unpacked_value)
         if as_type is NamedTuple
         else isinstance(unpacked_value, as_type)
     ):
         raise DeserializationError(
             f"Unpacked object was not expected type {as_type}, got {type(val)}"
         )
     return unpacked_value
 
 
 def _unpack_value(
-    val: JsonSerializableValue, whitelist_map: WhitelistMap, descent_path: str
-) -> PackableValue:
+    val: JsonSerializableValue,
+    whitelist_map: WhitelistMap,
+    context: UnpackContext,
+) -> UnpackedValue:
     if isinstance(val, list):
-        return [
-            _unpack_value(item, whitelist_map, f"{descent_path}[{idx}]")
-            for idx, item in enumerate(val)
-        ]
-    if isinstance(val, dict) and val.get("__class__"):
-        klass_name = cast(str, val.pop("__class__"))
-        if not whitelist_map.has_tuple_entry(klass_name):
-            raise DeserializationError(
-                f'Attempted to deserialize class "{klass_name}" which is not in the whitelist. '
-                "This error can occur due to version skew, verify processes are running "
-                f"expected versions.{_path_msg(descent_path)}"
-            )
+        return [_unpack_value(item, whitelist_map, context) for item in val]
 
-        serializer = whitelist_map.get_tuple_entry(klass_name)
-        return serializer.unpack(val, whitelist_map, descent_path)
-    if isinstance(val, dict) and val.get("__enum__"):
-        enum = cast(str, val["__enum__"])
-        name, member = enum.split(".")
-        if not whitelist_map.has_enum_entry(name):
-            raise DeserializationError(
-                f"Attempted to deserialize enum {name} which was not in the whitelist.\n"
-                "This error can occur due to version skew, verify processes are running "
-                f"expected versions.{_path_msg(descent_path)}"
-            )
-        enum_serializer = whitelist_map.get_enum_entry(name)
-        return enum_serializer.unpack(member)
-    if isinstance(val, dict) and "__set__" in val:
-        set_path = descent_path + "{}"
-        items = cast(List[JsonSerializableValue], val["__set__"])
-        return set([_unpack_value(item, whitelist_map, set_path) for item in items])
-    if isinstance(val, dict) and "__frozenset__" in val:
-        frz_set_path = descent_path + "{}"
-        items = cast(List[JsonSerializableValue], val["__frozenset__"])
-        return frozenset([_unpack_value(item, whitelist_map, frz_set_path) for item in items])
     if isinstance(val, dict):
-        return {
-            key: _unpack_value(value, whitelist_map, f"{descent_path}.{key}")
-            for key, value in val.items()
-        }
+        unpacked_vals = {k: _unpack_value(v, whitelist_map, context) for k, v in val.items()}
+        return _unpack_object(unpacked_vals, whitelist_map, context)
 
     return val
 
 
 ###################################################################################################
 # Validation
 ###################################################################################################
@@ -837,37 +975,9 @@
 
 
 ###################################################################################################
 # Utilities
 ###################################################################################################
 
 
-def _path_msg(descent_path: str) -> str:
-    if not descent_path:
-        return ""
-    else:
-        return f"\nDescent path: {descent_path}"
-
-
 def _root(val: Any) -> str:
     return f"<root:{val.__class__.__name__}>"
-
-
-# The below utilities are intended for use in `after_pack` and `before_unpack` hooks in custom
-# namedtuple serializers. They help in manipulating the packed representation of various objects.
-
-
-def is_packed_enum(val: object) -> TypeGuard[Mapping[str, str]]:
-    return isinstance(val, dict) and "__enum__" in val
-
-
-def copy_packed_set(
-    packed_set: Mapping[str, Sequence[JsonSerializableValue]],
-    as_type: Literal["__frozenset__", "__set__"],
-) -> Mapping[str, Sequence[JsonSerializableValue]]:
-    """Returns a copy of the packed collection."""
-    if "__set__" in packed_set:
-        return {as_type: packed_set["__set__"]}
-    elif "__frozenset__" in packed_set:
-        return {as_type: packed_set["__frozenset__"]}
-    else:
-        check.failed(f"Invalid packed set: {packed_set}")
```

### Comparing `dagster-1.3.1/dagster/_seven/__init__.py` & `dagster-1.3.2/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_seven/abc.py` & `dagster-1.3.2/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_seven/compat/pendulum.py` & `dagster-1.3.2/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/__init__.py` & `dagster-1.3.2/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/alert.py` & `dagster-1.3.2/dagster/_utils/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dagster._core.definitions.sensor_definition import DefaultSensorStatus, SensorDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._utils.backcompat import deprecation_warning
 
 if TYPE_CHECKING:
     from dagster._core.definitions.graph_definition import GraphDefinition
-    from dagster._core.definitions.pipeline_definition import PipelineDefinition
+    from dagster._core.definitions.job_definition import JobDefinition
     from dagster._core.definitions.run_status_sensor_definition import RunFailureSensorContext
     from dagster._core.definitions.selector import JobSelector, RepositorySelector
     from dagster._core.definitions.unresolved_asset_job_definition import (
         UnresolvedAssetJobDefinition,
     )
 
 
@@ -84,26 +84,26 @@
     smtp_type: str = "SSL",
     smtp_port: Optional[int] = None,
     name: Optional[str] = None,
     dagit_base_url: Optional[str] = None,
     monitored_jobs: Optional[
         Sequence[
             Union[
-                "PipelineDefinition",
+                "JobDefinition",
                 "GraphDefinition",
                 "UnresolvedAssetJobDefinition",
                 "RepositorySelector",
                 "JobSelector",
             ]
         ]
     ] = None,
     job_selection: Optional[
         Sequence[
             Union[
-                "PipelineDefinition",
+                "JobDefinition",
                 "GraphDefinition",
                 "UnresolvedAssetJobDefinition",
                 "RepositorySelector",
                 "JobSelector",
             ]
         ]
     ] = None,
```

### Comparing `dagster-1.3.1/dagster/_utils/backcompat.py` & `dagster-1.3.2/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/backoff.py` & `dagster-1.3.2/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/cached_method.py` & `dagster-1.3.2/dagster/_utils/cached_method.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 from functools import wraps
 from typing import AbstractSet, Callable, Dict, Hashable, Mapping, Tuple, Type, TypeVar
 
-from typing_extensions import Concatenate, Final, ParamSpec
+from typing_extensions import Concatenate, ParamSpec
 
 from dagster import _check as check
 
 S = TypeVar("S")
 T = TypeVar("T")
 T_Callable = TypeVar("T_Callable", bound=Callable)
 P = ParamSpec("P")
 
 
-class _Sentinel:
-    ...
-
-
-NO_VALUE_IN_CACHE_SENTINEL: Final = _Sentinel()
 NO_ARGS_HASH_VALUE = 0
 
 CACHED_METHOD_FIELD_SUFFIX = "_cached__internal__"
 
 
 def cached_method(method: Callable[Concatenate[S, P], T]) -> Callable[Concatenate[S, P], T]:
     """Caches the results of a method call.
@@ -52,34 +47,31 @@
             obj.a_method(arg1="a", arg2=5)
             obj.a_method(arg2=5, arg1="a")
             obj.a_method("a", 5)
 
     With this decorator, the first two would point to the same cache entry, and non-kwarg arguments
     are not allowed.
     """
+    cache_attr_name = method.__name__ + CACHED_METHOD_FIELD_SUFFIX
 
     @wraps(method)
-    def helper(self: S, *args: P.args, **kwargs: P.kwargs) -> T:
-        cache_attr_name = method.__name__ + CACHED_METHOD_FIELD_SUFFIX
+    def _cached_method_wrapper(self: S, *args: P.args, **kwargs: P.kwargs) -> T:
         if not hasattr(self, cache_attr_name):
             cache: Dict[Hashable, T] = {}
             setattr(self, cache_attr_name, cache)
         else:
             cache = getattr(self, cache_attr_name)
 
         key = _make_key(args, kwargs)
-        cached_result = cache.get(key, NO_VALUE_IN_CACHE_SENTINEL)
-        if not isinstance(cached_result, _Sentinel):
-            return cached_result
-        else:
+        if key not in cache:
             result = method(self, *args, **kwargs)
             cache[key] = result
-            return result
+        return cache[key]
 
-    return helper
+    return _cached_method_wrapper
 
 
 class _HashedSeq(list):
     """Adapted from https://github.com/python/cpython/blob/f9433fff476aa13af9cb314fcc6962055faa4085/Lib/functools.py#L432.
 
     This class guarantees that hash() will be called no more than once
     per element.  This is important because the lru_cache() will hash
```

### Comparing `dagster-1.3.1/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.2/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/dagster_type.py` & `dagster-1.3.2/dagster/_utils/dagster_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 from dagster._core.definitions.events import Failure, TypeCheck
+from dagster._core.definitions.graph_definition import GraphDefinition
 from dagster._core.definitions.pipeline_base import InMemoryPipeline
-from dagster._core.definitions.pipeline_definition import PipelineDefinition
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.execution.api import create_execution_plan
 from dagster._core.execution.context_creation_pipeline import scoped_pipeline_context
 from dagster._core.instance import DagsterInstance
 from dagster._core.types.dagster_type import resolve_dagster_type
 
 from .typing_api import is_typing_type
@@ -37,15 +37,15 @@
                 "Must pass in a type from dagster module. You passed {dagster_type} "
                 "which is part of python's typing module."
             ).format(dagster_type=dagster_type)
         )
 
     dagster_type = resolve_dagster_type(dagster_type)
 
-    pipeline = InMemoryPipeline(PipelineDefinition([], "empty"))
+    pipeline = InMemoryPipeline(GraphDefinition(node_defs=[], name="empty").to_job())
     pipeline_def = pipeline.get_definition()
 
     instance = DagsterInstance.ephemeral()
     execution_plan = create_execution_plan(pipeline)
     pipeline_run = instance.create_run_for_pipeline(pipeline_def)
     with scoped_pipeline_context(execution_plan, pipeline, {}, pipeline_run, instance) as context:
         type_check_context = context.for_type(dagster_type)
```

### Comparing `dagster-1.3.1/dagster/_utils/error.py` & `dagster-1.3.2/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/external.py` & `dagster-1.3.2/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/forked_pdb.py` & `dagster-1.3.2/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/hosted_user_process.py` & `dagster-1.3.2/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/indenting_printer.py` & `dagster-1.3.2/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/interrupts.py` & `dagster-1.3.2/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/log.py` & `dagster-1.3.2/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/merger.py` & `dagster-1.3.2/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/net.py` & `dagster-1.3.2/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/schedules.py` & `dagster-1.3.2/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/tags.py` & `dagster-1.3.2/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/temp_file.py` & `dagster-1.3.2/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/test/__init__.py` & `dagster-1.3.2/dagster/_utils/test/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,20 @@
     DependencyDefinition,
     NodeInvocation,
     _check as check,
 )
 from dagster._core.definitions import (
     GraphDefinition,
     InputMapping,
-    ModeDefinition,
+    JobDefinition,
     OpDefinition,
     OutputMapping,
-    PipelineDefinition,
 )
 from dagster._core.definitions.dependency import Node
-from dagster._core.definitions.job_definition import JobDefinition
+from dagster._core.definitions.executor_definition import in_process_executor
 from dagster._core.definitions.logger_definition import LoggerDefinition
 from dagster._core.definitions.pipeline_base import InMemoryPipeline
 from dagster._core.definitions.resource_definition import ScopedResourcesBuilder
 from dagster._core.execution.api import create_execution_plan
 from dagster._core.execution.context.system import PlanExecutionContext
 from dagster._core.execution.context_creation_pipeline import (
     create_context_creation_data,
@@ -54,18 +53,18 @@
 
 def create_test_pipeline_execution_context(
     logger_defs: Optional[Mapping[str, LoggerDefinition]] = None
 ) -> PlanExecutionContext:
     loggers = check.opt_mapping_param(
         logger_defs, "logger_defs", key_type=str, value_type=LoggerDefinition
     )
-    mode_def = ModeDefinition(logger_defs=loggers)
-    pipeline_def = PipelineDefinition(
-        name="test_legacy_context", node_defs=[], mode_defs=[mode_def]
-    )
+    pipeline_def = GraphDefinition(
+        name="test_legacy_context",
+        node_defs=[],
+    ).to_job(executor_def=in_process_executor, logger_defs=logger_defs)
     run_config: Dict[str, Dict[str, Dict]] = {"loggers": {key: {} for key in loggers}}
     pipeline_run = DagsterRun(pipeline_name="test_legacy_context", run_config=run_config)
     instance = DagsterInstance.ephemeral()
     execution_plan = create_execution_plan(pipeline=pipeline_def, run_config=run_config)
     creation_data = create_context_creation_data(
         InMemoryPipeline(pipeline_def),
         execution_plan,
@@ -91,15 +90,15 @@
 def _dep_key_of(node: Node) -> NodeInvocation:
     return NodeInvocation(node.definition.name, node.name)
 
 
 def build_job_with_input_stubs(
     job_def: JobDefinition, inputs: Mapping[str, Mapping[str, object]]
 ) -> JobDefinition:
-    check.inst_param(job_def, "pipeline_def", PipelineDefinition)
+    check.inst_param(job_def, "pipeline_def", JobDefinition)
     check.mapping_param(inputs, "inputs", key_type=str, value_type=dict)
 
     deps: Dict[NodeInvocation, Dict[str, object]] = defaultdict(dict)
     for node_name, dep_dict in job_def.dependencies.items():
         for input_name, dep in dep_dict.items():
             deps[node_name][input_name] = dep
```

### Comparing `dagster-1.3.1/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.2/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.2/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.2/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/timing.py` & `dagster-1.3.2/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/typing_api.py` & `dagster-1.3.2/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster/_utils/yaml_utils.py` & `dagster-1.3.2/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/dagster.egg-info/PKG-INFO` & `dagster-1.3.2/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.1
+Version: 1.3.2
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.1/dagster.egg-info/SOURCES.txt` & `dagster-1.3.2/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -117,32 +117,29 @@
 dagster/_core/definitions/input.py
 dagster/_core/definitions/instigation_logger.py
 dagster/_core/definitions/job_definition.py
 dagster/_core/definitions/load_assets_from_modules.py
 dagster/_core/definitions/logger_definition.py
 dagster/_core/definitions/logger_invocation.py
 dagster/_core/definitions/materialize.py
-dagster/_core/definitions/mode.py
 dagster/_core/definitions/multi_asset_sensor_definition.py
 dagster/_core/definitions/multi_dimensional_partitions.py
 dagster/_core/definitions/no_step_launcher.py
 dagster/_core/definitions/node_container.py
 dagster/_core/definitions/node_definition.py
 dagster/_core/definitions/observe.py
 dagster/_core/definitions/op_definition.py
 dagster/_core/definitions/op_invocation.py
 dagster/_core/definitions/output.py
 dagster/_core/definitions/partition.py
 dagster/_core/definitions/partition_key_range.py
 dagster/_core/definitions/partition_mapping.py
 dagster/_core/definitions/partitioned_schedule.py
 dagster/_core/definitions/pipeline_base.py
-dagster/_core/definitions/pipeline_definition.py
 dagster/_core/definitions/policy.py
-dagster/_core/definitions/preset.py
 dagster/_core/definitions/reconstruct.py
 dagster/_core/definitions/resolved_asset_deps.py
 dagster/_core/definitions/resource_annotation.py
 dagster/_core/definitions/resource_definition.py
 dagster/_core/definitions/resource_invocation.py
 dagster/_core/definitions/resource_requirement.py
 dagster/_core/definitions/run_config.py
```

### Comparing `dagster-1.3.1/dagster.egg-info/requires.txt` & `dagster-1.3.2/dagster.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.3.1/setup.py` & `dagster-1.3.2/setup.py`

 * *Files identical despite different names*

