# Comparing `tmp/mosaicml-cli-0.4.0a2.tar.gz` & `tmp/mosaicml-cli-0.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.0a2.tar", last modified: Mon Apr 24 23:16:08 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.0a3.tar", last modified: Tue Apr 25 22:15:59 2023, max compression
```

## Comparing `mosaicml-cli-0.4.0a2.tar` & `mosaicml-cli-0.4.0a3.tar`

### file list

```diff
@@ -1,192 +1,194 @@
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.653933 mosaicml-cli-0.4.0a2/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-24 23:16:08.653770 mosaicml-cli-0.4.0a2/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     7173 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/README.md
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.625951 mosaicml-cli-0.4.0a2/mcli/
--rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.626533 mosaicml-cli-0.4.0a2/mcli/api/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.626996 mosaicml-cli-0.4.0a2/mcli/api/cluster/
--rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/cluster/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.627500 mosaicml-cli-0.4.0a2/mcli/api/engine/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/engine/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    24296 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/engine/engine.py
--rw-r--r--   0 anna       (501) staff       (20)     8458 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/exceptions.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.628931 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/
--rw-r--r--   0 anna       (501) staff       (20)      879 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     3311 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     1044 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     1126 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.629506 mosaicml-cli-0.4.0a2/mcli/api/mint/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/mint/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6870 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/mint/shell.py
--rw-r--r--   0 anna       (501) staff       (20)     2216 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/mint/tty.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.630251 mosaicml-cli-0.4.0a2/mcli/api/model/
--rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/model/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/model/cluster_details.py
--rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/model/inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     7814 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/model/run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.632468 mosaicml-cli-0.4.0a2/mcli/api/runs/
--rw-r--r--   0 anna       (501) staff       (20)     1199 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_create_run.py
--rw-r--r--   0 anna       (501) staff       (20)     3926 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     7971 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 anna       (501) staff       (20)    10427 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     4910 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_start_run.py
--rw-r--r--   0 anna       (501) staff       (20)     5099 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.632766 mosaicml-cli-0.4.0a2/mcli/api/schema/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/schema/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.633403 mosaicml-cli-0.4.0a2/mcli/api/secrets/
--rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-24 22:56:35.000000 mosaicml-cli-0.4.0a2/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/typing_future.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.633804 mosaicml-cli-0.4.0a2/mcli/api/users/
--rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/users/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.634105 mosaicml-cli-0.4.0a2/mcli/cli/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/__init__.py
--rwxr-xr-x   0 anna       (501) staff       (20)     6384 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/cli.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.634577 mosaicml-cli-0.4.0a2/mcli/cli/common/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/common/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 anna       (501) staff       (20)     6950 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.634865 mosaicml-cli-0.4.0a2/mcli/cli/m_connect/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.635320 mosaicml-cli-0.4.0a2/mcli/cli/m_create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_create/m_create.py
--rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.635814 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/delete.py
--rw-r--r--   0 anna       (501) staff       (20)     5600 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.636064 mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.636702 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)    10343 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.638046 mosaicml-cli-0.4.0a2/mcli/cli/m_get/
--rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/clusters.py
--rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/display.py
--rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     4506 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/m_get.py
--rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/runs.py
--rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_get/users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.638484 mosaicml-cli-0.4.0a2/mcli/cli/m_init/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_init/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4113 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init.py
--rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.639126 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 anna       (501) staff       (20)     9321 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.639456 mosaicml-cli-0.4.0a2/mcli/cli/m_log/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_log/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6803 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.639727 mosaicml-cli-0.4.0a2/mcli/cli/m_ping/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1742 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.640137 mosaicml-cli-0.4.0a2/mcli/cli/m_predict/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.640541 mosaicml-cli-0.4.0a2/mcli/cli/m_root/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_root/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.640909 mosaicml-cli-0.4.0a2/mcli/cli/m_run/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_run/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     8099 2023-04-24 23:14:14.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.642300 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.642715 mosaicml-cli-0.4.0a2/mcli/cli/m_stop/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.643326 mosaicml-cli-0.4.0a2/mcli/cli/m_util/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_util/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_util/m_util.py
--rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/cli/m_util/util.py
--rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.644768 mosaicml-cli-0.4.0a2/mcli/models/
--rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/gpu_type.py
--rw-r--r--   0 anna       (501) staff       (20)    11810 2023-04-24 23:13:07.000000 mosaicml-cli-0.4.0a2/mcli/models/inference_deployment_config.py
--rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/mcli_cluster.py
--rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/models/mcli_envvar.py
--rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/mcli_secret.py
--rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/models/run_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.645030 mosaicml-cli-0.4.0a2/mcli/objects/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/objects/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.646652 mosaicml-cli-0.4.0a2/mcli/objects/secrets/
--rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.648016 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/base.py
--rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/env_var.py
--rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/mounted.py
--rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/oci.py
--rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.648317 mosaicml-cli-0.4.0a2/mcli/proto/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/proto/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.648560 mosaicml-cli-0.4.0a2/mcli/sdk/
--rw-r--r--   0 anna       (501) staff       (20)     1068 2023-04-24 23:12:43.000000 mosaicml-cli-0.4.0a2/mcli/sdk/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.651968 mosaicml-cli-0.4.0a2/mcli/utils/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_cli.py
--rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_config.py
--rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_date.py
--rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_docker.py
--rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_epilog.py
--rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_interactive.py
--rw-r--r--   0 anna       (501) staff       (20)     4130 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_logging.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_pypi.py
--rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_rich.py
--rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_run_status.py
--rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_spinner.py
--rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_string_functions.py
--rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_types.py
--rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/mcli/utils/utils_yaml.py
--rw-r--r--   0 anna       (501) staff       (20)     3886 2023-04-24 23:14:24.000000 mosaicml-cli-0.4.0a2/mcli/version.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.652874 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     4640 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-24 23:16:08.000000 mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a2/pyproject.toml
--rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-24 23:16:08.653981 mosaicml-cli-0.4.0a2/setup.cfg
--rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/setup.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-24 23:16:08.653488 mosaicml-cli-0.4.0a2/tests/
--rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-24 23:12:41.000000 mosaicml-cli-0.4.0a2/tests/test_config.py
--rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/tests/test_simple.py
--rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a2/tests/test_upgrade.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.880574 mosaicml-cli-0.4.0a3/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-04-25 22:15:59.880238 mosaicml-cli-0.4.0a3/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7173 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/README.md
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.816949 mosaicml-cli-0.4.0a3/mcli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)       54 2022-03-04 18:07:55.000000 mosaicml-cli-0.4.0a3/mcli/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.817643 mosaicml-cli-0.4.0a3/mcli/api/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/api/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.818303 mosaicml-cli-0.4.0a3/mcli/api/cluster/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.0a3/mcli/api/cluster/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4141 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.818765 mosaicml-cli-0.4.0a3/mcli/api/engine/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/api/engine/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    24296 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/engine/engine.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10685 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/exceptions.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.820795 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      879 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3421 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3311 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6111 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1052 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1134 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.821557 mosaicml-cli-0.4.0a3/mcli/api/mint/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/api/mint/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7005 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/mint/shell.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2489 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/mint/tty.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.822601 mosaicml-cli-0.4.0a3/mcli/api/model/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5735 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/cluster_details.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2987 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7814 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.826673 mosaicml-cli-0.4.0a3/mcli/api/runs/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-04-25 21:57:35.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2750 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3926 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7971 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10427 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4910 2023-04-25 21:57:35.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5099 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3937 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.827258 mosaicml-cli-0.4.0a3/mcli/api/schema/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/api/schema/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.0a3/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.828612 mosaicml-cli-0.4.0a3/mcli/api/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2365 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2998 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3697 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.0a3/mcli/api/typing_future.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.829239 mosaicml-cli-0.4.0a3/mcli/api/users/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/api/users/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2694 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.829697 mosaicml-cli-0.4.0a3/mcli/cli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a3/mcli/cli/__init__.py
+-rwxr-xr-x   0 tylerlee   (502) staff       (20)     6384 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/cli.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.830456 mosaicml-cli-0.4.0a3/mcli/cli/common/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/cli/common/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2670 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6950 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.830808 mosaicml-cli-0.4.0a3/mcli/cli/m_connect/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1541 2023-04-21 23:37:59.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.831512 mosaicml-cli-0.4.0a3/mcli/cli/m_create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    16874 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.832204 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6098 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5600 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.832528 mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3896 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.833341 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4367 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10262 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1860 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.835576 mosaicml-cli-0.4.0a3/mcli/cli/m_get/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6226 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6452 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/display.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5467 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4506 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9517 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/users.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.836382 mosaicml-cli-0.4.0a3/mcli/cli/m_init/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4113 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    13963 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.837226 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9005 2023-04-21 14:41:49.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9321 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.837584 mosaicml-cli-0.4.0a3/mcli/cli/m_log/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6803 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.837850 mosaicml-cli-0.4.0a3/mcli/cli/m_ping/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1742 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.838142 mosaicml-cli-0.4.0a3/mcli/cli/m_predict/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.838479 mosaicml-cli-0.4.0a3/mcli/cli/m_root/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.838785 mosaicml-cli-0.4.0a3/mcli/cli/m_run/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8099 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.840460 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2973 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1802 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      881 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.840859 mosaicml-cli-0.4.0a3/mcli/cli/m_stop/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3847 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.841486 mosaicml-cli-0.4.0a3/mcli/cli/m_util/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_util/util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    12743 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.846583 mosaicml-cli-0.4.0a3/mcli/models/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/gpu_type.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    11810 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/mcli_cluster.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      563 2022-09-13 15:17:57.000000 mosaicml-cli-0.4.0a3/mcli/models/mcli_envvar.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6156 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/mcli_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    19299 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/run_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.847461 mosaicml-cli-0.4.0a3/mcli/objects/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/objects/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.853218 mosaicml-cli-0.4.0a3/mcli/objects/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.858225 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.859425 mosaicml-cli-0.4.0a3/mcli/proto/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/proto/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.860194 mosaicml-cli-0.4.0a3/mcli/sdk/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1068 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/sdk/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.871833 mosaicml-cli-0.4.0a3/mcli/utils/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a3/mcli/utils/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5306 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_cli.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_date.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10453 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_docker.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_epilog.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4130 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_logging.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6614 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_pypi.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_rich.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4307 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_run_status.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_spinner.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_types.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_yaml.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3886 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/version.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.875457 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4676 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1546 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/pyproject.toml
+-rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-04-25 22:15:59.880775 mosaicml-cli-0.4.0a3/setup.cfg
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2965 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/setup.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.879176 mosaicml-cli-0.4.0a3/tests/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a3/tests/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/tests/conftest.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5991 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/tests/test_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.0a3/tests/test_simple.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a2/PKG-INFO` & `mosaicml-cli-0.4.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a2/README.md` & `mosaicml-cli-0.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.0a3/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.0a3/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/exceptions.py` & `mosaicml-cli-0.4.0a3/mcli/api/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from __future__ import annotations
 
 import functools
 import logging
 import re
 import textwrap
 from concurrent.futures import TimeoutError as FuturesTimeoutError
-from enum import Enum
+from enum import Enum, IntEnum
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional
 
 import requests
+from websockets.exceptions import ConnectionClosedError, InvalidStatusCode
 
 from mcli.utils.utils_logging import FAIL
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_MESSAGE = 'Unknown Error'
 
@@ -141,14 +142,29 @@
         self.message = message
 
     def __str__(self) -> str:
         error_message = f'Error: {self.message}'
         return error_message
 
 
+class MintServerException(MintException):
+    """Exception type for MINT server errors
+    """
+
+
+class MintRequestException(MintException):
+    """Exception type for bad requests to MINT
+    """
+
+
+class MintConnectionException(MintException):
+    """Exception type for bad connections to MINT
+    """
+
+
 class RunConfigException(MAPIException):
     """Thrown when a run could not be created due to an incomplete FinalRunConfig
     """
     MATCH_MESSAGE = 'Bad run request'
     FIELD_PATTERN = re.compile('([A-Za-z]+) is a required field')
 
     def __init__(self, status: HTTPStatus, message: str = DEFAULT_MESSAGE, description: Optional[str] = None):
@@ -240,7 +256,61 @@
                 logger.error(f'{FAIL} Request has timed out. Please check your internet '
                              'connection or extend the timeout using [bold]MCLI_TIMEOUT[/]')
                 return 1
 
         return wrapper
 
     return decorator
+
+
+class MintError(IntEnum):
+    """Enum of known websocket errors from MINT
+    """
+    OK = 1000
+    COMPLETED = 1001
+    BAD_REQUEST = 1002
+
+
+def handle_mint_errors(func):
+    """Decorator to handle errors from the MINT API"""
+
+    @functools.wraps(func)
+    async def decorated(*args, **kwargs):
+        try:
+            return await func(*args, **kwargs)
+        except ConnectionClosedError as e:
+            mint_handle_connection_closed(e)
+        except OSError as e:
+            if "Errno 61" in str(e):  # https://bugs.python.org/issue29980
+                e = MintConnectionException('Could not reach MosaicML platform')
+            raise e
+        except InvalidStatusCode as e:
+            # This is _probably_ auth related
+            raise MintException(f'Connection to run failed with code: {e.status_code}') from e
+
+    return decorated
+
+
+def mint_handle_connection_closed(e: ConnectionClosedError):
+    """Convert connection closed errors to MintExceptions, if needed
+
+    Args:
+        e (ConnectionClosedError): A websocket connection closed error
+
+    Raises:
+        MintRequestException: Raised when the user submitted a bad request
+        MintServerException: Raised when the server encountered an error
+    """
+    if e.code == MintError.OK:
+        # 1000: ConnectionClosedOK
+        # Connection closed normally
+        pass
+    elif e.code == MintError.COMPLETED:
+        # 1000: Going away
+        # Connection closed gracefully
+        logger.info(f'Connection to run closed: {e.reason}')
+    elif e.code == MintError.BAD_REQUEST:
+        # 1002: Protocol error
+        raise MintRequestException(f'Unable to connect to run. {e.reason}') from e
+    else:
+        raise MintServerException(f'Unexpected error connecting to run. {e.reason}\n'
+                                  'Please try again later.') from e
```

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     Arguments:
         deployment: Inference deployment to ping for a status check
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
     Raises:
         HTTPError: If pinging the endpoint fails
     """
-    resp: Response = requests.get(url=deployment.public_dns + '/ping', timeout=timeout)
+    resp: Response = requests.get(url=f'https://{deployment.public_dns}/ping', timeout=timeout)
     if resp.ok:
         return resp.json()
     else:
         resp.raise_for_status()
         return {}
```

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,13 +22,13 @@
         deployment: Inference deployment to send input to
         input: Input data to run prediction on in the form of dictionary
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
     Raises:
         HTTPError: If sending the request to the endpoint fails
     """
-    resp: Response = requests.post(url=deployment.public_dns + '/infer', timeout=timeout, json=inputs)
+    resp: Response = requests.post(url=f'https://{deployment.public_dns}/infer', timeout=timeout, json=inputs)
     if resp.ok:
         return resp.json()
     else:
         resp.raise_for_status()
         return {}
```

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.0a3/mcli/api/mint/shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import shutil
 import ssl
 import sys
-from typing import Dict, Optional, cast
+from typing import Any, Dict, List, Optional, cast
 
+import backoff
 from websockets.client import WebSocketClientProtocol
 from websockets.client import connect as ws_connect
-from websockets.exceptions import ConnectionClosedError, ConnectionClosedOK, InvalidStatusCode
 
-from mcli.api.exceptions import MintException
+from mcli.api.exceptions import MintConnectionException, MintException, MintServerException, handle_mint_errors
 from mcli.api.mint import tty
 from mcli.proto.mint_pb2 import MINTMessage, TerminalSize, UserInput
 from mcli.utils.utils_logging import FAIL, WARN
 from mcli.utils.utils_message_decoding import MessageDecoder
 
 logger = logging.getLogger(__name__)
 
@@ -69,17 +69,14 @@
 
     async def _connect(self, uri: str):
         """
         Connection helper
 
         Given a uri, connects to a websocket and streams data in the terminal shell
         """
-        # setup tty and save old settings. if settings aren't reset, the terminal will likely become non-responsive
-
-        shell_tty = tty.TTY()
 
         async def read_stdin(ws: WebSocketClientProtocol):
             """Reads the stdin and write to the websocket
             """
             while True:
                 char = sys.stdin.read()
                 if char:
@@ -109,58 +106,67 @@
                 new_size = shutil.get_terminal_size()
                 if new_size != size:
                     message = MINTMessage(terminal_size=TerminalSize(width=new_size.columns, height=new_size.lines))
                     await ws.send(message.SerializeToString())
                     size = new_size
                 await asyncio.sleep(0.1)
 
+        use_logger = logger if logger.isEnabledFor(logging.DEBUG) else None
         connect_params = {
             "uri": uri,
             "extra_headers": self.header,
             # Useful for debugging. If logging is set to DEBUG level, this will log debug statements
-            "logger": logger,
+            "logger": use_logger,
             # Set the close timeout to a small value. When the server closes connection, it often
             # does not respond to the client's close request. This keeps the waiting to a minimum.
             # If we start having reasons for the client to initiate the close, we may need to modify
             # this value.
             "close_timeout": 0.25,
             # Give enough time for MINT to get a connection from the agent
-            "open_timeout": 30,
+            # "open_timeout": 10,
         }
         if uri.startswith("wss:"):
             connect_params["ssl"] = ssl.SSLContext(ssl.PROTOCOL_TLS)
 
-        try:
+        # Maintain a list of tasks so that we can cancel them on retries
+        tasks: List[asyncio.Task] = []
+
+        def cancel_all_tasks(details):
+            del details
+            for task in tasks:
+                task.cancel()
+            tasks.clear()
+
+        @backoff.on_exception(
+            backoff.expo,
+            (MintServerException, MintConnectionException),
+            max_tries=10,
+            logger=use_logger,
+            on_backoff=cancel_all_tasks,
+        )
+        @handle_mint_errors
+        async def connect_and_handle_errors(connect_params: Dict[str, Any]):
             async with ws_connect(**connect_params) as ws:
-                # Start the read and write tasks to run until the connection closes
-                consumer_task = asyncio.create_task(write_stdout(ws))
-                producer_task = asyncio.create_task(read_stdin(ws))
-                monitor_task = asyncio.create_task(monitor_terminal_size(ws))
-                done, pending = await asyncio.wait(
-                    [consumer_task, producer_task, monitor_task],
-                    return_when=asyncio.FIRST_COMPLETED,
-                )
-                # Retrieve the results from the completed task(s) in case they errored
-                await asyncio.gather(*done)
-                # Cancel any remaining tasks
-                for task in pending:
-                    task.cancel()
-
-        except ConnectionClosedOK:
-            pass
-        except ConnectionClosedError as e:
-            raise MintException("MINT Shell unexpectedly closed") from e
-        except OSError as e:
-            if "Errno 61" in str(e):  # https://bugs.python.org/issue29980
-                e = MintException(f'Could not connect to {self.endpoint}')
-            raise e
-        except InvalidStatusCode as e:
-            raise MintException(f"Failed to run mint websocket with status code {e.status_code}") from e
-        finally:
-            shell_tty.reset()
+                with tty.TTY():
+                    # Start the read and write tasks to run until the connection closes
+                    consumer_task = asyncio.create_task(write_stdout(ws))
+                    producer_task = asyncio.create_task(read_stdin(ws))
+                    monitor_task = asyncio.create_task(monitor_terminal_size(ws))
+                    tasks.extend([consumer_task, producer_task, monitor_task])
+                    done, pending = await asyncio.wait(
+                        tasks,
+                        return_when=asyncio.FIRST_COMPLETED,
+                    )
+                    # Retrieve the results from the completed task(s) in case they errored
+                    await asyncio.gather(*done)
+                    # Cancel any remaining tasks
+                    for task in pending:
+                        task.cancel()
+
+        await connect_and_handle_errors(connect_params)
 
     def connect(self, run_name: str, rank: int = 0) -> int:
         """
         Connect to a run using the MINT Shell
 
         args:
             run_name (str): Name of run to connect to
```

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.0a3/mcli/api/mint/tty.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,22 @@
         pass
 
     def reset(self):
         """Reset the TTY to the original settings
         """
         pass
 
+    def __enter__(self):
+        self.setup()
+        return self
+
+    def __exit__(self, *args):
+        del args
+        self.reset()
+
 
 if os.name != 'nt' and os.environ.get("SKIP_TTY", "false").lower() != "true":
     # termios and tty only supported for Unix versions that support Posix termios style tty I/O control
     import termios
     import tty
 
     TTY_SUPPORTED = True
@@ -40,15 +48,14 @@
 
         fd: int = 0
         old_settings = None
 
         def __init__(self):
             self.fd = sys.stdin.fileno()
             self.old_settings = termios.tcgetattr(self.fd)
-            self.setup()
 
         def setup(self, when=termios.TCSAFLUSH):
             mode = termios.tcgetattr(self.fd)
 
             # See: https://man7.org/linux/man-pages/man3/termios.3.html
             mode[tty.LFLAG] &= ~(
                 # Disable signals so they are sent through to MINT
@@ -68,7 +75,15 @@
 
             # Set the mode
             termios.tcsetattr(self.fd, when, mode)
 
         def reset(self):
             if self.old_settings:
                 termios.tcsetattr(self.fd, termios.TCSADRAIN, self.old_settings)
+
+        def __enter__(self):
+            self.setup()
+            return self
+
+        def __exit__(self, *args):
+            del args
+            self.reset()
```

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.0a3/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.0a3/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.0a3/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/model/run.py` & `mosaicml-cli-0.4.0a3/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_start_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.0a3/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.0a3/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.0a3/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.0a3/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.0a3/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/typing_future.py` & `mosaicml-cli-0.4.0a3/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.0a3/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/cli.py` & `mosaicml-cli-0.4.0a3/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.0a3/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.0a3/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
         extracted: Dict[str, Any] = {
             DescribeRunDetailColumns.NAME.value: run.config.name,
             DescribeRunDetailColumns.RUN_ID.value: run.run_uid,
             DescribeRunDetailColumns.LAST_ATTEMPT_ID.value: run.last_attempt_id,
             DescribeRunDetailColumns.CLUSTER.value: run.config.cluster,
             DescribeRunDetailColumns.IMAGE.value: run.config.image,
-            DescribeRunDetailColumns.LAST_ATTEMPT_ID.value: run.last_attempt_id,
             DescribeRunDetailColumns.PRIORITY.value: priority.lower(),
         }
 
         return DescribeRunDetailDisplayItem(**extracted)
 
 
 @dataclass
```

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.0a3/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/config.py` & `mosaicml-cli-0.4.0a3/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/models/__init__.py` & `mosaicml-cli-0.4.0a3/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.0a3/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.0a3/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.4.0a3/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.0a3/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/models/run_config.py` & `mosaicml-cli-0.4.0a3/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.0a3/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.0a3/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.0a3/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.0a3/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/mcli/version.py` & `mosaicml-cli-0.4.0a3/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,13 +111,13 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.0a2"
+__version__ = "0.4.0a3"
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -142,10 +142,12 @@
 mcli/utils/utils_yaml.py
 mosaicml_cli.egg-info/PKG-INFO
 mosaicml_cli.egg-info/SOURCES.txt
 mosaicml_cli.egg-info/dependency_links.txt
 mosaicml_cli.egg-info/entry_points.txt
 mosaicml_cli.egg-info/requires.txt
 mosaicml_cli.egg-info/top_level.txt
+tests/__init__.py
+tests/conftest.py
 tests/test_config.py
 tests/test_simple.py
 tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a2/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -8,43 +8,43 @@
 pyyaml>=5.4.1
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 
 [all]
+sphinxemoji>=0.2.0
+myst-parser>=0.16.1
+radon>=5.1.0
 pytest>=6.2.5
+pre-commit>=2.17.0
 sphinx_external_toc>=0.3.0
-pylint>=2.12.2
+sphinx-copybutton>=0.5.0
+pytest-mock>=3.7.0
+sphinx>=4.4.0
 pyright>=1.1.256
-toml>=0.10.2
-myst-parser>=0.16.1
 sphinx-design
-sphinxcontrib-applehelp>=1.0.2
-pytest-cov>=4.0.0
-sphinxcontrib-jsmath>=1.0.1
-sphinxemoji>=0.2.0
-sphinxcontrib-htmlhelp>=2.0.0
-sphinxcontrib-images>=0.9.4
 sphinx-markdown-tables>=0.0.15
-sphinxext-opengraph>=0.6.1
-pytest-mock>=3.7.0
-isort>=5.9.3
-sphinx>=4.4.0
-furo>=2022.3.4
-sphinx-rtd-theme>=1.0.0
 sphinxcontrib-serializinghtml>=1.1.5
-yapf>=0.33.0
-sphinx-panels>=0.6.0
+sphinxcontrib-jsmath>=1.0.1
 sphinxcontrib-qthelp>=1.0.3
-radon>=5.1.0
-sphinx-copybutton>=0.5.0
-pre-commit>=2.17.0
+toml>=0.10.2
+sphinx-panels>=0.6.0
+sphinxcontrib-images>=0.9.4
 sphinxcontrib-katex>=0.8.6
+isort>=5.9.3
+pytest-cov>=4.0.0
+sphinx-rtd-theme>=1.0.0
+sphinxcontrib-applehelp>=1.0.2
+sphinxcontrib-htmlhelp>=2.0.0
 sphinx-argparse>=0.3.1
+yapf>=0.33.0
+pylint>=2.12.2
+sphinxext-opengraph>=0.6.1
+furo>=2022.3.4
 sphinxcontrib-devhelp>=1.0.2
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
```

### Comparing `mosaicml-cli-0.4.0a2/pyproject.toml` & `mosaicml-cli-0.4.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/setup.py` & `mosaicml-cli-0.4.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/tests/test_config.py` & `mosaicml-cli-0.4.0a3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a2/tests/test_upgrade.py` & `mosaicml-cli-0.4.0a3/tests/test_upgrade.py`

 * *Files identical despite different names*

