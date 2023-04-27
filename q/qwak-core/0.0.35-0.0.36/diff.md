# Comparing `tmp/qwak_core-0.0.35.tar.gz` & `tmp/qwak_core-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.35.tar", max compression
+gzip compressed data, was "qwak_core-0.0.36.tar", max compression
```

## Comparing `qwak_core-0.0.35.tar` & `qwak_core-0.0.36.tar`

### file list

```diff
@@ -1,535 +1,535 @@
--rw-r--r--   0        0        0      264 2023-04-25 08:08:14.301566 qwak_core-0.0.35/README.md
--rw-r--r--   0        0        0        0 2023-04-25 08:09:16.726023 qwak_core-0.0.35/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-04-25 08:09:16.750023 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-04-25 08:08:56.805878 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.754023 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-04-25 08:09:16.746023 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-04-25 08:08:56.453876 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.746023 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-04-25 08:09:16.750023 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-04-25 08:08:56.629877 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.750023 qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-04-25 08:09:16.742023 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-04-25 08:08:55.929872 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-04-25 08:09:16.742023 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-25 08:09:16.742023 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-04-25 08:08:56.105873 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.742023 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-04-25 08:09:16.746023 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-04-25 08:08:56.277875 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.746023 qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-04-25 08:09:16.726023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-04-25 08:08:55.749871 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-04-25 08:09:16.730023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-04-25 08:09:16.730023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-04-25 08:08:56.985880 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.730023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-04-25 08:09:16.734023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-04-25 08:08:57.337882 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.734023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-04-25 08:09:16.734023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-04-25 08:08:57.521884 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-04-25 08:09:16.738023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-25 08:09:16.730023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-04-25 08:08:57.161881 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.734023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-04-25 08:09:16.738023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-04-25 08:08:57.701885 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.738023 qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-04-25 08:09:16.782023 qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-04-25 08:09:00.217903 qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.782023 qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-04-25 08:09:16.782023 qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-04-25 08:09:00.401904 qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-04-25 08:09:16.786023 qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-04-25 08:09:16.850024 qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-04-25 08:09:05.469941 qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.850024 qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-04-25 08:09:16.850024 qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-04-25 08:09:05.665942 qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-04-25 08:09:16.854024 qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-04-25 08:09:16.854024 qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-04-25 08:09:06.689949 qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-04-25 08:09:16.858024 qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-04-25 08:09:16.854024 qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-04-25 08:09:06.481948 qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.854024 qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-04-25 08:09:16.858024 qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-04-25 08:09:06.901951 qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.858024 qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-04-25 08:09:16.858024 qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-04-25 08:09:07.097952 qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-04-25 08:09:16.862024 qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-04-25 08:09:16.922024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-04-25 08:09:12.289991 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.922024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-04-25 08:09:16.918024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-04-25 08:09:11.933988 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.918024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-04-25 08:09:16.918024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-04-25 08:09:12.109989 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.922024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-04-25 08:09:16.914024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-04-25 08:09:11.577985 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-04-25 08:09:16.914024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-04-25 08:09:16.914024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-04-25 08:09:11.757986 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.914024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-04-25 08:09:16.926025 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-04-25 08:09:12.817994 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.930024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-04-25 08:09:16.926025 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-04-25 08:09:12.645993 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.926025 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-04-25 08:09:16.922024 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-04-25 08:09:12.465992 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.926025 qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-04-25 08:09:16.966025 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-04-25 08:09:16.098018 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.970025 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-04-25 08:09:16.962025 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-04-25 08:09:15.726016 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.962025 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-04-25 08:09:16.966025 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-04-25 08:09:15.918017 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-04-25 08:09:16.966025 qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-04-25 08:09:16.886024 qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-04-25 08:09:09.045967 qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-04-25 08:09:16.886024 qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-04-25 08:09:16.886024 qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-04-25 08:09:08.865965 qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.886024 qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-04-25 08:09:16.874024 qwak_core-0.0.35/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-04-25 08:09:08.501963 qwak_core-0.0.35/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.878024 qwak_core-0.0.35/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-04-25 08:09:16.878024 qwak_core-0.0.35/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-04-25 08:09:08.681964 qwak_core-0.0.35/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.878024 qwak_core-0.0.35/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-04-25 08:09:16.878024 qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-04-25 08:09:09.225968 qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-04-25 08:09:16.882024 qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-04-25 08:09:16.882024 qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-04-25 08:09:09.617971 qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-04-25 08:09:16.882024 qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-04-25 08:09:16.894024 qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-04-25 08:09:09.989974 qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.894024 qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-04-25 08:09:16.894024 qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-25 08:09:10.165975 qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-25 08:09:16.898024 qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-04-25 08:09:16.870024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-04-25 08:09:07.905958 qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.870024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-04-25 08:09:16.870024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-04-25 08:09:08.109960 qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-04-25 08:09:16.874024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-04-25 08:09:16.866024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-04-25 08:09:07.501955 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.866024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-04-25 08:09:16.862024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-04-25 08:09:07.305954 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.862024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-04-25 08:09:16.866024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-04-25 08:09:07.709957 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-04-25 08:09:16.866024 qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-04-25 08:09:16.770023 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-04-25 08:08:59.305896 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.770023 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-25 08:09:16.774023 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-04-25 08:08:59.485898 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.774023 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-04-25 08:09:16.774023 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-04-25 08:08:59.673899 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-04-25 08:09:16.778023 qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-04-25 08:09:16.830024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-04-25 08:09:04.237932 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.830024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-04-25 08:09:16.826024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-04-25 08:09:04.041930 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-04-25 08:09:16.830024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-04-25 08:09:16.810024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-04-25 08:09:02.609920 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.810024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-04-25 08:09:16.806023 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-04-25 08:09:02.417919 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.810024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-04-25 08:09:16.802024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-04-25 08:09:01.861915 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.802024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-04-25 08:09:16.806023 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-04-25 08:09:02.241917 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-04-25 08:09:16.806023 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-04-25 08:09:16.810024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-04-25 08:09:02.785921 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.814024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-04-25 08:09:16.814024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-04-25 08:09:02.961923 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-04-25 08:09:16.814024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-04-25 08:09:16.802024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-04-25 08:09:02.049916 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.802024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-04-25 08:09:16.818024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-04-25 08:09:03.137924 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.818024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-04-25 08:09:16.830024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-04-25 08:09:16.278020 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.834024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-04-25 08:09:16.834024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-04-25 08:09:16.458021 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-04-25 08:09:16.834024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-04-25 08:09:16.834024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-04-25 08:09:04.829936 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.838024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-04-25 08:09:16.838024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-04-25 08:09:05.053938 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-04-25 08:09:16.838024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-04-25 08:09:16.842024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-04-25 08:09:05.273939 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.842024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-04-25 08:09:16.846024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-04-25 08:09:06.077945 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.846024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-04-25 08:09:16.842024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-04-25 08:09:05.873943 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-04-25 08:09:16.842024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-04-25 08:09:16.846024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-04-25 08:09:06.289946 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.846024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    13329 2023-04-25 08:09:16.818024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23039 2023-04-25 08:09:03.317925 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.818024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-04-25 08:09:16.822024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-04-25 08:09:03.497926 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.822024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-04-25 08:09:16.822024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-04-25 08:09:03.677928 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-04-25 08:09:16.822024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-04-25 08:09:16.826024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-04-25 08:09:03.857929 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.826024 qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-04-25 08:09:16.930024 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-04-25 08:09:12.993996 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.930024 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-04-25 08:09:16.934024 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-04-25 08:09:13.169997 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-25 08:09:16.934024 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-04-25 08:09:16.934024 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-04-25 08:09:13.349998 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.934024 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-04-25 08:09:16.938025 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-04-25 08:09:13.534000 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-25 08:09:16.938025 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-04-25 08:09:16.938025 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-04-25 08:09:13.722001 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-04-25 08:09:16.938025 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-04-25 08:09:16.942025 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-04-25 08:09:13.898002 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.942025 qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-04-25 08:09:16.898024 qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-04-25 08:09:10.337976 qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.898024 qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-04-25 08:09:16.898024 qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-25 08:09:10.513977 qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-25 08:09:16.902024 qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-04-25 08:09:16.786023 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-04-25 08:09:01.133910 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.790023 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-25 08:09:16.790023 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-04-25 08:09:01.313911 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.794023 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-04-25 08:09:16.794023 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-04-25 08:09:01.497912 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-04-25 08:09:16.798024 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-04-25 08:09:16.798024 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-04-25 08:09:01.677913 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.798024 qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-04-25 08:09:16.874024 qwak_core-0.0.35/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-04-25 08:09:08.309961 qwak_core-0.0.35/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-04-25 08:09:16.874024 qwak_core-0.0.35/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-04-25 08:09:16.942025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-04-25 08:09:14.078004 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.946025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-04-25 08:09:16.946025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-04-25 08:09:14.254005 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.946025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-04-25 08:09:16.946025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-04-25 08:09:14.434006 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.950025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-04-25 08:09:16.950025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-04-25 08:09:14.618008 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.950025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-25 08:09:16.950025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-04-25 08:09:14.802009 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.954025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-04-25 08:09:16.954025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-04-25 08:09:15.002010 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-04-25 08:09:16.954025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-04-25 08:09:16.958025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-04-25 08:09:15.186012 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.958025 qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-04-25 08:09:16.902024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-04-25 08:09:10.861980 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.906024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-04-25 08:09:16.910024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-04-25 08:09:11.393984 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.910024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-04-25 08:09:16.906024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-04-25 08:09:11.037981 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-04-25 08:09:16.906024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-04-25 08:09:16.910024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-04-25 08:09:11.217983 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.910024 qwak_core-0.0.35/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-04-25 08:09:16.890024 qwak_core-0.0.35/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-04-25 08:09:09.813972 qwak_core-0.0.35/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-04-25 08:09:16.894024 qwak_core-0.0.35/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-04-25 08:09:16.766023 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-04-25 08:09:00.769907 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-04-25 08:09:16.766023 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-04-25 08:09:16.766023 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-04-25 08:09:00.585905 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.766023 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-04-25 08:09:16.770023 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-04-25 08:09:00.949908 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-04-25 08:09:16.770023 qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-04-25 08:09:16.890024 qwak_core-0.0.35/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-04-25 08:09:09.417969 qwak_core-0.0.35/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-04-25 08:09:16.890024 qwak_core-0.0.35/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-04-25 08:09:16.902024 qwak_core-0.0.35/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-04-25 08:09:10.689979 qwak_core-0.0.35/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-04-25 08:09:16.902024 qwak_core-0.0.35/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-04-25 08:09:16.762023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-04-25 08:08:58.589891 qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.762023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-04-25 08:09:16.758023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-04-25 08:08:58.409890 qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-04-25 08:09:16.762023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-04-25 08:09:16.754023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-04-25 08:08:57.873886 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.754023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-04-25 08:09:16.754023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-04-25 08:08:58.053887 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.758023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-04-25 08:09:16.758023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-04-25 08:08:58.229889 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-04-25 08:09:16.758023 qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-04-25 08:09:16.962025 qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-04-25 08:09:15.546014 qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-04-25 08:09:16.962025 qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-04-25 08:09:16.958025 qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-04-25 08:09:15.366013 qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.958025 qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-04-25 08:09:16.778023 qwak_core-0.0.35/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-04-25 08:08:59.849900 qwak_core-0.0.35/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.778023 qwak_core-0.0.35/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3001 2023-04-25 08:09:16.778023 qwak_core-0.0.35/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2574 2023-04-25 08:09:00.033902 qwak_core-0.0.35/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-25 08:09:16.782023 qwak_core-0.0.35/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     1906 2023-04-25 08:09:18.118033 qwak_core-0.0.35/pyproject.toml
--rw-r--r--   0        0        0      447 2023-04-25 08:09:18.118033 qwak_core-0.0.35/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5478 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4255 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     2585 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-04-25 08:08:14.305566 qwak_core-0.0.35/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     8808 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     5933 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      829 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/schema.py
--rw-r--r--   0        0        0     2964 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/schema_entities.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5776 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-04-25 08:08:14.309566 qwak_core-0.0.35/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 qwak_core-0.0.35/setup.py
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-04-27 13:49:23.740425 qwak_core-0.0.36/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 13:50:26.540478 qwak_core-0.0.36/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-04-27 13:50:07.536461 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-04-27 13:50:07.192461 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-04-27 13:50:07.364462 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-04-27 13:50:06.680461 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-04-27 13:50:06.852461 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-04-27 13:50:07.024461 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-04-27 13:50:26.540478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-04-27 13:50:06.508461 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-04-27 13:50:26.540478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-04-27 13:50:07.708462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-04-27 13:50:26.548478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-04-27 13:50:08.048462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.548478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-04-27 13:50:26.548478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-04-27 13:50:08.224462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-04-27 13:50:07.876462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-04-27 13:50:08.396462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-04-27 13:50:10.864464 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.596478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-04-27 13:50:26.596478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-04-27 13:50:11.064464 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-04-27 13:50:26.596478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-04-27 13:50:15.828469 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.672478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-04-27 13:50:26.672478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-04-27 13:50:16.004469 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-04-27 13:50:26.672478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-04-27 13:50:16.880469 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-04-27 13:50:16.708469 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-04-27 13:50:17.056470 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-04-27 13:50:17.228470 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-04-27 13:50:22.216474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.744478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-04-27 13:50:21.860474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-04-27 13:50:22.040474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-04-27 13:50:26.732478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-04-27 13:50:21.508473 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-04-27 13:50:21.684474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-04-27 13:50:26.748478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-04-27 13:50:22.740475 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-04-27 13:50:26.748478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-04-27 13:50:22.568474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.748478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-04-27 13:50:26.744478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-04-27 13:50:22.392474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.744478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-04-27 13:50:25.912477 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-04-27 13:50:26.784478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-04-27 13:50:25.548477 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.784478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-04-27 13:50:25.732477 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-04-27 13:50:19.012471 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-04-27 13:50:26.704478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-04-27 13:50:18.836471 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-04-27 13:50:26.696478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-04-27 13:50:18.484471 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.696478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-04-27 13:50:18.656471 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-04-27 13:50:19.188471 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-04-27 13:50:26.704478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-04-27 13:50:19.568472 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-04-27 13:50:26.704478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-04-27 13:50:19.936472 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.716478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-04-27 13:50:26.716478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-27 13:50:20.108472 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-27 13:50:26.716478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-04-27 13:50:17.960470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-04-27 13:50:18.132470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-04-27 13:50:26.684478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-04-27 13:50:17.600470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-04-27 13:50:26.684478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-04-27 13:50:17.416470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.684478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-04-27 13:50:17.784470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-04-27 13:50:09.976464 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-04-27 13:50:10.152464 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-04-27 13:50:10.328464 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-04-27 13:50:14.784468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-04-27 13:50:14.612468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-04-27 13:50:13.212466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-04-27 13:50:26.628478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-04-27 13:50:13.040466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-04-27 13:50:12.496466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-04-27 13:50:26.628478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-04-27 13:50:12.868466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-04-27 13:50:26.628478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-04-27 13:50:13.388466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-04-27 13:50:13.564467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-04-27 13:50:12.684466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-04-27 13:50:13.736467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-04-27 13:50:26.092477 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-04-27 13:50:26.656478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-04-27 13:50:26.272477 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-04-27 13:50:26.656478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-04-27 13:50:26.656478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-04-27 13:50:15.308468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-04-27 13:50:15.480468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-04-27 13:50:15.652469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-04-27 13:50:16.360469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-04-27 13:50:16.180469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-04-27 13:50:16.532469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-04-27 13:50:13.916467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-04-27 13:50:14.088467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.644478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-04-27 13:50:26.644478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-04-27 13:50:14.264467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-04-27 13:50:26.644478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-04-27 13:50:14.440467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-04-27 13:50:22.912475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-04-27 13:50:23.084475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-04-27 13:50:23.256475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-04-27 13:50:23.436475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-04-27 13:50:23.616475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-04-27 13:50:23.788475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.764478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-04-27 13:50:20.280472 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-27 13:50:20.452473 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-04-27 13:50:26.604478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-04-27 13:50:11.776465 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.608478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-27 13:50:26.608478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-04-27 13:50:11.952465 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.612478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-04-27 13:50:26.612478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-04-27 13:50:12.128466 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-04-27 13:50:26.616478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-04-27 13:50:26.616478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-04-27 13:50:12.300466 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.620478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-04-27 13:50:18.304471 qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-04-27 13:50:26.696478 qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-04-27 13:50:26.764478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-04-27 13:50:23.964475 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.764478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-04-27 13:50:24.136476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-04-27 13:50:24.312476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-04-27 13:50:24.488476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-04-27 13:50:24.664476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-04-27 13:50:26.776478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-04-27 13:50:24.856476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-04-27 13:50:26.776478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-04-27 13:50:26.776478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-04-27 13:50:25.028476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-04-27 13:50:20.800473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-04-27 13:50:26.732478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-04-27 13:50:21.332473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.732478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-04-27 13:50:20.980473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-04-27 13:50:21.156473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-04-27 13:50:19.760472 qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-04-27 13:50:26.580478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-04-27 13:50:11.424465 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-04-27 13:50:26.580478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-04-27 13:50:11.244465 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-04-27 13:50:26.580478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-04-27 13:50:11.604465 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-04-27 13:50:19.376472 qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-04-27 13:50:20.624473 qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-04-27 13:50:09.276463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-04-27 13:50:09.100463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-04-27 13:50:08.568462 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.568478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-04-27 13:50:26.568478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-04-27 13:50:08.744463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.568478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-04-27 13:50:08.924463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-04-27 13:50:25.376477 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-04-27 13:50:26.784478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-04-27 13:50:25.204476 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-04-27 13:50:10.496464 qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3001 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2574 2023-04-27 13:50:10.668464 qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     1906 2023-04-27 13:50:28.260479 qwak_core-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-04-27 13:50:28.260479 qwak_core-0.0.36/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5478 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4255 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     2585 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0     1201 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     2006 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2961 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1730 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     8808 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     5933 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      829 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/schema.py
+-rw-r--r--   0        0        0     2964 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5776 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 qwak_core-0.0.36/setup.py
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.36/PKG-INFO
```

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&qwak/feature_store/sources/batch.proto\x12\x1aqwak.feature.store.sources\"\xb7\x05\n\x0b\x42\x61tchSource\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61te_created_column\x18\x03 \x01(\t\x12@\n\x0c\x61thenaSource\x18\x04 \x01(\x0b\x32(.qwak.feature.store.sources.AthenaSourceH\x00\x12>\n\x0bmongoSource\x18\x05 \x01(\x0b\x32\'.qwak.feature.store.sources.MongoSourceH\x00\x12:\n\tcsvSource\x18\x06 \x01(\x0b\x32%.qwak.feature.store.sources.CsvSourceH\x00\x12\x46\n\x0fsnowflakeSource\x18\x07 \x01(\x0b\x32+.qwak.feature.store.sources.SnowflakeSourceH\x00\x12\x42\n\rparquetSource\x18\x08 \x01(\x0b\x32).qwak.feature.store.sources.ParquetSourceH\x00\x12<\n\njdbcSource\x18\t \x01(\x0b\x32&.qwak.feature.store.sources.JdbcSourceH\x00\x12\x42\n\rverticaSource\x18\n \x01(\x0b\x32).qwak.feature.store.sources.VerticaSourceH\x00\x12\x44\n\x0e\x62igquerySource\x18\x0b \x01(\x0b\x32*.qwak.feature.store.sources.BigquerySourceH\x00\x12N\n\x13\x65lasticsearchSource\x18\x0c \x01(\x0b\x32/.qwak.feature.store.sources.ElasticsearchSourceH\x00\x42\x06\n\x04type\"{\n\x17\x46ileSystemConfiguration\x12X\n\x14\x61ws_s3_configuration\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.sources.AwsS3FileSystemConfigurationH\x00\x42\x06\n\x04type\"\x91\x01\n\x1c\x41wsS3FileSystemConfiguration\x12\x1e\n\x16\x61\x63\x63\x65ss_key_secret_name\x18\x01 \x01(\t\x12\x1e\n\x16secret_key_secret_name\x18\x02 \x01(\t\x12!\n\x19session_token_secret_name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\xce\x02\n\nJdbcSource\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x01 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x02 \x01(\t\x12\x10\n\x08\x64\x62_table\x18\x04 \x01(\t\x12\r\n\x05query\x18\x05 \x01(\t\x12>\n\x0bmysqlSource\x18\x06 \x01(\x0b\x32\'.qwak.feature.store.sources.MysqlSourceH\x00\x12H\n\x10postgresqlSource\x18\x07 \x01(\x0b\x32,.qwak.feature.store.sources.PostgresqlSourceH\x00\x12\x44\n\x0eredshiftSource\x18\x08 \x01(\x0b\x32*.qwak.feature.store.sources.RedshiftSourceH\x00\x42\x06\n\x04type\"\r\n\x0bMysqlSource\"\x12\n\x10PostgresqlSource\"i\n\x0eRedshiftSource\x12\x0f\n\x07\x64\x62_user\x18\x01 \x01(\t\x12\x14\n\x0ciam_role_arn\x18\x02 \x01(\t\x12\x15\n\raccess_key_id\x18\x03 \x01(\t\x12\x19\n\x11secret_access_key\x18\x04 \x01(\t\"/\n\x0c\x41thenaSource\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\xa0\x02\n\x0e\x42igquerySource\x12\x1f\n\x17\x63redentials_secret_name\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0f\n\x07project\x18\x04 \x01(\t\x12\x16\n\x0eparent_project\x18\x05 \x01(\t\x12\x0b\n\x03sql\x18\x06 \x01(\t\x12\x15\n\rviews_enabled\x18\x07 \x01(\x08\x12#\n\x17materialization_dataset\x18\x08 \x01(\tB\x02\x18\x01\x12#\n\x17materialization_project\x18\t \x01(\tB\x02\x18\x01\x12\x36\n*materialization_expiration_time_in_minutes\x18\n \x01(\tB\x02\x18\x01\"\xa3\x01\n\tCsvSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x17\n\x0fquote_character\x18\x02 \x01(\t\x12\x18\n\x10\x65scape_character\x18\x03 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x04 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\xab\x01\n\x0bMongoSource\x12\r\n\x05hosts\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x12\n\ncollection\x18\x05 \x01(\t\x12\x19\n\x11\x63onnection_params\x18\x06 \x01(\t\x12\x10\n\x08protocol\x18\x07 \x01(\t\"\xae\x01\n\x0fSnowflakeSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x0e\n\x06schema\x18\x05 \x01(\t\x12\x11\n\twarehouse\x18\x06 \x01(\t\x12\r\n\x05table\x18\x07 \x01(\t\x12\r\n\x05query\x18\x08 \x01(\t\"t\n\rParquetSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x02 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\x98\x01\n\rVerticaSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x06 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x07 \x01(\t\"\xbc\x01\n\x13\x45lasticsearchSource\x12\r\n\x05nodes\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08resource\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x16\n\x0e\x65xclude_fields\x18\x05 \x01(\t\x12\x13\n\x0bparse_dates\x18\x06 \x01(\x08\x12\x1c\n\x14username_secret_name\x18\x07 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x08 \x01(\tBX\n%com.qwak.ai.feature.store.sources.apiP\x01Z-qwak/featurestore/sources;featurestoresourcesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&qwak/feature_store/sources/batch.proto\x12\x1aqwak.feature.store.sources\"\xb7\x05\n\x0b\x42\x61tchSource\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61te_created_column\x18\x03 \x01(\t\x12@\n\x0c\x61thenaSource\x18\x04 \x01(\x0b\x32(.qwak.feature.store.sources.AthenaSourceH\x00\x12>\n\x0bmongoSource\x18\x05 \x01(\x0b\x32\'.qwak.feature.store.sources.MongoSourceH\x00\x12:\n\tcsvSource\x18\x06 \x01(\x0b\x32%.qwak.feature.store.sources.CsvSourceH\x00\x12\x46\n\x0fsnowflakeSource\x18\x07 \x01(\x0b\x32+.qwak.feature.store.sources.SnowflakeSourceH\x00\x12\x42\n\rparquetSource\x18\x08 \x01(\x0b\x32).qwak.feature.store.sources.ParquetSourceH\x00\x12<\n\njdbcSource\x18\t \x01(\x0b\x32&.qwak.feature.store.sources.JdbcSourceH\x00\x12\x42\n\rverticaSource\x18\n \x01(\x0b\x32).qwak.feature.store.sources.VerticaSourceH\x00\x12\x44\n\x0e\x62igquerySource\x18\x0b \x01(\x0b\x32*.qwak.feature.store.sources.BigquerySourceH\x00\x12N\n\x13\x65lasticsearchSource\x18\x0c \x01(\x0b\x32/.qwak.feature.store.sources.ElasticsearchSourceH\x00\x42\x06\n\x04type\"\xcd\x01\n\x17\x46ileSystemConfiguration\x12X\n\x14\x61ws_s3_configuration\x18\x01 \x01(\x0b\x32\x38.qwak.feature.store.sources.AwsS3FileSystemConfigurationH\x00\x12P\n\x10\x61ws_s3_anonymous\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.sources.AnonymousS3ConfigurationH\x00\x42\x06\n\x04type\"\x91\x01\n\x1c\x41wsS3FileSystemConfiguration\x12\x1e\n\x16\x61\x63\x63\x65ss_key_secret_name\x18\x01 \x01(\t\x12\x1e\n\x16secret_key_secret_name\x18\x02 \x01(\t\x12!\n\x19session_token_secret_name\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\x1a\n\x18\x41nonymousS3Configuration\"\xce\x02\n\nJdbcSource\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x01 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x02 \x01(\t\x12\x10\n\x08\x64\x62_table\x18\x04 \x01(\t\x12\r\n\x05query\x18\x05 \x01(\t\x12>\n\x0bmysqlSource\x18\x06 \x01(\x0b\x32\'.qwak.feature.store.sources.MysqlSourceH\x00\x12H\n\x10postgresqlSource\x18\x07 \x01(\x0b\x32,.qwak.feature.store.sources.PostgresqlSourceH\x00\x12\x44\n\x0eredshiftSource\x18\x08 \x01(\x0b\x32*.qwak.feature.store.sources.RedshiftSourceH\x00\x42\x06\n\x04type\"\r\n\x0bMysqlSource\"\x12\n\x10PostgresqlSource\"i\n\x0eRedshiftSource\x12\x0f\n\x07\x64\x62_user\x18\x01 \x01(\t\x12\x14\n\x0ciam_role_arn\x18\x02 \x01(\t\x12\x15\n\raccess_key_id\x18\x03 \x01(\t\x12\x19\n\x11secret_access_key\x18\x04 \x01(\t\"/\n\x0c\x41thenaSource\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\xa0\x02\n\x0e\x42igquerySource\x12\x1f\n\x17\x63redentials_secret_name\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0f\n\x07project\x18\x04 \x01(\t\x12\x16\n\x0eparent_project\x18\x05 \x01(\t\x12\x0b\n\x03sql\x18\x06 \x01(\t\x12\x15\n\rviews_enabled\x18\x07 \x01(\x08\x12#\n\x17materialization_dataset\x18\x08 \x01(\tB\x02\x18\x01\x12#\n\x17materialization_project\x18\t \x01(\tB\x02\x18\x01\x12\x36\n*materialization_expiration_time_in_minutes\x18\n \x01(\tB\x02\x18\x01\"\xa3\x01\n\tCsvSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x17\n\x0fquote_character\x18\x02 \x01(\t\x12\x18\n\x10\x65scape_character\x18\x03 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x04 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\xab\x01\n\x0bMongoSource\x12\r\n\x05hosts\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x12\n\ncollection\x18\x05 \x01(\t\x12\x19\n\x11\x63onnection_params\x18\x06 \x01(\t\x12\x10\n\x08protocol\x18\x07 \x01(\t\"\xae\x01\n\x0fSnowflakeSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x02 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x04 \x01(\t\x12\x0e\n\x06schema\x18\x05 \x01(\t\x12\x11\n\twarehouse\x18\x06 \x01(\t\x12\r\n\x05table\x18\x07 \x01(\t\x12\r\n\x05query\x18\x08 \x01(\t\"t\n\rParquetSource\x12\x0c\n\x04path\x18\x01 \x01(\t\x12U\n\x18\x66ilesystem_configuration\x18\x02 \x01(\x0b\x32\x33.qwak.feature.store.sources.FileSystemConfiguration\"\x98\x01\n\rVerticaSource\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x1c\n\x14username_secret_name\x18\x06 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x07 \x01(\t\"\xbc\x01\n\x13\x45lasticsearchSource\x12\r\n\x05nodes\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x10\n\x08resource\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x16\n\x0e\x65xclude_fields\x18\x05 \x01(\t\x12\x13\n\x0bparse_dates\x18\x06 \x01(\x08\x12\x1c\n\x14username_secret_name\x18\x07 \x01(\t\x12\x1c\n\x14password_secret_name\x18\x08 \x01(\tBX\n%com.qwak.ai.feature.store.sources.apiP\x01Z-qwak/featurestore/sources;featurestoresourcesb\x06proto3')
 
 
 
 _BATCHSOURCE = DESCRIPTOR.message_types_by_name['BatchSource']
 _FILESYSTEMCONFIGURATION = DESCRIPTOR.message_types_by_name['FileSystemConfiguration']
 _AWSS3FILESYSTEMCONFIGURATION = DESCRIPTOR.message_types_by_name['AwsS3FileSystemConfiguration']
+_ANONYMOUSS3CONFIGURATION = DESCRIPTOR.message_types_by_name['AnonymousS3Configuration']
 _JDBCSOURCE = DESCRIPTOR.message_types_by_name['JdbcSource']
 _MYSQLSOURCE = DESCRIPTOR.message_types_by_name['MysqlSource']
 _POSTGRESQLSOURCE = DESCRIPTOR.message_types_by_name['PostgresqlSource']
 _REDSHIFTSOURCE = DESCRIPTOR.message_types_by_name['RedshiftSource']
 _ATHENASOURCE = DESCRIPTOR.message_types_by_name['AthenaSource']
 _BIGQUERYSOURCE = DESCRIPTOR.message_types_by_name['BigquerySource']
 _CSVSOURCE = DESCRIPTOR.message_types_by_name['CsvSource']
@@ -50,14 +51,21 @@
 AwsS3FileSystemConfiguration = _reflection.GeneratedProtocolMessageType('AwsS3FileSystemConfiguration', (_message.Message,), {
   'DESCRIPTOR' : _AWSS3FILESYSTEMCONFIGURATION,
   '__module__' : 'qwak.feature_store.sources.batch_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.sources.AwsS3FileSystemConfiguration)
   })
 _sym_db.RegisterMessage(AwsS3FileSystemConfiguration)
 
+AnonymousS3Configuration = _reflection.GeneratedProtocolMessageType('AnonymousS3Configuration', (_message.Message,), {
+  'DESCRIPTOR' : _ANONYMOUSS3CONFIGURATION,
+  '__module__' : 'qwak.feature_store.sources.batch_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.feature.store.sources.AnonymousS3Configuration)
+  })
+_sym_db.RegisterMessage(AnonymousS3Configuration)
+
 JdbcSource = _reflection.GeneratedProtocolMessageType('JdbcSource', (_message.Message,), {
   'DESCRIPTOR' : _JDBCSOURCE,
   '__module__' : 'qwak.feature_store.sources.batch_pb2'
   # @@protoc_insertion_point(class_scope:qwak.feature.store.sources.JdbcSource)
   })
 _sym_db.RegisterMessage(JdbcSource)
 
@@ -146,36 +154,38 @@
   _BIGQUERYSOURCE.fields_by_name['materialization_dataset']._serialized_options = b'\030\001'
   _BIGQUERYSOURCE.fields_by_name['materialization_project']._options = None
   _BIGQUERYSOURCE.fields_by_name['materialization_project']._serialized_options = b'\030\001'
   _BIGQUERYSOURCE.fields_by_name['materialization_expiration_time_in_minutes']._options = None
   _BIGQUERYSOURCE.fields_by_name['materialization_expiration_time_in_minutes']._serialized_options = b'\030\001'
   _BATCHSOURCE._serialized_start=71
   _BATCHSOURCE._serialized_end=766
-  _FILESYSTEMCONFIGURATION._serialized_start=768
-  _FILESYSTEMCONFIGURATION._serialized_end=891
-  _AWSS3FILESYSTEMCONFIGURATION._serialized_start=894
-  _AWSS3FILESYSTEMCONFIGURATION._serialized_end=1039
-  _JDBCSOURCE._serialized_start=1042
-  _JDBCSOURCE._serialized_end=1376
-  _MYSQLSOURCE._serialized_start=1378
-  _MYSQLSOURCE._serialized_end=1391
-  _POSTGRESQLSOURCE._serialized_start=1393
-  _POSTGRESQLSOURCE._serialized_end=1411
-  _REDSHIFTSOURCE._serialized_start=1413
-  _REDSHIFTSOURCE._serialized_end=1518
-  _ATHENASOURCE._serialized_start=1520
-  _ATHENASOURCE._serialized_end=1567
-  _BIGQUERYSOURCE._serialized_start=1570
-  _BIGQUERYSOURCE._serialized_end=1858
-  _CSVSOURCE._serialized_start=1861
-  _CSVSOURCE._serialized_end=2024
-  _MONGOSOURCE._serialized_start=2027
-  _MONGOSOURCE._serialized_end=2198
-  _SNOWFLAKESOURCE._serialized_start=2201
-  _SNOWFLAKESOURCE._serialized_end=2375
-  _PARQUETSOURCE._serialized_start=2377
-  _PARQUETSOURCE._serialized_end=2493
-  _VERTICASOURCE._serialized_start=2496
-  _VERTICASOURCE._serialized_end=2648
-  _ELASTICSEARCHSOURCE._serialized_start=2651
-  _ELASTICSEARCHSOURCE._serialized_end=2839
+  _FILESYSTEMCONFIGURATION._serialized_start=769
+  _FILESYSTEMCONFIGURATION._serialized_end=974
+  _AWSS3FILESYSTEMCONFIGURATION._serialized_start=977
+  _AWSS3FILESYSTEMCONFIGURATION._serialized_end=1122
+  _ANONYMOUSS3CONFIGURATION._serialized_start=1124
+  _ANONYMOUSS3CONFIGURATION._serialized_end=1150
+  _JDBCSOURCE._serialized_start=1153
+  _JDBCSOURCE._serialized_end=1487
+  _MYSQLSOURCE._serialized_start=1489
+  _MYSQLSOURCE._serialized_end=1502
+  _POSTGRESQLSOURCE._serialized_start=1504
+  _POSTGRESQLSOURCE._serialized_end=1522
+  _REDSHIFTSOURCE._serialized_start=1524
+  _REDSHIFTSOURCE._serialized_end=1629
+  _ATHENASOURCE._serialized_start=1631
+  _ATHENASOURCE._serialized_end=1678
+  _BIGQUERYSOURCE._serialized_start=1681
+  _BIGQUERYSOURCE._serialized_end=1969
+  _CSVSOURCE._serialized_start=1972
+  _CSVSOURCE._serialized_end=2135
+  _MONGOSOURCE._serialized_start=2138
+  _MONGOSOURCE._serialized_end=2309
+  _SNOWFLAKESOURCE._serialized_start=2312
+  _SNOWFLAKESOURCE._serialized_end=2486
+  _PARQUETSOURCE._serialized_start=2488
+  _PARQUETSOURCE._serialized_end=2604
+  _VERTICASOURCE._serialized_start=2607
+  _VERTICASOURCE._serialized_end=2759
+  _ELASTICSEARCHSOURCE._serialized_start=2762
+  _ELASTICSEARCHSOURCE._serialized_end=2950
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -75,24 +75,28 @@
 
 global___BatchSource = BatchSource
 
 class FileSystemConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AWS_S3_CONFIGURATION_FIELD_NUMBER: builtins.int
+    AWS_S3_ANONYMOUS_FIELD_NUMBER: builtins.int
     @property
     def aws_s3_configuration(self) -> global___AwsS3FileSystemConfiguration: ...
+    @property
+    def aws_s3_anonymous(self) -> global___AnonymousS3Configuration: ...
     def __init__(
         self,
         *,
         aws_s3_configuration: global___AwsS3FileSystemConfiguration | None = ...,
+        aws_s3_anonymous: global___AnonymousS3Configuration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["aws_s3_configuration", b"aws_s3_configuration", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["aws_s3_configuration", b"aws_s3_configuration", "type", b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["aws_s3_configuration"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["aws_s3_anonymous", b"aws_s3_anonymous", "aws_s3_configuration", b"aws_s3_configuration", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["aws_s3_anonymous", b"aws_s3_anonymous", "aws_s3_configuration", b"aws_s3_configuration", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["aws_s3_configuration", "aws_s3_anonymous"] | None: ...
 
 global___FileSystemConfiguration = FileSystemConfiguration
 
 class AwsS3FileSystemConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACCESS_KEY_SECRET_NAME_FIELD_NUMBER: builtins.int
@@ -115,14 +119,25 @@
         session_token_secret_name: builtins.str = ...,
         bucket: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["access_key_secret_name", b"access_key_secret_name", "bucket", b"bucket", "secret_key_secret_name", b"secret_key_secret_name", "session_token_secret_name", b"session_token_secret_name"]) -> None: ...
 
 global___AwsS3FileSystemConfiguration = AwsS3FileSystemConfiguration
 
+class AnonymousS3Configuration(google.protobuf.message.Message):
+    """Anonymous S3 access"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___AnonymousS3Configuration = AnonymousS3Configuration
+
 class JdbcSource(google.protobuf.message.Message):
     """Jdbc Batch source"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     URL_FIELD_NUMBER: builtins.int
     USERNAME_SECRET_NAME_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/pyproject.toml` & `qwak_core-0.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.35"
+version = "0.0.36"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak"},
     {include = "_qwak_proto"},
```

### Comparing `qwak_core-0.0.35/qwak/automations/__init__.py` & `qwak_core-0.0.36/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/automations/automation_executions.py` & `qwak_core-0.0.36/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/automations/automations.py` & `qwak_core-0.0.36/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.36/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.36/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.36/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.36/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.36/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/alert_management/client.py` & `qwak_core-0.0.36/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/analytics/client.py` & `qwak_core-0.0.36/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/audience/client.py` & `qwak_core-0.0.36/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/automation_management/client.py` & `qwak_core-0.0.36/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.36/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.36/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.36/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.36/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/build_management/client.py` & `qwak_core-0.0.36/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.36/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.36/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/deployment/client.py` & `qwak_core-0.0.36/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.36/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.36/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.36/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.36/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.36/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/logging_client/client.py` & `qwak_core-0.0.36/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/model_management/client.py` & `qwak_core-0.0.36/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/project/client.py` & `qwak_core-0.0.36/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/secret_service/client.py` & `qwak_core-0.0.36/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.36/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.36/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.36/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.36/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.36/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.36/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.36/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.36/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.36/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.36/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/feature_store/online/client.py` & `qwak_core-0.0.36/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/const.py` & `qwak_core-0.0.36/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.36/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.36/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.36/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.36/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/singleton_meta.py` & `qwak_core-0.0.36/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/tool/auth.py` & `qwak_core-0.0.36/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.36/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.36/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/adapters/__init__.py` & `qwak_core-0.0.36/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.36/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.36/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.36/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.36/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.36/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/base.py` & `qwak_core-0.0.36/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/decorators/api.py` & `qwak_core-0.0.36/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.36/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/experiment_tracking.py` & `qwak_core-0.0.36/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/schema.py` & `qwak_core-0.0.36/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model/schema_entities.py` & `qwak_core-0.0.36/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.36/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.36/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.36/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.36/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.36/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.36/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/client.py` & `qwak_core-0.0.36/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.36/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/models/model.py` & `qwak_core-0.0.36/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.36/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.36/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.36/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/qwak_services_mock/services_mock.py` & `qwak_core-0.0.36/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.35/setup.py` & `qwak_core-0.0.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
  'protobuf>=3.10,<4',
  'python-jose',
  'requests',
  'typeguard>=2,<3']
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.35',
+    'version': '0.0.36',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.35/PKG-INFO` & `qwak_core-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.35
+Version: 0.0.36
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

