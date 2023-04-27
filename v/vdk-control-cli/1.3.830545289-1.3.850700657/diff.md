# Comparing `tmp/vdk-control-cli-1.3.830545289.tar.gz` & `tmp/vdk-control-cli-1.3.850700657.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.830545289.tar", last modified: Thu Apr  6 19:53:26 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.850700657.tar", last modified: Thu Apr 27 09:55:54 2023, max compression
```

## Comparing `vdk-control-cli-1.3.830545289.tar` & `vdk-control-cli-1.3.850700657.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    11236 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    13891 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5115 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2673 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12088 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    12040 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9834 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4768 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3458 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     2915 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-04-06 19:53:07.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-06 19:53:11.000000 vdk-control-cli-1.3.830545289/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-04-06 19:53:25.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2312 2023-04-06 19:53:26.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 19:53:25.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-06 19:53:25.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 19:53:25.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-06 19:53:25.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-06 19:53:25.000000 vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-04-06 19:53:11.000000 vdk-control-cli-1.3.830545289/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    11236 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14012 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5115 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12088 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    12040 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9834 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4768 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3458 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     2915 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-04-27 09:55:38.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 09:55:42.000000 vdk-control-cli-1.3.850700657/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-27 09:55:54.000000 vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-04-27 09:55:42.000000 vdk-control-cli-1.3.850700657/version.txt
```

### Comparing `vdk-control-cli-1.3.830545289/PKG-INFO` & `vdk-control-cli-1.3.850700657/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.830545289
+Version: 1.3.850700657
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.830545289/README.md` & `vdk-control-cli-1.3.850700657/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/setup.cfg` & `vdk-control-cli-1.3.850700657/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 install_requires = 
 	click==8.*
 	click-log==0.*
 	click-spinner==0.*
 	requests>=2.25
 	setuptools>=47.0
 	pluggy
-	vdk-control-service-api==1.0.6
+	vdk-control-service-api==1.0.9
 	tabulate
 	requests_oauthlib>=1.0
 	urllib3>=1.26.5
 	vdk-control-api-auth
 python_requires = >=3.7, <4
 
 [options.packages.find]
```

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.850700657/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.850700657/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,18 +128,18 @@
         schedule = local_config.get_schedule_cron()
         if len(schedule) == 0:
             log.warning(
                 "You have provided no schedule for your Data Job. "
                 "Note that your deployed job will not be scheduled and will only run when manually executed."
             )
         contacts = DataJobContacts(
-            local_config.get_contacts_notified_on_job_failure_user_error(),
-            local_config.get_contacts_notified_on_job_failure_platform_error(),
-            local_config.get_contacts_notified_on_job_success(),
-            local_config.get_contacts_notified_on_job_deploy(),
+            notified_on_job_failure_user_error=local_config.get_contacts_notified_on_job_failure_user_error(),
+            notified_on_job_failure_platform_error=local_config.get_contacts_notified_on_job_failure_platform_error(),
+            notified_on_job_success=local_config.get_contacts_notified_on_job_success(),
+            notified_on_job_deploy=local_config.get_contacts_notified_on_job_deploy(),
         )
         job.config = DataJobConfig(
             enable_execution_notifications=local_config.get_enable_execution_notifications(),
             notification_delay_period_minutes=local_config.get_notification_delay_period_minutes(),
             contacts=contacts,
             schedule=DataJobSchedule(schedule_cron=schedule),
         )
```

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.850700657/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.830545289
+Version: 1.3.850700657
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.830545289/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.850700657/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

