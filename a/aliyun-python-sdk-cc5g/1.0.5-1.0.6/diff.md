# Comparing `tmp/aliyun-python-sdk-cc5g-1.0.5.tar.gz` & `tmp/aliyun-python-sdk-cc5g-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cc5g-1.0.5.tar", last modified: Tue Apr  4 07:04:48 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cc5g-1.0.6.tar", last modified: Thu Apr 27 09:21:25 2023, max compression
```

## Comparing `aliyun-python-sdk-cc5g-1.0.5.tar` & `aliyun-python-sdk-cc5g-1.0.6.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4132 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/
--rw-r--r--   0 root         (0) root         (0)     2426 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AddDNSAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AddGroupDnsAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AddWirelessCloudConnectorToGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AttachVpcToNetLinkRequest.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateBatchOperateCardsTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3236 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateGroupAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateIoTCloudConnectorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     3051 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteBatchOperateCardsTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteGroupAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteIoTCloudConnectorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1678 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DetachVpcFromNetLinkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/FailCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetCardLockReasonRequest.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetCreateCustomerInformationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetDiagnoseResultForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetWirelessCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2024 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GrantNetLinkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListAPNsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2205 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListBatchOperateCardsTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListCardUsagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListDataPackagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListDiagnoseInfoForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListGroupAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListIoTCloudConnectorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListOrdersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1217 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2565 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2906 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorsRequest.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/LockCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ModifyWirelessCloudConnectorFeatureRequest.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/OpenCc5gServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/RebindCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2101 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/RemoveWirelessCloudConnectorFromGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ResumeCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/RevokeNetLinkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/StopCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/SubmitDiagnoseTaskForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/SwitchWirelessCloudConnectorToBusinessRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UnlockCardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3220 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateBatchOperateCardsTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2155 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     2677 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateDNSAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateGroupAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateGroupDnsAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2030 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-04 07:04:48.000000 aliyun-python-sdk-cc5g-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-04-04 07:04:47.000000 aliyun-python-sdk-cc5g-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AddDNSAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AddGroupDnsAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AddWirelessCloudConnectorToGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AttachVpcToNetLinkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateBatchOperateCardsTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateGroupAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateIoTCloudConnectorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteBatchOperateCardsTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteGroupAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteIoTCloudConnectorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DetachVpcFromNetLinkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/FailCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetCardLockReasonRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetCreateCustomerInformationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetDiagnoseResultForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetWirelessCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GrantNetLinkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListAPNsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListBatchOperateCardsTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListCardDayUsagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListCardUsagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListDataPackagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListDiagnoseInfoForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListGroupAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListIoTCloudConnectorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListOrdersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/LockCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ModifyWirelessCloudConnectorFeatureRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/OpenCc5gServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/RebindCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/RemoveWirelessCloudConnectorFromGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ResumeCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/RevokeNetLinkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/StopCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/SubmitDiagnoseTaskForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/SwitchWirelessCloudConnectorToBusinessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UnlockCardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateBatchOperateCardsTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateDNSAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateGroupAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateGroupDnsAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-04-27 09:21:25.000000 aliyun-python-sdk-cc5g-1.0.6/setup.py
```

### Comparing `aliyun-python-sdk-cc5g-1.0.5/LICENSE` & `aliyun-python-sdk-cc5g-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/PKG-INFO` & `aliyun-python-sdk-cc5g-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cc5g
-Version: 1.0.5
+Version: 1.0.6
 Summary: The cc5g module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cc5g
```

### Comparing `aliyun-python-sdk-cc5g-1.0.5/README.rst` & `aliyun-python-sdk-cc5g-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/PKG-INFO` & `aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cc5g
-Version: 1.0.5
+Version: 1.0.6
 Summary: The cc5g module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cc5g
```

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyun_python_sdk_cc5g.egg-info/SOURCES.txt` & `aliyun-python-sdk-cc5g-1.0.6/aliyun_python_sdk_cc5g.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 aliyunsdkcc5g/request/v20220314/GetCreateCustomerInformationRequest.py
 aliyunsdkcc5g/request/v20220314/GetDiagnoseResultForSingleCardRequest.py
 aliyunsdkcc5g/request/v20220314/GetWirelessCloudConnectorRequest.py
 aliyunsdkcc5g/request/v20220314/GrantNetLinkRequest.py
 aliyunsdkcc5g/request/v20220314/ListAPNsRequest.py
 aliyunsdkcc5g/request/v20220314/ListAuthorizationRulesRequest.py
 aliyunsdkcc5g/request/v20220314/ListBatchOperateCardsTasksRequest.py
+aliyunsdkcc5g/request/v20220314/ListCardDayUsagesRequest.py
 aliyunsdkcc5g/request/v20220314/ListCardUsagesRequest.py
 aliyunsdkcc5g/request/v20220314/ListCardsRequest.py
 aliyunsdkcc5g/request/v20220314/ListDataPackagesRequest.py
 aliyunsdkcc5g/request/v20220314/ListDiagnoseInfoForSingleCardRequest.py
 aliyunsdkcc5g/request/v20220314/ListGroupAuthorizationRulesRequest.py
 aliyunsdkcc5g/request/v20220314/ListIoTCloudConnectorBackhaulRouteRequest.py
 aliyunsdkcc5g/request/v20220314/ListOrdersRequest.py
```

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AddDNSAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AddDNSAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AddGroupDnsAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AddGroupDnsAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AddWirelessCloudConnectorToGroupRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AddWirelessCloudConnectorToGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/AttachVpcToNetLinkRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/AttachVpcToNetLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateBatchOperateCardsTaskRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateBatchOperateCardsTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateGroupAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateGroupAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateIoTCloudConnectorBackhaulRouteRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateIoTCloudConnectorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorGroupRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/CreateWirelessCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteBatchOperateCardsTaskRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteBatchOperateCardsTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteGroupAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteGroupAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteIoTCloudConnectorBackhaulRouteRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteIoTCloudConnectorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorGroupRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DeleteWirelessCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/DetachVpcFromNetLinkRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/DetachVpcFromNetLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/FailCardsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/FailCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetCardLockReasonRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetCardLockReasonRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetCardRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetCreateCustomerInformationRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetCreateCustomerInformationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetDiagnoseResultForSingleCardRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetDiagnoseResultForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GetWirelessCloudConnectorRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GetWirelessCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/GrantNetLinkRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/GrantNetLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListAPNsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListAPNsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListAuthorizationRulesRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListBatchOperateCardsTasksRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListBatchOperateCardsTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListCardUsagesRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListCardUsagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListCardsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListDataPackagesRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListDataPackagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListDiagnoseInfoForSingleCardRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListDiagnoseInfoForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListGroupAuthorizationRulesRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListGroupAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListIoTCloudConnectorBackhaulRouteRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListIoTCloudConnectorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListOrdersRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListOrdersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListRegionsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorGroupsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListWirelessCloudConnectorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ListZonesRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ListZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/LockCardsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/LockCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ModifyWirelessCloudConnectorFeatureRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ModifyWirelessCloudConnectorFeatureRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/OpenCc5gServiceRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/OpenCc5gServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/RebindCardsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/RebindCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/RemoveWirelessCloudConnectorFromGroupRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/RemoveWirelessCloudConnectorFromGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/ResumeCardsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/ResumeCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/RevokeNetLinkRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/RevokeNetLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/StopCardsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/StopCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/SubmitDiagnoseTaskForSingleCardRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/SubmitDiagnoseTaskForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/SwitchWirelessCloudConnectorToBusinessRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/SwitchWirelessCloudConnectorToBusinessRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UnlockCardsRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UnlockCardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateBatchOperateCardsTaskRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateBatchOperateCardsTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateCardRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateDNSAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateDNSAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateGroupAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateGroupAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateGroupDnsAuthorizationRuleRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateGroupDnsAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorGroupRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorRequest.py` & `aliyun-python-sdk-cc5g-1.0.6/aliyunsdkcc5g/request/v20220314/UpdateWirelessCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cc5g-1.0.5/setup.py` & `aliyun-python-sdk-cc5g-1.0.6/setup.py`

 * *Files identical despite different names*

