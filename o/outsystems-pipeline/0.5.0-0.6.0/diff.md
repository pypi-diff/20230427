# Comparing `tmp/outsystems-pipeline-0.5.0.tar.gz` & `tmp/outsystems-pipeline-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outsystems-pipeline-0.5.0.tar", last modified: Mon Oct 10 15:31:46 2022, max compression
+gzip compressed data, was "outsystems-pipeline-0.6.0.tar", last modified: Thu Apr 27 10:20:25 2023, max compression
```

## Comparing `outsystems-pipeline-0.5.0.tar` & `outsystems-pipeline-0.6.0.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/
--rw-r--r--   0 vsts      (1001) docker     (116)    11358 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (116)      574 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/NOTICE.md
--rw-r--r--   0 vsts      (1001) docker     (116)     2242 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)     2071 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/architecture_dashboard/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/architecture_dashboard/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1166 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/architecture_dashboard/ad_base.py
--rw-r--r--   0 vsts      (1001) docker     (116)     5766 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/architecture_dashboard/ad_tech_debt.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/bdd_framework/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/bdd_framework/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1782 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/bdd_framework/bdd_base.py
--rw-r--r--   0 vsts      (1001) docker     (116)      586 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/bdd_framework/bdd_runner.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/cicd_probe/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/cicd_probe/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1135 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/cicd_probe/cicd_base.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1507 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/cicd_probe/cicd_dependencies.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1191 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/cicd_probe/cicd_scan.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/exceptions/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)       48 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/app_does_not_exist.py
--rw-r--r--   0 vsts      (1001) docker     (116)       44 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/app_version_error.py
--rw-r--r--   0 vsts      (1001) docker     (116)       51 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/deployment_not_found.py
--rw-r--r--   0 vsts      (1001) docker     (116)       52 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/environment_not_found.py
--rw-r--r--   0 vsts      (1001) docker     (116)       64 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/impossible_action_deployment.py
--rw-r--r--   0 vsts      (1001) docker     (116)       52 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/invalid_json_response.py
--rw-r--r--   0 vsts      (1001) docker     (116)       50 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/invalid_parameters.py
--rw-r--r--   0 vsts      (1001) docker     (116)       53 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/manifest_does_not_exist.py
--rw-r--r--   0 vsts      (1001) docker     (116)       48 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/no_apps_available.py
--rw-r--r--   0 vsts      (1001) docker     (116)       46 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/no_deployments.py
--rw-r--r--   0 vsts      (1001) docker     (116)       53 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/not_enough_permissions.py
--rw-r--r--   0 vsts      (1001) docker     (116)       39 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/exceptions/server_error.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/file_helpers/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/file_helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1570 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/file_helpers/file.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/lifetime/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/lifetime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)    17341 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_applications.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3074 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_base.py
--rw-r--r--   0 vsts      (1001) docker     (116)    17096 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_deployments.py
--rw-r--r--   0 vsts      (1001) docker     (116)    11819 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_environments.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/manifest/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/manifest/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2632 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/manifest/manifest_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.112403 outsystems-pipeline-0.5.0/outsystems/osp_tool/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/osp_tool/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)      291 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/osp_tool/osp_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/outsystems/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6780 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/apply_configuration_values_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6700 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/continue_deployment_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (116)    10826 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py
--rw-r--r--   0 vsts      (1001) docker     (116)    18155 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (116)    21364 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2973 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/evaluate_test_results.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3207 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/fetch_lifetime_data.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3661 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/fetch_tech_debt.py
--rw-r--r--   0 vsts      (1001) docker     (116)     7611 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/generate_unit_testing_assembly.py
--rw-r--r--   0 vsts      (1001) docker     (116)     9800 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/start_deployment_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4645 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py
--rw-r--r--   0 vsts      (1001) docker     (116)     8092 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/pipeline/tag_modified_applications.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/outsystems/properties/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/properties/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1621 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/properties/properties_base.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3042 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/properties/properties_set_value.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/outsystems/vars/
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)      607 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/ad_vars.py
--rw-r--r--   0 vsts      (1001) docker     (116)      219 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/bdd_vars.py
--rw-r--r--   0 vsts      (1001) docker     (116)      357 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/cicd_vars.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1729 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/file_vars.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3488 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/lifetime_vars.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1055 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/manifest_vars.py
--rw-r--r--   0 vsts      (1001) docker     (116)      656 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/pipeline_vars.py
--rw-r--r--   0 vsts      (1001) docker     (116)      545 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/outsystems/vars/properties_vars.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/outsystems_pipeline.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     2242 2022-10-10 15:31:46.000000 outsystems-pipeline-0.5.0/outsystems_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)     2732 2022-10-10 15:31:46.000000 outsystems-pipeline-0.5.0/outsystems_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2022-10-10 15:31:46.000000 outsystems-pipeline-0.5.0/outsystems_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)      117 2022-10-10 15:31:46.000000 outsystems-pipeline-0.5.0/outsystems_pipeline.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       11 2022-10-10 15:31:46.000000 outsystems-pipeline-0.5.0/outsystems_pipeline.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)       38 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)     3446 2022-10-10 15:31:44.000000 outsystems-pipeline-0.5.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2022-10-10 15:31:46.116402 outsystems-pipeline-0.5.0/test/
--rw-r--r--   0 vsts      (1001) docker     (116)       47 2022-10-10 15:31:41.000000 outsystems-pipeline-0.5.0/test/test_deploy_latest_tags.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.688278 outsystems-pipeline-0.6.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11358 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      574 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/NOTICE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     2224 2023-04-27 10:20:25.688278 outsystems-pipeline-0.6.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2071 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.672278 outsystems-pipeline-0.6.0/outsystems/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.676278 outsystems-pipeline-0.6.0/outsystems/architecture_dashboard/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/architecture_dashboard/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1166 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/architecture_dashboard/ad_base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5766 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/architecture_dashboard/ad_tech_debt.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.676278 outsystems-pipeline-0.6.0/outsystems/bdd_framework/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/bdd_framework/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1782 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/bdd_framework/bdd_base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/bdd_framework/bdd_runner.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.676278 outsystems-pipeline-0.6.0/outsystems/cicd_probe/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/cicd_probe/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1135 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/cicd_probe/cicd_base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1507 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/cicd_probe/cicd_dependencies.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1191 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/cicd_probe/cicd_scan.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.676278 outsystems-pipeline-0.6.0/outsystems/exceptions/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/app_does_not_exist.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/app_version_error.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/deployment_not_found.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       52 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/environment_not_found.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       64 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/impossible_action_deployment.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       52 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/invalid_json_response.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       50 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/invalid_parameters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       53 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/manifest_does_not_exist.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/no_apps_available.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/no_deployments.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       53 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/not_enough_permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       50 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/osptool_error.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       39 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/exceptions/server_error.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.676278 outsystems-pipeline-0.6.0/outsystems/file_helpers/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/file_helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1570 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/file_helpers/file.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.680278 outsystems-pipeline-0.6.0/outsystems/lifetime/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/lifetime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17341 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_applications.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3074 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17096 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_deployments.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11819 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_environments.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.680278 outsystems-pipeline-0.6.0/outsystems/manifest/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/manifest/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2632 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/manifest/manifest_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.680278 outsystems-pipeline-0.6.0/outsystems/osp_tool/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/osp_tool/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/osp_tool/osp_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.680278 outsystems-pipeline-0.6.0/outsystems/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6780 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/apply_configuration_values_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6700 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/continue_deployment_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12987 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18155 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21364 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2973 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/evaluate_test_results.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9994 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/fetch_apps_packages.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3207 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/fetch_lifetime_data.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3661 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/fetch_tech_debt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7611 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/generate_unit_testing_assembly.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9800 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/start_deployment_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7193 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8092 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/pipeline/tag_modified_apps.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.684278 outsystems-pipeline-0.6.0/outsystems/properties/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/properties/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1621 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/properties/properties_base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3042 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/properties/properties_set_value.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.688278 outsystems-pipeline-0.6.0/outsystems/vars/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      607 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/ad_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      219 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/bdd_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/cicd_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1786 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/file_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/lifetime_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1055 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/manifest_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      656 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/pipeline_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      545 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/outsystems/vars/properties_vars.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.688278 outsystems-pipeline-0.6.0/outsystems_pipeline.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2224 2023-04-27 10:20:25.000000 outsystems-pipeline-0.6.0/outsystems_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2806 2023-04-27 10:20:25.000000 outsystems-pipeline-0.6.0/outsystems_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-27 10:20:25.000000 outsystems-pipeline-0.6.0/outsystems_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-04-27 10:20:25.000000 outsystems-pipeline-0.6.0/outsystems_pipeline.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-04-27 10:20:25.000000 outsystems-pipeline-0.6.0/outsystems_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-27 10:20:25.688278 outsystems-pipeline-0.6.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3407 2023-04-27 10:20:23.000000 outsystems-pipeline-0.6.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 10:20:25.688278 outsystems-pipeline-0.6.0/test/
+-rw-r--r--   0 vsts      (1001) docker     (123)       47 2023-04-27 10:20:18.000000 outsystems-pipeline-0.6.0/test/test_deploy_latest_tags.py
```

### Comparing `outsystems-pipeline-0.5.0/LICENSE` & `outsystems-pipeline-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/NOTICE.md` & `outsystems-pipeline-0.6.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/README.md` & `outsystems-pipeline-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/architecture_dashboard/ad_base.py` & `outsystems-pipeline-0.6.0/outsystems/architecture_dashboard/ad_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/architecture_dashboard/ad_tech_debt.py` & `outsystems-pipeline-0.6.0/outsystems/architecture_dashboard/ad_tech_debt.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/bdd_framework/bdd_base.py` & `outsystems-pipeline-0.6.0/outsystems/bdd_framework/bdd_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/bdd_framework/bdd_runner.py` & `outsystems-pipeline-0.6.0/outsystems/bdd_framework/bdd_runner.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/cicd_probe/cicd_base.py` & `outsystems-pipeline-0.6.0/outsystems/cicd_probe/cicd_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/cicd_probe/cicd_dependencies.py` & `outsystems-pipeline-0.6.0/outsystems/cicd_probe/cicd_dependencies.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/cicd_probe/cicd_scan.py` & `outsystems-pipeline-0.6.0/outsystems/cicd_probe/cicd_scan.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/file_helpers/file.py` & `outsystems-pipeline-0.6.0/outsystems/file_helpers/file.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_applications.py` & `outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_applications.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_base.py` & `outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_deployments.py` & `outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_deployments.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/lifetime/lifetime_environments.py` & `outsystems-pipeline-0.6.0/outsystems/lifetime/lifetime_environments.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/manifest/manifest_base.py` & `outsystems-pipeline-0.6.0/outsystems/manifest/manifest_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/apply_configuration_values_to_target_env.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/apply_configuration_values_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/continue_deployment_to_target_env.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/continue_deployment_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,26 +18,32 @@
 from outsystems.vars.cicd_vars import PROBE_HTTP_PROTO, PROBE_API_ENDPOINT, PROBE_API_VERSION
 # Functions
 from outsystems.lifetime.lifetime_environments import get_environment_key
 from outsystems.lifetime.lifetime_applications import export_app_oap
 from outsystems.file_helpers.file import load_data
 from outsystems.lifetime.lifetime_base import build_lt_endpoint
 from outsystems.cicd_probe.cicd_base import build_probe_endpoint
-from outsystems.osp_tool.osp_base import deploy_app_oap
+from outsystems.osp_tool.osp_base import call_osptool
 from outsystems.cicd_probe.cicd_dependencies import get_app_dependencies, sort_app_dependencies
-from outsystems.pipeline.deploy_latest_tags_to_target_env import generate_deployment_based_on_manifest, generate_regular_deployment
+from outsystems.pipeline.deploy_latest_tags_to_target_env import generate_deployment_based_on_manifest as generate_deployment_based_on_deploy_manifest, \
+    generate_regular_deployment
+from outsystems.pipeline.deploy_tags_to_target_env_with_manifest import generate_deployment_based_on_manifest as generate_deployment_based_on_trigger_manifest
 # Exceptions
 from outsystems.exceptions.invalid_parameters import InvalidParametersError
 
 
 # ############################################################# SCRIPT ##############################################################
-def generate_oap_list(app_data_list: list):
+def generate_oap_list(app_data_list: list, friendly_package_names: bool):
     app_oap_list = []
+    filename = ""
     for app in app_data_list:
-        filename = "{}{}".format(app["VersionKey"], APPLICATION_OAP_FILE)
+        if friendly_package_names:
+            filename = "{}_v{}{}".format(app["Name"].replace(" ", "_"), app["Version"].replace(".", "_"), APPLICATION_OAP_FILE)
+        else:
+            filename = "{}{}".format(app["VersionKey"], APPLICATION_OAP_FILE)
         app_oap_list.append({"app_name": app["Name"], "app_version": app["Version"], "app_key": app["Key"], "version_key": app["VersionKey"], "filename": filename})
     return app_oap_list
 
 
 def export_apps_oap(artifact_dir: str, lt_endpoint: str, lt_token: str, env_key: str, app_oap_list: list):
     print("Application Scope:", flush=True)
     for app in app_oap_list:
@@ -58,18 +64,18 @@
                 final_list.append(app_oap)
     return final_list
 
 
 def deploy_apps_oap(artifact_dir: str, dest_env: str, osp_tool_path: str, credentials: str, app_oap_list: list):
     for app in app_oap_list:
         oap_file_path = os.path.join(artifact_dir, APPLICATION_OAP_FOLDER, app["filename"])
-        deploy_app_oap(osp_tool_path, oap_file_path, dest_env, credentials)
+        call_osptool(osp_tool_path, oap_file_path, dest_env, credentials)
 
 
-def main(artifact_dir: str, lt_http_proto: str, lt_url: str, lt_api_endpoint: str, lt_api_version: int, lt_token: str, source_env: str, dest_env: str, apps: list, dep_manifest: list, dep_note: str, osp_tool_path: str, credentials: str, cicd_http_proto: str, cicd_url: str, cicd_api_endpoint: str, cicd_version: str):
+def main(artifact_dir: str, lt_http_proto: str, lt_url: str, lt_api_endpoint: str, lt_api_version: int, lt_token: str, source_env: str, dest_env: str, apps: list, dep_manifest: list, trigger_manifest: dict, include_test_apps: bool, dep_note: str, osp_tool_path: str, credentials: str, cicd_http_proto: str, cicd_url: str, cicd_api_endpoint: str, cicd_version: str, friendly_package_names: bool):
 
     app_data_list = []  # will contain the applications to deploy details from LT
 
     if lt_api_version == 1:  # LT for OS version < 11
         raise InvalidParametersError("Air Gap deployments are not supported for Deployment API v1")
 
     # Builds the LifeTime endpoint
@@ -80,20 +86,22 @@
     # Gets the environment key for the source environment
     src_env_key = get_environment_key(artifact_dir, lt_endpoint, lt_token, source_env)
 
     # If the manifest file is being used, the app versions MUST come from that file
     # Or else you might not be deploying the same app versions that were deployed in
     # previous pipeline steps
     if dep_manifest:
-        app_data_list = generate_deployment_based_on_manifest(artifact_dir, lt_endpoint, lt_token, src_env_key, source_env, apps, dep_manifest)
+        app_data_list = generate_deployment_based_on_deploy_manifest(artifact_dir, lt_endpoint, lt_token, src_env_key, source_env, apps, dep_manifest)
+    elif trigger_manifest:
+        app_data_list = generate_deployment_based_on_trigger_manifest(artifact_dir, lt_endpoint, lt_token, src_env_key, source_env, trigger_manifest, include_test_apps, False)
     else:
         app_data_list = generate_regular_deployment(artifact_dir, lt_endpoint, lt_token, src_env_key, apps)
 
     # Export binary files
-    app_oap_list = generate_oap_list(app_data_list)
+    app_oap_list = generate_oap_list(app_data_list, friendly_package_names)
     export_apps_oap(artifact_dir, lt_endpoint, lt_token, src_env_key, app_oap_list)
 
     # Generate deployment order
     sorted_oap_list = generate_deployment_order(artifact_dir, probe_endpoint, app_oap_list)
 
     print("\nDeployment Order:\n", flush=True)
     for oap in sorted_oap_list:
@@ -113,37 +121,41 @@
     parser.add_argument("-u", "--lt_url", type=str, required=True,
                         help="URL for LifeTime environment, without the API endpoint. Example: \"https://<lifetime_host>\"")
     parser.add_argument("-t", "--lt_token", type=str, required=True,
                         help="Token for LifeTime API calls.")
     parser.add_argument("-v", "--lt_api_version", type=int, default=LIFETIME_API_VERSION,
                         help="LifeTime API version number. If version <= 10, use 1, if version >= 11, use 2. Default: 2")
     parser.add_argument("-e", "--lt_endpoint", type=str, default=LIFETIME_API_ENDPOINT,
-                        help="(optional) Used to set the API endpoint for LifeTime, without the version. Default: \"lifetimeapi/rest\"")
+                        help="(Optional) Used to set the API endpoint for LifeTime, without the version. Default: \"lifetimeapi/rest\"")
     parser.add_argument("-s", "--source_env", type=str, required=True,
                         help="Name, as displayed in LifeTime, of the source environment where the apps are.")
     parser.add_argument("-d", "--destination_env", type=str, required=True,
                         help="Name, as displayed in LifeTime, of the destination environment where you want to deploy the apps. (if in Airgap mode should be the hostname of the destination environment where you want to deploy the apps)")
     parser.add_argument("-m", "--deploy_msg", type=str, default=DEPLOYMENT_MESSAGE,
                         help="Message you want to show on the deployment plans in LifeTime. Default: \"Automated deploy using OS Pipelines\".")
-    parser.add_argument("-l", "--app_list", type=str, required=True,
+    parser.add_argument("-l", "--app_list", type=str,
                         help="Comma separated list of apps you want to deploy. Example: \"App1,App2 With Spaces,App3_With_Underscores\"")
     parser.add_argument("-f", "--manifest_file", type=str,
-                        help="(optional) Manifest file path, used to promote the same application versions throughout the pipeline execution.")
+                        help="Manifest file path (either deployment or trigger), used to promote the same application versions throughout the pipeline execution.")
+    parser.add_argument("-i", "--include_test_apps", action='store_true',
+                        help="(Optional) Flag that indicates if applications marked as \"Test Application\" in the trigger manifest are included in the Air Gap deployment.")
     parser.add_argument("-o", "--osp_tool_path", type=str, required=True,
                         help="OSP Tool file path")
     parser.add_argument("-user", "--airgap_user", type=str, required=True,
                         help="Username with privileges to deploy applications on target environment")
     parser.add_argument("-pass", "--airgap_pass", type=str, required=True,
                         help="Password of the Username with priveleges to deploy applications on target environment")
     parser.add_argument("-pu", "--cicd_probe_url", type=str, required=True,
                         help="URL of the environment where the CI/CD Probe is installed (without the API endpoint).")
     parser.add_argument("-pv", "--cicd_probe_version", type=str, default=PROBE_API_VERSION,
-                        help="(optional) CI/CD Probe API version number.")
+                        help="(Optional) CI/CD Probe API version number.")
     parser.add_argument("-pe", "--cicd_probe_endpoint", type=str, default=PROBE_API_ENDPOINT,
-                        help="(optional) Used to set the API endpoint for CI/CD Probe, without the version.")
+                        help="(Optional) Used to set the API endpoint for CI/CD Probe, without the version.")
+    parser.add_argument("-n", "--friendly_package_names", action='store_true',
+                        help="Flag that indicates if downloaded application packages should have a user-friendly name. Example: \"AppName_v1_2_1\"")
 
     args = parser.parse_args()
 
     # Parse the artifact directory
     artifact_dir = args.artifacts
     # Parse the API endpoint
     lt_api_endpoint = args.lt_endpoint
@@ -162,22 +174,35 @@
     lt_version = args.lt_api_version
     # Parse the LT Token
     lt_token = args.lt_token
     # Parse Source Environment
     source_env = args.source_env
     # Parse Destination Environment
     dest_env = args.destination_env
-    # Parse App list
-    _apps = args.app_list
-    apps = _apps.split(',')
     # Parse Manifest file if it exists
+    # Based on the file content it can be a deployment manifest (list-based) or trigger manifest (dict-based)
     if args.manifest_file:
         manifest_file = load_data("", args.manifest_file)
     else:
         manifest_file = None
+    dep_manifest = manifest_file if type(manifest_file) is list else None
+    trigger_manifest = manifest_file if type(manifest_file) is dict else None
+    # Check if either an app list or a manifest file is being provided
+    if not args.app_list and not args.manifest_file:
+        raise InvalidParametersError("either --app_list or --manifest_file must be provided as arguments")
+
+    if dep_manifest and not args.app_list:
+        raise InvalidParametersError("--app_list parameter is required for Deployment Manifest operation")
+    # Parse App list
+    apps = None
+    if args.app_list:
+        _apps = args.app_list
+        apps = _apps.split(',')
+    # Parse Include Test Apps flag
+    include_test_apps = args.include_test_apps
     # Parse Deployment Message
     dep_note = args.deploy_msg
     # Parse OSP Tool path
     osp_tool_path = args.osp_tool_path
     # Parse Credentials for OSP Tool
     credentials = args.airgap_user + " " + args.airgap_pass
     # Parse the CICD Probe API endpoint
@@ -191,10 +216,12 @@
         cicd_url = cicd_url.replace("http://", "")
     else:
         cicd_url = cicd_url.replace("https://", "")
     if cicd_url.endswith("/"):
         cicd_url = cicd_url[:-1]
     # Parse CICD Probe API Version
     cicd_version = args.cicd_probe_version
+    # Parse Friendly Package Names flag
+    friendly_package_names = args.friendly_package_names
 
     # Calls the main script
-    main(artifact_dir, lt_http_proto, lt_url, lt_api_endpoint, lt_version, lt_token, source_env, dest_env, apps, manifest_file, dep_note, osp_tool_path, credentials, cicd_http_proto, cicd_url, cicd_api_endpoint, cicd_version)
+    main(artifact_dir, lt_http_proto, lt_url, lt_api_endpoint, lt_version, lt_token, source_env, dest_env, apps, dep_manifest, trigger_manifest, include_test_apps, dep_note, osp_tool_path, credentials, cicd_http_proto, cicd_url, cicd_api_endpoint, cicd_version, friendly_package_names)
```

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/evaluate_test_results.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/evaluate_test_results.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/fetch_lifetime_data.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/fetch_lifetime_data.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/fetch_tech_debt.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/fetch_tech_debt.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/generate_unit_testing_assembly.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/generate_unit_testing_assembly.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/start_deployment_to_target_env.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/start_deployment_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Python Modules
 import sys
 import os
 import argparse
+from pkg_resources import parse_version
 
 # Workaround for Jenkins:
 # Set the path to include the outsystems module
 # Jenkins exposes the workspace directory through env.
 if "WORKSPACE" in os.environ:
     sys.path.append(os.environ['WORKSPACE'])
 else:  # Else just add the project dir
@@ -16,29 +17,52 @@
 from outsystems.vars.file_vars import ARTIFACT_FOLDER
 from outsystems.vars.lifetime_vars import LIFETIME_HTTP_PROTO, LIFETIME_API_ENDPOINT, LIFETIME_API_VERSION
 
 # Functions
 from outsystems.file_helpers.file import load_data
 from outsystems.lifetime.lifetime_environments import get_environment_key
 from outsystems.lifetime.lifetime_base import build_lt_endpoint
-from outsystems.lifetime.lifetime_applications import set_application_version
+from outsystems.lifetime.lifetime_applications import set_application_version, get_running_app_version
+# Exceptions
+from outsystems.exceptions.invalid_parameters import InvalidParametersError
 
 
 # ############################################################# SCRIPT ##############################################################
+def valid_tag_number(artifact_dir: str, lt_endpoint: str, lt_token: str, env_name: str, env_key: str, app: dict):
+    # Get the app running version on the source environment. It will only retrieve tagged applications
+    running_app = get_running_app_version(artifact_dir, lt_endpoint, lt_token, env_key, app_name=app["ApplicationName"])
 
-def main(artifact_dir: str, lt_http_proto: str, lt_url: str, lt_api_endpoint: str, lt_api_version: int, lt_token: str, dest_env: str, app_list: list, dep_manifest: list):
+    if parse_version(running_app["Version"]) < parse_version(app["VersionNumber"]):
+        return True
+
+    print("Skipping tag! Application '{}' current tag ({}) on {} is greater than or equal to the manifest data ({}). ".format(app["ApplicationName"], running_app["Version"], env_name, app["VersionNumber"]), flush=True)
+    return False
+
+
+def main(artifact_dir: str, lt_http_proto: str, lt_url: str, lt_api_endpoint: str, lt_api_version: int, lt_token: str, dest_env: str, app_list: list, dep_manifest: list, trigger_manifest: dict, include_test_apps: bool):
     # Builds the LifeTime endpoint
     lt_endpoint = build_lt_endpoint(lt_http_proto, lt_url, lt_api_endpoint, lt_api_version)
     # Get the environment keys
     dest_env_key = get_environment_key(artifact_dir, lt_endpoint, lt_token, dest_env)
 
-    for deployed_app in dep_manifest:
-        if deployed_app["ApplicationName"] in app_list:
-            set_application_version(lt_endpoint, lt_token, dest_env_key, deployed_app["ApplicationKey"], deployed_app["ChangeLog"], deployed_app["Version"], None)
-            print("{} application successuflly tagged as {} on {}".format(deployed_app["ApplicationName"], deployed_app["Version"], dest_env), flush=True)
+    # the app versions MUST come from that a file
+    # either deployment or trigger manifest file
+    if dep_manifest:
+        for deployed_app in dep_manifest:
+            if deployed_app["ApplicationName"] in app_list:
+                set_application_version(lt_endpoint, lt_token, dest_env_key, deployed_app["ApplicationKey"], deployed_app["ChangeLog"], deployed_app["Version"], None)
+                print("{} application successuflly tagged as {} on {}".format(deployed_app["ApplicationName"], deployed_app["Version"], dest_env), flush=True)
+    elif trigger_manifest:
+        for deployed_app in trigger_manifest["ApplicationVersions"]:
+            if not deployed_app["IsTestApplication"] or (deployed_app["IsTestApplication"] and include_test_apps):
+                if valid_tag_number(artifact_dir, lt_endpoint, lt_token, dest_env, dest_env_key, deployed_app):
+                    set_application_version(lt_endpoint, lt_token, dest_env_key, deployed_app["ApplicationKey"], deployed_app["ChangeLog"], deployed_app["VersionNumber"], None)
+                    print("{} application successuflly tagged as {} on {}".format(deployed_app["ApplicationName"], deployed_app["VersionNumber"], dest_env), flush=True)
+                else:
+                    continue
 
 # End of main()
 
 
 if __name__ == "__main__":
     # Argument menu / parsing
     parser = argparse.ArgumentParser()
@@ -47,21 +71,23 @@
     parser.add_argument("-u", "--lt_url", type=str, required=True,
                         help="URL for LifeTime environment, without the API endpoint. Example: \"https://<lifetime_host>\"")
     parser.add_argument("-t", "--lt_token", type=str, required=True,
                         help="Token for LifeTime API calls.")
     parser.add_argument("-v", "--lt_api_version", type=int, default=LIFETIME_API_VERSION,
                         help="LifeTime API version number. If version <= 10, use 1, if version >= 11, use 2. Default: 2")
     parser.add_argument("-e", "--lt_endpoint", type=str, default=LIFETIME_API_ENDPOINT,
-                        help="(optional) Used to set the API endpoint for LifeTime, without the version. Default: \"lifetimeapi/rest\"")
+                        help="(Optional) Used to set the API endpoint for LifeTime, without the version. Default: \"lifetimeapi/rest\"")
     parser.add_argument("-d", "--destination_env", type=str, required=True,
                         help="Name, as displayed in LifeTime, of the destination environment where you want to deploy the apps. (if in Airgap mode should be the hostname of the destination environment where you want to deploy the apps)")
-    parser.add_argument("-l", "--app_list", type=str, required=True,
-                        help="Comma separated list of apps you want to deploy. Example: \"App1,App2 With Spaces,App3_With_Underscores\"")
+    parser.add_argument("-l", "--app_list", type=str,
+                        help="(Optional) Comma separated list of apps you want to tag. Example: \"App1,App2 With Spaces,App3_With_Underscores\"")
     parser.add_argument("-f", "--manifest_file", type=str, required=True,
-                        help="Manifest file path, used if you have a split pipeline for CI and CD, where the CI pipeline will generate the deployment manifest file.")
+                        help="Manifest file path (either deployment or trigger).")
+    parser.add_argument("-i", "--include_test_apps", action='store_true',
+                        help="(Optional) Flag that indicates if applications marked as \"Test Application\" in the trigger manifest are included for tagging.")
 
     args = parser.parse_args()
 
     # Parse the artifact directory
     artifact_dir = args.artifacts
     # Parse the API endpoint
     lt_api_endpoint = args.lt_endpoint
@@ -78,15 +104,30 @@
         lt_url = lt_url[:-1]
     # Parte LT API Version
     lt_version = args.lt_api_version
     # Parse the LT Token
     lt_token = args.lt_token
     # Parse Destination Environment
     dest_env = args.destination_env
+
+    # Parse Manifest file if it exists
+    # Based on the file content it can be a deployment manifest (list-based) or trigger manifest (dict-based)
+    manifest_file = None
+    if args.manifest_file:
+        manifest_file = load_data("", args.manifest_file)
+
+    dep_manifest = manifest_file if type(manifest_file) is list else None
+    trigger_manifest = manifest_file if type(manifest_file) is dict else None
+
+    if dep_manifest and not args.app_list:
+        raise InvalidParametersError("--app_list parameter is required for Deployment Manifest operation")
+
     # Parse App list
-    _apps = args.app_list
-    apps = _apps.split(',')
-    # Parse Manifest file
-    manifest_file = load_data("", args.manifest_file)
+    apps = None
+    if args.app_list:
+        _apps = args.app_list
+        apps = _apps.split(',')
 
+    # Parse Include Test Apps flag
+    include_test_apps = args.include_test_apps
     # Calls the main script
-    main(artifact_dir, lt_http_proto, lt_url, lt_api_endpoint, lt_version, lt_token, dest_env, apps, manifest_file)
+    main(artifact_dir, lt_http_proto, lt_url, lt_api_endpoint, lt_version, lt_token, dest_env, apps, dep_manifest, trigger_manifest, include_test_apps)  # type: ignore
```

### Comparing `outsystems-pipeline-0.5.0/outsystems/pipeline/tag_modified_applications.py` & `outsystems-pipeline-0.6.0/outsystems/pipeline/tag_modified_apps.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/properties/properties_base.py` & `outsystems-pipeline-0.6.0/outsystems/properties/properties_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/properties/properties_set_value.py` & `outsystems-pipeline-0.6.0/outsystems/properties/properties_set_value.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/vars/ad_vars.py` & `outsystems-pipeline-0.6.0/outsystems/vars/ad_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/vars/file_vars.py` & `outsystems-pipeline-0.6.0/outsystems/vars/file_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,7 +50,10 @@
 # Architecture Dashboard vars
 AD_FILE_PREFIX = "TechDebt"
 AD_LEVELS_FILE = ".levels.cache"
 AD_CATEGORIES_FILE = ".categories.cache"
 AD_INFRA_FILE = ".infrastructure.cache"
 AD_APP_FILE = ".application.cache"
 AD_FOLDER = "techdebt_data"
+
+# AirGap vars
+DEPLOYMENT_ORDER_FILE = "sorted_oap.list"
```

### Comparing `outsystems-pipeline-0.5.0/outsystems/vars/lifetime_vars.py` & `outsystems-pipeline-0.6.0/outsystems/vars/lifetime_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/vars/manifest_vars.py` & `outsystems-pipeline-0.6.0/outsystems/vars/manifest_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/vars/pipeline_vars.py` & `outsystems-pipeline-0.6.0/outsystems/vars/pipeline_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems/vars/properties_vars.py` & `outsystems-pipeline-0.6.0/outsystems/vars/properties_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.5.0/outsystems_pipeline.egg-info/SOURCES.txt` & `outsystems-pipeline-0.6.0/outsystems_pipeline.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 outsystems/exceptions/impossible_action_deployment.py
 outsystems/exceptions/invalid_json_response.py
 outsystems/exceptions/invalid_parameters.py
 outsystems/exceptions/manifest_does_not_exist.py
 outsystems/exceptions/no_apps_available.py
 outsystems/exceptions/no_deployments.py
 outsystems/exceptions/not_enough_permissions.py
+outsystems/exceptions/osptool_error.py
 outsystems/exceptions/server_error.py
 outsystems/file_helpers/__init__.py
 outsystems/file_helpers/file.py
 outsystems/lifetime/__init__.py
 outsystems/lifetime/lifetime_applications.py
 outsystems/lifetime/lifetime_base.py
 outsystems/lifetime/lifetime_deployments.py
@@ -39,20 +40,21 @@
 outsystems/pipeline/__init__.py
 outsystems/pipeline/apply_configuration_values_to_target_env.py
 outsystems/pipeline/continue_deployment_to_target_env.py
 outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py
 outsystems/pipeline/deploy_latest_tags_to_target_env.py
 outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py
 outsystems/pipeline/evaluate_test_results.py
+outsystems/pipeline/fetch_apps_packages.py
 outsystems/pipeline/fetch_lifetime_data.py
 outsystems/pipeline/fetch_tech_debt.py
 outsystems/pipeline/generate_unit_testing_assembly.py
 outsystems/pipeline/start_deployment_to_target_env.py
 outsystems/pipeline/tag_apps_based_on_manifest_data.py
-outsystems/pipeline/tag_modified_applications.py
+outsystems/pipeline/tag_modified_apps.py
 outsystems/properties/__init__.py
 outsystems/properties/properties_base.py
 outsystems/properties/properties_set_value.py
 outsystems/vars/__init__.py
 outsystems/vars/ad_vars.py
 outsystems/vars/bdd_vars.py
 outsystems/vars/cicd_vars.py
```

### Comparing `outsystems-pipeline-0.5.0/setup.py` & `outsystems-pipeline-0.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 
 Visit the `project repository <https://github.com/OutSystems/outsystems-pipeline>`_ on GitHub for instructions on how to build example OutSystems CI/CD pipelines with common DevOps automation tools, as well as documentation that will help you adapt the examples to your particular scenarios.
 
 
 What's new
 ==========
 
-**Trigger Manifest Artifact**
- * New function to create and execute a deployment plan based on the app versions on the manifest given by the latest version of the Trigger Pipeline LifeTime Plugin.
- * New function to set configuration item values on a target environment based on the values found on the manifest given by the latest version of the Trigger Pipeline LifeTime Plugin.
+**Fixed Python Dependencies**
+ * Fixed xunitparser dependency that was causing issues when trying to install the package on python environments higher than v3.8
+ * Removed pytest dependency that was not needed
+
+**Air Gap Operations**
+ * Added support for Trigger Manifest artifact on tag_apps_based_on_manifest_data and deploy_apps_to_target_env_with_airgap scripts.
+ * New function to download application packages from a target environment based on the application versions found on the given trigger manifest artifact.
 
-**LifeTime Deployment Operations**
- * New function to resume the execution of a deployment plan on a target environment where 2-stage deployments are enabled.
 
 Installing and upgrading
 ========================
 
 Install or upgrade outsystems-pipeline to the latest available version as follows:
 ::
 
@@ -51,16 +53,15 @@
     'Topic :: System :: Software Distribution'
 ]
 
 REQUIREMENTS = [
     'python-dateutil==2.7.5',
     'requests==2.20.1',
     'unittest-xml-reporting==2.2.1',
-    'xunitparser==1.3.3',
-    'pytest==4.3.0',
+    'xunitparser==1.3.4',
     'toposort==1.5'
 ]
 
 PACKAGES = [
     'outsystems',
     'outsystems.architecture_dashboard',
     'outsystems.bdd_framework',
@@ -81,15 +82,15 @@
             version = version_file.read().replace('\n', '')
     else:
         # dummy version
         version = '1.0.0'
 
     setup(
         name=NAME,
-        version='0.5.0',
+        version='0.6.0',
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         keywords=' '.join(KEYWORDS),
         author=AUTHOR,
         author_email=EMAIL,
         url=URL,
         license=LICENSE,
```

