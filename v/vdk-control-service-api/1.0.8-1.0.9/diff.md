# Comparing `tmp/vdk-control-service-api-1.0.8.tar.gz` & `tmp/vdk-control-service-api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-control-service-api-1.0.8.tar", last modified: Mon Apr 24 13:23:29 2023, max compression
+gzip compressed data, was "vdk-control-service-api-1.0.9.tar", last modified: Thu Apr 27 09:29:20 2023, max compression
```

## Comparing `vdk-control-service-api-1.0.8.tar` & `vdk-control-service-api-1.0.9.tar`

### file list

```diff
@@ -1,196 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20126 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6635 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.573642 vdk-control-service-api-1.0.8/taurus_datajob_api/
--rw-r--r--   0 root         (0) root         (0)     3386 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61119 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.573642 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5328 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.577642 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_info.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.py
--rw-r--r--   0 root         (0) root         (0)      384 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions.py
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.py
--rw-r--r--   0 root         (0) root         (0)      219 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_keytab.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_sources.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.577642 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      555 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)     3737 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_execution_api.py
--rw-r--r--   0 root         (0) root         (0)     3368 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_properties_api.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_service_api.py
--rw-r--r--   0 root         (0) root         (0)     3418 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_sources_api.py
--rw-r--r--   0 root         (0) root         (0)    18077 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/configuration.py
--rw-r--r--   0 root         (0) root         (0)     7117 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/model/
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6765 2023-04-24 13:23:11.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job.py
--rw-r--r--   0 root         (0) root         (0)     6849 2023-04-24 13:23:11.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_api_info.py
--rw-r--r--   0 root         (0) root         (0)     8809 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_config.py
--rw-r--r--   0 root         (0) root         (0)    11079 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_contacts.py
--rw-r--r--   0 root         (0) root         (0)    10382 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment_id.py
--rw-r--r--   0 root         (0) root         (0)    11264 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)    12532 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_logs.py
--rw-r--r--   0 root         (0) root         (0)     7013 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_request.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_mode.py
--rw-r--r--   0 root         (0) root         (0)     7116 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_page.py
--rw-r--r--   0 root         (0) root         (0)     4219 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_properties.py
--rw-r--r--   0 root         (0) root         (0)     6516 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_query_response.py
--rw-r--r--   0 root         (0) root         (0)     6534 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_query_response_with_error.py
--rw-r--r--   0 root         (0) root         (0)     6974 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_resources.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_schedule.py
--rw-r--r--   0 root         (0) root         (0)     6731 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_summary.py
--rw-r--r--   0 root         (0) root         (0)     5158 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_version.py
--rw-r--r--   0 root         (0) root         (0)     5936 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/models/
--rw-r--r--   0 root         (0) root         (0)     1856 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/
--rw-r--r--   0 root         (0) root         (0)     1937 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/
--rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9663 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/
--rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13125 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/get.py
--rw-r--r--   0 root         (0) root         (0)    16868 2023-04-24 13:23:17.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/
--rw-r--r--   0 root         (0) root         (0)      377 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-04-24 13:23:17.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/delete.py
--rw-r--r--   0 root         (0) root         (0)    10613 2023-04-24 13:23:18.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/get.py
--rw-r--r--   0 root         (0) root         (0)    15339 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/
--rw-r--r--   0 root         (0) root         (0)      401 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13798 2023-04-24 13:23:20.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/get.py
--rw-r--r--   0 root         (0) root         (0)    17659 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
--rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10729 2023-04-24 13:23:20.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    10952 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15525 2023-04-24 13:23:20.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
--rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14554 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/get.py
--rw-r--r--   0 root         (0) root         (0)    16006 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
--rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10452 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/get.py
--rw-r--r--   0 root         (0) root         (0)    13298 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/
--rw-r--r--   0 root         (0) root         (0)      399 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14185 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10765 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11021 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13907 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11209 2023-04-24 13:23:18.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12453 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/delete.py
--rw-r--r--   0 root         (0) root         (0)    11239 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/get.py
--rw-r--r--   0 root         (0) root         (0)    17624 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/
--rw-r--r--   0 root         (0) root         (0)      405 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11166 2023-04-24 13:23:18.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/put.py
--rw-r--r--   0 root         (0) root         (0)    13149 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/rest.py
--rw-r--r--   0 root         (0) root         (0)   100261 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.569642 vdk-control-service-api-1.0.8/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3149 2023-04-24 13:23:11.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job.py
--rw-r--r--   0 root         (0) root         (0)     3179 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_api_info.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_config.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_contacts.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_id.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_logs.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_request.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_mode.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_page.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_properties.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_query_response.py
--rw-r--r--   0 root         (0) root         (0)     3241 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_query_response_with_error.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_resources.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_summary.py
--rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_version.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/test/test_models/test_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_info/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_info/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_info/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_get.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/__init__.py
--rw-r--r--   0 root         (0) root         (0)      938 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_get.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      990 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_get.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10920 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:20.020834 vdk-control-service-api-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-04-27 09:29:20.020834 vdk-control-service-api-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12144 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-27 09:29:20.020834 vdk-control-service-api-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6641 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:20.008834 vdk-control-service-api-1.0.9/taurus_datajob_api/
+-rw-r--r--   0 root         (0) root         (0)     5247 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:20.012834 vdk-control-service-api-1.0.9/taurus_datajob_api/api/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63820 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api/data_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    43710 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api/data_jobs_deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)    50689 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api/data_jobs_execution_api.py
+-rw-r--r--   0 root         (0) root         (0)    18131 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api/data_jobs_properties_api.py
+-rw-r--r--   0 root         (0) root         (0)     9667 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api/data_jobs_service_api.py
+-rw-r--r--   0 root         (0) root         (0)    25739 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api/data_jobs_sources_api.py
+-rw-r--r--   0 root         (0) root         (0)    32241 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    17132 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7732 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:20.012834 vdk-control-service-api-1.0.9/taurus_datajob_api/models/
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_api_info.py
+-rw-r--r--   0 root         (0) root         (0)     6794 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_config.py
+-rw-r--r--   0 root         (0) root         (0)     5668 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     7116 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     7341 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_execution_logs.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_page.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     5085 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_query_response_with_error.py
+-rw-r--r--   0 root         (0) root         (0)     5165 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_resources.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     4900 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_version.py
+-rw-r--r--   0 root         (0) root         (0)     4504 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/models/error.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/taurus_datajob_api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:20.016834 vdk-control-service-api-1.0.9/test/
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_api_info.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_config.py
+-rw-r--r--   0 root         (0) root         (0)     4403 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     5651 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4176 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_execution_logs.py
+-rw-r--r--   0 root         (0) root         (0)     4275 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_page.py
+-rw-r--r--   0 root         (0) root         (0)     5066 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_query_response_with_error.py
+-rw-r--r--   0 root         (0) root         (0)     4244 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_resources.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     4533 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_data_job_version.py
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/test/test_data_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/test/test_data_jobs_deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     4813 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/test/test_data_jobs_execution_api.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/test/test_data_jobs_properties_api.py
+-rw-r--r--   0 root         (0) root         (0)     3550 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/test/test_data_jobs_service_api.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/test/test_data_jobs_sources_api.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-04-27 09:29:18.000000 vdk-control-service-api-1.0.9/test/test_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:29:20.020834 vdk-control-service-api-1.0.9/vdk_control_service_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/vdk_control_service_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/vdk_control_service_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/vdk_control_service_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/vdk_control_service_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-27 09:29:19.000000 vdk-control-service-api-1.0.9/vdk_control_service_api.egg-info/top_level.txt
```

### Comparing `vdk-control-service-api-1.0.8/PKG-INFO` & `vdk-control-service-api-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vdk-control-service-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Versatile Data Kit Control Service API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Versatile Data Kit Control Service API
-Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#x27;Authorization: Bearer [access-token-here]&#x27; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#39;Authorization: Bearer [access-token-here]&#39; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
```

### Comparing `vdk-control-service-api-1.0.8/setup.py` & `vdk-control-service-api-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,47 +2,48 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 from setuptools import setup, find_packages  # noqa: H301
 
-NAME = "vdk-control-service-api"
-VERSION = "1.0.8"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
-
+NAME = "vdk-control-service-api"
+VERSION = "1.0.9"
+PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
-    "certifi >= 14.5.14",
-    "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
-    "setuptools >= 21.0.0",
-    "typing_extensions ~= 4.3.0",
-    "urllib3 ~= 1.26.7",
+    "urllib3 >= 1.25.3",
+    "python-dateutil",
+    "pydantic",
+    "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Versatile Data Kit Control Service API",
     author="OpenAPI Generator community",
     author_email="team@openapitools.org",
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "Versatile Data Kit Control Service API"],
-    python_requires=">=3.7",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Apache 2.0",
+    long_description_content_type='text/markdown',
     long_description="""\
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#x27;Authorization: Bearer [access-token-here]&#x27; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#39;Authorization: Bearer [access-token-here]&#39; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
     """
 )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/__init__.py` & `vdk-control-service-api-1.0.9/test/test_data_jobs_service_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 # coding: utf-8
 
-# flake8: noqa
-
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-__version__ = "1.0.8"
 
-# import ApiClient
-from taurus_datajob_api.api_client import ApiClient
+import unittest
+
+import taurus_datajob_api
+from taurus_datajob_api.api.data_jobs_service_api import DataJobsServiceApi  # noqa: E501
+from taurus_datajob_api.rest import ApiException
+
+
+class TestDataJobsServiceApi(unittest.TestCase):
+    """DataJobsServiceApi unit test stubs"""
+
+    def setUp(self):
+        self.api = taurus_datajob_api.api.data_jobs_service_api.DataJobsServiceApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_info(self):
+        """Test case for info
+
+        Get API and Data Jobs Service info, list of supported python versions  # noqa: E501
+        """
+        pass
 
-# import Configuration
-from taurus_datajob_api.configuration import Configuration
 
-# import exceptions
-from taurus_datajob_api.exceptions import OpenApiException
-from taurus_datajob_api.exceptions import ApiAttributeError
-from taurus_datajob_api.exceptions import ApiTypeError
-from taurus_datajob_api.exceptions import ApiValueError
-from taurus_datajob_api.exceptions import ApiKeyError
-from taurus_datajob_api.exceptions import ApiException
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_api.py` & `vdk-control-service-api-1.0.9/test/test_data_jobs_properties_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,34 +2,46 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs.post import DataJobCreate
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name.delete import DataJobDelete
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_keytab.get import DataJobKeytabDownload
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name.get import DataJobRead
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_team_new_team.put import DataJobTeamUpdate
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name.put import DataJobUpdate
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs.get import JobsQuery
-
-
-class DataJobsApi(
-    DataJobCreate,
-    DataJobDelete,
-    DataJobKeytabDownload,
-    DataJobRead,
-    DataJobTeamUpdate,
-    DataJobUpdate,
-    JobsQuery,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
-    """
-    pass
+import unittest
+
+import taurus_datajob_api
+from taurus_datajob_api.api.data_jobs_properties_api import DataJobsPropertiesApi  # noqa: E501
+from taurus_datajob_api.rest import ApiException
+
+
+class TestDataJobsPropertiesApi(unittest.TestCase):
+    """DataJobsPropertiesApi unit test stubs"""
+
+    def setUp(self):
+        self.api = taurus_datajob_api.api.data_jobs_properties_api.DataJobsPropertiesApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_data_job_properties_read(self):
+        """Test case for data_job_properties_read
+
+        Get Data Job properties.  # noqa: E501
+        """
+        pass
+
+    def test_data_job_properties_update(self):
+        """Test case for data_job_properties_update
+
+        Update Data Job properties.  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py` & `vdk-control-service-api-1.0.9/test/test_data_job_mode.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.delete import DeploymentDelete
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments.get import DeploymentList
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.patch import DeploymentPatch
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.get import DeploymentRead
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments.post import DeploymentUpdate
-
-
-class DataJobsDeploymentApi(
-    DeploymentDelete,
-    DeploymentList,
-    DeploymentPatch,
-    DeploymentRead,
-    DeploymentUpdate,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
-    """
-    pass
+import unittest
+import datetime
+
+import taurus_datajob_api
+from taurus_datajob_api.models.data_job_mode import DataJobMode  # noqa: E501
+from taurus_datajob_api.rest import ApiException
+
+class TestDataJobMode(unittest.TestCase):
+    """DataJobMode unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testDataJobMode(self):
+        """Test DataJobMode"""
+        # inst = DataJobMode()
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_execution_api.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # coding: utf-8
 
+# flake8: noqa
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.get import DataJobDeploymentExecutionList
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.delete import DataJobExecutionCancel
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions.get import DataJobExecutionList
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.get import DataJobExecutionRead
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.post import DataJobExecutionStart
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs.get import DataJobLogsDownload
-
-
-class DataJobsExecutionApi(
-    DataJobDeploymentExecutionList,
-    DataJobExecutionCancel,
-    DataJobExecutionList,
-    DataJobExecutionRead,
-    DataJobExecutionStart,
-    DataJobLogsDownload,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
-    """
-    pass
+# import models into model package
+from taurus_datajob_api.models.data_job import DataJob
+from taurus_datajob_api.models.data_job_api_info import DataJobApiInfo
+from taurus_datajob_api.models.data_job_config import DataJobConfig
+from taurus_datajob_api.models.data_job_contacts import DataJobContacts
+from taurus_datajob_api.models.data_job_deployment import DataJobDeployment
+from taurus_datajob_api.models.data_job_deployment_status import DataJobDeploymentStatus
+from taurus_datajob_api.models.data_job_execution import DataJobExecution
+from taurus_datajob_api.models.data_job_execution_logs import DataJobExecutionLogs
+from taurus_datajob_api.models.data_job_execution_request import DataJobExecutionRequest
+from taurus_datajob_api.models.data_job_mode import DataJobMode
+from taurus_datajob_api.models.data_job_page import DataJobPage
+from taurus_datajob_api.models.data_job_query_response import DataJobQueryResponse
+from taurus_datajob_api.models.data_job_query_response_with_error import DataJobQueryResponseWithError
+from taurus_datajob_api.models.data_job_resources import DataJobResources
+from taurus_datajob_api.models.data_job_schedule import DataJobSchedule
+from taurus_datajob_api.models.data_job_summary import DataJobSummary
+from taurus_datajob_api.models.data_job_version import DataJobVersion
+from taurus_datajob_api.models.error import Error
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_properties_api.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,33 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties.get import DataJobPropertiesRead
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties.put import DataJobPropertiesUpdate
 
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+from aenum import Enum, no_arg
 
-class DataJobsPropertiesApi(
-    DataJobPropertiesRead,
-    DataJobPropertiesUpdate,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+
+
+
+class DataJobMode(str, Enum):
     """
-    pass
+    The execution mode that the data job is deployed in. Data Jobs used for development or testing purposes are marked as testing. This is used by Operations team on platform rollout and infrastructure changes adoption. For example, rollout and validation of testing jobs first, then proceeding with release data jobs. Also, testing and release jobs may have different limits and SLA targets.
+    """
+
+    """
+    allowed enum values
+    """
+    TESTING = 'testing'
+    RELEASE = 'release'
+
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_service_api.py` & `vdk-control-service-api-1.0.9/test/test_data_jobs_sources_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,53 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_info.get import Info
 
+import unittest
 
-class DataJobsServiceApi(
-    Info,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import taurus_datajob_api
+from taurus_datajob_api.api.data_jobs_sources_api import DataJobsSourcesApi  # noqa: E501
+from taurus_datajob_api.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestDataJobsSourcesApi(unittest.TestCase):
+    """DataJobsSourcesApi unit test stubs"""
+
+    def setUp(self):
+        self.api = taurus_datajob_api.api.data_jobs_sources_api.DataJobsSourcesApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_data_job_sources_download(self):
+        """Test case for data_job_sources_download
+
+        Download data job source code. | (Not Implemented)  # noqa: E501
+        """
+        pass
+
+    def test_sources_delete(self):
+        """Test case for sources_delete
+
+        Delete Data Job source.  # noqa: E501
+        """
+        pass
+
+    def test_sources_upload(self):
+        """Test case for sources_upload
+
+        Upload Data Job source code. | (Stable)  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_sources_api.py` & `vdk-control-service-api-1.0.9/test/test_data_job_contacts.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,26 +2,56 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_sources.get import DataJobSourcesDownload
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_sources.delete import SourcesDelete
-from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_sources.post import SourcesUpload
 
+import unittest
+import datetime
 
-class DataJobsSourcesApi(
-    DataJobSourcesDownload,
-    SourcesDelete,
-    SourcesUpload,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import taurus_datajob_api
+from taurus_datajob_api.models.data_job_contacts import DataJobContacts  # noqa: E501
+from taurus_datajob_api.rest import ApiException
+
+class TestDataJobContacts(unittest.TestCase):
+    """DataJobContacts unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test DataJobContacts
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `DataJobContacts`
+        """
+        model = taurus_datajob_api.models.data_job_contacts.DataJobContacts()  # noqa: E501
+        if include_optional :
+            return DataJobContacts(
+                notified_on_job_failure_user_error = ["auserov@example.mail.com"], 
+                notified_on_job_failure_platform_error = ["auserov@example.mail.com"], 
+                notified_on_job_success = ["auserov@example.mail.com"], 
+                notified_on_job_deploy = ["auserov@example.mail.com"]
+            )
+        else :
+            return DataJobContacts(
+        )
+        """
+
+    def testDataJobContacts(self):
+        """Test DataJobContacts"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-    Do not edit the class manually.
-    """
-    pass
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/configuration.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,99 +2,74 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
+import http.client as httplib
 from taurus_datajob_api.exceptions import ApiValueError
 
-
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems',
-    'uniqueItems', 'maxProperties', 'minProperties',
+    'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
+    """This class contains various settings of the API client.
 
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format.
 
     :Example:
     """
 
     _default = None
 
-    def __init__(
-        self,
-        host=None,
-        discard_unknown_keys=False,
-        disabled_client_side_validations="",
-        server_index=None,
-        server_variables=None,
-        server_operation_index=None,
-        server_operation_variables=None,
-    ):
+    def __init__(self, host=None,
+                 api_key=None, api_key_prefix=None,
+                 username=None, password=None,
+                 access_token=None,
+                 server_index=None, server_variables=None,
+                 server_operation_index=None, server_operation_variables=None,
+                 ssl_ca_cert=None,
+                 ):
         """Constructor
         """
         self._base_path = "http://localhost" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -104,15 +79,36 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.api_key = {}
+        if api_key:
+            self.api_key = api_key
+        """dict to store API key(s)
+        """
+        self.api_key_prefix = {}
+        if api_key_prefix:
+            self.api_key_prefix = api_key_prefix
+        """dict to store API prefix (e.g. Bearer)
+        """
+        self.refresh_api_key_hook = None
+        """function hook to refresh API key if expired
+        """
+        self.username = username
+        """Username for HTTP basic authentication
+        """
+        self.password = password
+        """Password for HTTP basic authentication
+        """
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("taurus_datajob_api")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -131,15 +127,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = None
+        self.ssl_ca_cert = ssl_ca_cert
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -167,16 +163,25 @@
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -186,46 +191,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -271,23 +279,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -361,15 +369,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.0.8".\
+               "SDK Package Version: 1.0.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/exceptions.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-import dataclasses
-import typing
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from urllib3._collections import HTTPHeaderDict
+    Do not edit the class manually.
+"""
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
@@ -97,34 +95,27 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-T = typing.TypeVar("T")
+class ApiException(OpenApiException):
 
-
-@dataclasses.dataclass
-class ApiException(OpenApiException, typing.Generic[T]):
-    status: int
-    reason: str
-    api_response: typing.Optional[T] = None
-
-    @property
-    def body(self) -> typing.Union[str, bytes, None]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.data
-
-    @property
-    def headers(self) -> typing.Optional[HTTPHeaderDict]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.getheaders()
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
+        else:
+            self.status = status
+            self.reason = reason
+            self.body = None
+            self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
@@ -132,14 +123,38 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
+
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_deployment.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,123 +2,96 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from taurus_datajob_api import schemas  # noqa: F401
+    Do not edit the class manually.
+"""
 
 
-class DataJob(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from datetime import datetime
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+from taurus_datajob_api.models.data_job_mode import DataJobMode
+from taurus_datajob_api.models.data_job_resources import DataJobResources
+from taurus_datajob_api.models.data_job_schedule import DataJobSchedule
 
-    Data Job Details
+class DataJobDeployment(BaseModel):
     """
+    A deployment of the Data Job
+    """
+    vdk_version: Optional[StrictStr] = Field(None, description="A specific VDK version to use")
+    job_version: Optional[StrictStr] = Field(None, description="Job version (can be Git commit)")
+    python_version: Optional[StrictStr] = Field(None, description="A python release version (supported by the service) to be used for job deployments.")
+    mode: Optional[DataJobMode] = None
+    id: Optional[StrictStr] = Field(None, description="String that identifies a single deployment of a Data Job. Currently only one single deployment per Data Job is possible.<br> In the future:<br> It's recommended to use following ids - development, testing, production. However users are free to come up with their own. For example, this enables the creation of 3 different deployments, using the same Data Job code:<br> `development  deployment  --deployment-id development`<br> `testing deployment  --deployment-id testing`<br> `production deployment  --deployment-id prod` ")
+    enabled: Optional[StrictBool] = Field(None, description="Enable/disable flag")
+    deployed_by: Optional[StrictStr] = Field(None, description="User or service that deployed the Data Job")
+    deployed_date: Optional[datetime] = Field(None, description="The Data Job deployment date")
+    schedule: Optional[DataJobSchedule] = None
+    resources: Optional[DataJobResources] = None
+    __properties = ["vdk_version", "job_version", "python_version", "mode", "id", "enabled", "deployed_by", "deployed_date", "schedule", "resources"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobDeployment:
+        """Create an instance of DataJobDeployment from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of schedule
+        if self.schedule:
+            _dict['schedule'] = self.schedule.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of resources
+        if self.resources:
+            _dict['resources'] = self.resources.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobDeployment:
+        """Create an instance of DataJobDeployment from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobDeployment.parse_obj(obj)
+
+        _obj = DataJobDeployment.parse_obj({
+            "vdk_version": obj.get("vdk_version"),
+            "job_version": obj.get("job_version"),
+            "python_version": obj.get("python_version"),
+            "mode": obj.get("mode"),
+            "id": obj.get("id"),
+            "enabled": obj.get("enabled"),
+            "deployed_by": obj.get("deployed_by"),
+            "deployed_date": obj.get("deployed_date"),
+            "schedule": DataJobSchedule.from_dict(obj.get("schedule")) if obj.get("schedule") is not None else None,
+            "resources": DataJobResources.from_dict(obj.get("resources")) if obj.get("resources") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "job_name",
-            "description",
-            "config",
-        }
-        
-        class properties:
-            job_name = schemas.StrSchema
-            description = schemas.StrSchema
-        
-            @staticmethod
-            def config() -> typing.Type['DataJobConfig']:
-                return DataJobConfig
-            team = schemas.StrSchema
-            __annotations__ = {
-                "job_name": job_name,
-                "description": description,
-                "config": config,
-                "team": team,
-            }
-    
-    job_name: MetaOapg.properties.job_name
-    description: MetaOapg.properties.description
-    config: 'DataJobConfig'
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["job_name"]) -> MetaOapg.properties.job_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["config"]) -> 'DataJobConfig': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["team"]) -> MetaOapg.properties.team: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["job_name", "description", "config", "team", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["job_name"]) -> MetaOapg.properties.job_name: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> 'DataJobConfig': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["team"]) -> typing.Union[MetaOapg.properties.team, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["job_name", "description", "config", "team", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        job_name: typing.Union[MetaOapg.properties.job_name, str, ],
-        description: typing.Union[MetaOapg.properties.description, str, ],
-        config: 'DataJobConfig',
-        team: typing.Union[MetaOapg.properties.team, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJob':
-        return super().__new__(
-            cls,
-            *_args,
-            job_name=job_name,
-            description=description,
-            config=config,
-            team=team,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from taurus_datajob_api.model.data_job_config import DataJobConfig
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_api_info.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_deployment_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,118 +2,102 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from taurus_datajob_api import schemas  # noqa: F401
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-class DataJobApiInfo(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+from taurus_datajob_api.models.data_job_contacts import DataJobContacts
+from taurus_datajob_api.models.data_job_mode import DataJobMode
+from taurus_datajob_api.models.data_job_resources import DataJobResources
+from taurus_datajob_api.models.data_job_schedule import DataJobSchedule
 
-    API and Data Job service information, list of supported python versions
+class DataJobDeploymentStatus(BaseModel):
     """
+    A deployment status of the Data Job, which includes information such as last deployment date, and who deployed the Data Job.
+    """
+    vdk_version: Optional[StrictStr] = Field(None, description="A specific VDK version to use")
+    job_version: Optional[StrictStr] = Field(None, description="Job version (can be Git commit)")
+    python_version: Optional[StrictStr] = Field(None, description="A python release version (supported by the service) to be used for job deployments.")
+    mode: Optional[DataJobMode] = None
+    id: Optional[StrictStr] = Field(None, description="String that identifies a single deployment of a Data Job. Currently only one single deployment per Data Job is possible.<br> In the future:<br> It's recommended to use following ids - development, testing, production. However users are free to come up with their own. For example, this enables the creation of 3 different deployments, using the same Data Job code:<br> `development  deployment  --deployment-id development`<br> `testing deployment  --deployment-id testing`<br> `production deployment  --deployment-id prod` ")
+    enabled: Optional[StrictBool] = Field(None, description="Enable/disable flag")
+    contacts: Optional[DataJobContacts] = None
+    schedule: Optional[DataJobSchedule] = None
+    resources: Optional[DataJobResources] = None
+    last_deployed_date: Optional[StrictStr] = Field(None, description="The date and time in UTC of the last deployment of the data job")
+    last_deployed_by: Optional[StrictStr] = Field(None, description="The username of the user who modified the data job last")
+    __properties = ["vdk_version", "job_version", "python_version", "mode", "id", "enabled", "contacts", "schedule", "resources", "last_deployed_date", "last_deployed_by"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobDeploymentStatus:
+        """Create an instance of DataJobDeploymentStatus from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of contacts
+        if self.contacts:
+            _dict['contacts'] = self.contacts.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of schedule
+        if self.schedule:
+            _dict['schedule'] = self.schedule.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of resources
+        if self.resources:
+            _dict['resources'] = self.resources.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobDeploymentStatus:
+        """Create an instance of DataJobDeploymentStatus from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobDeploymentStatus.parse_obj(obj)
+
+        _obj = DataJobDeploymentStatus.parse_obj({
+            "vdk_version": obj.get("vdk_version"),
+            "job_version": obj.get("job_version"),
+            "python_version": obj.get("python_version"),
+            "mode": obj.get("mode"),
+            "id": obj.get("id"),
+            "enabled": obj.get("enabled"),
+            "contacts": DataJobContacts.from_dict(obj.get("contacts")) if obj.get("contacts") is not None else None,
+            "schedule": DataJobSchedule.from_dict(obj.get("schedule")) if obj.get("schedule") is not None else None,
+            "resources": DataJobResources.from_dict(obj.get("resources")) if obj.get("resources") is not None else None,
+            "last_deployed_date": obj.get("last_deployed_date"),
+            "last_deployed_by": obj.get("last_deployed_by")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "supported_python_versions",
-            "api_version",
-        }
-        
-        class properties:
-            api_version = schemas.StrSchema
-            
-            
-            class supported_python_versions(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'supported_python_versions':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "api_version": api_version,
-                "supported_python_versions": supported_python_versions,
-            }
-    
-    supported_python_versions: MetaOapg.properties.supported_python_versions
-    api_version: MetaOapg.properties.api_version
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["api_version"]) -> MetaOapg.properties.api_version: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["supported_python_versions"]) -> MetaOapg.properties.supported_python_versions: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["api_version", "supported_python_versions", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["api_version"]) -> MetaOapg.properties.api_version: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["supported_python_versions"]) -> MetaOapg.properties.supported_python_versions: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["api_version", "supported_python_versions", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        supported_python_versions: typing.Union[MetaOapg.properties.supported_python_versions, list, tuple, ],
-        api_version: typing.Union[MetaOapg.properties.api_version, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJobApiInfo':
-        return super().__new__(
-            cls,
-            *_args,
-            supported_python_versions=supported_python_versions,
-            api_version=api_version,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment_id.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,69 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
+
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
 import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+import json
+
+
+
+from pydantic import BaseModel, Field, StrictStr
 
-import frozendict  # noqa: F401
+class DataJobVersion(BaseModel):
+    """
+    Data Job version
+    """
+    version_sha: StrictStr = Field(..., description="SHA hash which specifies the latest deployed version of the data job")
+    __properties = ["version_sha"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobVersion:
+        """Create an instance of DataJobVersion from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobVersion:
+        """Create an instance of DataJobVersion from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobVersion.parse_obj(obj)
+
+        _obj = DataJobVersion.parse_obj({
+            "version_sha": obj.get("version_sha")
+        })
+        return _obj
 
-from taurus_datajob_api import schemas  # noqa: F401
-DataJobDeploymentId = schemas.StrSchema
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_logs.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,79 +2,75 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from taurus_datajob_api import schemas  # noqa: F401
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-class DataJobExecutionLogs(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, Field, StrictFloat, StrictInt
 
-    Executions of a Data Job
+class DataJobResources(BaseModel):
     """
+    Resource cofiguration of a data Data Job Deployment.
+    """
+    cpu_request: Optional[StrictFloat] = Field(None, description="Initial CPU shares in deciCores (1 dCore = 0.1 Core = 100 mCores)")
+    cpu_limit: Optional[StrictFloat] = Field(None, description="Max CPU shares in deciCores (1 dCore = 0.1 Core = 100 mCores)")
+    memory_request: Optional[StrictInt] = Field(None, description="Initial Memory in MiB.")
+    memory_limit: Optional[StrictInt] = Field(None, description="Max Memory in MiB.")
+    __properties = ["cpu_request", "cpu_limit", "memory_request", "memory_limit"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobResources:
+        """Create an instance of DataJobResources from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobResources:
+        """Create an instance of DataJobResources from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobResources.parse_obj(obj)
+
+        _obj = DataJobResources.parse_obj({
+            "cpu_request": obj.get("cpu_request"),
+            "cpu_limit": obj.get("cpu_limit"),
+            "memory_request": obj.get("memory_request"),
+            "memory_limit": obj.get("memory_limit")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            logs = schemas.StrSchema
-            __annotations__ = {
-                "logs": logs,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["logs"]) -> MetaOapg.properties.logs: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["logs", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["logs"]) -> typing.Union[MetaOapg.properties.logs, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["logs", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        logs: typing.Union[MetaOapg.properties.logs, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJobExecutionLogs':
-        return super().__new__(
-            cls,
-            *_args,
-            logs=logs,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_request.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,117 +2,87 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from taurus_datajob_api import schemas  # noqa: F401
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-class DataJobExecutionRequest(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from taurus_datajob_api.models.data_job_contacts import DataJobContacts
+from taurus_datajob_api.models.data_job_schedule import DataJobSchedule
 
-    Request to start execution of Data Job. The job must have been deployed before that (see Deployment API) and will run its latest version.
+class DataJobConfig(BaseModel):
     """
+    Data Job configuration properties.
+    """
+    db_default_type: Optional[StrictStr] = Field(None, description="Default DB connection provided for the job, e.g. 'TRINO', 'IMPALA', 'REDSHIFT'.<br> ")
+    contacts: Optional[DataJobContacts] = None
+    schedule: Optional[DataJobSchedule] = None
+    generate_keytab: Optional[StrictBool] = Field(True, description="Enable Disable flag for generating secret with keytab")
+    enable_execution_notifications: Optional[StrictBool] = Field(True, description="(Optional) Specifies whether to dispatch email notifications per data job execution.")
+    notification_delay_period_minutes: Optional[StrictInt] = Field(240, description="(Optional) Specifies the time (in minutes) a job execution is allowed to be delayed from its schedule before an alert is triggered. The value of this property for each data job is exposed as a Prometheus metric by the service at the /data-jobs/debug/prometheus endpoint. These metrics (taurus_datajob_notification_delay) are subsequently used in JobDelay Prometheus rules to generate the alerts. ")
+    __properties = ["db_default_type", "contacts", "schedule", "generate_keytab", "enable_execution_notifications", "notification_delay_period_minutes"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobConfig:
+        """Create an instance of DataJobConfig from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of contacts
+        if self.contacts:
+            _dict['contacts'] = self.contacts.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of schedule
+        if self.schedule:
+            _dict['schedule'] = self.schedule.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobConfig:
+        """Create an instance of DataJobConfig from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobConfig.parse_obj(obj)
+
+        _obj = DataJobConfig.parse_obj({
+            "db_default_type": obj.get("db_default_type"),
+            "contacts": DataJobContacts.from_dict(obj.get("contacts")) if obj.get("contacts") is not None else None,
+            "schedule": DataJobSchedule.from_dict(obj.get("schedule")) if obj.get("schedule") is not None else None,
+            "generate_keytab": obj.get("generate_keytab") if obj.get("generate_keytab") is not None else True,
+            "enable_execution_notifications": obj.get("enable_execution_notifications") if obj.get("enable_execution_notifications") is not None else True,
+            "notification_delay_period_minutes": obj.get("notification_delay_period_minutes") if obj.get("notification_delay_period_minutes") is not None else 240
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            started_by = schemas.StrSchema
-            
-            
-            class args(
-                schemas.DictSchema
-            ):
-            
-            
-                class MetaOapg:
-                    additional_properties = schemas.AnyTypeSchema
-                
-                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    # dict_instance[name] accessor
-                    return super().__getitem__(name)
-                
-                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    return super().get_item_oapg(name)
-            
-                def __new__(
-                    cls,
-                    *_args: typing.Union[dict, frozendict.frozendict, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[MetaOapg.additional_properties, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-                ) -> 'args':
-                    return super().__new__(
-                        cls,
-                        *_args,
-                        _configuration=_configuration,
-                        **kwargs,
-                    )
-            __annotations__ = {
-                "started_by": started_by,
-                "args": args,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["started_by"]) -> MetaOapg.properties.started_by: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["args"]) -> MetaOapg.properties.args: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["started_by", "args", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["started_by"]) -> typing.Union[MetaOapg.properties.started_by, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["args"]) -> typing.Union[MetaOapg.properties.args, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["started_by", "args", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        started_by: typing.Union[MetaOapg.properties.started_by, str, schemas.Unset] = schemas.unset,
-        args: typing.Union[MetaOapg.properties.args, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJobExecutionRequest':
-        return super().__new__(
-            cls,
-            *_args,
-            started_by=started_by,
-            args=args,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_mode.py` & `vdk-control-service-api-1.0.9/test/test_data_job_execution_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,50 +2,54 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from taurus_datajob_api import schemas  # noqa: F401
-
-
-class DataJobMode(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""
+
 
-    The execution mode that the data job is deployed in. Data Jobs used for development or testing purposes are marked as testing. This is used by Operations team on platform rollout and infrastructure changes adoption. For example, rollout and validation of testing jobs first, then proceeding with release data jobs. Also, testing and release jobs may have different limits and SLA targets.
-    """
+import unittest
+import datetime
 
+import taurus_datajob_api
+from taurus_datajob_api.models.data_job_execution_request import DataJobExecutionRequest  # noqa: E501
+from taurus_datajob_api.rest import ApiException
+
+class TestDataJobExecutionRequest(unittest.TestCase):
+    """DataJobExecutionRequest unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test DataJobExecutionRequest
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `DataJobExecutionRequest`
+        """
+        model = taurus_datajob_api.models.data_job_execution_request.DataJobExecutionRequest()  # noqa: E501
+        if include_optional :
+            return DataJobExecutionRequest(
+                started_by = 'schedule/runtime', 
+                args = {"key":"value"}
+            )
+        else :
+            return DataJobExecutionRequest(
+        )
+        """
+
+    def testDataJobExecutionRequest(self):
+        """Test DataJobExecutionRequest"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "testing": "TESTING",
-            "release": "RELEASE",
-        }
-    
-    @schemas.classproperty
-    def TESTING(cls):
-        return cls("testing")
-    
-    @schemas.classproperty
-    def RELEASE(cls):
-        return cls("release")
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_page.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_execution.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,121 +2,109 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from taurus_datajob_api import schemas  # noqa: F401
+    Do not edit the class manually.
+"""
 
 
-class DataJobPage(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from datetime import datetime
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr, validator
+from taurus_datajob_api.models.data_job_deployment import DataJobDeployment
 
-    Page object containing Data Jobs list with information for total elements and pages
+class DataJobExecution(BaseModel):
     """
+    Executions of a Data Job
+    """
+    id: Optional[StrictStr] = Field(None, description="Data Job Execution ID")
+    job_name: Optional[StrictStr] = Field(None, description="Data Job name")
+    status: Optional[StrictStr] = Field(None, description="The current status")
+    type: Optional[StrictStr] = Field(None, description="Execution type - manual or scheduled")
+    start_time: Optional[datetime] = Field(None, description="Start of execution")
+    end_time: Optional[datetime] = Field(None, description="Start of execution")
+    started_by: Optional[StrictStr] = Field(None, description="User or service that started the execution (e.g manual/auserov@example.mail.com or scheduled/runtime)")
+    logs_url: Optional[StrictStr] = Field(None, description="URL link to persisted logs in central location. Logs generally should be available for longer time. The link is available only if operators have configured it during installation of Control Service. During install operators can conifgure logs to be presisted to log aggregator service whose link can be exposed here. ")
+    message: Optional[StrictStr] = Field(None, description="Message (usually error) during execution")
+    op_id: Optional[StrictStr] = Field(None, description="Operation id used for tracing calls between different services")
+    deployment: Optional[DataJobDeployment] = None
+    __properties = ["id", "job_name", "status", "type", "start_time", "end_time", "started_by", "logs_url", "message", "op_id", "deployment"]
+
+    @validator('status')
+    def status_validate_enum(cls, v):
+        if v is None:
+            return v
+        if v not in ('submitted', 'running', 'succeeded', 'cancelled', 'skipped', 'user_error', 'platform_error'):
+            raise ValueError("must be one of enum values ('submitted', 'running', 'succeeded', 'cancelled', 'skipped', 'user_error', 'platform_error')")
+        return v
+
+    @validator('type')
+    def type_validate_enum(cls, v):
+        if v is None:
+            return v
+        if v not in ('manual', 'scheduled'):
+            raise ValueError("must be one of enum values ('manual', 'scheduled')")
+        return v
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobExecution:
+        """Create an instance of DataJobExecution from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of deployment
+        if self.deployment:
+            _dict['deployment'] = self.deployment.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobExecution:
+        """Create an instance of DataJobExecution from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobExecution.parse_obj(obj)
+
+        _obj = DataJobExecution.parse_obj({
+            "id": obj.get("id"),
+            "job_name": obj.get("job_name"),
+            "status": obj.get("status"),
+            "type": obj.get("type"),
+            "start_time": obj.get("start_time"),
+            "end_time": obj.get("end_time"),
+            "started_by": obj.get("started_by"),
+            "logs_url": obj.get("logs_url"),
+            "message": obj.get("message"),
+            "op_id": obj.get("op_id"),
+            "deployment": DataJobDeployment.from_dict(obj.get("deployment")) if obj.get("deployment") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            
-            
-            class content(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.DictSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'content':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            totalItems = schemas.IntSchema
-            totalPages = schemas.IntSchema
-            __annotations__ = {
-                "content": content,
-                "totalItems": totalItems,
-                "totalPages": totalPages,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["content"]) -> MetaOapg.properties.content: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["totalItems"]) -> MetaOapg.properties.totalItems: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["totalPages"]) -> MetaOapg.properties.totalPages: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["content", "totalItems", "totalPages", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["content"]) -> typing.Union[MetaOapg.properties.content, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["totalItems"]) -> typing.Union[MetaOapg.properties.totalItems, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["totalPages"]) -> typing.Union[MetaOapg.properties.totalPages, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["content", "totalItems", "totalPages", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
-        totalItems: typing.Union[MetaOapg.properties.totalItems, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJobPage':
-        return super().__new__(
-            cls,
-            *_args,
-            content=content,
-            totalItems=totalItems,
-            totalPages=totalPages,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_properties.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,58 +2,73 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from taurus_datajob_api import schemas  # noqa: F401
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-class DataJobProperties(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Any, Dict, List, Optional
+from pydantic import BaseModel, Field, StrictInt, conlist
 
-    Properties of a Data Job
+class DataJobPage(BaseModel):
     """
+    Page object containing Data Jobs list with information for total elements and pages
+    """
+    content: Optional[conlist(Dict[str, Any])] = None
+    total_items: Optional[StrictInt] = Field(None, alias="totalItems", description="Number of elements which meet the given query requirement")
+    total_pages: Optional[StrictInt] = Field(None, alias="totalPages", description="Number of pages with elements which meet the given query requirement")
+    __properties = ["content", "totalItems", "totalPages"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobPage:
+        """Create an instance of DataJobPage from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobPage:
+        """Create an instance of DataJobPage from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobPage.parse_obj(obj)
+
+        _obj = DataJobPage.parse_obj({
+            "content": obj.get("content"),
+            "total_items": obj.get("totalItems"),
+            "total_pages": obj.get("totalPages")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        additional_properties = schemas.DictSchema
-    
-    def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-        return super().get_item_oapg(name)
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[MetaOapg.additional_properties, dict, frozendict.frozendict, ],
-    ) -> 'DataJobProperties':
-        return super().__new__(
-            cls,
-            *_args,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_query_response.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_contacts.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,116 +2,75 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from taurus_datajob_api import schemas  # noqa: F401
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-class DataJobQueryResponse(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictStr, conlist
 
-    Query response containing Data Jobs
+class DataJobContacts(BaseModel):
     """
+    Data Job contacts
+    """
+    notified_on_job_failure_user_error: Optional[conlist(StrictStr)] = Field(None, description="List of email addresses to be notified on job execution failure caused by user code or user configuration problem. E.g. if the job contains a SQL script with a syntax error. ")
+    notified_on_job_failure_platform_error: Optional[conlist(StrictStr)] = Field(None, description="List of email addresses to be notified on job execution failure caused by a platform problem")
+    notified_on_job_success: Optional[conlist(StrictStr)] = Field(None, description="List of email addresses to be notified on job execution success")
+    notified_on_job_deploy: Optional[conlist(StrictStr)] = Field(None, description="List of email addresses to be notified of job deployment outcome")
+    __properties = ["notified_on_job_failure_user_error", "notified_on_job_failure_platform_error", "notified_on_job_success", "notified_on_job_deploy"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobContacts:
+        """Create an instance of DataJobContacts from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobContacts:
+        """Create an instance of DataJobContacts from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobContacts.parse_obj(obj)
+
+        _obj = DataJobContacts.parse_obj({
+            "notified_on_job_failure_user_error": obj.get("notified_on_job_failure_user_error"),
+            "notified_on_job_failure_platform_error": obj.get("notified_on_job_failure_platform_error"),
+            "notified_on_job_success": obj.get("notified_on_job_success"),
+            "notified_on_job_deploy": obj.get("notified_on_job_deploy")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            
-            
-            class errors(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.DictSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'errors':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-        
-            @staticmethod
-            def data() -> typing.Type['DataJobPage']:
-                return DataJobPage
-            __annotations__ = {
-                "errors": errors,
-                "data": data,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["errors"]) -> MetaOapg.properties.errors: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["data"]) -> 'DataJobPage': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["errors", "data", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["errors"]) -> typing.Union[MetaOapg.properties.errors, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["data"]) -> typing.Union['DataJobPage', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["errors", "data", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        errors: typing.Union[MetaOapg.properties.errors, list, tuple, schemas.Unset] = schemas.unset,
-        data: typing.Union['DataJobPage', schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJobQueryResponse':
-        return super().__new__(
-            cls,
-            *_args,
-            errors=errors,
-            data=data,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from taurus_datajob_api.model.data_job_page import DataJobPage
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_schedule.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_query_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,79 +2,75 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from taurus_datajob_api import schemas  # noqa: F401
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-class DataJobSchedule(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Any, Dict, List, Optional
+from pydantic import BaseModel, Field, conlist
+from taurus_datajob_api.models.data_job_page import DataJobPage
 
-    Schedule configuration
+class DataJobQueryResponse(BaseModel):
     """
+    Query response containing Data Jobs
+    """
+    errors: Optional[conlist(Dict[str, Any])] = Field(None, description="Errors while making query (validation errors, exceptions, etc)")
+    data: Optional[DataJobPage] = None
+    __properties = ["errors", "data"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobQueryResponse:
+        """Create an instance of DataJobQueryResponse from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobQueryResponse:
+        """Create an instance of DataJobQueryResponse from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobQueryResponse.parse_obj(obj)
+
+        _obj = DataJobQueryResponse.parse_obj({
+            "errors": obj.get("errors"),
+            "data": DataJobPage.from_dict(obj.get("data")) if obj.get("data") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            schedule_cron = schemas.StrSchema
-            __annotations__ = {
-                "schedule_cron": schedule_cron,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["schedule_cron"]) -> MetaOapg.properties.schedule_cron: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["schedule_cron", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["schedule_cron"]) -> typing.Union[MetaOapg.properties.schedule_cron, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["schedule_cron", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        schedule_cron: typing.Union[MetaOapg.properties.schedule_cron, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJobSchedule':
-        return super().__new__(
-            cls,
-            *_args,
-            schedule_cron=schedule_cron,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_version.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_summary.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,84 +2,75 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from taurus_datajob_api import schemas  # noqa: F401
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
 
-class DataJobVersion(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
 
-    Data Job version
+class DataJobSummary(BaseModel):
     """
+    Data Job summary
+    """
+    job_name: StrictStr = Field(..., description="Data Job name")
+    team: StrictStr = Field(..., description="Team name")
+    description: StrictStr = Field(..., description="Description")
+    source_url: Optional[StrictStr] = Field(None, description="Link to source code.")
+    __properties = ["job_name", "team", "description", "source_url"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobSummary:
+        """Create an instance of DataJobSummary from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobSummary:
+        """Create an instance of DataJobSummary from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobSummary.parse_obj(obj)
+
+        _obj = DataJobSummary.parse_obj({
+            "job_name": obj.get("job_name"),
+            "team": obj.get("team"),
+            "description": obj.get("description"),
+            "source_url": obj.get("source_url")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "version_sha",
-        }
-        
-        class properties:
-            version_sha = schemas.StrSchema
-            __annotations__ = {
-                "version_sha": version_sha,
-            }
-    
-    version_sha: MetaOapg.properties.version_sha
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["version_sha"]) -> MetaOapg.properties.version_sha: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["version_sha", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["version_sha"]) -> MetaOapg.properties.version_sha: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["version_sha", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        version_sha: typing.Union[MetaOapg.properties.version_sha, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DataJobVersion':
-        return super().__new__(
-            cls,
-            *_args,
-            version_sha=version_sha,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `vdk-control-service-api-1.0.8/taurus_datajob_api/model/error.py` & `vdk-control-service-api-1.0.9/test/test_data_job_query_response_with_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,106 +2,57 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from taurus_datajob_api import schemas  # noqa: F401
-
-
-class Error(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""
 
-    Contains description for one or more errors detected.
-    """
 
+import unittest
+import datetime
 
-    class MetaOapg:
-        required = {
-            "messages",
-        }
-        
-        class properties:
-            
-            
-            class messages(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'messages':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "messages": messages,
-            }
-    
-    messages: MetaOapg.properties.messages
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["messages", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["messages", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        messages: typing.Union[MetaOapg.properties.messages, list, tuple, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'Error':
-        return super().__new__(
-            cls,
-            *_args,
-            messages=messages,
-            _configuration=_configuration,
-            **kwargs,
+import taurus_datajob_api
+from taurus_datajob_api.models.data_job_query_response_with_error import DataJobQueryResponseWithError  # noqa: E501
+from taurus_datajob_api.rest import ApiException
+
+class TestDataJobQueryResponseWithError(unittest.TestCase):
+    """DataJobQueryResponseWithError unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test DataJobQueryResponseWithError
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `DataJobQueryResponseWithError`
+        """
+        model = taurus_datajob_api.models.data_job_query_response_with_error.DataJobQueryResponseWithError()  # noqa: E501
+        if include_optional :
+            return DataJobQueryResponseWithError(
+                errors = {"application/json":[{"message":"Validation error of type FieldUndefined","locations":[],"description":"Field 'someField' in type 'DataJob' is undefined","validationErrorType":"FieldUndefined","queryPath":["jobs","content","someField"],"extensions":null,"errorType":"ValidationError","path":null}]}, 
+                data = taurus_datajob_api.models.data_job_page.DataJobPage(
+                    content = {"application/json":[{"jobName":"starshot-processing-vmc-fact-daily","config":{"team":"starshot","description":"Data Job responsible for transforming vmc related fact tables on daily basis","schedule":{"scheduleCron":"5 0 * 8 *","nextRun":1618914371},"sourceUrl":"https://github.com/product-analytics/data-jobs/tree/master/starshot-processing-vmc-fact-daily","contacts":{"notifiedOnJobFailureUserError":"[auser@example.mail.com]","notifiedOnJobFailurePlatformError":"[auser2@example.mail.com, auser@example.mail.com]","notifiedOnJobSuccess":"[auser@example.mail.com]","notifiedOnJobDeploy":"[auser2@example.mail.com, auser@example.mail.com]"}}},"..."]}, 
+                    total_items = 100, 
+                    total_pages = 5, )
+            )
+        else :
+            return DataJobQueryResponseWithError(
         )
+        """
+
+    def testDataJobQueryResponseWithError(self):
+        """Test DataJobQueryResponseWithError"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job.py` & `vdk-control-service-api-1.0.9/test/test_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,54 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.model.data_job import DataJob
-from taurus_datajob_api import configuration
+from taurus_datajob_api.models.error import Error  # noqa: E501
+from taurus_datajob_api.rest import ApiException
 
+class TestError(unittest.TestCase):
+    """Error unit test stubs"""
 
-class TestDataJob(unittest.TestCase):
-    """DataJob unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test Error
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `Error`
+        """
+        model = taurus_datajob_api.models.error.Error()  # noqa: E501
+        if include_optional :
+            return Error(
+                messages = ["Data Job starshot-processing-vmc-fact-daily not found"]
+            )
+        else :
+            return Error(
+                messages = ["Data Job starshot-processing-vmc-fact-daily not found"],
+        )
+        """
+
+    def testError(self):
+        """Test Error"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_config.py` & `vdk-control-service-api-1.0.9/vdk_control_service_api.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-# coding: utf-8
+Metadata-Version: 2.1
+Name: vdk-control-service-api
+Version: 1.0.9
+Summary: Versatile Data Kit Control Service API
+Home-page: 
+Author: OpenAPI Generator community
+Author-email: team@openapitools.org
+License: Apache 2.0
+Keywords: OpenAPI,OpenAPI-Generator,Versatile Data Kit Control Service API
+Description-Content-Type: text/markdown
 
-"""
-    Versatile Data Kit Control Service API
-
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
-
-    The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-
-import taurus_datajob_api
-from taurus_datajob_api.model.data_job_config import DataJobConfig
-from taurus_datajob_api import configuration
-
-
-class TestDataJobConfig(unittest.TestCase):
-    """DataJobConfig unit test stubs"""
-    _configuration = configuration.Configuration()
-
-
-if __name__ == '__main__':
-    unittest.main()
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#39;Authorization: Bearer [access-token-here]&#39; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
+
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_contacts.py` & `vdk-control-service-api-1.0.9/test/test_data_job_schedule.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,24 +2,53 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.model.data_job_contacts import DataJobContacts
-from taurus_datajob_api import configuration
+from taurus_datajob_api.models.data_job_schedule import DataJobSchedule  # noqa: E501
+from taurus_datajob_api.rest import ApiException
 
+class TestDataJobSchedule(unittest.TestCase):
+    """DataJobSchedule unit test stubs"""
 
-class TestDataJobContacts(unittest.TestCase):
-    """DataJobContacts unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test DataJobSchedule
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `DataJobSchedule`
+        """
+        model = taurus_datajob_api.models.data_job_schedule.DataJobSchedule()  # noqa: E501
+        if include_optional :
+            return DataJobSchedule(
+                schedule_cron = '0 0 13 * 5'
+            )
+        else :
+            return DataJobSchedule(
+        )
+        """
+
+    def testDataJobSchedule(self):
+        """Test DataJobSchedule"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment.py` & `vdk-control-service-api-1.0.9/test/test_data_jobs_deployment_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,24 +2,67 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
 
 import taurus_datajob_api
-from taurus_datajob_api.model.data_job_deployment import DataJobDeployment
-from taurus_datajob_api import configuration
+from taurus_datajob_api.api.data_jobs_deployment_api import DataJobsDeploymentApi  # noqa: E501
+from taurus_datajob_api.rest import ApiException
+
+
+class TestDataJobsDeploymentApi(unittest.TestCase):
+    """DataJobsDeploymentApi unit test stubs"""
+
+    def setUp(self):
+        self.api = taurus_datajob_api.api.data_jobs_deployment_api.DataJobsDeploymentApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_deployment_delete(self):
+        """Test case for deployment_delete
+
+        Delete Deployment of a Data Job. Currently executing Data Job will be left to finish.  | (Stable)   # noqa: E501
+        """
+        pass
+
+    def test_deployment_list(self):
+        """Test case for deployment_list
+
+        Get Data Job deployments. | (Stable)  # noqa: E501
+        """
+        pass
+
+    def test_deployment_patch(self):
+        """Test case for deployment_patch
+
+        Patch a deployment of a Data Job. Use it to change the configuration of a data job. For example: to enable or disable deployment, to change the vdk version. The operation is guranteed to be synchrounous so it cannot be used to deploy new version of a data job - job_version cannot be changed using PATCH. Use POST .../deployments for this. | (Stable)   # noqa: E501
+        """
+        pass
+
+    def test_deployment_read(self):
+        """Test case for deployment_read
+
+        Get Data Job deployments. | (Stable)  # noqa: E501
+        """
+        pass
 
+    def test_deployment_update(self):
+        """Test case for deployment_update
 
-class TestDataJobDeployment(unittest.TestCase):
-    """DataJobDeployment unit test stubs"""
-    _configuration = configuration.Configuration()
+        Creates or updates a deployment of a Data Job. | (Stable)  # noqa: E501
+        """
+        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_id.py` & `vdk-control-service-api-1.0.9/test/test_data_job_api_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,24 +2,56 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.model.data_job_deployment_id import DataJobDeploymentId
-from taurus_datajob_api import configuration
+from taurus_datajob_api.models.data_job_api_info import DataJobApiInfo  # noqa: E501
+from taurus_datajob_api.rest import ApiException
 
+class TestDataJobApiInfo(unittest.TestCase):
+    """DataJobApiInfo unit test stubs"""
 
-class TestDataJobDeploymentId(unittest.TestCase):
-    """DataJobDeploymentId unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test DataJobApiInfo
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `DataJobApiInfo`
+        """
+        model = taurus_datajob_api.models.data_job_api_info.DataJobApiInfo()  # noqa: E501
+        if include_optional :
+            return DataJobApiInfo(
+                api_version = '', 
+                supported_python_versions = ["python3.7","python3.8","python3.9"]
+            )
+        else :
+            return DataJobApiInfo(
+                api_version = '',
+                supported_python_versions = ["python3.7","python3.8","python3.9"],
+        )
+        """
+
+    def testDataJobApiInfo(self):
+        """Test DataJobApiInfo"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_status.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/data_job_execution_logs.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,69 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-
-import taurus_datajob_api
-from taurus_datajob_api.model.data_job_deployment_status import DataJobDeploymentStatus
-from taurus_datajob_api import configuration
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""
 
-class TestDataJobDeploymentStatus(unittest.TestCase):
-    """DataJobDeploymentStatus unit test stubs"""
-    _configuration = configuration.Configuration()
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
+
+class DataJobExecutionLogs(BaseModel):
+    """
+    Executions of a Data Job
+    """
+    logs: Optional[StrictStr] = Field(None, description="The logs of the data job execution.")
+    __properties = ["logs"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> DataJobExecutionLogs:
+        """Create an instance of DataJobExecutionLogs from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> DataJobExecutionLogs:
+        """Create an instance of DataJobExecutionLogs from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return DataJobExecutionLogs.parse_obj(obj)
+
+        _obj = DataJobExecutionLogs.parse_obj({
+            "logs": obj.get("logs")
+        })
+        return _obj
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution.py` & `vdk-control-service-api-1.0.9/test/test_data_job_deployment.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,67 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.model.data_job_execution import DataJobExecution
-from taurus_datajob_api import configuration
+from taurus_datajob_api.models.data_job_deployment import DataJobDeployment  # noqa: E501
+from taurus_datajob_api.rest import ApiException
 
+class TestDataJobDeployment(unittest.TestCase):
+    """DataJobDeployment unit test stubs"""
 
-class TestDataJobExecution(unittest.TestCase):
-    """DataJobExecution unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test DataJobDeployment
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `DataJobDeployment`
+        """
+        model = taurus_datajob_api.models.data_job_deployment.DataJobDeployment()  # noqa: E501
+        if include_optional :
+            return DataJobDeployment(
+                vdk_version = '2.1', 
+                job_version = '11a403ba', 
+                python_version = '3.9', 
+                mode = 'release', 
+                id = 'release', 
+                enabled = False, 
+                deployed_by = 'auserov@example.mail.com', 
+                deployed_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                schedule = taurus_datajob_api.models.data_job_schedule.DataJobSchedule(
+                    schedule_cron = '0 0 13 * 5', ), 
+                resources = taurus_datajob_api.models.data_job_resources.DataJobResources(
+                    cpu_request = 10, 
+                    cpu_limit = 20, 
+                    memory_request = 1024, 
+                    memory_limit = 2048, )
+            )
+        else :
+            return DataJobDeployment(
+        )
+        """
+
+    def testDataJobDeployment(self):
+        """Test DataJobDeployment"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_logs.py` & `vdk-control-service-api-1.0.9/taurus_datajob_api/models/error.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,24 +2,69 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-
-import taurus_datajob_api
-from taurus_datajob_api.model.data_job_execution_logs import DataJobExecutionLogs
-from taurus_datajob_api import configuration
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""
 
-class TestDataJobExecutionLogs(unittest.TestCase):
-    """DataJobExecutionLogs unit test stubs"""
-    _configuration = configuration.Configuration()
 
+from __future__ import annotations
+from inspect import getfullargspec
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import List
+from pydantic import BaseModel, Field, StrictStr, conlist
+
+class Error(BaseModel):
+    """
+    Contains description for one or more errors detected.
+    """
+    messages: conlist(StrictStr) = Field(..., description="Error messages")
+    __properties = ["messages"]
+
+    class Config:
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Error:
+        """Create an instance of Error from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> Error:
+        """Create an instance of Error from a dict"""
+        if obj is None:
+            return None
+
+        if type(obj) is not dict:
+            return Error.parse_obj(obj)
+
+        _obj = Error.parse_obj({
+            "messages": obj.get("messages")
+        })
+        return _obj
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_request.py` & `vdk-control-service-api-1.0.9/test/test_data_job_page.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,55 @@
 
 """
     Versatile Data Kit Control Service API
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.model.data_job_execution_request import DataJobExecutionRequest
-from taurus_datajob_api import configuration
+from taurus_datajob_api.models.data_job_page import DataJobPage  # noqa: E501
+from taurus_datajob_api.rest import ApiException
 
+class TestDataJobPage(unittest.TestCase):
+    """DataJobPage unit test stubs"""
 
-class TestDataJobExecutionRequest(unittest.TestCase):
-    """DataJobExecutionRequest unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test DataJobPage
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `DataJobPage`
+        """
+        model = taurus_datajob_api.models.data_job_page.DataJobPage()  # noqa: E501
+        if include_optional :
+            return DataJobPage(
+                content = {"application/json":[{"jobName":"starshot-processing-vmc-fact-daily","config":{"team":"starshot","description":"Data Job responsible for transforming vmc related fact tables on daily basis","schedule":{"scheduleCron":"5 0 * 8 *","nextRun":1618914371},"sourceUrl":"https://github.com/product-analytics/data-jobs/tree/master/starshot-processing-vmc-fact-daily","contacts":{"notifiedOnJobFailureUserError":"[auser@example.mail.com]","notifiedOnJobFailurePlatformError":"[auser2@example.mail.com, auser@example.mail.com]","notifiedOnJobSuccess":"[auser@example.mail.com]","notifiedOnJobDeploy":"[auser2@example.mail.com, auser@example.mail.com]"}}},"..."]}, 
+                total_items = 100, 
+                total_pages = 5
+            )
+        else :
+            return DataJobPage(
+        )
+        """
+
+    def testDataJobPage(self):
+        """Test DataJobPage"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

