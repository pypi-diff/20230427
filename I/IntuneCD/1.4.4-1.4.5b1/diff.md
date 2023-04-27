# Comparing `tmp/IntuneCD-1.4.4.tar.gz` & `tmp/IntuneCD-1.4.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.4.tar", last modified: Tue Apr  4 10:48:47 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.5b1.tar", last modified: Wed Apr 26 11:12:03 2023, max compression
```

## Comparing `IntuneCD-1.4.4.tar` & `IntuneCD-1.4.5b1.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:48:47.280986 IntuneCD-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-04 10:48:47.280986 IntuneCD-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-04 10:48:47.284987 IntuneCD-1.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:48:47.256985 IntuneCD-1.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:48:47.276986 IntuneCD-1.4.4/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_apns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/run_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:48:47.280986 IntuneCD-1.4.4/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-04 10:48:47.000000 IntuneCD-1.4.4/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-04 10:48:47.000000 IntuneCD-1.4.4/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:48:47.000000 IntuneCD-1.4.4/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-04 10:48:47.000000 IntuneCD-1.4.4/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-04 10:48:47.000000 IntuneCD-1.4.4/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 10:48:47.000000 IntuneCD-1.4.4/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:48:47.280986 IntuneCD-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_get_added_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_group_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-04 10:48:35.000000 IntuneCD-1.4.4/tests/test_update_frontend.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.188841 IntuneCD-1.4.5b1/
+-rw-r--r--   0 tobias     (501) staff       (20)     1059 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/LICENSE
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-26 11:12:03.188928 IntuneCD-1.4.5b1/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     2697 2023-01-24 09:42:37.000000 IntuneCD-1.4.5b1/README.md
+-rw-r--r--   0 tobias     (501) staff       (20)      103 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b1/pyproject.toml
+-rw-r--r--   0 tobias     (501) staff       (20)      999 2023-04-26 11:12:03.189267 IntuneCD-1.4.5b1/setup.cfg
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.158575 IntuneCD-1.4.5b1/src/
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.183579 IntuneCD-1.4.5b1/src/IntuneCD/
+-rw-r--r--   0 tobias     (501) staff       (20)        0 2022-05-03 19:33:01.000000 IntuneCD-1.4.5b1/src/IntuneCD/__init__.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2344 2023-04-26 08:18:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3938 2023-03-20 07:54:18.000000 IntuneCD-1.4.5b1/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2241 2023-04-24 14:54:23.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1327 2023-04-24 14:55:45.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2665 2023-04-24 14:48:58.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1865 2023-04-24 15:05:44.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4651 2023-04-24 14:59:21.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1370 2023-04-24 15:09:16.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1090 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2473 2023-04-24 15:00:03.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1454 2023-04-24 15:11:10.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1655 2023-04-24 15:17:25.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2386 2023-04-24 15:16:50.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2718 2023-04-24 15:16:10.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1245 2023-04-24 15:01:01.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2359 2023-04-24 15:08:23.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2926 2023-04-24 15:07:34.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2508 2023-04-24 15:04:54.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1378 2023-04-24 15:09:54.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2467 2023-04-24 15:10:36.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1445 2023-04-24 15:11:43.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1754 2023-04-24 15:02:06.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2710 2023-04-24 15:14:33.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3289 2023-04-24 15:13:25.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4962 2023-04-26 06:18:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1486 2023-04-24 15:12:12.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2589 2023-04-24 15:15:17.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1312 2023-04-24 14:57:10.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1961 2023-04-24 15:06:47.000000 IntuneCD-1.4.5b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)      548 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b1/src/IntuneCD/check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      515 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b1/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1933 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)    15819 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b1/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3701 2023-03-08 08:59:36.000000 IntuneCD-1.4.5b1/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3198 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10342 2023-04-03 08:56:31.000000 IntuneCD-1.4.5b1/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7753 2023-04-26 06:19:45.000000 IntuneCD-1.4.5b1/src/IntuneCD/graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)      622 2022-08-09 15:09:09.000000 IntuneCD-1.4.5b1/src/IntuneCD/load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      987 2023-04-25 09:24:15.000000 IntuneCD-1.4.5b1/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12362 2023-04-26 06:16:38.000000 IntuneCD-1.4.5b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12356 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10507 2023-04-03 08:56:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/run_update.py
+-rw-r--r--   0 tobias     (501) staff       (20)      934 2023-03-06 07:57:06.000000 IntuneCD-1.4.5b1/src/IntuneCD/save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8139 2023-04-26 06:20:45.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7924 2023-04-26 06:20:55.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3524 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7443 2023-03-06 09:55:38.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3741 2023-04-25 08:44:13.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9333 2023-04-26 06:21:22.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7166 2023-04-26 06:22:17.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7662 2023-04-26 06:22:59.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8890 2023-04-26 06:23:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2630 2023-03-20 12:09:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)    11609 2023-04-26 06:24:16.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8676 2023-04-26 06:25:08.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)      749 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 tobias     (501) staff       (20)    24247 2023-04-26 06:25:49.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9030 2023-04-26 06:27:25.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8039 2023-04-26 06:28:00.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8389 2023-04-26 06:28:30.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10573 2023-04-26 06:29:03.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    16073 2023-04-26 06:29:38.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8346 2023-04-26 06:30:03.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7158 2023-04-26 06:30:40.000000 IntuneCD-1.4.5b1/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.184508 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     3153 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        1 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      179 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      102 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        9 2023-04-26 11:12:03.000000 IntuneCD-1.4.5b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-04-26 11:12:03.188651 IntuneCD-1.4.5b1/tests/
+-rw-r--r--   0 tobias     (501) staff       (20)     2042 2023-04-26 06:14:42.000000 IntuneCD-1.4.5b1/tests/test_archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2005 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      848 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2096 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7233 2023-04-04 06:15:28.000000 IntuneCD-1.4.5b1/tests/test_documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)      953 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_get_added_removed.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9753 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12241 2023-03-08 09:16:49.000000 IntuneCD-1.4.5b1/tests/test_graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)    14412 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2980 2023-03-08 10:43:23.000000 IntuneCD-1.4.5b1/tests/test_group_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1279 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1622 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_match.py
+-rw-r--r--   0 tobias     (501) staff       (20)      559 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1888 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2292 2023-01-24 09:42:30.000000 IntuneCD-1.4.5b1/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.4/LICENSE` & `IntuneCD-1.4.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/PKG-INFO` & `IntuneCD-1.4.5b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.4
+Version: 1.4.5b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.4/README.md` & `IntuneCD-1.4.5b1/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/setup.cfg` & `IntuneCD-1.4.5b1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.4
+version = 1.4.5.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.5b1/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_AppProtection.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,39 +20,48 @@
     Saves all App Protection policies in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: List of policies to exclude from the backup
     :param token: Token to use for authenticating the request
     """
-    config_count = 0
+
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "App Protection/"
     data = makeapirequest(ENDPOINT, token)
 
-    assignment_responses = batch_assignment(data, "deviceAppManagement/", "/assignments", token, app_protection=True)
+    assignment_responses = batch_assignment(
+        data, "deviceAppManagement/", "/assignments", token, app_protection=True
+    )
 
     # If profile is ManagedAppConfiguration, skip to next
     for profile in data["value"]:
         if profile["@odata.type"] == "#microsoft.graph.targetedManagedAppConfiguration":
             continue
 
-        config_count += 1
+        results["config_count"] += 1
 
         if "assignments" not in exclude:
             assignments = get_object_assignment(profile["id"], assignment_responses)
             if assignments:
                 profile["assignments"] = assignments
 
         profile = remove_keys(profile)
 
         print("Backing up App Protection: " + profile["displayName"])
 
         if "targetedAppManagementLevels" in profile:
-            fname = clean_filename(f"{profile['displayName']}_{profile['targetedAppManagementLevels']}")
+            fname = clean_filename(
+                f"{profile['displayName']}_{profile['targetedAppManagementLevels']}"
+            )
         else:
-            fname = clean_filename(f"{profile['displayName']}_{str(profile['@odata.type'].split('.')[2])}")
+            fname = clean_filename(
+                f"{profile['displayName']}_{str(profile['@odata.type'].split('.')[2])}"
+            )
 
         # Save App Protection as JSON or YAML depending on configured value in
         # "-o"
         save_output(output, configpath, fname, profile)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_managedGPlay.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python3
 
 """
-This module backs up Apple Push Notification setting in Intune.
+This module backs up Managed Google Play setting in Intune.
 """
 
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
 from .save_output import save_output
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate"
+ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings"
 
 
-# Get APNs information and save in specified path
+# Get Managed Google Play information and save in specified path
 def savebackup(path, output, token):
     """
-    Save Apple Push Notification setting to a JSON or YAML file.
+    Saves Managed Google Play information in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
-
-    configpath = path + "/" + "Apple Push Notification/"
+    results = {"config_count": 0, "outputs": []}
+    configpath = f"{path}/Managed Google Play/"
     data = makeapirequest(ENDPOINT, token)
 
     if data:
-        config_count += 1
+        results["config_count"] += 1
         data = remove_keys(data)
-        print("Backing up Apple Push Notification: " + data["appleIdentifier"])
+        print("Backing up Managed Google Play: " + data["ownerUserPrincipalName"])
 
         # Get filename without illegal characters
-        fname = clean_filename(data["appleIdentifier"])
-        # Save APNs as JSON or YAML depending on configured value in "-o"
+        fname = clean_filename(data["ownerUserPrincipalName"])
+        # Save Managed Google Play as JSON or YAML depending on configured
+        # value in "-o"
         save_output(output, configpath, fname, data)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_appConfiguration.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "App Configuration/"
     data = makeapirequest(ENDPOINT, token)
 
     if data["value"]:
         assignment_responses = batch_assignment(
             data, "deviceAppManagement/mobileAppConfigurations/", "/assignments", token
         )
 
         for profile in data["value"]:
-            config_count += 1
+            results["config_count"] += 1
             if "assignments" not in exclude:
                 assignments = get_object_assignment(profile["id"], assignment_responses)
                 if assignments:
                     profile["assignments"] = assignments
 
             profile = remove_keys(profile)
 
@@ -64,8 +64,10 @@
             fname = clean_filename(
                 f"{profile['displayName']}_{str(profile['@odata.type'].split('.')[2])}"
             )
             # Save App Configuration as JSON or YAML depending on configured value
             # in "-o"
             save_output(output, configpath, fname, profile)
 
-    return config_count
+            results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,34 +20,39 @@
     Saves all Apple Enrollment Profiles in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Enrollment Profiles/Apple/"
     data = makeapirequest(ENDPOINT, token)
 
     if data["value"]:
         profile_ids = []
         for profile in data["value"]:
             profile_ids.append(profile["id"])
 
         batch_profile_data = batch_request(
-            profile_ids, "deviceManagement/depOnboardingSettings/", "/enrollmentProfiles", token
+            profile_ids,
+            "deviceManagement/depOnboardingSettings/",
+            "/enrollmentProfiles",
+            token,
         )
 
         for profile in batch_profile_data:
-            config_count += 1
+            results["config_count"] += 1
             for value in profile["value"]:
                 value = remove_keys(value)
 
                 print("Backing up Apple enrollment profile: " + value["displayName"])
 
                 # Get filename without illegal characters
                 fname = clean_filename(value["displayName"])
                 # Save Apple Enrollment Profile as JSON or YAML depending on
                 # configured value in "-o"
                 save_output(output, configpath, fname, value)
 
-    return config_count
+                results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_applications.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,47 +42,65 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
 
     data = makeapirequest(ENDPOINT, token, q_param)
-    assignment_responses = batch_assignment(data, "deviceAppManagement/mobileApps/", "/assignments", token)
+    assignment_responses = batch_assignment(
+        data, "deviceAppManagement/mobileApps/", "/assignments", token
+    )
 
     for app in data["value"]:
         app_name = ""
         platform = ""
-        config_count += 1
+        results["config_count"] += 1
 
         if "assignments" not in exclude:
             assignments = get_object_assignment(app["id"], assignment_responses)
             if assignments:
                 app["assignments"] = assignments
 
         app = remove_keys(app)
         app.pop("description", None)
 
         # If app type is VPP, add Apple ID to the name as the app can exist
         # multiple times
         if app["@odata.type"] == "#microsoft.graph.iosVppApp":
-            app_name = app["displayName"] + "_iOSVppApp_" + str(app["vppTokenAppleId"].split("@")[0])
+            app_name = (
+                app["displayName"]
+                + "_iOSVppApp_"
+                + str(app["vppTokenAppleId"].split("@")[0])
+            )
         elif app["@odata.type"] == "#microsoft.graph.macOsVppApp":
-            app_name = app["displayName"] + "_macOSVppApp_" + str(app["vppTokenAppleId"].split("@")[0])
+            app_name = (
+                app["displayName"]
+                + "_macOSVppApp_"
+                + str(app["vppTokenAppleId"].split("@")[0])
+            )
         # If app type is Win32 or MSI, add version to the name as multiple
         # versions can exist
         elif app["@odata.type"] == "#microsoft.graph.win32LobApp":
             if app["displayVersion"] is None:
                 app_name = app["displayName"] + "_Win32"
             else:
-                app_name = app["displayName"] + "_Win32_" + str(app["displayVersion"]).replace(".", "_")
+                app_name = (
+                    app["displayName"]
+                    + "_Win32_"
+                    + str(app["displayVersion"]).replace(".", "_")
+                )
         elif app["@odata.type"] == "#microsoft.graph.windowsMobileMSI":
-            app_name = app["displayName"] + "_WinMSI_" + str(app["productVersion"]).replace(".", "_")
+            app_name = (
+                app["displayName"]
+                + "_WinMSI_"
+                + str(app["productVersion"]).replace(".", "_")
+            )
         # If app is not VPP, Win32 or MSI only add the app type to the name
         else:
             app_name = app["displayName"] + "_" + str(app["@odata.type"].split(".")[2])
 
         # Get application platform
         if match("ios", str(app["@odata.type"]).lower()) is True:
             platform = "iOS"
@@ -106,8 +124,10 @@
         configpath = f"{path}/Applications/{platform}/"
 
         # Get filename without illegal characters
         fname = clean_filename(app_name)
 
         save_output(output, configpath, fname, app)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_assignmentFilters.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,24 +19,26 @@
     Saves all Filter in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Filters/"
     data = makeapirequest(ENDPOINT, token)
 
     if data:
         for assign_filter in data["value"]:
-            config_count += 1
+            results["config_count"] += 1
             assign_filter = remove_keys(assign_filter)
             print("Backing up Filter: " + assign_filter["displayName"])
 
             # Get filename without illegal characters
             fname = clean_filename(assign_filter["displayName"])
             # Save Filters as JSON or YAML depending on configured value in
             # "-o"
             save_output(output, configpath, fname, assign_filter)
 
-    return config_count
+            results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_compliance.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,37 +21,53 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Compliance Policies/Policies/"
-    q_param = {"$expand": "scheduledActionsForRule($expand=scheduledActionConfigurations)"}
+    q_param = {
+        "$expand": "scheduledActionsForRule($expand=scheduledActionConfigurations)"
+    }
     data = makeapirequest(ENDPOINT, token, q_param)
 
-    assignment_responses = batch_assignment(data, "deviceManagement/deviceCompliancePolicies/", "/assignments", token)
+    assignment_responses = batch_assignment(
+        data, "deviceManagement/deviceCompliancePolicies/", "/assignments", token
+    )
 
     for policy in data["value"]:
-        config_count += 1
+        results["config_count"] += 1
         print("Backing up compliance policy: " + policy["displayName"])
 
         if "assignments" not in exclude:
             assignments = get_object_assignment(policy["id"], assignment_responses)
             if assignments:
                 policy["assignments"] = assignments
 
         policy = remove_keys(policy)
         for rule in policy["scheduledActionsForRule"]:
             remove_keys(rule)
         if policy["scheduledActionsForRule"]:
-            for scheduled_config in policy["scheduledActionsForRule"][0]["scheduledActionConfigurations"]:
+            for scheduled_config in policy["scheduledActionsForRule"][0][
+                "scheduledActionConfigurations"
+            ]:
                 remove_keys(scheduled_config)
 
         # Get filename without illegal characters
         fname = clean_filename(policy["displayName"])
+
         # Save Compliance policy as JSON or YAML depending on configured value
         # in "-o"
-        save_output(output, configpath, f"{fname}_" + str(policy["@odata.type"].split(".")[2]), policy)
+        save_output(
+            output,
+            configpath,
+            f"{fname}_" + str(policy["@odata.type"].split(".")[2]),
+            policy,
+        )
+
+        results["outputs"].append(
+            f"{fname}_" + str(policy["@odata.type"].split(".")[2])
+        )
 
-    return config_count
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_compliancePartner.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,40 +6,44 @@
 
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
 from .save_output import save_output
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners"
+ENDPOINT = (
+    "https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners"
+)
 
 
 # Get all Compliance Partners and save them in specified path
 def savebackup(path, output, token):
     """
     Saves all Compliance Partners in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Partner Connections/Compliance/"
     data = makeapirequest(ENDPOINT, token)
 
     for partner in data["value"]:
         if partner["partnerState"] == "unknown":
             continue
 
-        config_count += 1
+        results["config_count"] += 1
         print("Backing up Compliance Partner: " + partner["displayName"])
 
         partner = remove_keys(partner)
 
         # Get filename without illegal characters
         fname = clean_filename(partner["displayName"])
         # Save Compliance policy as JSON or YAML depending on configured
         # value in "-o"
         save_output(output, configpath, fname, partner)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_conditionalAccess.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,28 +19,32 @@
     Saves all Conditional Access in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Conditional Access/"
     data = makeapirequest(ENDPOINT, token)
 
     if data["value"]:
         for policy in data["value"]:
-            config_count += 1
+            results["config_count"] += 1
             print("Backing up Conditional Access policy: " + policy["displayName"])
 
             policy = makeapirequest(f"{ENDPOINT}/{policy['id']}", token)
             if policy["grantControls"]:
-                policy["grantControls"].pop("authenticationStrength@odata.context", None)
+                policy["grantControls"].pop(
+                    "authenticationStrength@odata.context", None
+                )
             policy = remove_keys(policy)
 
             # Get filename without illegal characters
             fname = clean_filename(policy["displayName"])
             # Save Conditional Access as JSON or YAML depending on configured
             # value in "-o"
             save_output(output, configpath, fname, policy)
 
-    return config_count
+            results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_configurationPolicies.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 """
 This module backs up all Configuration Policies in Intune.
 """
 
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
-from .graph_batch import batch_assignment, get_object_assignment, batch_request, get_object_details
+from .graph_batch import (
+    batch_assignment,
+    get_object_assignment,
+    batch_request,
+    get_object_details,
+)
 from .save_output import save_output
 from .remove_keys import remove_keys
 
 # Set MS Graph base endpoint
 BASE_ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement"
 
 
@@ -21,26 +26,30 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Settings Catalog/"
     policies = makeapirequest(BASE_ENDPOINT + "/configurationPolicies", token)
     policy_ids = []
     for policy in policies["value"]:
         policy_ids.append(policy["id"])
 
-    assignment_responses = batch_assignment(policies, "deviceManagement/configurationPolicies/", "/assignments", token)
-    policy_settings_batch = batch_request(policy_ids, "deviceManagement/configurationPolicies/", "/settings", token)
+    assignment_responses = batch_assignment(
+        policies, "deviceManagement/configurationPolicies/", "/assignments", token
+    )
+    policy_settings_batch = batch_request(
+        policy_ids, "deviceManagement/configurationPolicies/", "/settings", token
+    )
 
     for policy in policies["value"]:
-        config_count += 1
+        results["config_count"] += 1
         name = policy["name"]
         print("Backing up configuration policy: " + name)
 
         settings = get_object_details(policy["id"], policy_settings_batch)
 
         if settings:
             policy["settings"] = settings
@@ -54,8 +63,10 @@
 
         # Get filename without illegal characters
         fname = clean_filename(name)
         # Save Configuration Policy as JSON or YAML depending on configured
         # value in "-o"
         save_output(output, configpath, fname, policy)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Custom Attributes/"
     data = makeapirequest(ENDPOINT, token)
     script_ids = []
     for script in data["value"]:
         script_ids.append(script["id"])
 
     assignment_responses = batch_assignment(
@@ -45,15 +45,15 @@
         token,
     )
     script_data_responses = batch_request(
         script_ids, "deviceManagement/deviceCustomAttributeShellScripts/", "", token
     )
 
     for script_data in script_data_responses:
-        config_count += 1
+        results["config_count"] += 1
         if "assignments" not in exclude:
             assignments = get_object_assignment(script_data["id"], assignment_responses)
             if assignments:
                 script_data["assignments"] = assignments
 
         script_data = remove_keys(script_data)
 
@@ -61,15 +61,17 @@
 
         # Get filename without illegal characters
         fname = clean_filename(script_data["displayName"])
 
         # Save Shell script as JSON or YAML depending on configured value in "-o"
         save_output(output, configpath, fname, script_data)
 
+        results["outputs"].append(fname)
+
         # Save Shell script data to the script data folder
         if not os.path.exists(configpath + "Script Data/"):
             os.makedirs(configpath + "Script Data/")
         decoded = base64.b64decode(script_data["scriptContent"]).decode("utf-8")
         f = open(configpath + "Script Data/" + script_data["fileName"], "w")
         f.write(decoded)
 
-    return config_count
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,23 +19,25 @@
     Save Device Management Setting to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
 
     configpath = path + "/" + "Device Management Settings/"
     data = makeapirequest(ENDPOINT, token)
 
     if data:
-        config_count += 1
+        results["config_count"] += 1
         data = remove_keys(data)
         print("Backing up Device Management Settings")
 
         # Get filename without illegal characters
         fname = clean_filename("settings")
         # Save settings as JSON or YAML depending on configured value in "-o"
         save_output(output, configpath, fname, data)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,53 +9,64 @@
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
 from .save_output import save_output
 from .remove_keys import remove_keys
 from .graph_batch import batch_assignment, get_object_assignment
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations"
+ENDPOINT = (
+    "https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations"
+)
 
 
 # Get all Enrollment Configurations and save them in specified path
 def savebackup(path, output, exclude, token):
     """
     Saves all Enrollment Configurations in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Enrollment Configurations/"
     data = makeapirequest(ENDPOINT, token)
 
-    assignment_responses = batch_assignment(data, "deviceManagement/deviceEnrollmentConfigurations/", "/assignments", token)
+    assignment_responses = batch_assignment(
+        data, "deviceManagement/deviceEnrollmentConfigurations/", "/assignments", token
+    )
 
     for config in data["value"]:
-        if config["@odata.type"] == "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration":
+        if (
+            config["@odata.type"]
+            == "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
+        ):
             continue
-        config_count += 1
+        results["config_count"] += 1
         config_type = config.get("deviceEnrollmentConfigurationType", None)
         config_type = config_type[0].upper() + config_type[1:]
         config_type = re.findall("[A-Z][^A-Z]*", config_type)
         config_type = " ".join(config_type)
 
         print(f"Backing up Enrollment Config {config_type}: " + config["displayName"])
 
         if "assignments" not in exclude:
             assignments = get_object_assignment(config["id"], assignment_responses)
             if assignments:
                 config["assignments"] = assignments
 
-        fname = clean_filename(f"{config['displayName']}_{str(config['@odata.type']).split('.')[2]}")
+        fname = clean_filename(
+            f"{config['displayName']}_{str(config['@odata.type']).split('.')[2]}"
+        )
 
         config = remove_keys(config)
 
         # Get filename without illegal characters
         fname = clean_filename(fname)
         # Save Enrollment Configuration as JSON or YAML depending on configured
         # value in "-o"
         save_output(output, configpath, fname, config)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,59 +7,71 @@
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
 from .graph_batch import batch_assignment, get_object_assignment
 from .save_output import save_output
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations"
+ENDPOINT = (
+    "https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations"
+)
 APP_ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/mobileApps"
 
 
 # Get all Windows Enrollment Status Page profiles and save them in specified path
 def savebackup(path, output, exclude, token):
     """
     Saves all Windows Enrollment Status Page profiles in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Enrollment Profiles/Windows/ESP/"
     data = makeapirequest(ENDPOINT, token)
 
-    assignment_responses = batch_assignment(data, "deviceManagement/deviceEnrollmentConfigurations/", "/assignments", token)
+    assignment_responses = batch_assignment(
+        data, "deviceManagement/deviceEnrollmentConfigurations/", "/assignments", token
+    )
 
     for profile in data["value"]:
-        if profile["@odata.type"] == "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration":
-            config_count += 1
+        if (
+            profile["@odata.type"]
+            == "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
+        ):
+            results["config_count"] += 1
             if "assignments" not in exclude:
                 assignments = get_object_assignment(profile["id"], assignment_responses)
                 if assignments:
                     profile["assignments"] = assignments
 
             profile = remove_keys(profile)
 
             # If the profile contains apps, get the name of the app
             if "selectedMobileAppIds" in profile:
                 app_ids = profile["selectedMobileAppIds"]
                 app_names = []
                 for app_id in app_ids:
                     app_data = makeapirequest(APP_ENDPOINT + "/" + app_id, token)
-                    app = {"name": app_data["displayName"], "type": app_data["@odata.type"]}
+                    app = {
+                        "name": app_data["displayName"],
+                        "type": app_data["@odata.type"],
+                    }
                     app_names.append(app)
                 if app_names:
                     profile.pop("selectedMobileAppIds", None)
                     profile["selectedMobileAppNames"] = app_names
 
             print("Backing up Enrollment Status Page: " + profile["displayName"])
 
             # Get filename without illegal characters
             fname = clean_filename(profile["displayName"])
             # Save Windows Enrollment Profile as JSON or YAML depending on
             # configured value in "-o"
             save_output(output, configpath, fname, profile)
 
-    return config_count
+            results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,28 +21,31 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Group Policy Configurations/"
     data = makeapirequest(ENDPOINT, token)
 
-    assignment_responses = batch_assignment(data, "deviceManagement/groupPolicyConfigurations/", "/assignments", token)
+    assignment_responses = batch_assignment(
+        data, "deviceManagement/groupPolicyConfigurations/", "/assignments", token
+    )
 
     for profile in data["value"]:
-        config_count += 1
-        definition_endpoint = f"{ENDPOINT}/{profile['id']}/definitionValues?$expand=definition"
+        results["config_count"] += 1
+        definition_endpoint = (
+            f"{ENDPOINT}/{profile['id']}/definitionValues?$expand=definition"
+        )
         # Get definitions
         definitions = makeapirequest(definition_endpoint, token)
 
         if definitions:
-
             profile["definitionValues"] = definitions["value"]
 
             for definition in profile["definitionValues"]:
                 presentation_endpoint = (
                     f"{ENDPOINT}/{profile['id']}/definitionValues/{definition['id']}/"
                     f"presentationValues?$expand=presentation "
                 )
@@ -59,8 +62,10 @@
         print("Backing up profile: " + profile["displayName"])
 
         # Get filename without illegal characters
         fname = clean_filename(profile["displayName"])
 
         save_output(output, configpath, fname, profile)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_vppTokens.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 #!/usr/bin/env python3
 
 """
-This module backs up Managed Google Play setting in Intune.
+This module backs up all VPP tokens in Intune.
 """
 
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
 from .save_output import save_output
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings"
+ENDPOINT = "https://graph.microsoft.com/beta/deviceAppManagement/vppTokens"
 
 
-# Get Managed Google Play information and save in specified path
+# Get all VPP tokens and save them in specified path
 def savebackup(path, output, token):
     """
-    Saves Managed Google Play information in Intune to a JSON or YAML file.
+    Save all VPP tokens in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
-    configpath = f"{path}/Managed Google Play/"
+    results = {"config_count": 0, "outputs": []}
+    configpath = f"{path}/Apple VPP Tokens/"
     data = makeapirequest(ENDPOINT, token)
 
-    if data:
-        config_count += 1
-        data = remove_keys(data)
-        print("Backing up Managed Google Play: " + data["ownerUserPrincipalName"])
+    for vpp_token in data["value"]:
+        results["config_count"] += 1
+        token_name = vpp_token["displayName"]
+        vpp_token = remove_keys(vpp_token)
+
+        print(f"Backing up VPP token: {token_name}")
 
         # Get filename without illegal characters
-        fname = clean_filename(data["ownerUserPrincipalName"])
-        # Save Managed Google Play as JSON or YAML depending on configured
-        # value in "-o"
-        save_output(output, configpath, fname, data)
+        fname = clean_filename(token_name)
+
+        # Save token as JSON or YAML depending on configured value in "-o"
+        save_output(output, configpath, fname, vpp_token)
+
+        results["outputs"].append(fname)
 
-    return config_count
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_managementIntents.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,41 +21,47 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Management Intents/"
     intents = makeapirequest(BASE_ENDPOINT + "/intents", token)
     templates = makeapirequest(TEMPLATE_ENDPOINT, token)
 
-    assignment_responses = batch_assignment(intents, "deviceManagement/intents/", "/assignments", token)
+    assignment_responses = batch_assignment(
+        intents, "deviceManagement/intents/", "/assignments", token
+    )
     intent_responses = batch_intents(intents, token)
 
     if intent_responses:
         for intent_value in intent_responses["value"]:
-            config_count += 1
+            results["config_count"] += 1
             print("Backing up Intent: " + intent_value["displayName"])
 
             for template in templates["value"]:
                 if intent_value["templateId"] == template["id"]:
                     template_type = template["displayName"]
 
             configpath = path + "/" + "Management Intents/" + template_type + "/"
 
             if "assignments" not in exclude:
-                assignments = get_object_assignment(intent_value["id"], assignment_responses)
+                assignments = get_object_assignment(
+                    intent_value["id"], assignment_responses
+                )
                 if assignments:
                     intent_value["assignments"] = assignments
 
             for setting in intent_value["settingsDelta"]:
                 setting.pop("id", None)
             intent_value.pop("id", None)
 
             # Get filename without illegal characters
             fname = clean_filename(intent_value["displayName"])
             # Save Intent as JSON or YAML depending on configured value in "-o"
             save_output(output, configpath, fname, intent_value)
 
-    return config_count
+            results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_managementPartner.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,27 +19,29 @@
     Saves Management Partner information in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Partner Connections/Management/"
     data = makeapirequest(ENDPOINT, token)
 
     for partner in data["value"]:
         if partner["isConfigured"] is False:
             continue
 
-        config_count += 1
+        results["config_count"] += 1
         print("Backing up Management Partner: " + partner["displayName"])
 
         partner = remove_keys(partner)
 
         # Get filename without illegal characters
         fname = clean_filename(partner["displayName"])
         # Save Compliance policy as JSON or YAML depending on configured
         # value in "-o"
         save_output(output, configpath, fname, partner)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_notificationTemplate.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,34 +6,36 @@
 
 from .clean_filename import clean_filename
 from .graph_request import makeapirequest
 from .save_output import save_output
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates"
+ENDPOINT = (
+    "https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates"
+)
 
 
 # Get all Notification Templates and save them in specified path
 def savebackup(path, output, token):
     """
     Saves all Notification Templates in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Compliance Policies/Message Templates/"
     q_param = "?$expand=localizedNotificationMessages"
     data = makeapirequest(ENDPOINT, token, q_param)
 
     for template in data["value"]:
-        config_count += 1
+        results["config_count"] += 1
         print("Backing up Notification message template: " + template["displayName"])
         q_param = "?$expand=localizedNotificationMessages"
         template_data = makeapirequest(ENDPOINT + "/" + template["id"], token, q_param)
 
         template_data = remove_keys(template_data)
 
         for locale in template_data["localizedNotificationMessages"]:
@@ -41,8 +43,10 @@
 
         # Get filename without illegal characters
         fname = clean_filename(template_data["displayName"])
         # Save Notification template as JSON or YAML depending on configured
         # value in "-o"
         save_output(output, configpath, fname, template_data)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_powershellScripts.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Scripts/Powershell/"
     data = makeapirequest(ENDPOINT, token)
     if data["value"]:
         script_ids = []
         for script in data["value"]:
             script_ids.append(script["id"])
 
@@ -40,15 +40,15 @@
             data, "deviceManagement/deviceManagementScripts/", "/assignments", token
         )
         script_data_responses = batch_request(
             script_ids, "deviceManagement/deviceManagementScripts/", "", token
         )
 
         for script_data in script_data_responses:
-            config_count += 1
+            results["config_count"] += 1
             if "assignments" not in exclude:
                 assignments = get_object_assignment(
                     script_data["id"], assignment_responses
                 )
                 if assignments:
                     script_data["assignments"] = assignments
 
@@ -58,15 +58,17 @@
 
             # Get filename without illegal characters
             fname = clean_filename(script_data["displayName"])
             # Save Powershell script as JSON or YAML depending on configured value
             # in "-o"
             save_output(output, configpath, fname, script_data)
 
+            results["outputs"].append(fname)
+
             # Save Powershell script data to the script data folder
             if not os.path.exists(configpath + "Script Data/"):
                 os.makedirs(configpath + "Script Data/")
             decoded = base64.b64decode(script_data["scriptContent"]).decode("utf-8")
             f = open(configpath + "Script Data/" + script_data["fileName"], "w")
             f.write(decoded)
 
-    return config_count
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,52 +24,64 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = f"{path}/Proactive Remediations/"
     data = makeapirequest(ENDPOINT, token)
     if data["value"]:
         pr_ids = []
         for script in data["value"]:
             pr_ids.append(script["id"])
 
-        assignment_responses = batch_assignment(data, "deviceManagement/deviceHealthScripts/", "/assignments", token)
-        pr_data_responses = batch_request(pr_ids, "deviceManagement/deviceHealthScripts/", "", token)
+        assignment_responses = batch_assignment(
+            data, "deviceManagement/deviceHealthScripts/", "/assignments", token
+        )
+        pr_data_responses = batch_request(
+            pr_ids, "deviceManagement/deviceHealthScripts/", "", token
+        )
 
         for pr_details in pr_data_responses:
             if "Microsoft" not in pr_details["publisher"]:
-                config_count += 1
+                results["config_count"] += 1
                 if "assignments" not in exclude:
-                    assignments = get_object_assignment(pr_details["id"], assignment_responses)
+                    assignments = get_object_assignment(
+                        pr_details["id"], assignment_responses
+                    )
                     if assignments:
                         pr_details["assignments"] = assignments
 
                 pr_details = remove_keys(pr_details)
 
                 print(f"Backing up Proactive Remediation: {pr_details['displayName']}")
 
                 # Get filename without illegal characters
                 fname = clean_filename(pr_details["displayName"])
 
                 # Save Proactive Remediation as JSON or YAML depending on
                 # configured value in "-o"
                 save_output(output, configpath, fname, pr_details)
 
+                results["outputs"].append(fname)
+
                 if not os.path.exists(f"{configpath}/Script Data"):
                     os.makedirs(f"{configpath}/Script Data")
 
                 # Save detection script to the Script Data folder
-                config_count += 1
-                decoded = base64.b64decode(pr_details["detectionScriptContent"]).decode("utf-8")
+                results["config_count"] += 1
+                decoded = base64.b64decode(pr_details["detectionScriptContent"]).decode(
+                    "utf-8"
+                )
                 f = open(f"{configpath}/Script Data/{fname}_DetectionScript.ps1", "w")
                 f.write(decoded)
                 # Save remediation script to the Script Data folder
-                config_count += 1
-                decoded = base64.b64decode(pr_details["remediationScriptContent"]).decode("utf-8")
+                results["config_count"] += 1
+                decoded = base64.b64decode(
+                    pr_details["remediationScriptContent"]
+                ).decode("utf-8")
                 f = open(f"{configpath}/Script Data/{fname}_RemediationScript.ps1", "w")
                 f.write(decoded)
 
-    return config_count
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_profiles.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,57 +24,64 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Device Configurations/"
     data = makeapirequest(ENDPOINT, token)
 
-    assignment_responses = batch_assignment(data, "deviceManagement/deviceConfigurations/", "/assignments", token)
+    assignment_responses = batch_assignment(
+        data, "deviceManagement/deviceConfigurations/", "/assignments", token
+    )
 
     for profile in data["value"]:
-        config_count += 1
+        results["config_count"] += 1
         if "assignments" not in exclude:
             assignments = get_object_assignment(profile["id"], assignment_responses)
             if assignments:
                 profile["assignments"] = assignments
 
         pid = profile["id"]
         profile = remove_keys(profile)
 
         print("Backing up profile: " + profile["displayName"])
 
         # Get filename without illegal characters
-        fname = clean_filename(f"{profile['displayName']}_{str(profile['@odata.type']).split('.')[2]}")
+        fname = clean_filename(
+            f"{profile['displayName']}_{str(profile['@odata.type']).split('.')[2]}"
+        )
 
         # If profile is custom macOS or iOS, decode the payload
         if (profile["@odata.type"] == "#microsoft.graph.macOSCustomConfiguration") or (
             profile["@odata.type"] == "#microsoft.graph.iosCustomConfiguration"
         ):
             decoded = base64.b64decode(profile["payload"]).decode("utf-8")
 
             if not os.path.exists(configpath + "/" + "mobileconfig/"):
                 os.makedirs(configpath + "/" + "mobileconfig/")
             # Save decoded payload as .mobileconfig
-            config_count += 1
-            f = open(configpath + "/" + "mobileconfig/" + profile["payloadFileName"], "w")
+            results["config_count"] += 1
+            f = open(
+                configpath + "/" + "mobileconfig/" + profile["payloadFileName"], "w"
+            )
             f.write(decoded)
             # Save Device Configuration as JSON or YAML depending on configured
             # value in "-o"
             save_output(output, configpath, fname, profile)
 
+            results["outputs"].append(fname)
+
         # If Device Configuration is custom Win10 and the OMA settings are
         # encrypted, get them in plain text
         elif profile["@odata.type"] == "#microsoft.graph.windows10CustomConfiguration":
             if profile["omaSettings"]:
                 if profile["omaSettings"][0]["isEncrypted"] is True:
-
                     omas = []
                     for setting in profile["omaSettings"]:
                         if setting["isEncrypted"]:
                             decoded_oma = {}
                             oma_value = makeapirequest(
                                 ENDPOINT
                                 + "/"
@@ -97,13 +104,17 @@
                     profile.pop("omaSettings")
                     profile["omaSettings"] = omas
 
             # Save Device Configuration as JSON or YAML depending on configured
             # value in "-o"
             save_output(output, configpath, fname, profile)
 
+            results["outputs"].append(fname)
+
         # If Device Configuration are not custom, save it as JSON or YAML
         # depending on configured value in "-o"
         else:
             save_output(output, configpath, fname, profile)
 
-    return config_count
+            results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,27 +19,29 @@
     Saves all Remote Assistance Partners in Intune to a JSON or YAML file.
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Partner Connections/Remote Assistance/"
     data = makeapirequest(ENDPOINT, token)
 
     for partner in data["value"]:
         if partner["onboardingStatus"] == "notOnboarded":
             continue
 
-        config_count += 1
+        results["config_count"] += 1
         print("Backing up Remote Assistance Partner: " + partner["displayName"])
 
         partner = remove_keys(partner)
 
         # Get filename without illegal characters
         fname = clean_filename(partner["displayName"])
         # Save Compliance policy as JSON or YAML depending on configured
         # value in "-o"
         save_output(output, configpath, fname, partner)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_shellScripts.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,30 +27,30 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Scripts/Shell/"
     data = makeapirequest(ENDPOINT, token)
     script_ids = []
     for script in data["value"]:
         script_ids.append(script["id"])
 
     assignment_responses = batch_assignment(
         data, "deviceManagement/deviceShellScripts/", "?$expand=assignments", token
     )
     script_data_responses = batch_request(
         script_ids, "deviceManagement/deviceShellScripts/", "", token
     )
 
     for script_data in script_data_responses:
-        config_count += 1
+        results["config_count"] += 1
         if "assignments" not in exclude:
             assignments = get_object_assignment(script_data["id"], assignment_responses)
             if assignments:
                 script_data["assignments"] = assignments
 
         script_data = remove_keys(script_data)
 
@@ -58,15 +58,17 @@
 
         # Get filename without illegal characters
         fname = clean_filename(script_data["displayName"])
 
         # Save Shell script as JSON or YAML depending on configured value in "-o"
         save_output(output, configpath, fname, script_data)
 
+        results["outputs"].append(fname)
+
         # Save Shell script data to the script data folder
         if not os.path.exists(configpath + "Script Data/"):
             os.makedirs(configpath + "Script Data/")
         decoded = base64.b64decode(script_data["scriptContent"]).decode("utf-8")
         f = open(configpath + "Script Data/" + script_data["fileName"], "w")
         f.write(decoded)
 
-    return config_count
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.5b1/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,24 +21,27 @@
 
     :param path: Path to save the backup to
     :param output: Format the backup will be saved as
     :param exclude: If "assignments" is in the list, it will not back up the assignments
     :param token: Token to use for authenticating the request
     """
 
-    config_count = 0
+    results = {"config_count": 0, "outputs": []}
     configpath = path + "/" + "Enrollment Profiles/Windows/"
     data = makeapirequest(ENDPOINT, token)
 
     assignment_responses = batch_assignment(
-        data, "deviceManagement/windowsAutopilotDeploymentProfiles/", "/assignments", token
+        data,
+        "deviceManagement/windowsAutopilotDeploymentProfiles/",
+        "/assignments",
+        token,
     )
 
     for profile in data["value"]:
-        config_count += 1
+        results["config_count"] += 1
         if "assignments" not in exclude:
             assignments = get_object_assignment(profile["id"], assignment_responses)
             if assignments:
                 profile["assignments"] = assignments
 
         profile = remove_keys(profile)
 
@@ -46,8 +49,10 @@
 
         # Get filename without illegal characters
         fname = clean_filename(profile["displayName"])
         # Save Windows Enrollment Profile as JSON or YAML depending on
         # configured value in "-o"
         save_output(output, configpath, fname, profile)
 
-    return config_count
+        results["outputs"].append(fname)
+
+    return results
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/check_file.py` & `IntuneCD-1.4.5b1/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.5b1/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.5b1/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.5b1/src/IntuneCD/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.5b1/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.5b1/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.5b1/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.5b1/src/IntuneCD/graph_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,14 +114,46 @@
         pass
     else:
         raise Exception(
             "Request failed with ", response.status_code, " - ", response.text
         )
 
 
+def makeapirequestDelete(
+    deleteEndpoint, token, q_param=None, jdata=None, status_code=200
+):
+    """
+    This function makes a DELETE request to the Microsoft Graph API.
+
+    :param deleteEndpoint: The endpoint to make the request to.
+    :param token: The token to use for authenticating the request.
+    :param q_param: The query parameters to use for the request.
+    :param jdata: The JSON data to use for the request.
+    :param status_code: The status code to expect from the request.
+    """
+
+    headers = {
+        "Content-Type": "application/json",
+        "Authorization": "Bearer {0}".format(token["access_token"]),
+    }
+
+    if q_param is not None:
+        response = requests.delete(
+            deleteEndpoint, headers=headers, params=q_param, data=jdata
+        )
+    else:
+        response = requests.delete(deleteEndpoint, headers=headers, data=jdata)
+    if response.status_code == status_code:
+        pass
+    else:
+        raise Exception(
+            "Request failed with ", response.status_code, " - ", response.text
+        )
+
+
 def makeapirequestPost(patchEndpoint, token, q_param=None, jdata=None, status_code=200):
     """
     This function makes a POST request to the Microsoft Graph API.
 
     :param patchEndpoint: The endpoint to make the request to.
     :param token: The token to use for authenticating the request.
     :param q_param: The query parameters to use for the request.
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/load_file.py` & `IntuneCD-1.4.5b1/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.5b1/src/IntuneCD/remove_keys.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,12 +31,13 @@
         "highestAvailableVersion",
         "token",
         "lastSyncDateTime",
         "isReadOnly",
         "secretReferenceValueId",
         "isEncrypted",
         "modifiedDateTime",
+        "deployedAppCount",
     }
     for k in keys:
         data.pop(k, None)
 
     return data
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.5b1/src/IntuneCD/run_backup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import sys
 import base64
 import argparse
 
 from io import StringIO
 from .get_authparams import getAuth
 from .update_frontend import update_frontend
+from .archive import move_to_archive
 
 REPO_DIR = os.environ.get("REPO_DIR")
 
 
 def start():
     parser = argparse.ArgumentParser(description="Save backup of Intune configurations")
     parser.add_argument(
@@ -151,155 +152,167 @@
         args.localauth,
         args.certauth,
         args.interactiveauth,
         tenant="DEV",
     )
 
     def run_backup(path, output, exclude, token):
-        config_count = 0
+        results = []
 
         if "AppConfigurations" not in exclude:
             from .backup_appConfiguration import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "AppProtection" not in exclude:
             from .backup_AppProtection import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "APNs" not in exclude:
             from .backup_apns import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "VPP" not in exclude:
             from .backup_vppTokens import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "Applications" not in exclude:
             from .backup_applications import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "Compliance" not in exclude:
             from .backup_compliance import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "DeviceManagementSettings" not in exclude:
             from .backup_deviceManagementSettings import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "NotificationTemplate" not in exclude:
             from .backup_notificationTemplate import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "Profiles" not in exclude:
             from .backup_profiles import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "GPOConfigurations" not in exclude:
             from .backup_groupPolicyConfiguration import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "AppleEnrollmentProfile" not in exclude:
             from .backup_appleEnrollmentProfile import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "WindowsEnrollmentProfile" not in exclude:
             from .backup_windowsEnrollmentProfile import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "EnrollmentStatusPage" not in exclude:
             from .backup_enrollmentStatusPage import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "EnrollmentConfigurations" not in exclude:
             from .backup_enrollmentConfigurations import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if args.autopilot == "True":
             from .backup_autopilotDevices import savebackup
 
             savebackup(path, output, token)
 
         if "Filters" not in exclude:
             from .backup_assignmentFilters import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "ManagedGooglePlay" not in exclude:
             from .backup_managedGPlay import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "Intents" not in exclude:
             from .backup_managementIntents import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "CompliancePartner" not in exclude:
             from .backup_compliancePartner import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "ManagementPartner" not in exclude:
             from .backup_managementPartner import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "RemoteAssistancePartner" not in exclude:
             from .backup_remoteAssistancePartner import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         if "ProactiveRemediation" not in exclude:
             from .backup_proactiveRemediation import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "PowershellScripts" not in exclude:
             from .backup_powershellScripts import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "ShellScripts" not in exclude:
             from .backup_shellScripts import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "CustomAttributes" not in exclude:
             from .backup_customAttributeShellScript import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "ConfigurationPolicies" not in exclude:
             from .backup_configurationPolicies import savebackup
 
-            config_count += savebackup(path, output, exclude, token)
+            results.append(savebackup(path, output, exclude, token))
 
         if "ConditionalAccess" not in exclude:
             from .backup_conditionalAccess import savebackup
 
-            config_count += savebackup(path, output, token)
+            results.append(savebackup(path, output, token))
 
         from .assignment_report import get_group_report
 
         get_group_report(path, output)
 
+        config_count = sum([result.get("config_count", 0) for result in results])
+
+        created_files = [
+            output
+            for result in results
+            if result.get("outputs", None)
+            for output in result.get("outputs", None)
+            if output is not None
+        ]
+
+        move_to_archive(path, created_files, output)
+
         return config_count
 
     if args.output == "json" or args.output == "yaml":
         if token is None:
             raise Exception("Token is empty, please check os.environ variables")
 
         if args.exclude:
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.5b1/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/run_update.py` & `IntuneCD-1.4.5b1/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/save_output.py` & `IntuneCD-1.4.5b1/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_appConfiguration.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all App Configuration Assignments in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 from .check_file import check_file
 from .load_file import load_file
 
@@ -68,14 +73,15 @@
                 if mem_data["value"]:
                     for val in mem_data["value"]:
                         if (
                             repo_data["@odata.type"] == val["@odata.type"]
                             and repo_data["displayName"] == val["displayName"]
                         ):
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 if data["value"]:
                     print("-" * 90)
                     mem_id = data["value"]["id"]
                     # Remove keys before using DeepDiff
                     data = remove_keys(data)
                     repo_data.pop("targetedMobileApps", None)
@@ -172,8 +178,18 @@
                             "App Configuration created with id: " + post_request["id"]
                         )
                     else:
                         print(
                             "App configured in App Configuration profile could not be found, skipping creation"
                         )
 
+        # If any App Configurations are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing App Configuration from Intune: " + val["displayName"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_appProtection.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all App Protection Policies in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 from .check_file import check_file
 from .load_file import load_file
 
@@ -81,19 +86,21 @@
                         ):
                             if (
                                 repo_data["targetedAppManagementLevels"]
                                 == val["targetedAppManagementLevels"]
                                 and repo_data["displayName"] == val["displayName"]
                             ):
                                 data["value"] = val
+                                mem_data["value"].remove(val)
                         elif (
                             repo_data["@odata.type"] == val["@odata.type"]
                             and repo_data["displayName"] == val["displayName"]
                         ):
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 if data["value"]:
                     print("-" * 90)
                     mem_id = data["value"]["id"]
                     # Remove keys before using DeepDiff
                     data["value"] = remove_keys(data["value"])
 
@@ -164,8 +171,20 @@
                                 f"deviceAppManagement/{platform}",
                                 "assign",
                                 token,
                                 status_code=204,
                             )
                         print("App Protection created with id: " + post_request["id"])
 
+        # If any App Protections are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing App Protection from Intune: " + val["displayName"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}managedAppPolicies/{val['id']}",
+                        token,
+                        status_code=204,
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_compliance.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all Compliance Policies in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .remove_keys import remove_keys
 from .load_file import load_file
 from .check_file import check_file
 from .diff_summary import DiffSummary
 
@@ -69,14 +74,15 @@
                 if mem_data["value"]:
                     for val in mem_data["value"]:
                         if (
                             repo_data["@odata.type"] == val["@odata.type"]
                             and repo_data["displayName"] == val["displayName"]
                         ):
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 if data["value"]:
                     print("-" * 90)
                     mem_id = data["value"]["id"]
                     data["value"] = remove_keys(data["value"])
 
                     if data["value"]["scheduledActionsForRule"]:
@@ -200,8 +206,18 @@
                                 "assign",
                                 token,
                             )
                         print(
                             "Compliance Policy created with id: " + post_request["id"]
                         )
 
+        # If any Compliance Policies are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing Compliance Policy from Intune: " + val["displayName"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_conditionalAccess.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all Conditional Access Policy's in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 
 # Set MS Graph endpoint
 ENDPOINT = "https://graph.microsoft.com/beta/identity/conditionalAccess/policies"
 
@@ -45,14 +50,15 @@
                 repo_data["conditions"].pop("users", None)
 
                 data = {"value": ""}
                 if mem_data["value"]:
                     for val in mem_data["value"]:
                         if repo_data["displayName"] == val["displayName"]:
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 # If Conditional Access policy exists, continue
                 if data["value"]:
                     if "id" not in data["value"]:
                         continue
                     print("-" * 90)
 
@@ -145,8 +151,21 @@
 
                         if post_request:
                             print(
                                 "Conditional Access policy created with id: "
                                 + post_request["id"]
                             )
 
+        # If any Conditional Access policy are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print(
+                    "Removing Conditional Access Policy from Intune: "
+                    + val["displayName"]
+                )
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=204
+                    )
+
     return diff_count
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_configurationPolicies.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all Settings Catalog assignments in Intune,
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPut, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPut,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
@@ -58,14 +63,15 @@
                 repo_data.pop("assignments", None)
 
                 data = {"value": ""}
                 if mem_data["value"]:
                     for val in mem_data["value"]:
                         if repo_data["name"] == val["name"]:
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 if (
                     "templateReference" in repo_data
                     and repo_data["templateReference"].get("templateDisplayName")
                     == "Endpoint detection and response"
                 ):
                     print("-" * 90)
@@ -134,14 +140,15 @@
                     print("-" * 90)
                     print(
                         "Configuration Policy not found, creating Policy: "
                         + repo_data["name"]
                     )
                     if report is False:
                         repo_data.pop("settingCount", None)
+                        repo_data.pop("creationSource", None)
                         request_json = json.dumps(repo_data)
                         post_request = makeapirequestPost(
                             ENDPOINT,
                             token,
                             q_param=None,
                             jdata=request_json,
                             status_code=201,
@@ -160,8 +167,18 @@
                                 token,
                             )
                         print(
                             "Configuration Policy created with id: "
                             + post_request["id"]
                         )
 
+        # If any Configuration Policies are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing Configuration Policy from Intune: " + val["name"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 """
 
 import json
 import os
 import base64
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
@@ -64,14 +69,15 @@
                 repo_data.pop("assignments", None)
 
                 data = {"value": ""}
                 if mem_shellScript["value"]:
                     for val in mem_shellScript["value"]:
                         if repo_data["displayName"] == val["displayName"]:
                             data["value"] = val
+                            mem_shellScript["value"].remove(val)
 
                 # If Custom Attribute Shell script exists, continue
                 if data["value"]:
                     print("-" * 90)
                     q_param = None
                     # Get Shell script details
                     mem_data = makeapirequest(
@@ -188,8 +194,18 @@
                                 post_request["id"],
                                 "deviceManagement/deviceManagementScripts",
                                 "assign",
                                 token,
                             )
                         print("Custom Attribute created with id: " + post_request["id"])
 
+        # If any Custom Attribute scripts are left in mem_shellScript, remove them from Intune as they are not in the repo
+        if mem_shellScript.get("value", None) is not None:
+            for val in mem_shellScript["value"]:
+                print("-" * 90)
+                print("Removing Custom Attribute from Intune: " + val["displayName"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 """
 
 import json
 import os
 import re
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .diff_summary import DiffSummary
 
@@ -83,31 +88,32 @@
                         ):
                             if (
                                 repo_data["@odata.type"] == val["@odata.type"]
                                 and repo_data["displayName"] == val["displayName"]
                                 and repo_data["platformType"] == val["platformType"]
                             ):
                                 data["value"] = val
+                                intune_data["value"].remove(val)
                         else:
                             if (
                                 repo_data["@odata.type"] == val["@odata.type"]
                                 and repo_data["displayName"] == val["displayName"]
                             ):
                                 data["value"] = val
+                                intune_data["value"].remove(val)
 
                 # If Enrollment Configuration exists, continue
                 if data["value"]:
                     print("-" * 90)
                     # Get Enrollment Configuration data from Intune
                     mem_id = data["value"]["id"]
                     mem_priority = data["value"]["priority"]
                     repo_priority = repo_data["priority"]
                     # Remove keys from data that should not be compared
                     data["value"] = remove_keys(data["value"])
-
                     if repo_priority != mem_priority and mem_priority != 0:
                         mem_priority = makeapirequest(
                             f"{ENDPOINT}/{mem_id}?$select=priority", token
                         ).get("priority", "")
                         if repo_priority != mem_priority:
                             print(
                                 f"Updating Enrollment Config {config_type} Priority: "
@@ -232,8 +238,26 @@
                                 token,
                             )
                         print(
                             f"Enrollment Config {config_type} created with id: "
                             + post_request["id"]
                         )
 
+        # If any Enrollment Configurations are left in intune_data, remove them from Intune as they are not in the repo
+        if intune_data.get("value", None) is not None:
+            for val in intune_data["value"]:
+                if (
+                    val["@odata.type"]
+                    == "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
+                ):
+                    continue
+                print("-" * 90)
+                print(
+                    "Removing Enrollment Configuration from Intune: "
+                    + val["displayName"]
+                )
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all Windows Enrollment Status Page Profiles in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
@@ -66,14 +71,15 @@
                 if mem_data["value"]:
                     for val in mem_data["value"]:
                         if (
                             repo_data["displayName"] == val["displayName"]
                             and repo_data["@odata.type"] == val["@odata.type"]
                         ):
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 # If Enrollment Status Page Profile exists, continue
                 if data["value"]:
                     print("-" * 90)
                     mem_id = data["value"]["id"]
                     # Remove keys before using DeepDiff
                     mem_data["value"][0] = remove_keys(mem_data["value"][0])
@@ -176,8 +182,27 @@
                                 status_code=200,
                             )
                         print(
                             "Enrollment Status Page profile created with id: "
                             + post_request["id"]
                         )
 
+        # If any ESP are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                if val["displayName"] == "All users and all devices":
+                    continue
+                if (
+                    val["@odata.type"]
+                    == "#microsoft.graph.windowsEnrollmentStatusPageConfiguration"
+                ):
+                    print("-" * 90)
+                    print(
+                        "Removing Enrollment Status Page profile from Intune: "
+                        + val["displayName"]
+                    )
+                    if report is False:
+                        makeapirequestDelete(
+                            f"{ENDPOINT}/{val['id']}", token, status_code=200
+                        )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all group policy configurations in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
@@ -414,14 +419,15 @@
                     # If display name and type matches, add Intune data to data variable
                     if (
                         repo_data["displayName"] == val["displayName"]
                         and repo_data["policyConfigurationIngestionType"]
                         == val["policyConfigurationIngestionType"]
                     ):
                         data = val
+                        mem_configs.remove(val)
 
             # If data was found, continue
             if data:
                 print("-" * 90)
                 mem_id = data["id"]
                 data = remove_keys(data)
 
@@ -560,8 +566,21 @@
                             token,
                         )
                     print(
                         "Group Policy Configuration created with id: "
                         + post_request["id"]
                     )
 
+        # If any Group Policy Configuration are left in mem_configs, remove them from Intune as they are not in the repo
+        if mem_configs is not None:
+            for val in mem_configs:
+                print("-" * 90)
+                print(
+                    "Removing Group Policy Configuration from Intune: "
+                    + val["displayName"]
+                )
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=204
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_managementIntents.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 import json
 import os
 import glob
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPost
+from .graph_request import makeapirequest, makeapirequestPost, makeapirequestDelete
 from .graph_batch import batch_intents, batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .load_file import load_file
 from .diff_summary import DiffSummary
 
 # Set MS Graph base endpoint
 BASE_ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement"
@@ -66,14 +66,15 @@
                 mem_data = {}
                 for intent in intent_responses["value"]:
                     if (
                         repo_data["displayName"] == intent["displayName"]
                         and repo_data["templateId"] == intent["templateId"]
                     ):
                         mem_data = intent
+                        intent_responses["value"].remove(intent)
 
                 if (
                     repo_data.get("templateId")
                     == "e44c2ca3-2f9a-400a-a113-6cc88efd773d"
                 ):
                     print(
                         "Endpoint detection and response is currently not supported..."
@@ -193,8 +194,18 @@
                                 "deviceManagement/intents",
                                 "assign",
                                 token,
                                 status_code=204,
                             )
                         print("Intent created with id: " + post_request["id"])
 
+        # If any Intents are left in intent_responses, remove them from Intune as they are not in the repo
+        if intent_responses.get("value", None) is not None:
+            for val in intent_responses["value"]:
+                print("-" * 90)
+                print("Removing Management Intent from Intune: " + val["displayName"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{BASE_ENDPOINT}/intents/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_notificationTemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 This module is used to update all Notification Templates in Intune.
 """
 
 import json
 import os
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
 ENDPOINT = (
@@ -30,15 +35,14 @@
     """
 
     diff_summary = []
     # Set Notification Template path
     configpath = path + "/" + "Compliance Policies/Message Templates/"
     # If Notification Template path exists, continue
     if os.path.exists(configpath):
-
         # Get notification templates
         mem_data = makeapirequest(ENDPOINT, token)
 
         for filename in os.listdir(configpath):
             file = check_file(configpath, filename)
             if file is False:
                 continue
@@ -46,16 +50,19 @@
             # and set query parameter
             with open(file) as f:
                 repo_data = load_file(filename, f)
 
                 data = {"value": ""}
                 if mem_data["value"]:
                     for val in mem_data["value"]:
+                        if val["displayName"] == "EnrollmentNotificationInternalMEO":
+                            continue
                         if repo_data["displayName"] == val["displayName"]:
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 # If Notification Template exists, continue
                 if data["value"]:
                     print("-" * 90)
                     # Get Notification Template data from Intune
                     q_param = "?$expand=localizedNotificationMessages"
                     mem_template_data = makeapirequest(
@@ -166,8 +173,22 @@
                                 status_code=200,
                             )
                         print(
                             "Notification template created with id: "
                             + template_post_request["id"]
                         )
 
+        # If any Notification Template are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                if val["displayName"] == "EnrollmentNotificationInternalMEO":
+                    continue
+                print("-" * 90)
+                print(
+                    "Removing Notification template from Intune: " + val["displayName"]
+                )
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_shellScripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 #!/usr/bin/env python3
 
 """
-This module is used to update all PowerShell scripts in Intune.
+This module is used to update all Shell Scripts in Intune.
 """
 
 import json
 import os
 import base64
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts"
+ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts"
+ASSIGNMENT_ENDPOINT = (
+    "https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts"
+)
 
 
 def update(path, token, assignment=False, report=False, create_groups=False):
     """
-    This function updates all Powershell scripts in Intune if,
-    the configuration in Intune differs from the JSON/YAML file.
+    This function updates all Shell scripts in Intune if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
     """
 
     diff_summary = []
-    # Set Powershell script path
-    configpath = path + "/" + "Scripts/Powershell"
-    # If Powershell script path exists, continue
+    # Set Shell scritp path
+    configpath = path + "/" + "Scripts/Shell"
+    # If Shell script path exists, continue
     if os.path.exists(configpath):
         # Get scripts
-        mem_powershellScript = makeapirequest(ENDPOINT, token)
+        mem_shellScript = makeapirequest(ENDPOINT, token)
         # Get current assignment
         mem_assignments = batch_assignment(
-            mem_powershellScript,
+            mem_shellScript,
             "deviceManagement/deviceManagementScripts/",
             "/assignments",
             token,
         )
 
         for filename in os.listdir(configpath):
             file = check_file(configpath, filename)
@@ -58,23 +65,25 @@
                 # Create object to pass in to assignment function
                 assign_obj = {}
                 if "assignments" in repo_data:
                     assign_obj = repo_data["assignments"]
                 repo_data.pop("assignments", None)
 
                 data = {"value": ""}
-                if mem_powershellScript["value"]:
-                    for val in mem_powershellScript["value"]:
+                if mem_shellScript["value"]:
+                    for val in mem_shellScript["value"]:
                         if repo_data["displayName"] == val["displayName"]:
                             data["value"] = val
+                            mem_shellScript["value"].remove(val)
 
-                # If Powershell script exists, continue
+                # If Shell script exists, continue
                 if data["value"]:
                     print("-" * 90)
-                    # Get Powershell script details
+                    q_param = None
+                    # Get Shell script details
                     mem_data = makeapirequest(
                         ENDPOINT + "/" + data["value"]["id"], token
                     )
                     mem_id = mem_data["id"]
                     # Remove keys before using DeepDiff
                     mem_data = remove_keys(mem_data)
 
@@ -99,34 +108,34 @@
                             repo_data,
                             ignore_order=True,
                             exclude_paths="root['scriptContent']",
                         ).get("values_changed", {})
 
                         # If any changed values are found, push them to Intune
                         if pdiff or cdiff and report is False:
-                            powershell_bytes = repo_payload_config.encode("utf-8")
+                            shell_bytes = repo_payload_config.encode("utf-8")
                             repo_data["scriptContent"] = base64.b64encode(
-                                powershell_bytes
+                                shell_bytes
                             ).decode("utf-8")
                             request_data = json.dumps(repo_data)
                             q_param = None
                             makeapirequestPatch(
                                 ENDPOINT + "/" + mem_id, token, q_param, request_data
                             )
 
                         diff_config = DiffSummary(
                             data=cdiff,
                             name=repo_data["displayName"],
-                            type="Powershell Script",
+                            type="Shell Script",
                         )
 
                         diff_script = DiffSummary(
                             data=pdiff,
                             name="",
-                            type="Powershell Script",
+                            type="Shell Script",
                             message="Script changed, check commit history for details",
                             notify=False,
                         )
 
                         diff_config.diffs += diff_script.diffs
                         diff_config.count += diff_script.count
 
@@ -143,19 +152,19 @@
                                 request_data,
                                 mem_id,
                                 "deviceManagement/deviceManagementScripts",
                                 "assign",
                                 token,
                             )
 
-                # If Powershell script does not exist, create it and assign
+                # If Shell script does not exist, create it and assign
                 else:
                     print("-" * 90)
                     print(
-                        "Powershell script not found, creating script: "
+                        "Shell script not found, creating script: "
                         + repo_data["displayName"]
                     )
                     if report is False:
                         request_json = json.dumps(repo_data)
                         post_request = makeapirequestPost(
                             ENDPOINT,
                             token,
@@ -174,12 +183,20 @@
                             post_assignment_update(
                                 request_data,
                                 post_request["id"],
                                 "deviceManagement/deviceManagementScripts",
                                 "assign",
                                 token,
                             )
-                        print(
-                            "Powershell script created with id: " + post_request["id"]
-                        )
+                        print("Shell script created with id: " + post_request["id"])
+
+        # If any Shell Scripts are left in mem_shellScript, remove them from Intune as they are not in the repo
+        if mem_shellScript.get("value", None) is not None:
+            for val in mem_shellScript["value"]:
+                print("-" * 90)
+                print("Removing Shell Script from Intune: " + val["displayName"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
 
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_proactiveRemediation.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 """
 
 import json
 import os
 import base64
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 from .clean_filename import clean_filename
@@ -63,14 +68,15 @@
                 repo_data.pop("assignments", None)
 
                 data = {"value": ""}
                 if mem_proactiveRemediation["value"]:
                     for val in mem_proactiveRemediation["value"]:
                         if repo_data["displayName"] == val["displayName"]:
                             data["value"] = val
+                            mem_proactiveRemediation["value"].remove(val)
 
                 # If Powershell script exists, continue
                 if data["value"]:
                     print("-" * 90)
                     q_param = None
                     # Get Powershell script details
                     mem_data = makeapirequest(
@@ -216,8 +222,22 @@
                                 token,
                             )
                         print(
                             "Proactive Remediation created with id: "
                             + post_request["id"]
                         )
 
+        # If any Proactive Remediations are left in mem_proactiveRemediation, remove them from Intune as they are not in the repo
+        if mem_proactiveRemediation.get("value", None) is not None:
+            for val in mem_proactiveRemediation["value"]:
+                if val.get("publisher", None) != "Microsoft":
+                    print("-" * 90)
+                    print(
+                        "Removing Proactive Remediation from Intune: "
+                        + val["displayName"]
+                    )
+                    if report is False:
+                        makeapirequestDelete(
+                            f"{ENDPOINT}/{val['id']}", token, status_code=200
+                        )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 
 import json
 import os
 import base64
 import plistlib
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
@@ -69,14 +74,15 @@
 
                     for val in mem_data["value"]:
                         if (
                             repo_data["@odata.type"] == val["@odata.type"]
                             and repo_data["displayName"] == val["displayName"]
                         ):
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
                 if data["value"]:
                     print("-" * 90)
                     mem_id = data["value"]["id"]
                     # Remove keys before using DeepDiff
                     data["value"] = remove_keys(data["value"])
 
@@ -335,8 +341,18 @@
                                 request_data,
                                 post_request["id"],
                                 "deviceManagement/deviceConfigurations",
                                 "assign",
                                 token,
                             )
 
+        # If any Profiles are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing Profile from Intune: " + val["displayName"])
+                if report is False:
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
+
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.5b1/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 #!/usr/bin/env python3
 
 """
-This module is used to update all Shell Scripts in Intune.
+This module is used to update all Windows Enrollment Profiles in Intune.
 """
 
 import json
 import os
-import base64
 
 from deepdiff import DeepDiff
-from .graph_request import makeapirequest, makeapirequestPatch, makeapirequestPost
+from .graph_request import (
+    makeapirequest,
+    makeapirequestPatch,
+    makeapirequestPost,
+    makeapirequestDelete,
+)
 from .graph_batch import batch_assignment, get_object_assignment
 from .update_assignment import update_assignment, post_assignment_update
 from .check_file import check_file
 from .load_file import load_file
 from .remove_keys import remove_keys
 from .diff_summary import DiffSummary
 
 # Set MS Graph endpoint
-ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts"
-ASSIGNMENT_ENDPOINT = (
-    "https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts"
-)
+ENDPOINT = "https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles"
 
 
 def update(path, token, assignment=False, report=False, create_groups=False):
     """
-    This function updates all Shell scripts in Intune if the configuration in Intune differs from the JSON/YAML file.
+    This function updates all Windows Enrollment Profiles in Intune,
+    if the configuration in Intune differs from the JSON/YAML file.
 
     :param path: Path to where the backup is saved
     :param token: Token to use for authenticating the request
     :param assignment: Boolean to determine if assignments should be updated
     """
 
     diff_summary = []
-    # Set Shell scritp path
-    configpath = path + "/" + "Scripts/Shell"
-    # If Shell script path exists, continue
+    # Set Windows Enrollment Profile path
+    configpath = path + "/" + "Enrollment Profiles/Windows"
+    # If Windows Enrollment Profile path exists, continue
     if os.path.exists(configpath):
-        # Get scripts
-        mem_shellScript = makeapirequest(ENDPOINT, token)
+        # Get enrollment profiles
+        mem_data = makeapirequest(ENDPOINT, token)
         # Get current assignment
         mem_assignments = batch_assignment(
-            mem_shellScript,
-            "deviceManagement/deviceManagementScripts/",
+            mem_data,
+            "deviceManagement/windowsAutopilotDeploymentProfiles/",
             "/assignments",
             token,
         )
 
         for filename in os.listdir(configpath):
             file = check_file(configpath, filename)
             if file is False:
@@ -60,105 +62,73 @@
                 # Create object to pass in to assignment function
                 assign_obj = {}
                 if "assignments" in repo_data:
                     assign_obj = repo_data["assignments"]
                 repo_data.pop("assignments", None)
 
                 data = {"value": ""}
-                if mem_shellScript["value"]:
-                    for val in mem_shellScript["value"]:
+                if mem_data["value"]:
+                    for val in mem_data["value"]:
                         if repo_data["displayName"] == val["displayName"]:
                             data["value"] = val
+                            mem_data["value"].remove(val)
 
-                # If Shell script exists, continue
+                # If Windows Enrollment Profile exists, continue
                 if data["value"]:
                     print("-" * 90)
-                    q_param = None
-                    # Get Shell script details
-                    mem_data = makeapirequest(
-                        ENDPOINT + "/" + data["value"]["id"], token
-                    )
-                    mem_id = mem_data["id"]
+                    mem_id = data["value"]["id"]
                     # Remove keys before using DeepDiff
-                    mem_data = remove_keys(mem_data)
+                    data["value"] = remove_keys(data["value"])
 
-                    # Check if script data is saved and read the file
-                    if os.path.exists(
-                        configpath + "/Script Data/" + repo_data["fileName"]
-                    ):
-                        with open(
-                            configpath + "/Script Data/" + repo_data["fileName"], "r"
-                        ) as f:
-                            repo_payload_config = f.read()
-
-                        mem_payload_config = base64.b64decode(
-                            mem_data["scriptContent"]
-                        ).decode("utf-8")
-
-                        pdiff = DeepDiff(
-                            mem_payload_config, repo_payload_config, ignore_order=True
-                        ).get("values_changed", {})
-                        cdiff = DeepDiff(
-                            mem_data,
-                            repo_data,
-                            ignore_order=True,
-                            exclude_paths="root['scriptContent']",
-                        ).get("values_changed", {})
-
-                        # If any changed values are found, push them to Intune
-                        if pdiff or cdiff and report is False:
-                            shell_bytes = repo_payload_config.encode("utf-8")
-                            repo_data["scriptContent"] = base64.b64encode(
-                                shell_bytes
-                            ).decode("utf-8")
-                            request_data = json.dumps(repo_data)
-                            q_param = None
-                            makeapirequestPatch(
-                                ENDPOINT + "/" + mem_id, token, q_param, request_data
-                            )
-
-                        diff_config = DiffSummary(
-                            data=cdiff,
-                            name=repo_data["displayName"],
-                            type="Shell Script",
-                        )
+                    diff = DeepDiff(data["value"], repo_data, ignore_order=True).get(
+                        "values_changed", {}
+                    )
 
-                        diff_script = DiffSummary(
-                            data=pdiff,
-                            name="",
-                            type="Shell Script",
-                            message="Script changed, check commit history for details",
-                            notify=False,
+                    # If any changed values are found, push them to Intune
+                    if diff and report is False:
+                        if repo_data["managementServiceAppId"]:
+                            pass
+                        else:
+                            repo_data["managementServiceAppId"] = ""
+                        request_data = json.dumps(repo_data)
+                        q_param = None
+                        makeapirequestPatch(
+                            ENDPOINT + "/" + mem_id, token, q_param, request_data
                         )
 
-                        diff_config.diffs += diff_script.diffs
-                        diff_config.count += diff_script.count
+                    diff_profile = DiffSummary(
+                        data=diff,
+                        name=repo_data["displayName"],
+                        type="Windows Enrollment Profile",
+                    )
 
-                        diff_summary.append(diff_config)
+                    diff_summary.append(diff_profile)
 
                     if assignment:
                         mem_assign_obj = get_object_assignment(mem_id, mem_assignments)
                         update = update_assignment(
                             assign_obj, mem_assign_obj, token, create_groups
                         )
                         if update is not None:
-                            request_data = {"deviceManagementScriptAssignments": update}
-                            post_assignment_update(
-                                request_data,
-                                mem_id,
-                                "deviceManagement/deviceManagementScripts",
-                                "assign",
-                                token,
-                            )
+                            for target in update:
+                                request_data = {"target": target["target"]}
+                                post_assignment_update(
+                                    request_data,
+                                    mem_id,
+                                    "deviceManagement/windowsAutopilotDeploymentProfiles",
+                                    "assignments",
+                                    token,
+                                    status_code=201,
+                                )
 
-                # If Shell script does not exist, create it and assign
+                # If Autopilot profile does not exist, create it and assign
                 else:
                     print("-" * 90)
                     print(
-                        "Shell script not found, creating script: "
+                        "Autopilot profile not found, creating profile: "
                         + repo_data["displayName"]
                     )
                     if report is False:
                         request_json = json.dumps(repo_data)
                         post_request = makeapirequestPost(
                             ENDPOINT,
                             token,
@@ -167,20 +137,36 @@
                             status_code=201,
                         )
                         mem_assign_obj = []
                         assignment = update_assignment(
                             assign_obj, mem_assign_obj, token, create_groups
                         )
                         if assignment is not None:
-                            request_data = {
-                                "deviceManagementScriptAssignments": assignment
-                            }
-                            post_assignment_update(
-                                request_data,
-                                post_request["id"],
-                                "deviceManagement/deviceManagementScripts",
-                                "assign",
-                                token,
-                            )
-                        print("Shell script created with id: " + post_request["id"])
+                            for target in assignment:
+                                request_data = {"target": target["target"]}
+                                post_assignment_update(
+                                    request_data,
+                                    post_request["id"],
+                                    "deviceManagement/windowsAutopilotDeploymentProfiles",
+                                    "assignments",
+                                    token,
+                                    status_code=201,
+                                )
+                        print(
+                            "Autopilot profile created with id: " + post_request["id"]
+                        )
+
+        # If any Windows Enrollment Profile are left in mem_data, remove them from Intune as they are not in the repo
+        if mem_data.get("value", None) is not None:
+            for val in mem_data["value"]:
+                print("-" * 90)
+                print("Removing Autopilot Profile from Intune: " + val["displayName"])
+                if report is False:
+                    # Remove assignments so we can delete the profile
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}/assignments", token, status_code=200
+                    )
+                    makeapirequestDelete(
+                        f"{ENDPOINT}/{val['id']}", token, status_code=200
+                    )
 
     return diff_summary
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.5b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.4
+Version: 1.4.5b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.4/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.5b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/IntuneCD/__init__.py
+src/IntuneCD/archive.py
 src/IntuneCD/assignment_report.py
 src/IntuneCD/backup_AppProtection.py
 src/IntuneCD/backup_apns.py
 src/IntuneCD/backup_appConfiguration.py
 src/IntuneCD/backup_appleEnrollmentProfile.py
 src/IntuneCD/backup_applications.py
 src/IntuneCD/backup_assignmentFilters.py
@@ -68,14 +69,15 @@
 src/IntuneCD/update_windowsEnrollmentProfile.py
 src/IntuneCD.egg-info/PKG-INFO
 src/IntuneCD.egg-info/SOURCES.txt
 src/IntuneCD.egg-info/dependency_links.txt
 src/IntuneCD.egg-info/entry_points.txt
 src/IntuneCD.egg-info/requires.txt
 src/IntuneCD.egg-info/top_level.txt
+tests/test_archive.py
 tests/test_check_file.py
 tests/test_clean_filename.py
 tests/test_diff_summary.py
 tests/test_documentation_functions.py
 tests/test_get_added_removed.py
 tests/test_get_authparams.py
 tests/test_graph_batch.py
```

### Comparing `IntuneCD-1.4.4/tests/test_check_file.py` & `IntuneCD-1.4.5b1/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_clean_filename.py` & `IntuneCD-1.4.5b1/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_diff_summary.py` & `IntuneCD-1.4.5b1/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_documentation_functions.py` & `IntuneCD-1.4.5b1/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_get_added_removed.py` & `IntuneCD-1.4.5b1/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_get_authparams.py` & `IntuneCD-1.4.5b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_graph_batch.py` & `IntuneCD-1.4.5b1/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_graph_request.py` & `IntuneCD-1.4.5b1/tests/test_graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_group_report.py` & `IntuneCD-1.4.5b1/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_load_file.py` & `IntuneCD-1.4.5b1/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_match.py` & `IntuneCD-1.4.5b1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_remove_keys.py` & `IntuneCD-1.4.5b1/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_save_output.py` & `IntuneCD-1.4.5b1/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.4/tests/test_update_frontend.py` & `IntuneCD-1.4.5b1/tests/test_update_frontend.py`

 * *Files identical despite different names*

