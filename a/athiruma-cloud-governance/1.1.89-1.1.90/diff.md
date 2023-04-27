# Comparing `tmp/athiruma-cloud-governance-1.1.89.tar.gz` & `tmp/athiruma-cloud-governance-1.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athiruma-cloud-governance-1.1.89.tar", last modified: Thu Apr 27 04:23:44 2023, max compression
+gzip compressed data, was "athiruma-cloud-governance-1.1.90.tar", last modified: Thu Apr 27 17:57:34 2023, max compression
```

## Comparing `athiruma-cloud-governance-1.1.89.tar` & `athiruma-cloud-governance-1.1.90.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.283676 athiruma-cloud-governance-1.1.89/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/LICENSE
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      100 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/MANIFEST.in
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-04-27 04:23:44.283676 athiruma-cloud-governance-1.1.89/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/README.md
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.272675 athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-04-27 04:23:44.000000 athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9295 2023-04-27 04:23:44.000000 athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/SOURCES.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-04-27 04:23:44.000000 athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/dependency_links.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-04-27 04:23:44.000000 athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/not-zip-safe
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      608 2023-04-27 04:23:44.000000 athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/requires.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-04-27 04:23:44.000000 athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/top_level.txt
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.273675 athiruma-cloud-governance-1.1.89/cloud_governance/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.273675 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.273675 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.273675 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10761 2023-04-26 13:57:03.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10983 2023-04-26 05:48:39.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3473 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11021 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5263 2023-04-26 05:48:39.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6612 2023-04-26 11:33:43.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.273675 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/monitor/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1439 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.273675 athiruma-cloud-governance-1.1.89/cloud_governance/common/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.273675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.274675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.274675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13290 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.274675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.274675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4589 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.274675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.274675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19858 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.274675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1797 2023-04-19 05:12:45.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/price.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11967 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/sts/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/utils/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3210 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/utils/utils.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1746 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/gcp/google_account.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.275675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.276675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.276675 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.276675 athiruma-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2523 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11528 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.276675 athiruma-cloud-governance-1.1.89/cloud_governance/common/google_drive/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/google_drive/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/google_drive/google_drive_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10366 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.276675 athiruma-cloud-governance-1.1.89/cloud_governance/common/jira/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/jira/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/jira/jira.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9134 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/jira/jira_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.277675 athiruma-cloud-governance-1.1.89/cloud_governance/common/ldap/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/ldap/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2500 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/ldap/ldap_search.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.277675 athiruma-cloud-governance-1.1.89/cloud_governance/common/logger/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/logger/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      466 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/logger/init_logger.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1578 2023-03-09 13:52:50.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/logger/logger_time_stamp.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.277675 athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-04-16 06:07:13.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/gmail.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15245 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/mail_message.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6165 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/postfix.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.277675 athiruma-cloud-governance-1.1.89/cloud_governance/common/tool/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/tool/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/common/tool/tool.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.278675 athiruma-cloud-governance-1.1.89/cloud_governance/main/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/main/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    18288 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/main/environment_variables.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/main/environment_variables_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/main/es_uploader.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16298 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/main/main.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      776 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/main/run_cloud_resource_orchestration.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.278675 athiruma-cloud-governance-1.1.89/cloud_governance/policy/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.279676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7428 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6305 2023-04-18 07:13:29.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_explorer.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15631 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5350 2023-03-03 18:04:44.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_in_use.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4452 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9741 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_idle.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_run.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8141 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_stop.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2538 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/empty_roles.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3027 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ip_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6776 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/monthly_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2906 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/nat_gateway_unused.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2839 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/s3_inactive.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5680 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/skipped_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51727 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3505 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_snapshots.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.279676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/azure/cost_billing_reports.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.279676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14218 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.280676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5384 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_baremetal.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4583 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_vm.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.280676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.280676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.280676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.280676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.281675 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25600 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3776 2023-04-19 05:44:11.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41752 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.281675 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8869 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-04-20 10:33:28.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11803 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6139 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.281675 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-03-22 05:22:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.282676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    27642 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9166 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14370 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.282676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17153 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1712 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.282676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.283676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1116 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.283676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3795 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.283676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.283676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 04:23:44.283676 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-04-27 04:23:44.318676 athiruma-cloud-governance-1.1.89/setup.cfg
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2928 2023-04-27 04:22:45.000000 athiruma-cloud-governance-1.1.89/setup.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.887103 athiruma-cloud-governance-1.1.90/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/LICENSE
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      100 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/MANIFEST.in
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-04-27 17:57:34.887103 athiruma-cloud-governance-1.1.90/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/README.md
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.855103 athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-04-27 17:57:34.000000 athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9295 2023-04-27 17:57:34.000000 athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/SOURCES.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-04-27 17:57:34.000000 athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/dependency_links.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-04-27 17:57:34.000000 athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/not-zip-safe
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      608 2023-04-27 17:57:34.000000 athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/requires.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-04-27 17:57:34.000000 athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/top_level.txt
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.855103 athiruma-cloud-governance-1.1.90/cloud_governance/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.855103 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.855103 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.856103 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    12298 2023-04-27 17:56:57.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10983 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3473 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11021 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5317 2023-04-27 17:56:57.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6612 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.856103 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1439 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.856103 athiruma-cloud-governance-1.1.90/cloud_governance/common/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.856103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.856103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.856103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13290 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.856103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.857103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4803 2023-04-27 17:56:57.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.857103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.857103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19858 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.857103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1797 2023-04-19 05:12:45.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.857103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/price.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11967 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/sts/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3210 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/utils.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1746 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/google_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.858103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.859103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.859103 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.859103 athiruma-cloud-governance-1.1.90/cloud_governance/common/elasticsearch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/elasticsearch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2523 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11528 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.860103 athiruma-cloud-governance-1.1.90/cloud_governance/common/google_drive/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/google_drive/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10366 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.860103 athiruma-cloud-governance-1.1.90/cloud_governance/common/jira/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/jira/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/jira/jira.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9134 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/jira/jira_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.860103 athiruma-cloud-governance-1.1.90/cloud_governance/common/ldap/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/ldap/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2500 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/ldap/ldap_search.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.861103 athiruma-cloud-governance-1.1.90/cloud_governance/common/logger/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/logger/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      466 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/logger/init_logger.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1578 2023-03-09 13:52:50.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/logger/logger_time_stamp.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.861103 athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-04-16 06:07:13.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/gmail.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15245 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/mail_message.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6165 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/postfix.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.861103 athiruma-cloud-governance-1.1.90/cloud_governance/common/tool/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/tool/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/common/tool/tool.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.862103 athiruma-cloud-governance-1.1.90/cloud_governance/main/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/main/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    18288 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/main/environment_variables.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/main/environment_variables_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/main/es_uploader.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16298 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/main/main.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      776 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/main/run_cloud_resource_orchestration.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.862103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.864103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7428 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6305 2023-04-18 07:13:29.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15631 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5350 2023-03-03 18:04:44.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_in_use.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4452 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9741 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_idle.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_run.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8141 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_stop.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2538 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/empty_roles.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3027 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ip_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6776 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/monthly_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2906 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/nat_gateway_unused.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2839 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/s3_inactive.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5680 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/skipped_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51727 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3505 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_snapshots.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.865103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/azure/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.865103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14218 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.866103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5384 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4583 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_vm.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.866103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.866103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.866103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.866103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.870103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25600 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3776 2023-04-19 05:44:11.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41752 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.871103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8869 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-04-20 10:33:28.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11803 2023-04-27 16:28:58.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6139 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.871103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-03-22 05:22:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.884103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    27642 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9166 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14370 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.885103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17153 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1712 2023-04-25 12:08:40.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.885103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.885103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1116 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.885103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3795 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.886103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.886103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-04-27 17:57:34.886103 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-04-27 17:57:34.887103 athiruma-cloud-governance-1.1.90/setup.cfg
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2928 2023-04-27 17:57:28.000000 athiruma-cloud-governance-1.1.90/setup.py
```

### Comparing `athiruma-cloud-governance-1.1.89/LICENSE` & `athiruma-cloud-governance-1.1.90/LICENSE`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/PKG-INFO` & `athiruma-cloud-governance-1.1.90/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiruma-cloud-governance
-Version: 1.1.89
+Version: 1.1.90
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `athiruma-cloud-governance-1.1.89/README.md` & `athiruma-cloud-governance-1.1.90/README.md`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/PKG-INFO` & `athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiruma-cloud-governance
-Version: 1.1.89
+Version: 1.1.90
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/SOURCES.txt` & `athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/athiruma_cloud_governance.egg-info/requires.txt` & `athiruma-cloud-governance-1.1.90/athiruma_cloud_governance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py`

 * *Files 12% similar despite different names*

```diff
@@ -168,14 +168,38 @@
                     source['ticket_opened_date'] = ticket_opened_date.date()
                     source['forecast'] = user_forecast
                     source['user'] = user
                     self.__cost_over_usage.es_operations.upload_to_elasticsearch(index=self.__es_index_cro, data=source, id=ticket_id)
                     upload_data[ticket_id] = source
         return upload_data
 
+    @logger_time_stamp
+    def update_in_progress_ticket_cost(self):
+        """
+        This method updates the in-progress tickets costs
+        :return:
+        """
+        query = {"query": {"match_phrase": {"ticket_id_state.keyword": "in-progress"}}}
+        in_progress_es_tickets = self.__cost_over_usage.es_operations.fetch_data_by_es_query(query=query, es_index=self.__es_index_cro)
+        for in_progress_ticket in in_progress_es_tickets:
+            source_data = in_progress_ticket.get('_source')
+            ticket_id = source_data.get('ticket_id')
+            if source_data.get('account_name').lower() in self.__account_name.lower():
+                user = source_data.get('user', '')
+                if not user:
+                    user = source_data.get('user_cro')
+                ticket_opened_date = datetime.strptime(source_data.get('ticket_opened_date'), "%Y-%m-%d")
+                duration = int(source_data.get('duration', 0))
+                user_project = source_data.get('project')
+                user_cost = self.get_user_cost_data(user, requested_date=ticket_opened_date, user_project=user_project)
+                user_forecast = self.get_user_cost_data(user, requested_date=datetime.utcnow(), user_project=user_project, forecast=True, duration=duration)
+                source_data['actual_cost'] = user_cost
+                source_data['forecast'] = user_forecast
+                self.__cost_over_usage.es_operations.upload_to_elasticsearch(index=self.__es_index_cro, data=source_data, id=ticket_id)
+
     @typeguard.typechecked
     @logger_time_stamp
     def run(self, monitor_data: dict):
         """
         This method run data collection methods
         :param monitor_data:
         :return:
```

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,18 @@
         This method start the cro process methods
         1. Send alert to cost over usage users
         2. Tag the new instances
         3. monitor and upload the new instances' data
         4. Monitor the Jira ticket progressing
         :return:
         """
-        # self.send_cro_alerts()
+        self.send_cro_alerts()
         self.run_cloud_resources()
-        # self.save_current_timestamp()
+        self.cro_reports.update_in_progress_ticket_cost()
+        self.save_current_timestamp()
 
     @logger_time_stamp
     def run(self):
         """
         This method start the aws CRO operations
         :return:
         """
```

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime, timedelta
 
 import boto3
 
+from cloud_governance.common.logger.init_logger import logger
+
 
 class CostExplorerOperations:
     """
     This class extracts the price data from AWS Cost Explorer
     """
 
     START_DAY = 1
@@ -88,15 +90,19 @@
         This method return the cost forecasting
         @param start_date:
         @param end_date:
         @param granularity:
         @param cost_metric:
         @return:
         """
-        return self.cost_explorer_client.get_cost_forecast(
-            TimePeriod={
-                'Start': start_date,
-                'End': end_date
-            },
-            Granularity=granularity,
-            Metric=cost_metric, **kwargs
-        )
+        try:
+            return self.cost_explorer_client.get_cost_forecast(
+                TimePeriod={
+                    'Start': start_date,
+                    'End': end_date
+                },
+                Granularity=granularity,
+                Metric=cost_metric, **kwargs
+            )
+        except Exception as err:
+            logger.info(err)
+            return {'Total': {'Amount': 0}}
```

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/price.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/aws/utils/utils.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/gcp/google_account.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/google_account.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elastic_upload.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/google_drive/google_drive_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/google_drive/upload_to_gsheet.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/jira/jira.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/jira/jira_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/jira/jira_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/ldap/ldap_search.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/logger/logger_time_stamp.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/gmail.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/mail_message.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/mail_message.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/common/mails/postfix.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/common/mails/postfix.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/main/environment_variables.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/main/environment_variables.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/main/es_uploader.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/main/main.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/main/main.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/main/run_cloud_resource_orchestration.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/main/run_cloud_resource_orchestration.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_explorer.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_explorer_payer_billings.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer_payer_billings.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/cost_over_usage.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_in_use.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ebs_unattached.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_idle.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_idle.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_run.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ec2_stop.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_stop.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/empty_roles.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/empty_roles.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/ip_unattached.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/ip_unattached.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/monthly_report.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/monthly_report.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/nat_gateway_unused.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/nat_gateway_unused.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/s3_inactive.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/s3_inactive.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/skipped_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/skipped_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_cluster_resource.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/aws/zombie_snapshots.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/azure/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/gcp/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/gcp/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/ibm_cost_report.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_baremetal.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/ibm/tag_vm.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_vm.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `athiruma-cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.89/setup.py` & `athiruma-cloud-governance-1.1.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.89'
+__version__ = '1.1.90'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

