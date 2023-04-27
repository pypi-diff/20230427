# Comparing `tmp/scalyr-agent-2-2.2.1.tar.gz` & `tmp/scalyr-agent-2-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scalyr-agent-2-2.2.1.tar", last modified: Wed Mar 29 10:25:18 2023, max compression
+gzip compressed data, was "dist/scalyr-agent-2-2.2.2.tar", last modified: Thu Apr 27 02:03:04 2023, max compression
```

## Comparing `scalyr-agent-2-2.2.1.tar` & `scalyr-agent-2-2.2.2.tar`

### file list

```diff
@@ -1,663 +1,663 @@
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      192 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/DESCRIPTION.rst
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      121 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/MANIFEST.in
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1440 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/PKG-INFO
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10490 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/README.md
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        5 2023-03-29 10:07:51.000000 scalyr-agent-2-2.2.1/VERSION
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/agent_build/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/agent_build/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    45443 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build/package_builders.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/agent_build_refactored/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1532 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    27448 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/docker_image_builders.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/agent_build_refactored/managed_packages/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/agent_build_refactored/managed_packages/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1272 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/managed_packages/build_dependencies_versions.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    83176 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/managed_packages/managed_packages_builders.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    29503 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/prepare_agent_filesystem.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1890 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6483 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/constants.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13780 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/boto3_tools.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7342 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/cleanup_ec2_objects.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      807 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/constants.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    44787 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/agent_build_refactored/tools/runner.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/benchmarks/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/benchmarks/micro/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      845 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/conftest.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3245 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/test_add_events_request_serialization.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4558 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/test_calculate_hash_digest.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8185 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/test_compression_algorithms.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6774 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/test_date_parsing.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5583 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/test_event_serialization.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5291 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/test_json_serialization.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4537 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/benchmarks/micro/test_syslog_parsing.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2713 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/time_utils.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3189 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/benchmarks/micro/utils.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/pylint_plugins/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/pylint_plugins/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8386 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/pylint_plugins/bundled_imports_checker.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5973 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/pylint_plugins/py2exe_checker.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4008 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/pylint_plugins/windows_monitors_import_checker.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      293 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/pyproject.toml
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        5 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/VERSION
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4629 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10972 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/__scalyr__.py
--rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)   109170 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/agent_main.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    46374 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/agent_status.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3948 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/all_tests.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2360 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/build_info.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       31 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15717 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/apache_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    97208 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/docker_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10645 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/garbage_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20360 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/graphite_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    29852 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/journald_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8819 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/journald_utils.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    41648 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/kubernetes_events_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   183855 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/kubernetes_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    56392 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/kubernetes_openmetrics_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    54803 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/linux_process_metrics.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31989 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/linux_system_metrics.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    52475 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/mysql_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14821 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/nginx_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23149 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/openmetrics_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22305 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/postgres_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20830 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/redis_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8821 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/shell_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    21115 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/snmp_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4770 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/symlink_file_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    90788 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/syslog_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4610 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/test_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    27305 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/tomcat_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13682 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/url_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    51104 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/windows_event_log_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    25943 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/windows_process_metrics.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24929 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/windows_system_metrics.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7997 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/compat.py
--rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)    72241 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/config_main.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12452 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/config_util.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   188732 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/configuration.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28157 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/connection.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      227 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5121 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/checkpoints.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    71248 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/copying_manager.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    67749 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/worker.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12571 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/date_parsing_utils.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1312 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/constants.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3389 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/decorators.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1286 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/timing.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/json_lib/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2414 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/json_lib/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2071 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/json_lib/exceptions.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28693 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/json_lib/objects.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    29162 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/json_lib/parser.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1661 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/json_lib/serializer.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20484 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/line_matcher.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   177421 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/log_processing.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2014 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/log_watcher.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/metrics/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/metrics/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7411 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/metrics/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    21898 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/metrics/functions.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2257 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10313 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/annotation_config.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3267 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/auto_flushing_rotating_file.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23867 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/blocking_rate_limiter.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   115766 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/k8s.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    30552 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/server_processors.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23396 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/monitors_manager.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15750 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/platform_controller.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5754 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/platform_linux.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    55319 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/platform_posix.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/platform_tests/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/platform_tests/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4822 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/platform_tests/run_platform_test.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    36442 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/platform_windows.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24346 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/profiler.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4648 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/pytest_util.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9376 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/remote_shell.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2458 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/requests_connection.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7833 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/run_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    97149 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/scalyr_client.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    88555 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/scalyr_logging.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49790 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/scalyr_monitor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19888 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/test_base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8196 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/test_util.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       20 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/certifi/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       63 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/certifi/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       41 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/certifi/__main__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      716 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/certifi/core.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1559 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31254 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/big5freq.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1757 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/big5prober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9411 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/chardistribution.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3787 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/charsetgroupprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5110 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/charsetprober.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/cli/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        1 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/cli/__init__.py
--rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)     2738 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/cli/chardetect.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3590 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/codingstatemachine.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1134 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/compat.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1855 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/cp949prober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1661 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/enums.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3950 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/escprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10510 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/escsm.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3749 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/eucjpprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13546 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euckrfreq.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1748 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euckrprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31621 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euctwfreq.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1747 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euctwprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20715 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/gb2312freq.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1754 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/gb2312prober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13838 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/hebrewprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    25777 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/jisfreq.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19643 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/jpcntx.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12839 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langbulgarianmodel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17948 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langcyrillicmodel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12688 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langgreekmodel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11345 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langhebrewmodel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12592 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langhungarianmodel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11290 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langthaimodel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11102 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langturkishmodel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5370 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/latin1prober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3413 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/mbcharsetprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2012 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/mbcsgroupprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    25481 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/mbcssm.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5657 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/sbcharsetprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3546 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/sbcsgroupprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3774 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/sjisprober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11990 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/universaldetector.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2766 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/utf8prober.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      242 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/version.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      620 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      932 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/_common.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2678 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/easter.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/parser/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1766 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/parser/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    58796 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/parser/_parser.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13247 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/parser/isoparser.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24904 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/relativedelta.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    66557 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/rrule.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      444 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12977 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/_common.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2569 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/_factories.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    62857 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/tz.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12935 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/win.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tzwin.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1965 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/utils.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/zoneinfo/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5889 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/zoneinfo/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2392 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/zoneinfo/rebuild.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       20 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3299 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/codec.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      232 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/compat.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11390 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/core.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    32979 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/idnadata.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1749 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/intranges.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   184931 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/uts46data.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pg8000/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6925 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pg8000/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      472 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pg8000/_version.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    89513 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pg8000/core.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      102 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    33368 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/cpp.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3177 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/ctokens.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    42889 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/lex.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   135805 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/yacc.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2251 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/ygen.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      175 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/ber/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/ber/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    38266 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/ber/decoder.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16317 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/ber/encoder.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      237 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/ber/eoo.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/cer/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/cer/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1267 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/cer/decoder.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4998 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/cer/encoder.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/der/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/der/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      200 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/der/decoder.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1139 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/der/encoder.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/compat/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/compat/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      201 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/compat/binary.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      709 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/compat/octets.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3044 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/debug.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      129 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/error.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10706 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2043 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/char.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7279 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/constraint.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       84 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/error.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5725 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/namedtype.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2163 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/namedval.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4499 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/tag.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2392 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/tagmap.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    44623 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/univ.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      565 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/useful.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4732 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7720 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/_auth.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      481 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/_compat.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4049 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/_socketio.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10330 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/charset.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49041 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/connections.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      853 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/CLIENT.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      680 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/COMMAND.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2228 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/CR.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12297 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/ER.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      372 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/FIELD_TYPE.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      214 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/FLAG.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      334 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/SERVER_STATUS.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12235 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/converters.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17238 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/cursors.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3716 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/err.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      658 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/optionfile.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12024 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/protocol.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      600 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3195 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4615 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_DictCursor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3766 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_SSCursor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14810 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_basic.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24462 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_connection.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2188 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_converters.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4188 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_cursor.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      670 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_err.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20100 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_issues.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3562 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_load_local.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2590 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_nextset.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      737 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_optionfile.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      170 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      243 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10192 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31423 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3035 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7688 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3193 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      360 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/times.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      180 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/util.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      173 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/borrower/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/borrower/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1307 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/borrower/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      272 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/borrower/pyfile.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      199 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      528 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/null.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49768 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/pysnmp.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    36571 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/symtable.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      498 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/compat.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20537 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/compiler.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3256 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/debug.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1498 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/error.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/lexer/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/lexer/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       86 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/lexer/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10623 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/lexer/smi.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      356 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/mibinfo.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      162 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      475 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/dialect.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      240 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/null.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    50209 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/smi.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      141 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/smiv1.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      161 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/smiv1compat.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      141 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/smiv2.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1338 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      765 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/callback.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4357 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/ftpclient.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3510 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/httpclient.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4280 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/localfile.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1588 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/url.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      125 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3121 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/pyfile.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4529 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/pypackage.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1034 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/stub.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/writer/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/writer/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      253 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/writer/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1294 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/writer/callback.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2935 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/writer/pyfile.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      178 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1146 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/cache.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1707 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/base.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4905 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1979 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1063 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp6.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3660 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dispatch.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3581 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/base.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7218 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      466 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/udp.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1277 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/udp6.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1490 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/unix.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1605 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dispatch.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       84 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/udp.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       85 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/udp6.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       85 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/unix.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      124 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asynsock/dispatch.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7367 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       70 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/error.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      328 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/sockfix.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3544 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/sockmsg.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      577 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/base.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2135 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1201 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/udp.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1181 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/unix.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2125 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dispatch.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3280 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/debug.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28826 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/config.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7816 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/engine.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2322 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/observer.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22499 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdgen.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14569 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdrsp.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10725 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/config.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2373 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/context.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2726 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/mibvar.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    18961 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntforg.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4258 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntfrcv.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9350 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/cmdgen.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6228 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/ntforg.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       35 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/error.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      256 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      299 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17478 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/cmdgen.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6456 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/ntforg.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4749 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/transport.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      302 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19477 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/cmdgen.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5452 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/ntforg.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      464 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23368 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/cmdgen.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9081 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1384 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/ntforg.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4383 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/ntforg.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4757 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/transport.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12185 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/auth.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1891 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/context.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11055 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/lcd.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1323 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/transport.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      299 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    18180 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/cmdgen.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5193 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/ntforg.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2034 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/transport.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2626 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/varbinds.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1031 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/nextid.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/acmod/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/acmod/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4755 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/acmod/rfc3415.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      675 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/acmod/void.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      213 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8174 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/v1.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5044 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/v2c.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      651 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/verdec.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1015 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/cache.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5221 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/errind.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      948 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/error.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1652 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3932 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/cache.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20926 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc2576.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    36484 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc3412.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/proxy/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/proxy/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10100 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/proxy/rfc2576.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3833 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1155.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3131 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1157.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      411 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1901.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22493 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1902.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5474 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1905.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1262 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc3411.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22071 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc3412.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1454 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      749 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/cache.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      285 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aes192.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      289 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aes256.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1273 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aesbase.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5336 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/des3.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19737 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc2576.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      101 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      595 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3300 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3298 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      644 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/noauth.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1991 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/localkey.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      564 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/base.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4371 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/des.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      656 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/nopriv.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49620 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/service.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4508 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/aes.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15638 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/builder.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2108 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/compiler.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1778 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/error.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      158 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/exval.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2866 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/indices.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9316 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/instrum.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      159 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/ASN1-ENUMERATION.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      409 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/ASN1-REFINEMENT.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      382 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/ASN1.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3366 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4335 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7871 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-USM-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      773 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1158-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7572 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1213-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16257 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10212 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7057 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-MPD-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19428 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10654 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-PROXY-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20639 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-TARGET-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3872 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    33020 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3442 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34031 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2193 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-CONF.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31290 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    43970 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-SMI.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12988 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TC.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3268 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TM.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16398 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      622 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1006 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      874 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      899 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1894 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      412 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7507 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    35285 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/rfc1902.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12703 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/view.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      902 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2927 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/_compat.py
--rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)   101789 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/client.py
--rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)    37374 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/connection.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1224 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/exceptions.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10563 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/lock.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11944 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/sentinel.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      666 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/utils.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/repoze/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      154 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/repoze/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/repoze/lru/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15032 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/repoze/lru/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28468 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/repoze/lru/tests.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4141 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      441 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/__version__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1096 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/_internal_utils.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    21344 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/adapters.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6496 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/api.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10207 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/auth.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      453 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/certs.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1782 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/compat.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    18430 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/cookies.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3161 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/exceptions.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3515 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/help.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      757 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/hooks.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34308 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/models.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      542 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/packages.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    30137 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/sessions.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4188 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/status_codes.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3005 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/structures.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    30529 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/utils.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    33045 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/six.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       47 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    32006 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/socks.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2913 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/sockshandler.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2753 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/win_inet_pton.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/tcollector/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       76 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/tcollector/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49877 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/tcollector/tcollector.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2763 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10811 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/_collections.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       63 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/_version.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20070 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/connection.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    39013 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/connectionpool.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      957 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_appengine_environ.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_securetransport/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_securetransport/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17632 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_securetransport/bindings.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13922 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_securetransport/low_level.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11010 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/appengine.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4538 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16874 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34417 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/securetransport.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7097 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/socks.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8217 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/exceptions.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8579 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/fields.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2440 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/filepost.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/backports/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/backports/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1417 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/backports/makefile.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34666 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/six.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19786 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/poolmanager.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5985 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/request.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28276 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/response.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1155 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4901 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/connection.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1605 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/proxy.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      498 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/queue.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4225 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/request.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3510 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/response.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22001 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/retry.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17165 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/ssl_.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5758 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/ssl_match_hostname.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6895 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/ssltransport.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10003 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/timeout.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14030 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/url.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5404 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/wait.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/__init__.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       82 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6859 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/compat.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4463 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/fnmatch.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8304 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/impl.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   105753 2023-03-29 10:07:44.000000 scalyr-agent-2-2.2.1/scalyr_agent/util.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent_2.egg-info/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1440 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent_2.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    27719 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent_2.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        1 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent_2.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       80 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/scalyr_agent_2.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      461 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/setup.cfg
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13691 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/setup.py
-drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 10:25:18.000000 scalyr-agent-2-2.2.1/win32/
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/win32/__init__.py
--rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1943 2023-03-29 07:23:07.000000 scalyr-agent-2-2.2.1/win32/dynamic_modules.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      192 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/DESCRIPTION.rst
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      121 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/MANIFEST.in
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1440 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/PKG-INFO
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10490 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/README.md
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        5 2023-04-27 01:47:01.000000 scalyr-agent-2-2.2.2/VERSION
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/agent_build/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    45443 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build/package_builders.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/agent_build_refactored/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1532 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    27448 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/docker_image_builders.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/agent_build_refactored/managed_packages/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/managed_packages/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1272 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/managed_packages/build_dependencies_versions.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    83176 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/managed_packages/managed_packages_builders.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    29503 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/prepare_agent_filesystem.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1890 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6483 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/constants.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13780 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/boto3_tools.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7342 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/cleanup_ec2_objects.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      807 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/constants.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    44787 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/agent_build_refactored/tools/runner.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/benchmarks/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/benchmarks/micro/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      845 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/conftest.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3245 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/test_add_events_request_serialization.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4558 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/test_calculate_hash_digest.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8185 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/test_compression_algorithms.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6774 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/test_date_parsing.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5583 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/test_event_serialization.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5291 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/test_json_serialization.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4537 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/test_syslog_parsing.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2713 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/time_utils.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3189 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/benchmarks/micro/utils.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/pylint_plugins/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/pylint_plugins/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8386 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/pylint_plugins/bundled_imports_checker.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5973 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/pylint_plugins/py2exe_checker.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4008 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/pylint_plugins/windows_monitors_import_checker.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      293 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/pyproject.toml
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        5 2023-04-27 02:03:03.000000 scalyr-agent-2-2.2.2/scalyr_agent/VERSION
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4629 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10972 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/__scalyr__.py
+-rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)   109170 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/agent_main.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    46374 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/agent_status.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3948 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/all_tests.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2360 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/build_info.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       31 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15717 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/apache_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    97208 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/docker_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10645 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/garbage_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20360 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/graphite_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    29852 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/journald_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8819 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/journald_utils.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    41648 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/kubernetes_events_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   183855 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/kubernetes_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    56392 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/kubernetes_openmetrics_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    54803 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/linux_process_metrics.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31989 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/linux_system_metrics.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    52475 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/mysql_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14821 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/nginx_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23149 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/openmetrics_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22940 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/postgres_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20830 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/redis_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8821 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/shell_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    21115 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/snmp_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4770 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/symlink_file_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    90788 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/syslog_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4610 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/test_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    27305 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/tomcat_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13682 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/url_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    51104 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/windows_event_log_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    25943 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/windows_process_metrics.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24929 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/windows_system_metrics.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7997 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/compat.py
+-rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)    72241 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/config_main.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12452 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/config_util.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   188732 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/configuration.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28157 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/connection.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      227 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5121 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/checkpoints.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    71248 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/copying_manager.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    67749 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/worker.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12571 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/date_parsing_utils.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1312 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/constants.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3389 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/decorators.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1286 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/timing.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/json_lib/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2414 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/json_lib/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2071 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/json_lib/exceptions.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28693 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/json_lib/objects.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    29162 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/json_lib/parser.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1661 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/json_lib/serializer.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20484 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/line_matcher.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   177421 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/log_processing.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2014 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/log_watcher.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/metrics/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/metrics/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7411 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/metrics/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    21898 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/metrics/functions.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2257 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10313 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/annotation_config.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3267 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/auto_flushing_rotating_file.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23867 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/blocking_rate_limiter.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   115766 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/k8s.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    30552 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/server_processors.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23396 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/monitors_manager.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15750 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/platform_controller.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5754 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/platform_linux.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    55319 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/platform_posix.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/platform_tests/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/platform_tests/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4822 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/platform_tests/run_platform_test.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    36442 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/platform_windows.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24346 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/profiler.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4648 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/pytest_util.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9376 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/remote_shell.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2458 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/requests_connection.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7833 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/run_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    97149 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/scalyr_client.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    88555 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/scalyr_logging.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49790 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/scalyr_monitor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19888 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/test_base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8196 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/test_util.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       20 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/certifi/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       63 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/certifi/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       41 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/certifi/__main__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      716 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/certifi/core.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1559 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31254 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/big5freq.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1757 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/big5prober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9411 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/chardistribution.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3787 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/charsetgroupprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5110 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/charsetprober.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/cli/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        1 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/cli/__init__.py
+-rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)     2738 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/cli/chardetect.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3590 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/codingstatemachine.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1134 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/compat.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1855 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/cp949prober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1661 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/enums.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3950 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/escprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10510 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/escsm.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3749 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/eucjpprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13546 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euckrfreq.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1748 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euckrprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31621 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euctwfreq.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1747 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euctwprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20715 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/gb2312freq.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1754 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/gb2312prober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13838 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/hebrewprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    25777 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/jisfreq.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19643 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/jpcntx.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12839 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17948 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langcyrillicmodel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12688 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langgreekmodel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11345 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langhebrewmodel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12592 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langhungarianmodel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11290 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langthaimodel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11102 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langturkishmodel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5370 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/latin1prober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3413 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/mbcharsetprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2012 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    25481 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/mbcssm.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5657 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/sbcharsetprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3546 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3774 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/sjisprober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11990 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/universaldetector.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2766 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/utf8prober.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      242 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/version.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      620 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      932 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/_common.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2678 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/easter.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/parser/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1766 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/parser/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    58796 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/parser/_parser.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13247 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/parser/isoparser.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24904 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/relativedelta.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    66557 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/rrule.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      444 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12977 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/_common.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2569 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/_factories.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    62857 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/tz.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12935 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/win.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tzwin.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1965 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/utils.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/zoneinfo/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5889 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/zoneinfo/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2392 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/zoneinfo/rebuild.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       20 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3299 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/codec.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      232 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/compat.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11390 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/core.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    32979 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/idnadata.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1749 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/intranges.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   184931 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/uts46data.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pg8000/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6925 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pg8000/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      472 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pg8000/_version.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    89513 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pg8000/core.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      102 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    33368 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/cpp.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3177 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/ctokens.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    42889 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/lex.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   135805 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/yacc.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2251 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/ygen.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      175 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/ber/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/ber/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    38266 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/ber/decoder.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16317 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/ber/encoder.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      237 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/ber/eoo.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/cer/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/cer/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1267 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/cer/decoder.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4998 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/cer/encoder.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/der/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/der/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      200 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/der/decoder.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1139 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/der/encoder.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/compat/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/compat/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      201 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/compat/binary.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      709 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/compat/octets.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3044 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/debug.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      129 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/error.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10706 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2043 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/char.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7279 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/constraint.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       84 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/error.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5725 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/namedtype.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2163 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/namedval.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4499 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/tag.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2392 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/tagmap.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    44623 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/univ.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      565 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/useful.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4732 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7720 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/_auth.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      481 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/_compat.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4049 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/_socketio.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10330 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/charset.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49041 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/connections.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      853 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/CLIENT.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      680 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/COMMAND.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2228 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/CR.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12297 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/ER.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      372 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/FIELD_TYPE.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      214 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/FLAG.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      334 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/SERVER_STATUS.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12235 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/converters.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17238 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/cursors.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3716 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/err.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      658 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/optionfile.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12024 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/protocol.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      600 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3195 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4615 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_DictCursor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3766 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_SSCursor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14810 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_basic.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    24462 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_connection.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2188 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_converters.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4188 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_cursor.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      670 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_err.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20100 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_issues.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3562 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_load_local.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2590 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_nextset.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      737 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_optionfile.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      170 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      243 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10192 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31423 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3035 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7688 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3193 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      360 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/times.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      180 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/util.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      173 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/borrower/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/borrower/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1307 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/borrower/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      272 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/borrower/pyfile.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      199 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      528 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/null.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49768 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/pysnmp.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    36571 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/symtable.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      498 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/compat.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20537 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/compiler.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3256 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/debug.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1498 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/error.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/lexer/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/lexer/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       86 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/lexer/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10623 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/lexer/smi.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      356 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/mibinfo.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      162 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      475 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/dialect.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      240 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/null.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    50209 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/smi.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      141 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/smiv1.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      161 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/smiv1compat.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      141 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/smiv2.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1338 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      765 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/callback.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4357 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/ftpclient.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3510 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/httpclient.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4280 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/localfile.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1588 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/url.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      125 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3121 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/pyfile.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4529 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/pypackage.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1034 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/stub.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/writer/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/writer/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      253 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/writer/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1294 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/writer/callback.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2935 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/writer/pyfile.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      178 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1146 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/cache.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1707 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/base.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4905 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1979 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1063 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp6.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3660 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dispatch.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3581 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/base.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7218 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      466 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/udp.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1277 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/udp6.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1490 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/unix.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1605 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dispatch.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       84 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/udp.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       85 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/udp6.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       85 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/dgram/unix.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      124 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asynsock/dispatch.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7367 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       70 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/error.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      328 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/sockfix.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3544 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/sockmsg.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      577 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/base.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2135 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1201 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/udp.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1181 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/unix.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2125 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dispatch.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3280 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/debug.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28826 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/config.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7816 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/engine.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2322 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/observer.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22499 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdgen.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14569 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdrsp.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10725 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/config.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2373 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/context.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2726 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/mibvar.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    18961 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntforg.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4258 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntfrcv.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9350 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/cmdgen.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6228 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/ntforg.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       35 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/error.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      256 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      299 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17478 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/cmdgen.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6456 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/ntforg.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4749 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/transport.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      302 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19477 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/cmdgen.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5452 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/ntforg.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      464 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    23368 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/cmdgen.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9081 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1384 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/ntforg.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4383 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/ntforg.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4757 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/transport.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12185 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/auth.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1891 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/context.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11055 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/lcd.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1323 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/transport.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      299 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    18180 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/cmdgen.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5193 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/ntforg.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2034 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/transport.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2626 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/varbinds.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1031 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/nextid.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/acmod/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/acmod/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4755 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/acmod/rfc3415.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      675 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/acmod/void.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      213 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8174 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/v1.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5044 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/v2c.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      651 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/verdec.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1015 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/cache.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5221 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/errind.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      948 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/error.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1652 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3932 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/cache.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20926 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc2576.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    36484 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc3412.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/proxy/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/proxy/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10100 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/proxy/rfc2576.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3833 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1155.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3131 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1157.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      411 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1901.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22493 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1902.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5474 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1905.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1262 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc3411.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22071 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc3412.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1454 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      749 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/cache.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      285 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aes192.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      289 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aes256.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1273 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aesbase.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5336 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/des3.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19737 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc2576.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      101 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      595 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3300 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3298 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      644 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/noauth.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1991 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/localkey.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      564 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/base.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4371 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/des.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      656 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/nopriv.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49620 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/service.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4508 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/aes.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15638 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/builder.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2108 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/compiler.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1778 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/error.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      158 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/exval.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2866 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/indices.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     9316 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/instrum.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      159 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/ASN1-ENUMERATION.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      409 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/ASN1-REFINEMENT.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      382 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/ASN1.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3366 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4335 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7871 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-USM-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      773 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1158-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7572 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1213-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16257 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10212 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7057 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-MPD-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19428 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10654 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-PROXY-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20639 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-TARGET-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3872 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    33020 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3442 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34031 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2193 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-CONF.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    31290 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    43970 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-SMI.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12988 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TC.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3268 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TM.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16398 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      622 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1006 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      874 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      899 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1894 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      412 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7507 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       59 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    35285 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/rfc1902.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    12703 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/view.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      902 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2927 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/_compat.py
+-rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)   101789 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/client.py
+-rwxrwxr-x   0 jenkins   (2000) jenkins  (58501)    37374 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/connection.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1224 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/exceptions.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10563 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/lock.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11944 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/sentinel.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      666 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/utils.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/repoze/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      154 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/repoze/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/repoze/lru/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    15032 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/repoze/lru/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28468 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/repoze/lru/tests.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4141 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      441 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/__version__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1096 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/_internal_utils.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    21344 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/adapters.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6496 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/api.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10207 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/auth.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      453 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/certs.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1782 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/compat.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    18430 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/cookies.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3161 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/exceptions.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3515 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/help.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      757 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/hooks.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34308 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/models.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      542 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/packages.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    30137 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/sessions.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4188 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/status_codes.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3005 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/structures.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    30529 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/utils.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    33045 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/six.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       47 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    32006 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/socks.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2913 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/sockshandler.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2753 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/win_inet_pton.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/tcollector/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       76 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/tcollector/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    49877 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/tcollector/tcollector.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2763 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10811 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/_collections.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       63 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/_version.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    20070 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/connection.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    39013 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/connectionpool.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      957 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_appengine_environ.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_securetransport/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17632 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13922 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    11010 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/appengine.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4538 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    16874 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34417 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/securetransport.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     7097 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/socks.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8217 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/exceptions.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8579 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/fields.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     2440 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/filepost.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/backports/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/backports/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1417 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/backports/makefile.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    34666 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/six.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    19786 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/poolmanager.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5985 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/request.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    28276 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/response.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1155 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4901 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/connection.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1605 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/proxy.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      498 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/queue.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4225 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/request.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     3510 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/response.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    22001 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/retry.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    17165 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/ssl_.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5758 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/ssl_match_hostname.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6895 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/ssltransport.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    10003 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/timeout.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    14030 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/url.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     5404 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/wait.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/__init__.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       82 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     6859 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/compat.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     4463 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/fnmatch.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     8304 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/impl.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)   105753 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/scalyr_agent/util.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent_2.egg-info/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1440 2023-04-27 02:03:03.000000 scalyr-agent-2-2.2.2/scalyr_agent_2.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    27719 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/scalyr_agent_2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        1 2023-04-27 02:03:03.000000 scalyr-agent-2-2.2.2/scalyr_agent_2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)       80 2023-04-27 02:03:03.000000 scalyr-agent-2-2.2.2/scalyr_agent_2.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)      461 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/setup.cfg
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)    13691 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/setup.py
+drwxrwxr-x   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 02:03:04.000000 scalyr-agent-2-2.2.2/win32/
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)        0 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/win32/__init__.py
+-rw-rw-r--   0 jenkins   (2000) jenkins  (58501)     1943 2023-04-27 01:46:34.000000 scalyr-agent-2-2.2.2/win32/dynamic_modules.py
```

### Comparing `scalyr-agent-2-2.2.1/PKG-INFO` & `scalyr-agent-2-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scalyr-agent-2
-Version: 2.2.1
+Version: 2.2.2
 Summary: The Python modules that implements Scalyr Agent 2
 Home-page: https://www.scalyr.com/help/scalyr-agent-2
 Author: Scalyr, Inc
 Author-email: contact@scalyr.com
 License: Apache
 Description: Scalyr Agent
         ============
```

### Comparing `scalyr-agent-2-2.2.1/README.md` & `scalyr-agent-2-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build/package_builders.py` & `scalyr-agent-2-2.2.2/agent_build/package_builders.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/__init__.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/docker_image_builders.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/docker_image_builders.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/managed_packages/build_dependencies_versions.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/managed_packages/build_dependencies_versions.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/managed_packages/managed_packages_builders.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/managed_packages/managed_packages_builders.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/prepare_agent_filesystem.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/prepare_agent_filesystem.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/tools/__init__.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/tools/constants.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/tools/constants.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/boto3_tools.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/boto3_tools.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/cleanup_ec2_objects.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/cleanup_ec2_objects.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/tools/run_in_ec2/constants.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/tools/run_in_ec2/constants.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/agent_build_refactored/tools/runner.py` & `scalyr-agent-2-2.2.2/agent_build_refactored/tools/runner.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/conftest.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/conftest.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/test_add_events_request_serialization.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/test_add_events_request_serialization.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/test_calculate_hash_digest.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/test_calculate_hash_digest.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/test_compression_algorithms.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/test_compression_algorithms.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/test_date_parsing.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/test_date_parsing.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/test_event_serialization.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/test_event_serialization.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/test_json_serialization.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/test_json_serialization.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/test_syslog_parsing.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/test_syslog_parsing.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/time_utils.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/time_utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/benchmarks/micro/utils.py` & `scalyr-agent-2-2.2.2/benchmarks/micro/utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/pylint_plugins/bundled_imports_checker.py` & `scalyr-agent-2-2.2.2/pylint_plugins/bundled_imports_checker.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/pylint_plugins/py2exe_checker.py` & `scalyr-agent-2-2.2.2/pylint_plugins/py2exe_checker.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/pylint_plugins/windows_monitors_import_checker.py` & `scalyr-agent-2-2.2.2/pylint_plugins/windows_monitors_import_checker.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/__scalyr__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/__scalyr__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/agent_main.py` & `scalyr-agent-2-2.2.2/scalyr_agent/agent_main.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/agent_status.py` & `scalyr-agent-2-2.2.2/scalyr_agent/agent_status.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/all_tests.py` & `scalyr-agent-2-2.2.2/scalyr_agent/all_tests.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/build_info.py` & `scalyr-agent-2-2.2.2/scalyr_agent/build_info.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/apache_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/apache_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/docker_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/docker_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/garbage_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/garbage_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/graphite_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/graphite_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/journald_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/journald_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/journald_utils.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/journald_utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/kubernetes_events_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/kubernetes_events_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/kubernetes_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/kubernetes_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/kubernetes_openmetrics_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/kubernetes_openmetrics_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/linux_process_metrics.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/linux_process_metrics.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/linux_system_metrics.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/linux_system_metrics.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/mysql_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/mysql_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/nginx_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/nginx_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/openmetrics_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/openmetrics_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/postgres_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/postgres_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,27 @@
     __monitor__,
     "database_port",
     "Optional (defaults to `5432`). Port for PostgreSQL.",
     convert_to=int,
 )
 define_config_option(
     __monitor__,
+    "use_ssl",
+    (
+        "Optional (defaults to False). Whether to connect to PostgreSQL over SSL. "
+        "Note: Self-signed server certs are not supported at this time. "
+        "Additionally, server cert validation and hostname checking is only "
+        "performed on Python 2.7.9 and newer. Older Python versions are vulnerable "
+        "to MitM attacks."
+    ),
+    convert_to=bool,
+    default=False,
+)
+define_config_option(
+    __monitor__,
     "database_name",
     "Name of the PostgreSQL database the Scalyr Agent will connect to.",
     convert_to=six.text_type,
 )
 define_config_option(
     __monitor__,
     "database_username",
@@ -269,14 +282,15 @@
     }
 
     def connect(self):
         try:
             conn = pg8000.connect(
                 user=self._user,
                 host=self._host,
+                ssl=self._use_ssl,
                 port=self._port,
                 database=self._database,
                 password=self._password,
             )
             self._db = conn
             self._cursor = self._db.cursor()
             self._gather_db_information()
@@ -394,26 +408,29 @@
 
     def __str__(self):
         return "DB(%r:%r, %r)" % (self._host, self._port, self._version)
 
     def __repr__(self):
         return self.__str__()
 
-    def __init__(self, host, port, database, username, password, logger=None):
+    def __init__(
+        self, host, port, database, username, password, use_ssl=False, logger=None
+    ):
         """Constructor:
 
         @param database: database we are connecting to
         @param host: database host being connected to
         @param port: database port being connected to
         @param username: username to connect with
         @param password: password to establish connection
         """
 
         self._host = host
         self._port = port
+        self._use_ssl = use_ssl
         self._database = database
         self._user = username
         self._password = password
         self._logger = logger
 
         self._db = None
         self._cursor = None
@@ -511,14 +528,15 @@
         #             file.
         #   _logger:  The logger instance to report errors/warnings/etc.
 
         # determine how we are going to connect
         database = None
         host = "localhost"
         port = 5432
+        use_ssl = self._config.get("use_ssl", False)
         username = None
         password = None
         if "database_host" in self._config:
             host = self._config["database_host"]
         if "database_port" in self._config:
             port = self._config["database_port"]
         if "database_name" in self._config:
@@ -537,14 +555,15 @@
                 "database_name, database_username and database_password must be specified in the configuration."
             )
 
         self._db = PostgreSQLDb(
             database=database,
             host=host,
             port=port,
+            use_ssl=use_ssl,
             username=username,
             password=password,
             logger=self._logger,
         )
 
     def gather_sample(self):
         """Invoked once per sample interval to gather a statistic."""
```

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/redis_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/redis_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/shell_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/shell_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/snmp_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/snmp_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/symlink_file_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/symlink_file_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/syslog_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/syslog_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/test_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/test_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/tomcat_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/tomcat_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/url_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/url_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/windows_event_log_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/windows_event_log_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/windows_process_metrics.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/windows_process_metrics.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/builtin_monitors/windows_system_metrics.py` & `scalyr-agent-2-2.2.2/scalyr_agent/builtin_monitors/windows_system_metrics.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/compat.py` & `scalyr-agent-2-2.2.2/scalyr_agent/compat.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/config_main.py` & `scalyr-agent-2-2.2.2/scalyr_agent/config_main.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/config_util.py` & `scalyr-agent-2-2.2.2/scalyr_agent/config_util.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/configuration.py` & `scalyr-agent-2-2.2.2/scalyr_agent/configuration.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/connection.py` & `scalyr-agent-2-2.2.2/scalyr_agent/connection.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/checkpoints.py` & `scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/checkpoints.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/copying_manager.py` & `scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/copying_manager.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/copying_manager/worker.py` & `scalyr-agent-2-2.2.2/scalyr_agent/copying_manager/worker.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/date_parsing_utils.py` & `scalyr-agent-2-2.2.2/scalyr_agent/date_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/constants.py` & `scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/constants.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/decorators.py` & `scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/decorators.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/instrumentation/timing.py` & `scalyr-agent-2-2.2.2/scalyr_agent/instrumentation/timing.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/json_lib/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/json_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/json_lib/exceptions.py` & `scalyr-agent-2-2.2.2/scalyr_agent/json_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/json_lib/objects.py` & `scalyr-agent-2-2.2.2/scalyr_agent/json_lib/objects.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/json_lib/parser.py` & `scalyr-agent-2-2.2.2/scalyr_agent/json_lib/parser.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/json_lib/serializer.py` & `scalyr-agent-2-2.2.2/scalyr_agent/json_lib/serializer.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/line_matcher.py` & `scalyr-agent-2-2.2.2/scalyr_agent/line_matcher.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/log_processing.py` & `scalyr-agent-2-2.2.2/scalyr_agent/log_processing.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/log_watcher.py` & `scalyr-agent-2-2.2.2/scalyr_agent/log_watcher.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/metrics/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/metrics/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/metrics/functions.py` & `scalyr-agent-2-2.2.2/scalyr_agent/metrics/functions.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/annotation_config.py` & `scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/annotation_config.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/auto_flushing_rotating_file.py` & `scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/auto_flushing_rotating_file.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/blocking_rate_limiter.py` & `scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/blocking_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/k8s.py` & `scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/k8s.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/monitor_utils/server_processors.py` & `scalyr-agent-2-2.2.2/scalyr_agent/monitor_utils/server_processors.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/monitors_manager.py` & `scalyr-agent-2-2.2.2/scalyr_agent/monitors_manager.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/platform_controller.py` & `scalyr-agent-2-2.2.2/scalyr_agent/platform_controller.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/platform_linux.py` & `scalyr-agent-2-2.2.2/scalyr_agent/platform_linux.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/platform_posix.py` & `scalyr-agent-2-2.2.2/scalyr_agent/platform_posix.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/platform_tests/run_platform_test.py` & `scalyr-agent-2-2.2.2/scalyr_agent/platform_tests/run_platform_test.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/platform_windows.py` & `scalyr-agent-2-2.2.2/scalyr_agent/platform_windows.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/profiler.py` & `scalyr-agent-2-2.2.2/scalyr_agent/profiler.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/pytest_util.py` & `scalyr-agent-2-2.2.2/scalyr_agent/pytest_util.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/remote_shell.py` & `scalyr-agent-2-2.2.2/scalyr_agent/remote_shell.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/requests_connection.py` & `scalyr-agent-2-2.2.2/scalyr_agent/requests_connection.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/run_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/run_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/scalyr_client.py` & `scalyr-agent-2-2.2.2/scalyr_agent/scalyr_client.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/scalyr_logging.py` & `scalyr-agent-2-2.2.2/scalyr_agent/scalyr_logging.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/scalyr_monitor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/scalyr_monitor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/test_base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/test_base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/test_util.py` & `scalyr-agent-2-2.2.2/scalyr_agent/test_util.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/certifi/core.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/certifi/core.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/big5freq.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/big5prober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/chardistribution.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/charsetgroupprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/charsetprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/cli/chardetect.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/codingstatemachine.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/compat.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/cp949prober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/enums.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/escprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/escsm.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/eucjpprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euckrfreq.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euckrprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euctwfreq.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/euctwprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/gb2312freq.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/gb2312prober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/hebrewprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/jisfreq.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/jpcntx.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langbulgarianmodel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langcyrillicmodel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langgreekmodel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langhebrewmodel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langhungarianmodel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langthaimodel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/langturkishmodel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/latin1prober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/mbcharsetprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/mbcsgroupprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/mbcssm.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/sbcharsetprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/sbcsgroupprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/sjisprober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/universaldetector.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/chardet/utf8prober.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/_common.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/easter.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/parser/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/parser/_parser.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/parser/isoparser.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/relativedelta.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/rrule.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/_common.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/_factories.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/tz.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/tz/win.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/utils.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/zoneinfo/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/dateutil/zoneinfo/rebuild.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/codec.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/codec.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/core.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/core.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/idnadata.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/intranges.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/idna/uts46data.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pg8000/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pg8000/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pg8000/core.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pg8000/core.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/cpp.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/ctokens.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/lex.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/lex.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/yacc.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/ply/ygen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/ber/decoder.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/ber/decoder.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/ber/encoder.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/ber/encoder.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/cer/decoder.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/cer/decoder.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/cer/encoder.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/cer/encoder.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/codec/der/encoder.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/codec/der/encoder.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/compat/octets.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/compat/octets.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/debug.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/debug.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/char.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/char.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/constraint.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/constraint.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/namedtype.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/namedtype.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/namedval.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/namedval.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/tag.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/tag.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/tagmap.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/tagmap.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/univ.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/univ.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pyasn1/type/useful.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pyasn1/type/useful.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/_auth.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/_auth.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/_socketio.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/_socketio.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/charset.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/charset.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/connections.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/connections.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/CLIENT.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/COMMAND.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/CR.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/constants/ER.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/converters.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/converters.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/cursors.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/cursors.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/err.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/err.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/optionfile.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/protocol.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/protocol.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_DictCursor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_SSCursor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_basic.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_connection.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_converters.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_cursor.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_err.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_err.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_issues.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_load_local.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_nextset.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/test_optionfile.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pymysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/borrower/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/borrower/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/null.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/null.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/pysnmp.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/pysnmp.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/codegen/symtable.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/codegen/symtable.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/compiler.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/compiler.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/debug.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/debug.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/error.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/error.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/lexer/smi.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/lexer/smi.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/parser/smi.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/parser/smi.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/callback.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/callback.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/ftpclient.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/ftpclient.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/httpclient.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/httpclient.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/localfile.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/localfile.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/reader/url.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/reader/url.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/pyfile.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/pyfile.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/pypackage.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/pypackage.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/searcher/stub.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/searcher/stub.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/writer/callback.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/writer/callback.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysmi/writer/pyfile.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysmi/writer/pyfile.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/cache.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/cache.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp6.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dgram/udp6.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncio/dispatch.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncio/dispatch.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/udp6.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/udp6.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/unix.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dgram/unix.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/asyncore/dispatch.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/asyncore/dispatch.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/sockmsg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/sockmsg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/udp.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/udp.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/unix.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dgram/unix.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/carrier/twisted/dispatch.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/carrier/twisted/dispatch.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/debug.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/debug.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/config.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/config.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/engine.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/engine.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/observer.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/observer.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdgen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdgen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdrsp.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/cmdrsp.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/config.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/config.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/context.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/context.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/mibvar.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/mibvar.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntforg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntforg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntfrcv.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/ntfrcv.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/cmdgen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/cmdgen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/ntforg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/entity/rfc3413/oneliner/ntforg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/cmdgen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/cmdgen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/ntforg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/ntforg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncio/transport.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncio/transport.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/cmdgen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/cmdgen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/ntforg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/ntforg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/cmdgen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/cmdgen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/ntforg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/compat/ntforg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/ntforg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/sync/ntforg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/asyncore/transport.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/asyncore/transport.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/auth.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/auth.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/context.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/context.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/lcd.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/lcd.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/transport.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/transport.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/cmdgen.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/cmdgen.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/ntforg.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/ntforg.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/twisted/transport.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/twisted/transport.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/hlapi/varbinds.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/hlapi/varbinds.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/nextid.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/nextid.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/acmod/rfc3415.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/acmod/rfc3415.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/acmod/void.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/acmod/void.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/v1.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/v1.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/v2c.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/v2c.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/api/verdec.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/api/verdec.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/cache.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/cache.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/errind.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/errind.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/error.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/error.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/cache.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/cache.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc2576.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc2576.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc3412.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/mpmod/rfc3412.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/proxy/rfc2576.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/proxy/rfc2576.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1155.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1155.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1157.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1157.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1902.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1902.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc1905.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc1905.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc3411.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc3411.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/rfc3412.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/rfc3412.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/cache.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/cache.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aesbase.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/aesbase.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/des3.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/eso/priv/des3.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc2576.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc2576.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/noauth.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/auth/noauth.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/localkey.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/localkey.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/base.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/base.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/des.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/des.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/nopriv.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/priv/nopriv.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/service.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3414/service.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/aes.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/proto/secmod/rfc3826/priv/aes.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/builder.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/builder.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/compiler.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/compiler.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/error.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/error.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/indices.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/indices.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/instrum.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/instrum.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-USM-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1158-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1158-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1213-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/RFC1213-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-MPD-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-MPD-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-PROXY-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-PROXY-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-TARGET-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-TARGET-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-CONF.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-CONF.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-SMI.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-SMI.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TC.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TC.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TM.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/SNMPv2-TM.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/rfc1902.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/rfc1902.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/pysnmp/smi/view.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/pysnmp/smi/view.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/_compat.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/_compat.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/client.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/client.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/connection.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/connection.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/exceptions.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/lock.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/lock.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/sentinel.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/sentinel.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/redis/utils.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/redis/utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/repoze/lru/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/repoze/lru/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/repoze/lru/tests.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/repoze/lru/tests.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/_internal_utils.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/adapters.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/api.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/api.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/auth.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/auth.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/compat.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/compat.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/cookies.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/exceptions.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/help.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/help.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/hooks.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/models.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/models.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/packages.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/packages.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/sessions.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/status_codes.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/structures.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/structures.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/requests/utils.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/requests/utils.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/six.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/six.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/socks.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/socks.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/sockshandler.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/sockshandler.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/socks/win_inet_pton.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/socks/win_inet_pton.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/tcollector/tcollector.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/tcollector/tcollector.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/_collections.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/connection.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/connectionpool.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_appengine_environ.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_securetransport/bindings.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/_securetransport/low_level.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/appengine.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/ntlmpool.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/pyopenssl.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/securetransport.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/contrib/socks.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/exceptions.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/fields.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/filepost.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/backports/makefile.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/packages/six.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/poolmanager.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/request.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/response.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/__init__.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/connection.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/proxy.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/request.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/response.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/retry.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/ssl_.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/ssl_match_hostname.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/ssltransport.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/timeout.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/url.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party/urllib3/util/wait.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/compat.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/fnmatch.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/third_party_python2/glob2/impl.py` & `scalyr-agent-2-2.2.2/scalyr_agent/third_party_python2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent/util.py` & `scalyr-agent-2-2.2.2/scalyr_agent/util.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent_2.egg-info/PKG-INFO` & `scalyr-agent-2-2.2.2/scalyr_agent_2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scalyr-agent-2
-Version: 2.2.1
+Version: 2.2.2
 Summary: The Python modules that implements Scalyr Agent 2
 Home-page: https://www.scalyr.com/help/scalyr-agent-2
 Author: Scalyr, Inc
 Author-email: contact@scalyr.com
 License: Apache
 Description: Scalyr Agent
         ============
```

### Comparing `scalyr-agent-2-2.2.1/scalyr_agent_2.egg-info/SOURCES.txt` & `scalyr-agent-2-2.2.2/scalyr_agent_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/setup.py` & `scalyr-agent-2-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `scalyr-agent-2-2.2.1/win32/dynamic_modules.py` & `scalyr-agent-2-2.2.2/win32/dynamic_modules.py`

 * *Files identical despite different names*

