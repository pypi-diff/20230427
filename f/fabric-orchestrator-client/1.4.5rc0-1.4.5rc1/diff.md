# Comparing `tmp/fabric-orchestrator-client-1.4.5rc0.tar.gz` & `tmp/fabric-orchestrator-client-1.4.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.4.5rc0.tar", last modified: Thu Apr 27 13:32:52 2023, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.4.5rc1.tar", last modified: Thu Apr 27 14:17:27 2023, max compression
```

## Comparing `fabric-orchestrator-client-1.4.5rc0.tar` & `fabric-orchestrator-client-1.4.5rc1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.774515 fabric-orchestrator-client-1.4.5rc0/
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)       59 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)     9582 2023-04-27 13:32:52.773683 fabric-orchestrator-client-1.4.5rc0/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     9155 2023-04-26 15:48:39.000000 fabric-orchestrator-client-1.4.5rc0/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.710284 fabric-orchestrator-client-1.4.5rc0/fabric_cf/
--rw-r--r--   0 kthare10   (503) staff       (20)       25 2023-04-27 13:32:40.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.711068 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)    18562 2023-04-26 15:51:34.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/orchestrator_proxy.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.715721 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/
--rw-r--r--   0 kthare10   (503) staff       (20)     3004 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.721030 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/
--rw-r--r--   0 kthare10   (503) staff       (20)      397 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     9597 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)    38371 2023-04-26 15:46:01.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8826 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3748 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)    25128 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8240 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/configuration.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.742462 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/
--rw-r--r--   0 kthare10   (503) staff       (20)     2496 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3055 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3420 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8496 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3435 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3412 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0 kthare10   (503) staff       (20)    10903 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3422 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4999 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3832 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)     6211 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4253 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3163 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5771 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5063 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3870 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4994 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3831 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4971 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3819 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5224 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3963 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3413 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3882 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)    12988 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/rest.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.746367 fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)     9582 2023-04-27 13:32:52.000000 fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     3364 2023-04-27 13:32:52.000000 fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-04-27 13:32:52.000000 fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       88 2023-04-27 13:32:52.000000 fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       15 2023-04-27 13:32:52.000000 fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       96 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-04-27 13:32:52.774799 fabric-orchestrator-client-1.4.5rc0/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)     1250 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/setup.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 13:32:52.772674 fabric-orchestrator-client-1.4.5rc0/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)      896 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_resource.py
--rw-r--r--   0 kthare10   (503) staff       (20)      950 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_resources.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1206 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_resources_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      872 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_slice.py
--rw-r--r--   0 kthare10   (503) staff       (20)      930 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_slice_details.py
--rw-r--r--   0 kthare10   (503) staff       (20)      880 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_slices.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2052 2023-04-26 15:44:08.000000 fabric-orchestrator-client-1.4.5rc0/test/test_slices_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      880 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_sliver.py
--rw-r--r--   0 kthare10   (503) staff       (20)      888 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_slivers.py
--rw-r--r--   0 kthare10   (503) staff       (20)      998 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_slivers_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      998 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_no_content.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1032 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_no_content_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)      996 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_paginated.py
--rw-r--r--   0 kthare10   (503) staff       (20)      972 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_single.py
--rw-r--r--   0 kthare10   (503) staff       (20)      988 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status400_bad_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1038 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status400_bad_request_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1002 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status401_unauthorized.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1052 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status401_unauthorized_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      978 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status403_forbidden.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1028 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status403_forbidden_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      972 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status404_not_found.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1022 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status404_not_found_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1062 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status500_internal_server_error.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1112 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      888 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_version.py
--rw-r--r--   0 kthare10   (503) staff       (20)      814 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_version_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      922 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc0/test/test_version_data.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.484574 fabric-orchestrator-client-1.4.5rc1/
+-rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/LICENSE
+-rw-r--r--   0 kthare10   (503) staff       (20)       59 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/MANIFEST.in
+-rw-r--r--   0 kthare10   (503) staff       (20)     9665 2023-04-27 14:17:27.483719 fabric-orchestrator-client-1.4.5rc1/PKG-INFO
+-rw-r--r--   0 kthare10   (503) staff       (20)     9238 2023-04-27 14:14:10.000000 fabric-orchestrator-client-1.4.5rc1/README.md
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.439866 fabric-orchestrator-client-1.4.5rc1/fabric_cf/
+-rw-r--r--   0 kthare10   (503) staff       (20)       25 2023-04-27 14:17:07.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/__init__.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.440679 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/
+-rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)    18242 2023-04-27 14:16:42.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/orchestrator_proxy.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.442901 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/
+-rw-r--r--   0 kthare10   (503) staff       (20)     3004 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/__init__.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.446381 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/
+-rw-r--r--   0 kthare10   (503) staff       (20)      397 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     9597 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)    37827 2023-04-27 14:15:28.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     8826 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3748 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)    25128 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     8240 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/configuration.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.460633 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/
+-rw-r--r--   0 kthare10   (503) staff       (20)     2496 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3055 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3420 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     8496 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3435 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3412 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0 kthare10   (503) staff       (20)    10903 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3422 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     4999 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3832 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     6211 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     4253 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3163 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     5771 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     5063 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3870 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     4994 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3831 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     4971 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3819 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     5224 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3963 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3413 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     3882 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0 kthare10   (503) staff       (20)    12988 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/rest.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.463125 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/
+-rw-r--r--   0 kthare10   (503) staff       (20)     9665 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/PKG-INFO
+-rw-r--r--   0 kthare10   (503) staff       (20)     3364 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       88 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/requires.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       15 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/top_level.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       96 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/requirements.txt
+-rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-04-27 14:17:27.484738 fabric-orchestrator-client-1.4.5rc1/setup.cfg
+-rw-r--r--   0 kthare10   (503) staff       (20)     1250 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/setup.py
+drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.482475 fabric-orchestrator-client-1.4.5rc1/test/
+-rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/__init__.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      896 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_resource.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      950 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_resources.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1206 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_resources_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      872 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slice.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      930 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slice_details.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      880 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slices.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     2018 2023-04-27 14:14:27.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slices_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      880 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_sliver.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      888 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slivers.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      998 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slivers_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      998 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1032 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      996 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_paginated.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      972 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_single.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      988 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1038 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1002 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1052 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      978 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1028 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      972 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1022 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1062 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error.py
+-rw-r--r--   0 kthare10   (503) staff       (20)     1112 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      888 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_version.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      814 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_version_api.py
+-rw-r--r--   0 kthare10   (503) staff       (20)      922 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_version_data.py
```

### Comparing `fabric-orchestrator-client-1.4.5rc0/LICENSE` & `fabric-orchestrator-client-1.4.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/PKG-INFO` & `fabric-orchestrator-client-1.4.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.4.5rc0
+Version: 1.4.5rc1
 Summary: Fabric Orchestrator API
 Home-page: https://github.com/fabric-testbed/OrchestratorClient
 Author-email: kthare10@unc.edu
 Keywords: Swagger,Fabric Orchestrator API
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -115,17 +115,17 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://127.0.0.1:8700/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ResourcesApi* | [**portalresources_get**](docs/ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
-*ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources
+*ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 *SlicesApi* | [**slices_create_post**](docs/SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
-*SlicesApi* | [**slices_delete_email_delete**](docs/SlicesApi.md#slices_delete_email_delete) | **DELETE** /slices/delete/{email} | Delete all slices of a user identified by an email within a project.
+*SlicesApi* | [**slices_delete_delete**](docs/SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 *SlicesApi* | [**slices_delete_slice_id_delete**](docs/SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 *SlicesApi* | [**slices_get**](docs/SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 *SlicesApi* | [**slices_modify_slice_id_accept_post**](docs/SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
 *SlicesApi* | [**slices_modify_slice_id_put**](docs/SlicesApi.md#slices_modify_slice_id_put) | **PUT** /slices/modify/{slice_id} | Modify an existing slice
 *SlicesApi* | [**slices_renew_slice_id_post**](docs/SlicesApi.md#slices_renew_slice_id_post) | **POST** /slices/renew/{slice_id} | Renew slice
 *SlicesApi* | [**slices_slice_id_get**](docs/SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
 *SliversApi* | [**slivers_get**](docs/SliversApi.md#slivers_get) | **GET** /slivers | Retrieve a listing of user slivers
```

### Comparing `fabric-orchestrator-client-1.4.5rc0/README.md` & `fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fabric-orchestrator-client
+Version: 1.4.5rc1
+Summary: Fabric Orchestrator API
+Home-page: https://github.com/fabric-testbed/OrchestratorClient
+Author-email: kthare10@unc.edu
+Keywords: Swagger,Fabric Orchestrator API
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI](https://img.shields.io/pypi/v/fabric-orchestrator-client?style=plastic)](https://pypi.org/project/fabric-orchestrator-client/)
 
 # Fabric Orchestrator swagger-client
 This is Fabric Orchestrator API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
@@ -102,17 +115,17 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://127.0.0.1:8700/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ResourcesApi* | [**portalresources_get**](docs/ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
-*ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources
+*ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 *SlicesApi* | [**slices_create_post**](docs/SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
-*SlicesApi* | [**slices_delete_email_delete**](docs/SlicesApi.md#slices_delete_email_delete) | **DELETE** /slices/delete/{email} | Delete all slices of a user identified by an email within a project.
+*SlicesApi* | [**slices_delete_delete**](docs/SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 *SlicesApi* | [**slices_delete_slice_id_delete**](docs/SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 *SlicesApi* | [**slices_get**](docs/SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 *SlicesApi* | [**slices_modify_slice_id_accept_post**](docs/SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
 *SlicesApi* | [**slices_modify_slice_id_put**](docs/SlicesApi.md#slices_modify_slice_id_put) | **PUT** /slices/modify/{slice_id} | Modify an existing slice
 *SlicesApi* | [**slices_renew_slice_id_post**](docs/SlicesApi.md#slices_renew_slice_id_post) | **POST** /slices/renew/{slice_id} | Renew slice
 *SlicesApi* | [**slices_slice_id_get**](docs/SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
 *SliversApi* | [**slivers_get**](docs/SliversApi.md#slivers_get) | **GET** /slivers | Retrieve a listing of user slivers
```

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,37 +242,34 @@
                 topology.load(graph_string=model)
 
             return Status.OK, topology
         except Exception as e:
             traceback.print_exc()
             return Status.FAILURE, e
 
-    def delete(self, *, token: str, slice_id: str = None, email: str = None) -> Tuple[Status, Union[Exception, None]]:
+    def delete(self, *, token: str, slice_id: str = None) -> Tuple[Status, Union[Exception, None]]:
         """
         Delete a slice
         @param token fabric token
         @param slice_id slice id
-        @param email email
         @return Tuple containing Status and Exception/Json containing deletion status
         """
         if token is None:
             return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Token {token} must be specified")
 
         try:
             # Set the tokens
             self.slices_api.api_client.configuration.api_key['Authorization'] = token
             self.slices_api.api_client.configuration.api_key_prefix['Authorization'] = 'Bearer'
 
             if slice_id is not None:
                 self.slices_api.slices_delete_slice_id_delete(slice_id=slice_id)
-            elif email is not None:
-                self.slices_api.slices_delete_email_delete(email=email)
             else:
-                return Status.INVALID_ARGUMENTS, OrchestratorProxyException(f"Either Slice Id {slice_id} "
-                                                                            f"or Email {email} must be specified")
+                self.slices_api.slices_delete_delete()
+
             return Status.OK, None
         except Exception as e:
             return Status.FAILURE, e
 
     def slices(self, *, token: str, includes: List[SliceState] = None, excludes: List[SliceState] = None,
                name: str = None, limit: int = 20, offset: int = 0, slice_id: str = None) -> Tuple[Status, Union[Exception, List[Slice]]]:
         """
```

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,77 +140,69 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def slices_delete_email_delete(self, email, **kwargs):  # noqa: E501
-        """Delete all slices of a user identified by an email within a project.  # noqa: E501
+    def slices_delete_delete(self, **kwargs):  # noqa: E501
+        """Delete all slices for a User within a project.  # noqa: E501
 
-        Request to delete all slices of a user identified by an email within a project.    # noqa: E501
+        Delete all slices for a User within a project. User identity email and project id is available in the bearer token.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.slices_delete_email_delete(email, async_req=True)
+        >>> thread = api.slices_delete_delete(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str email: User's email address (required)
         :return: Status200OkNoContent
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.slices_delete_email_delete_with_http_info(email, **kwargs)  # noqa: E501
+            return self.slices_delete_delete_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.slices_delete_email_delete_with_http_info(email, **kwargs)  # noqa: E501
+            (data) = self.slices_delete_delete_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def slices_delete_email_delete_with_http_info(self, email, **kwargs):  # noqa: E501
-        """Delete all slices of a user identified by an email within a project.  # noqa: E501
+    def slices_delete_delete_with_http_info(self, **kwargs):  # noqa: E501
+        """Delete all slices for a User within a project.  # noqa: E501
 
-        Request to delete all slices of a user identified by an email within a project.    # noqa: E501
+        Delete all slices for a User within a project. User identity email and project id is available in the bearer token.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.slices_delete_email_delete_with_http_info(email, async_req=True)
+        >>> thread = api.slices_delete_delete_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str email: User's email address (required)
         :return: Status200OkNoContent
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['email']  # noqa: E501
+        all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method slices_delete_email_delete" % key
+                    " to method slices_delete_delete" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'email' is set
-        if ('email' not in params or
-                params['email'] is None):
-            raise ValueError("Missing the required parameter `email` when calling `slices_delete_email_delete`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'email' in params:
-            path_params['email'] = params['email']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -220,15 +212,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/slices/delete/{email}', 'DELETE',
+            '/slices/delete', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Status200OkNoContent',  # noqa: E501
@@ -237,14 +229,15 @@
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def slices_delete_slice_id_delete(self, slice_id, **kwargs):  # noqa: E501
         """Delete slice.  # noqa: E501
+
         Request to delete slice. On success, resources associated with slice or sliver are stopped if necessary, de-provisioned and un-allocated at the respective sites.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.slices_delete_slice_id_delete(slice_id, async_req=True)
         >>> result = thread.get()
         :param async_req bool
         :param str slice_id: Slice identified by universally unique identifier (required)
```

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/PKG-INFO` & `fabric-orchestrator-client-1.4.5rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fabric-orchestrator-client
-Version: 1.4.5rc0
-Summary: Fabric Orchestrator API
-Home-page: https://github.com/fabric-testbed/OrchestratorClient
-Author-email: kthare10@unc.edu
-Keywords: Swagger,Fabric Orchestrator API
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI](https://img.shields.io/pypi/v/fabric-orchestrator-client?style=plastic)](https://pypi.org/project/fabric-orchestrator-client/)
 
 # Fabric Orchestrator swagger-client
 This is Fabric Orchestrator API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
@@ -115,17 +102,17 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://127.0.0.1:8700/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ResourcesApi* | [**portalresources_get**](docs/ResourcesApi.md#portalresources_get) | **GET** /portalresources | Retrieve a listing and description of available resources for portal
-*ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources
+*ResourcesApi* | [**resources_get**](docs/ResourcesApi.md#resources_get) | **GET** /resources | Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
 *SlicesApi* | [**slices_create_post**](docs/SlicesApi.md#slices_create_post) | **POST** /slices/create | Create slice
-*SlicesApi* | [**slices_delete_email_delete**](docs/SlicesApi.md#slices_delete_email_delete) | **DELETE** /slices/delete/{email} | Delete all slices of a user identified by an email within a project.
+*SlicesApi* | [**slices_delete_delete**](docs/SlicesApi.md#slices_delete_delete) | **DELETE** /slices/delete | Delete all slices for a User within a project.
 *SlicesApi* | [**slices_delete_slice_id_delete**](docs/SlicesApi.md#slices_delete_slice_id_delete) | **DELETE** /slices/delete/{slice_id} | Delete slice.
 *SlicesApi* | [**slices_get**](docs/SlicesApi.md#slices_get) | **GET** /slices | Retrieve a listing of user slices
 *SlicesApi* | [**slices_modify_slice_id_accept_post**](docs/SlicesApi.md#slices_modify_slice_id_accept_post) | **POST** /slices/modify/{slice_id}/accept | Accept the last modify an existing slice
 *SlicesApi* | [**slices_modify_slice_id_put**](docs/SlicesApi.md#slices_modify_slice_id_put) | **PUT** /slices/modify/{slice_id} | Modify an existing slice
 *SlicesApi* | [**slices_renew_slice_id_post**](docs/SlicesApi.md#slices_renew_slice_id_post) | **POST** /slices/renew/{slice_id} | Renew slice
 *SlicesApi* | [**slices_slice_id_get**](docs/SlicesApi.md#slices_slice_id_get) | **GET** /slices/{slice_id} | slice properties
 *SliversApi* | [**slivers_get**](docs/SliversApi.md#slivers_get) | **GET** /slivers | Retrieve a listing of user slivers
```

### Comparing `fabric-orchestrator-client-1.4.5rc0/fabric_orchestrator_client.egg-info/SOURCES.txt` & `fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/setup.py` & `fabric-orchestrator-client-1.4.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_resource.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_resources.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_resources_api.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_slice.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_slice_details.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_slices.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_slices_api.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_slices_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     def test_slices_create_post(self):
         """Test case for slices_create_post
 
         Create slice  # noqa: E501
         """
         pass
 
-    def test_slices_delete_email_delete(self):
-        """Test case for slices_delete_email_delete
+    def test_slices_delete_delete(self):
+        """Test case for slices_delete_delete
 
-        Delete all slices of a user identified by an email within a project.  # noqa: E501
+        Delete all slices for a User within a project.  # noqa: E501
         """
         pass
 
     def test_slices_delete_slice_id_delete(self):
         """Test case for slices_delete_slice_id_delete
 
         Delete slice.  # noqa: E501
```

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_sliver.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_slivers.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_slivers_api.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_version.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_version_api.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc0/test/test_version_data.py` & `fabric-orchestrator-client-1.4.5rc1/test/test_version_data.py`

 * *Files identical despite different names*

