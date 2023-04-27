# Comparing `tmp/dagster-graphql-1.3.1.tar.gz` & `tmp/dagster-graphql-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.1.tar", last modified: Thu Apr 20 20:47:19 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.2.tar", last modified: Thu Apr 27 19:31:28 2023, max compression
```

## Comparing `dagster-graphql-1.3.1.tar` & `dagster-graphql-1.3.2.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.755718 dagster-graphql-1.3.1/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-20 20:47:19.755718 dagster-graphql-1.3.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.691717 dagster-graphql-1.3.1/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.695718 dagster-graphql-1.3.1/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21649 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.707718 dagster-graphql-1.3.1/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18443 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.711718 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11579 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8860 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     5032 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7594 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12620 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15390 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8258 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10803 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8080 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.735718 dagster-graphql-1.3.1/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40174 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    14982 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18079 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16228 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    11017 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     4947 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    22897 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.735718 dagster-graphql-1.3.1/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20899 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    16816 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.743718 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11072 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39733 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1262 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.751718 dagster-graphql-1.3.1/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25590 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    36131 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4051 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.751718 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8314 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7971 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29755 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.751718 dagster-graphql-1.3.1/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6376 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:47:19.691717 dagster-graphql-1.3.1/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4100 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-20 20:47:19.000000 dagster-graphql-1.3.1/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-20 20:47:19.755718 dagster-graphql-1.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1455 2023-04-20 20:39:02.000000 dagster-graphql-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.799791 dagster-graphql-1.3.2/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-27 19:31:28.799791 dagster-graphql-1.3.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.471790 dagster-graphql-1.3.2/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.475790 dagster-graphql-1.3.2/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21649 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.551791 dagster-graphql-1.3.2/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18443 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.559791 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11579 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7454 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12620 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15183 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8258 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10803 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    20758 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.711791 dagster-graphql-1.3.2/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40629 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    15150 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18079 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10989 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    23351 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.715791 dagster-graphql-1.3.2/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20899 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    16816 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.727791 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11072 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39816 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.791791 dagster-graphql-1.3.2/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    25590 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    36271 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4051 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.795791 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8314 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29755 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.795791 dagster-graphql-1.3.2/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6376 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:28.471790 dagster-graphql-1.3.2/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 19:31:28.000000 dagster-graphql-1.3.2/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-27 19:31:28.799791 dagster-graphql-1.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-27 18:30:33.000000 dagster-graphql-1.3.2/setup.py
```

### Comparing `dagster-graphql-1.3.1/LICENSE` & `dagster-graphql-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/PKG-INFO` & `dagster-graphql-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.1
+Version: 1.3.2
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/__init__.py` & `dagster-graphql-1.3.2/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/cli.py` & `dagster-graphql-1.3.2/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/client/client.py` & `dagster-graphql-1.3.2/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.2/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/client/query.py` & `dagster-graphql-1.3.2/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.2/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,14 @@
             raise DagsterError(
                 "forceSynchronousSubmission is not supported for pure asset backfills"
             )
 
         if backfill_params.get("fromFailure"):
             raise DagsterError("fromFailure is not supported for pure asset backfills")
 
-        if backfill_params.get("allPartitions"):
-            raise DagsterError("allPartitions is not supported for pure asset backfills")
-
         asset_graph = ExternalAssetGraph.from_workspace(graphene_info.context)
 
         location_names = set(
             repo_handle.code_location_origin.location_name
             for repo_handle in asset_graph.repository_handles_by_key.values()
         )
 
@@ -157,16 +154,17 @@
 
         backfill = PartitionBackfill.from_asset_partitions(
             asset_graph=asset_graph,
             backfill_id=backfill_id,
             tags=tags,
             backfill_timestamp=backfill_timestamp,
             asset_selection=asset_selection,
-            partition_names=backfill_params["partitionNames"],
+            partition_names=backfill_params.get("partitionNames"),
             dynamic_partitions_store=CachingInstanceQueryer(graphene_info.context.instance),
+            all_partitions=backfill_params.get("allPartitions", False),
         )
     else:
         raise DagsterError(
             "Backfill requested without specifying partition set selector or asset selection"
         )
 
     graphene_info.context.instance.add_backfill(backfill)
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus
 from dagster._core.storage.tags import RESUME_RETRY_TAG
 from dagster._core.utils import make_new_run_id
 from dagster._utils.merger import merge_dicts
 
 from ..external import ensure_valid_config, get_external_execution_plan_or_raise
-from ..utils import ExecutionParams, UserFacingGraphQLError
+from ..utils import ExecutionParams
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.util import ResolveInfo
 
 
 def _get_run(instance: DagsterInstance, run_id: str) -> DagsterRun:
     run = instance.get_run_by_id(run_id)
@@ -57,37 +57,23 @@
 
 
 def create_valid_pipeline_run(
     graphene_info: "ResolveInfo",
     external_pipeline: ExternalPipeline,
     execution_params: ExecutionParams,
 ) -> DagsterRun:
-    from ...schema.errors import GrapheneNoModeProvidedError
-
-    mode: Optional[str]
-    if execution_params.mode is None and len(external_pipeline.available_modes) > 1:
-        raise UserFacingGraphQLError(
-            GrapheneNoModeProvidedError(external_pipeline.name, external_pipeline.available_modes)
-        )
-    elif execution_params.mode is None and len(external_pipeline.available_modes) == 1:
-        mode = external_pipeline.available_modes[0]
-
-    else:
-        mode = execution_params.mode
-
-    ensure_valid_config(external_pipeline, mode, execution_params.run_config)
+    ensure_valid_config(external_pipeline, execution_params.run_config)
 
     step_keys_to_execute, known_state = compute_step_keys_to_execute(
         graphene_info, execution_params
     )
 
     external_execution_plan = get_external_execution_plan_or_raise(
         graphene_info=graphene_info,
         external_pipeline=external_pipeline,
-        mode=mode,
         run_config=execution_params.run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
     )
     tags = merge_dicts(external_pipeline.tags, execution_params.execution_metadata.tags)
 
     pipeline_run = graphene_info.context.instance.create_run(
@@ -102,15 +88,14 @@
         if execution_params.selector.asset_selection
         else None,
         solid_selection=execution_params.selector.solid_selection,
         solids_to_execute=frozenset(execution_params.selector.solid_selection)
         if execution_params.selector.solid_selection
         else None,
         run_config=execution_params.run_config,
-        mode=mode,
         step_keys_to_execute=step_keys_to_execute,
         tags=tags,
         root_run_id=execution_params.execution_metadata.root_run_id,
         parent_run_id=execution_params.execution_metadata.parent_run_id,
         status=DagsterRunStatus.NOT_STARTED,
         external_pipeline_origin=external_pipeline.get_external_origin(),
         pipeline_code_origin=external_pipeline.get_python_origin(),
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/external.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,26 +66,23 @@
                     pipeline=GraphenePipeline(ctx.get_full_external_job(selector)),
                 )
             )
 
     return external_pipeline
 
 
-def ensure_valid_config(
-    external_pipeline: ExternalPipeline, mode: Optional[str], run_config: object
-) -> object:
+def ensure_valid_config(external_pipeline: ExternalPipeline, run_config: object) -> object:
     from ..schema.pipelines.config import GrapheneRunConfigValidationInvalid
 
     check.inst_param(external_pipeline, "external_pipeline", ExternalPipeline)
-    check.opt_str_param(mode, "mode")
     # do not type check run_config so that validate_config_from_snap throws
 
     validated_config = validate_config_from_snap(
         config_schema_snapshot=external_pipeline.config_schema_snapshot,
-        config_type_key=check.not_none(external_pipeline.root_config_key_for_mode(mode)),
+        config_type_key=check.not_none(external_pipeline.root_config_key),
         config_value=run_config,
     )
 
     if not validated_config.success:
         raise UserFacingGraphQLError(
             GrapheneRunConfigValidationInvalid.for_validation_errors(
                 external_pipeline, validated_config.errors
@@ -94,23 +91,21 @@
 
     return validated_config
 
 
 def get_external_execution_plan_or_raise(
     graphene_info: "ResolveInfo",
     external_pipeline: ExternalPipeline,
-    mode: Optional[str],
     run_config: Mapping[str, object],
     step_keys_to_execute: Optional[Sequence[str]],
     known_state: Optional[KnownExecutionState],
 ) -> ExternalExecutionPlan:
     return graphene_info.context.get_external_execution_plan(
         external_pipeline=external_pipeline,
         run_config=run_config,
-        mode=check.not_none(mode),
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
     )
 
 
 @capture_error
 def fetch_repositories(graphene_info: "ResolveInfo") -> GrapheneRepositoryConnection:
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,44 +331,39 @@
 
 
 @capture_error
 def validate_pipeline_config(
     graphene_info: "ResolveInfo",
     selector: PipelineSelector,
     run_config: Union[str, Mapping[str, object]],
-    mode: Optional[str],
 ) -> "GraphenePipelineConfigValidationValid":
     from ..schema.pipelines.config import GraphenePipelineConfigValidationValid
 
     check.inst_param(selector, "selector", PipelineSelector)
-    check.opt_str_param(mode, "mode")
 
     external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
-    ensure_valid_config(external_pipeline, mode, run_config)
+    ensure_valid_config(external_pipeline, run_config)
     return GraphenePipelineConfigValidationValid(pipeline_name=external_pipeline.name)
 
 
 @capture_error
 def get_execution_plan(
     graphene_info: "ResolveInfo",
     selector: PipelineSelector,
     run_config: Mapping[str, Any],
-    mode: Optional[str],
 ) -> "GrapheneExecutionPlan":
     from ..schema.execution import GrapheneExecutionPlan
 
     check.inst_param(selector, "selector", PipelineSelector)
-    check.opt_str_param(mode, "mode")
 
     external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
-    ensure_valid_config(external_pipeline, mode, run_config)
+    ensure_valid_config(external_pipeline, run_config)
     return GrapheneExecutionPlan(
         graphene_info.context.get_external_execution_plan(
             external_pipeline=external_pipeline,
-            mode=mode,  # type: ignore  # (unclear if None accepted)
             run_config=run_config,
             step_keys_to_execute=None,
             known_state=None,
         )
     )
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/run_config_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from typing import TYPE_CHECKING, Mapping, Optional
 
 import dagster._check as check
 from dagster._config import validate_config_from_snap
 from dagster._core.host_representation import RepresentedPipeline
+from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 
+from dagster_graphql.schema.errors import GrapheneModeNotFoundError
 from dagster_graphql.schema.util import ResolveInfo
 
 from .external import get_external_pipeline_or_raise
 from .utils import PipelineSelector, UserFacingGraphQLError, capture_error
 
 if TYPE_CHECKING:
     from ..schema.pipelines.config import (
         GraphenePipelineConfigValidationValid,
     )
     from ..schema.run_config import GrapheneRunConfigSchema
 
 
 @capture_error
 def resolve_run_config_schema_or_error(
-    graphene_info: ResolveInfo, selector: PipelineSelector, mode: Optional[str]
+    graphene_info: ResolveInfo, selector: PipelineSelector, mode: Optional[str] = None
 ) -> "GrapheneRunConfigSchema":
-    from ..schema.errors import GrapheneModeNotFoundError
     from ..schema.run_config import GrapheneRunConfigSchema
 
     check.inst_param(selector, "selector", PipelineSelector)
-    check.opt_str_param(mode, "mode")
 
-    external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
-
-    if mode is None:
-        mode = external_pipeline.get_default_mode_name()
+    # Mode has been eliminated from the definitions layer, so we perform a "shallow" check for
+    # invalid mode. This is temporary and will be removed when the GQL API transitions to
+    # job/op/graph.
+    if mode and mode != DEFAULT_MODE_NAME:
+        return GrapheneModeNotFoundError(selector=selector, mode=mode)
 
-    if not external_pipeline.has_mode(mode):
-        raise UserFacingGraphQLError(GrapheneModeNotFoundError(mode=mode, selector=selector))
+    external_pipeline = get_external_pipeline_or_raise(graphene_info, selector)
 
     return GrapheneRunConfigSchema(
         represented_pipeline=external_pipeline,
-        mode=mode,
+        mode=DEFAULT_MODE_NAME,
     )
 
 
 @capture_error
 def resolve_is_run_config_valid(
     graphene_info: ResolveInfo,
     represented_pipeline: RepresentedPipeline,
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.2/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/asset_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 from ..implementation.loader import (
     BatchMaterializationLoader,
     CrossRepoAssetDependedByLoader,
     StaleStatusLoader,
 )
 from . import external
 from .asset_key import GrapheneAssetKey
+from .auto_materialize_policy import GrapheneAutoMaterializePolicy
 from .dagster_types import (
     GrapheneDagsterType,
     GrapheneListDagsterType,
     GrapheneNullableDagsterType,
     GrapheneRegularDagsterType,
     to_dagster_type,
 )
@@ -206,14 +207,15 @@
     dependedBy = non_null_list(GrapheneAssetDependency)
     dependedByKeys = non_null_list(GrapheneAssetKey)
     dependencies = non_null_list(GrapheneAssetDependency)
     dependencyKeys = non_null_list(GrapheneAssetKey)
     description = graphene.String()
     freshnessInfo = graphene.Field(GrapheneAssetFreshnessInfo)
     freshnessPolicy = graphene.Field(GrapheneFreshnessPolicy)
+    autoMaterializePolicy = graphene.Field(GrapheneAutoMaterializePolicy)
     graphName = graphene.String()
     groupName = graphene.String()
     id = graphene.NonNull(graphene.ID)
     isObservable = graphene.NonNull(graphene.Boolean)
     isPartitioned = graphene.NonNull(graphene.Boolean)
     isSource = graphene.NonNull(graphene.Boolean)
     jobNames = non_null_list(graphene.String)
@@ -702,14 +704,21 @@
     def resolve_freshnessPolicy(
         self, _graphene_info: ResolveInfo
     ) -> Optional[GrapheneFreshnessPolicy]:
         if self._external_asset_node.freshness_policy:
             return GrapheneFreshnessPolicy(self._external_asset_node.freshness_policy)
         return None
 
+    def resolve_autoMaterializePolicy(
+        self, _graphene_info: ResolveInfo
+    ) -> Optional[GrapheneAutoMaterializePolicy]:
+        if self._external_asset_node.auto_materialize_policy:
+            return GrapheneAutoMaterializePolicy(self._external_asset_node.auto_materialize_policy)
+        return None
+
     def resolve_jobNames(self, _graphene_info: ResolveInfo) -> Sequence[str]:
         return self._external_asset_node.job_names
 
     def resolve_jobs(self, _graphene_info: ResolveInfo) -> Sequence[GraphenePipeline]:
         job_names = self._external_asset_node.job_names or []
         return [
             GraphenePipeline(self._external_repository.get_full_external_job(job_name))
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
         "dagster_graphql.schema.partition_sets.GraphenePartitionStatusCounts"
     )
     isAssetBackfill = graphene.NonNull(graphene.Boolean)
     assetBackfillData = graphene.Field(GrapheneAssetBackfillData)
 
     hasCancelPermission = graphene.NonNull(graphene.Boolean)
     hasResumePermission = graphene.NonNull(graphene.Boolean)
+    user = graphene.Field(graphene.String)
 
     def __init__(self, backfill_job: PartitionBackfill):
         self._backfill_job = check.inst_param(backfill_job, "backfill_job", PartitionBackfill)
 
         self._records = None
         self._partition_run_data = None
 
@@ -304,20 +305,20 @@
             self._backfill_job.get_partitions_status_counts_and_totals_by_asset(
                 graphene_info.context
             )
         )
 
         asset_partition_status_counts = []
 
-        for asset_key, partitions_counts in status_counts_by_asset.items():
-            counts_by_status = partitions_counts[0]
+        for asset_key, asset_status in status_counts_by_asset.items():
+            (counts_by_status, total_num_partitions) = asset_status
             asset_partition_status_counts.append(
                 GrapheneAssetPartitionsStatusCounts(
                     assetKey=asset_key,
-                    numPartitionsTargeted=partitions_counts[1],
+                    numPartitionsTargeted=total_num_partitions,
                     numPartitionsRequested=counts_by_status[BackfillPartitionsStatus.REQUESTED],
                     numPartitionsCompleted=counts_by_status[BackfillPartitionsStatus.COMPLETED],
                     numPartitionsFailed=counts_by_status[BackfillPartitionsStatus.FAILED],
                 )
             )
 
         root_partitions_subset = self._backfill_job.get_target_root_partitions_subset(
@@ -360,14 +361,17 @@
         if self._backfill_job.partition_set_origin is None:
             return graphene_info.context.has_permission(Permissions.LAUNCH_PARTITION_BACKFILL)
         location_name = self._backfill_job.partition_set_origin.selector.location_name
         return graphene_info.context.has_permission_for_location(
             Permissions.LAUNCH_PARTITION_BACKFILL, location_name
         )
 
+    def resolve_user(self, _graphene_info: ResolveInfo) -> Optional[str]:
+        return self._backfill_job.user
+
 
 class GraphenePartitionBackfillOrError(graphene.Union):
     class Meta:
         types = (GraphenePartitionBackfill, GraphenePythonError)
         name = "PartitionBackfillOrError"
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,14 @@
 
     def resolve_jobs(self, _graphene_info: ResolveInfo):
         return [
             GrapheneJob(pipeline, self._batch_loader)
             for pipeline in sorted(
                 self._repository.get_all_external_jobs(), key=lambda pipeline: pipeline.name
             )
-            if pipeline.is_job
         ]
 
     def resolve_usedSolid(self, _graphene_info: ResolveInfo, name):
         return get_solid(self._repository, name)
 
     def resolve_usedSolids(self, _graphene_info: ResolveInfo):
         return get_solids(self._repository)
@@ -366,19 +365,23 @@
     nodes = non_null_list(GrapheneRepository)
 
     class Meta:
         name = "RepositoryConnection"
 
 
 class GrapheneWorkspace(graphene.ObjectType):
+    id = graphene.NonNull(graphene.String)
     locationEntries = non_null_list(GrapheneWorkspaceLocationEntry)
 
     class Meta:
         name = "Workspace"
 
+    def resolve_id(self, _graphene_info: ResolveInfo):
+        return "Workspace"
+
 
 class GrapheneLocationStateChangeEvent(graphene.ObjectType):
     event_type = graphene.NonNull(GrapheneLocationStateChangeEventType)
     message = graphene.NonNull(graphene.String)
     location_name = graphene.NonNull(graphene.String)
     server_id = graphene.Field(graphene.String)
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         return RunsFilter(
             run_ids=self.runIds if self.runIds else None,
             pipeline_name=self.pipelineName,
             tags=tags,
             statuses=statuses,
             snapshot_id=self.snapshotId,
             updated_after=updated_after,
-            mode=self.mode,
             created_before=created_before,
         )
 
 
 class GrapheneStepOutputHandle(graphene.InputObjectType):
     stepKey = graphene.NonNull(graphene.String)
     outputName = graphene.NonNull(graphene.String)
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         return [
             GrapheneDaemonStatus(daemon_status)
             for daemon_status in self._instance.get_daemon_statuses().values()
         ]
 
 
 class GrapheneInstance(graphene.ObjectType):
+    id = graphene.NonNull(graphene.String)
     info = graphene.Field(graphene.String)
     runLauncher = graphene.Field(GrapheneRunLauncher)
     runQueuingSupported = graphene.NonNull(graphene.Boolean)
     executablePath = graphene.NonNull(graphene.String)
     daemonHealth = graphene.NonNull(GrapheneDaemonHealth)
     hasInfo = graphene.NonNull(graphene.Boolean)
     hasCapturedLogManager = graphene.NonNull(graphene.Boolean)
@@ -101,14 +102,17 @@
     class Meta:
         name = "Instance"
 
     def __init__(self, instance):
         super().__init__()
         self._instance = check.inst_param(instance, "instance", DagsterInstance)
 
+    def resolve_id(self, _graphene_info: ResolveInfo):
+        return "Instance"
+
     def resolve_hasInfo(self, graphene_info: ResolveInfo) -> bool:
         return graphene_info.context.show_instance_config
 
     def resolve_info(self, graphene_info: ResolveInfo):
         return self._instance.info_str() if graphene_info.context.show_instance_config else None
 
     def resolve_runLauncher(self, _graphene_info: ResolveInfo):
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/instigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from dagster._core.storage.pipeline_run import DagsterRun, RunsFilter
 from dagster._core.storage.tags import REPOSITORY_LABEL_TAG, TagType, get_tag_type
 from dagster._core.workspace.permissions import Permissions
 from dagster._seven.compat.pendulum import to_timezone
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.yaml_utils import dump_run_config_yaml
 
+from dagster_graphql.schema.asset_key import GrapheneAssetKey
+
 from ..implementation.fetch_instigators import get_tick_log_events
 from ..implementation.fetch_schedules import get_schedule_next_tick
 from ..implementation.fetch_sensors import get_sensor_next_tick
 from ..implementation.loader import RepositoryScopedBatchLoader
 from ..implementation.utils import UserFacingGraphQLError
 from .errors import (
     GrapheneError,
@@ -304,14 +306,17 @@
         return [GrapheneRunRequest(run_request) for run_request in self._run_requests]
 
 
 class GrapheneRunRequest(graphene.ObjectType):
     runKey = graphene.String()
     tags = non_null_list(GraphenePipelineTag)
     runConfigYaml = graphene.NonNull(graphene.String)
+    assetSelection = graphene.List(graphene.NonNull(GrapheneAssetKey))
+
+    _run_request: RunRequest
 
     class Meta:
         name = "RunRequest"
 
     def __init__(self, run_request):
         super().__init__(runKey=run_request.run_key)
         self._run_request = check.inst_param(run_request, "run_request", RunRequest)
@@ -322,14 +327,22 @@
             for key, value in self._run_request.tags.items()
             if get_tag_type(key) != TagType.HIDDEN
         ]
 
     def resolve_runConfigYaml(self, _graphene_info: ResolveInfo):
         return dump_run_config_yaml(self._run_request.run_config)
 
+    def resolve_assetSelection(self, _graphene_info: ResolveInfo):
+        if self._run_request.asset_selection:
+            return [
+                GrapheneAssetKey(path=asset_key.path)
+                for asset_key in self._run_request.asset_selection
+            ]
+        return None
+
 
 class GrapheneDryRunInstigationTicks(graphene.ObjectType):
     results = non_null_list(GrapheneDryRunInstigationTick)
     cursor = graphene.NonNull(graphene.Float)
 
     class Meta:
         name = "DryRunInstigationTicks"
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import datetime
 from typing import List, Optional, Sequence
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.time_window_partitions import PartitionRangeStatus
 from dagster._core.events import DagsterEventType
 from dagster._core.host_representation.external import ExternalExecutionPlan, ExternalPipeline
-from dagster._core.host_representation.external_data import ExternalPresetData
+from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME, ExternalPresetData
 from dagster._core.storage.pipeline_run import (
     DagsterRunStatus,
     PipelineRunStatsSnapshot,
     RunRecord,
     RunsFilter,
 )
 from dagster._core.storage.tags import REPOSITORY_LABEL_TAG, TagType, get_tag_type
@@ -372,15 +373,15 @@
 
     def __init__(self, record: RunRecord):
         check.inst_param(record, "record", RunRecord)
         pipeline_run = record.dagster_run
         super().__init__(
             runId=pipeline_run.run_id,
             status=pipeline_run.status.value,
-            mode=pipeline_run.mode,
+            mode=DEFAULT_MODE_NAME,
         )
         self._pipeline_run = pipeline_run
         self._run_record = record
         self._run_stats: Optional[PipelineRunStatsSnapshot] = None
 
     def _get_permission_value(self, permission: Permissions, graphene_info: ResolveInfo) -> bool:
         location_name = (
@@ -569,15 +570,16 @@
             if self._run_stats is None or self._run_stats.end_time is None:
                 self._run_stats = graphene_info.context.instance.get_run_stats(self.runId)
             return self._run_stats.end_time
         return run_record.end_time
 
     def resolve_updateTime(self, graphene_info: ResolveInfo):
         run_record = self._get_run_record(graphene_info.context.instance)
-        return datetime_as_float(run_record.update_timestamp)
+        updated = run_record.update_timestamp.timestamp()
+        return datetime_as_float(datetime.datetime.utcfromtimestamp(updated))
 
 
 class GrapheneIPipelineSnapshotMixin:
     # Mixin this class to implement IPipelineSnapshot
     #
     # Graphene has some strange properties that make it so that you cannot
     # implement ABCs nor use properties in an overridable way. So the way
@@ -865,15 +867,15 @@
     def resolve_presets(self, _graphene_info: ResolveInfo):
         return [
             GraphenePipelinePreset(preset, self._external_pipeline.name)
             for preset in sorted(self._external_pipeline.active_presets, key=lambda item: item.name)
         ]
 
     def resolve_isJob(self, _graphene_info: ResolveInfo):
-        return self._external_pipeline.is_job
+        return True
 
     def resolve_isAssetJob(self, graphene_info: ResolveInfo):
         handle = self._external_pipeline.repository_handle
         location = graphene_info.context.get_code_location(handle.location_name)
         repository = location.get_repository(handle.repository_name)
         return bool(repository.get_external_asset_nodes(self._external_pipeline.name))
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/roots/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,58 +702,60 @@
         mode: str,
         runConfigData: Optional[Any] = None,  # custom scalar (GrapheneRunConfigData)
     ):
         return validate_pipeline_config(
             graphene_info,
             pipeline_selector_from_graphql(pipeline),
             parse_run_config_input(runConfigData or {}, raise_on_error=False),
-            mode,
         )
 
     def resolve_executionPlanOrError(
         self,
         graphene_info: ResolveInfo,
         pipeline: GraphenePipelineSelector,
         mode: str,
         runConfigData: Optional[Any] = None,  # custom scalar (GrapheneRunConfigData)
     ):
         return get_execution_plan(
             graphene_info,
             pipeline_selector_from_graphql(pipeline),
             parse_run_config_input(runConfigData or {}, raise_on_error=True),  # type: ignore  # (possible str)
-            mode,
         )
 
     def resolve_runConfigSchemaOrError(
         self,
         graphene_info: ResolveInfo,
         selector: GraphenePipelineSelector,
         mode: Optional[str] = None,
     ):
         return resolve_run_config_schema_or_error(
-            graphene_info,
-            pipeline_selector_from_graphql(selector),
-            mode,
+            graphene_info, pipeline_selector_from_graphql(selector), mode
         )
 
     def resolve_instance(self, graphene_info: ResolveInfo):
         return GrapheneInstance(graphene_info.context.instance)
 
     def resolve_assetNodes(
         self,
         graphene_info: ResolveInfo,
         loadMaterializations: bool,
         group: Optional[GrapheneAssetGroupSelector] = None,
         pipeline: Optional[GraphenePipelineSelector] = None,
         assetKeys: Optional[Sequence[GrapheneAssetKeyInput]] = None,
     ) -> Sequence[GrapheneAssetNode]:
-        resolved_asset_keys = set(
-            AssetKey.from_graphql_input(asset_key_input) for asset_key_input in assetKeys or []
-        )
-        use_all_asset_keys = len(resolved_asset_keys) == 0
+        if assetKeys == []:
+            return []
+        elif not assetKeys:
+            use_all_asset_keys = True
+            resolved_asset_keys = None
+        else:
+            use_all_asset_keys = False
+            resolved_asset_keys = set(
+                AssetKey.from_graphql_input(asset_key_input) for asset_key_input in assetKeys or []
+            )
 
         repo = None
 
         dynamic_partitions_loader = CachingDynamicPartitionsLoader(graphene_info.context.instance)
         if group is not None:
             group_name = group.groupName
             repo_sel = RepositorySelector.from_graphql_input(group)
@@ -794,15 +796,17 @@
                 else []
             )
         else:
             results = get_asset_nodes(graphene_info)
 
         # Filter down to requested asset keys
         results = [
-            node for node in results if use_all_asset_keys or node.assetKey in resolved_asset_keys
+            node
+            for node in results
+            if use_all_asset_keys or node.assetKey in check.not_none(resolved_asset_keys)
         ]
 
         if not results:
             return []
 
         materialization_loader = BatchMaterializationLoader(
             instance=graphene_info.context.instance,
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.2/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.2/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.1/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.2/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.1
+Version: 1.3.2
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.1/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.2/dagster_graphql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 dagster_graphql/implementation/execution/backfill.py
 dagster_graphql/implementation/execution/dynamic_partitions.py
 dagster_graphql/implementation/execution/launch_execution.py
 dagster_graphql/implementation/execution/run_lifecycle.py
 dagster_graphql/schema/__init__.py
 dagster_graphql/schema/asset_graph.py
 dagster_graphql/schema/asset_key.py
+dagster_graphql/schema/auto_materialize_policy.py
 dagster_graphql/schema/backfill.py
 dagster_graphql/schema/config_type_or_error.py
 dagster_graphql/schema/config_types.py
 dagster_graphql/schema/dagster_types.py
 dagster_graphql/schema/env_vars.py
 dagster_graphql/schema/errors.py
 dagster_graphql/schema/execution.py
```

### Comparing `dagster-graphql-1.3.1/setup.py` & `dagster-graphql-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.1",
+        "dagster==1.3.2",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

