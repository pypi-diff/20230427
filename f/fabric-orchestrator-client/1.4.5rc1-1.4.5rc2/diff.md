# Comparing `tmp/fabric-orchestrator-client-1.4.5rc1.tar.gz` & `tmp/fabric-orchestrator-client-1.4.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.4.5rc1.tar", last modified: Thu Apr 27 14:17:27 2023, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.4.5rc2.tar", last modified: Thu Apr 27 14:45:49 2023, max compression
```

## Comparing `fabric-orchestrator-client-1.4.5rc1.tar` & `fabric-orchestrator-client-1.4.5rc2.tar`

### file list

```diff
@@ -1,84 +1,82 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.484574 fabric-orchestrator-client-1.4.5rc1/
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)       59 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)     9665 2023-04-27 14:17:27.483719 fabric-orchestrator-client-1.4.5rc1/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     9238 2023-04-27 14:14:10.000000 fabric-orchestrator-client-1.4.5rc1/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.439866 fabric-orchestrator-client-1.4.5rc1/fabric_cf/
--rw-r--r--   0 kthare10   (503) staff       (20)       25 2023-04-27 14:17:07.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.440679 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)    18242 2023-04-27 14:16:42.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/orchestrator_proxy.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.442901 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/
--rw-r--r--   0 kthare10   (503) staff       (20)     3004 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.446381 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/
--rw-r--r--   0 kthare10   (503) staff       (20)      397 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     9597 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)    37827 2023-04-27 14:15:28.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8826 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3748 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)    25128 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8240 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/configuration.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.460633 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/
--rw-r--r--   0 kthare10   (503) staff       (20)     2496 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3055 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3420 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0 kthare10   (503) staff       (20)     8496 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3435 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3412 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0 kthare10   (503) staff       (20)    10903 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3422 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4999 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3832 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)     6211 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4253 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3163 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5771 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5063 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3870 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4994 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3831 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4971 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3819 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5224 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3963 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3413 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3882 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)    12988 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/rest.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.463125 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)     9665 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     3364 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       88 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       15 2023-04-27 14:17:27.000000 fabric-orchestrator-client-1.4.5rc1/fabric_orchestrator_client.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       96 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-04-27 14:17:27.484738 fabric-orchestrator-client-1.4.5rc1/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)     1250 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/setup.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-04-27 14:17:27.482475 fabric-orchestrator-client-1.4.5rc1/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)      896 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_resource.py
--rw-r--r--   0 kthare10   (503) staff       (20)      950 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_resources.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1206 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_resources_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      872 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slice.py
--rw-r--r--   0 kthare10   (503) staff       (20)      930 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slice_details.py
--rw-r--r--   0 kthare10   (503) staff       (20)      880 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slices.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2018 2023-04-27 14:14:27.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slices_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      880 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_sliver.py
--rw-r--r--   0 kthare10   (503) staff       (20)      888 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slivers.py
--rw-r--r--   0 kthare10   (503) staff       (20)      998 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_slivers_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      998 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1032 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)      996 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_paginated.py
--rw-r--r--   0 kthare10   (503) staff       (20)      972 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_single.py
--rw-r--r--   0 kthare10   (503) staff       (20)      988 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1038 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1002 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1052 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      978 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1028 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      972 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1022 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1062 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1112 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)      888 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_version.py
--rw-r--r--   0 kthare10   (503) staff       (20)      814 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_version_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)      922 2023-04-26 15:40:23.000000 fabric-orchestrator-client-1.4.5rc1/test/test_version_data.py
+-rw-r--r--   0        0        0      793 2023-04-26 15:40:23.465964 fabric-orchestrator-client-1.4.5rc2/.gitignore
+-rw-r--r--   0        0        0     1030 2023-04-26 15:40:23.466117 fabric-orchestrator-client-1.4.5rc2/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-04-26 15:41:55.675644 fabric-orchestrator-client-1.4.5rc2/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-04-26 15:40:23.466598 fabric-orchestrator-client-1.4.5rc2/.travis.yml
+-rw-r--r--   0        0        0      770 2023-04-26 15:40:23.466720 fabric-orchestrator-client-1.4.5rc2/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2023-04-26 15:40:23.466874 fabric-orchestrator-client-1.4.5rc2/LICENSE
+-rw-r--r--   0        0        0       59 2023-04-26 15:40:23.466976 fabric-orchestrator-client-1.4.5rc2/MANIFEST.in
+-rw-r--r--   0        0        0     9238 2023-04-27 14:14:10.812023 fabric-orchestrator-client-1.4.5rc2/README.md
+-rw-r--r--   0        0        0     4263 2023-04-26 15:40:23.467492 fabric-orchestrator-client-1.4.5rc2/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    17437 2023-04-27 14:13:41.019129 fabric-orchestrator-client-1.4.5rc2/docs/SlicesApi.md
+-rw-r--r--   0        0        0     3740 2023-04-26 15:40:23.467758 fabric-orchestrator-client-1.4.5rc2/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2023-04-26 15:40:23.467848 fabric-orchestrator-client-1.4.5rc2/docs/Success.md
+-rw-r--r--   0        0        0      352 2023-04-26 15:40:23.467956 fabric-orchestrator-client-1.4.5rc2/docs/Version.md
+-rw-r--r--   0        0        0       25 2023-04-27 14:45:41.678604 fabric-orchestrator-client-1.4.5rc2/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:40:23.468205 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    18242 2023-04-27 14:16:42.757203 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3004 2023-04-26 15:40:23.468935 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      397 2023-04-26 15:40:23.469207 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     9597 2023-04-26 15:40:23.469422 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    37827 2023-04-27 14:15:28.756924 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     8826 2023-04-26 15:40:23.470273 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2023-04-26 15:40:23.470436 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25128 2023-04-26 15:40:23.470934 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2023-04-26 15:40:23.471203 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2496 2023-04-26 15:40:23.471469 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3055 2023-04-26 15:40:23.471836 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2023-04-26 15:40:23.472041 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     8496 2023-04-26 15:40:23.472177 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3435 2023-04-26 15:40:23.472301 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2023-04-26 15:40:23.472417 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0    10903 2023-04-26 15:40:23.472557 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2023-04-26 15:40:23.472786 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2023-04-26 15:40:23.473011 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2023-04-26 15:40:23.473249 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2023-04-26 15:40:23.473435 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2023-04-26 15:40:23.473667 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2023-04-26 15:40:23.473821 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2023-04-26 15:40:23.474000 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2023-04-26 15:40:23.474170 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2023-04-26 15:40:23.474381 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2023-04-26 15:40:23.474575 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2023-04-26 15:40:23.474684 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2023-04-26 15:40:23.474811 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2023-04-26 15:40:23.474951 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2023-04-26 15:40:23.475187 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2023-04-26 15:40:23.475372 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2023-04-26 15:40:23.475530 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2023-04-26 15:40:23.475718 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12988 2023-04-26 15:40:23.475947 fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-04-26 15:40:23.476133 fabric-orchestrator-client-1.4.5rc2/git_push.sh
+-rw-r--r--   0        0        0      858 2023-04-27 14:44:21.925037 fabric-orchestrator-client-1.4.5rc2/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-26 15:40:23.476661 fabric-orchestrator-client-1.4.5rc2/test-requirements.txt
+-rw-r--r--   0        0        0        0 2023-04-26 15:40:23.476861 fabric-orchestrator-client-1.4.5rc2/test/__init__.py
+-rw-r--r--   0        0        0      896 2023-04-26 15:40:23.477112 fabric-orchestrator-client-1.4.5rc2/test/test_resource.py
+-rw-r--r--   0        0        0      950 2023-04-26 15:40:23.477290 fabric-orchestrator-client-1.4.5rc2/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2023-04-26 15:40:23.477483 fabric-orchestrator-client-1.4.5rc2/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2023-04-26 15:40:23.477600 fabric-orchestrator-client-1.4.5rc2/test/test_slice.py
+-rw-r--r--   0        0        0      930 2023-04-26 15:40:23.477904 fabric-orchestrator-client-1.4.5rc2/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2023-04-26 15:40:23.478094 fabric-orchestrator-client-1.4.5rc2/test/test_slices.py
+-rw-r--r--   0        0        0     2018 2023-04-27 14:14:27.288721 fabric-orchestrator-client-1.4.5rc2/test/test_slices_api.py
+-rw-r--r--   0        0        0      880 2023-04-26 15:40:23.478444 fabric-orchestrator-client-1.4.5rc2/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2023-04-26 15:40:23.478592 fabric-orchestrator-client-1.4.5rc2/test/test_slivers.py
+-rw-r--r--   0        0        0      998 2023-04-26 15:40:23.478740 fabric-orchestrator-client-1.4.5rc2/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2023-04-26 15:40:23.478959 fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2023-04-26 15:40:23.479170 fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2023-04-26 15:40:23.479288 fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2023-04-26 15:40:23.479425 fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2023-04-26 15:40:23.479559 fabric-orchestrator-client-1.4.5rc2/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2023-04-26 15:40:23.479796 fabric-orchestrator-client-1.4.5rc2/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2023-04-26 15:40:23.479977 fabric-orchestrator-client-1.4.5rc2/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2023-04-26 15:40:23.480089 fabric-orchestrator-client-1.4.5rc2/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2023-04-26 15:40:23.480236 fabric-orchestrator-client-1.4.5rc2/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2023-04-26 15:40:23.480412 fabric-orchestrator-client-1.4.5rc2/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2023-04-26 15:40:23.480569 fabric-orchestrator-client-1.4.5rc2/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2023-04-26 15:40:23.480666 fabric-orchestrator-client-1.4.5rc2/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2023-04-26 15:40:23.480772 fabric-orchestrator-client-1.4.5rc2/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2023-04-26 15:40:23.480866 fabric-orchestrator-client-1.4.5rc2/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2023-04-26 15:40:23.481010 fabric-orchestrator-client-1.4.5rc2/test/test_version.py
+-rw-r--r--   0        0        0      814 2023-04-26 15:40:23.481202 fabric-orchestrator-client-1.4.5rc2/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2023-04-26 15:40:23.481367 fabric-orchestrator-client-1.4.5rc2/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-04-26 15:40:23.481527 fabric-orchestrator-client-1.4.5rc2/tox.ini
+-rw-r--r--   0        0        0     9936 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.4.5rc2/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.4.5rc1/LICENSE` & `fabric-orchestrator-client-1.4.5rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/PKG-INFO` & `fabric-orchestrator-client-1.4.5rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fabric-orchestrator-client
-Version: 1.4.5rc1
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
```

### Comparing `fabric-orchestrator-client-1.4.5rc1/README.md` & `fabric-orchestrator-client-1.4.5rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: fabric-orchestrator-client
+Version: 1.4.5rc2
+Summary: Fabric Orchestrator API
+Keywords: Swagger,Fabric Orchestrator API
+Author-email: Komal Thareja <kthare10@renci.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Dist: certifi >= 14.05.14
+Requires-Dist: six >= 1.10
+Requires-Dist: python_dateutil >= 2.5.3
+Requires-Dist: fabric-fim==1.4.10
+Requires-Dist: requests>=2.28.1
+Project-URL: Home, https://fabric-testbed.net/
+Project-URL: Sources, https://github.com/fabric-testbed/OrchestratorClient
+
 [![PyPI](https://img.shields.io/pypi/v/fabric-orchestrator-client?style=plastic)](https://pypi.org/project/fabric-orchestrator-client/)
 
 # Fabric Orchestrator swagger-client
 This is Fabric Orchestrator API
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
@@ -227,7 +246,8 @@
 proxy = OrchestratorProxy(orchestrator_host=orchestrator_host)
 status, reservation = proxy.renew_slice(token=token, slice_id=slice_id,
                                         new_lease_end_time=new_time.strftime('%Y-%m-%d %H:%M:%S %z'))
 ```
 ## Author
 
 kthare10@unc.edu
+
```

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.4.5rc2/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_resource.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_resources.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_resources_api.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_slice.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_slice_details.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_slices.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_slices_api.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_sliver.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_slivers.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_slivers_api.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_version.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_version_api.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.4.5rc1/test/test_version_data.py` & `fabric-orchestrator-client-1.4.5rc2/test/test_version_data.py`

 * *Files identical despite different names*

