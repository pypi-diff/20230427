# Comparing `tmp/antchain_twc-1.8.8.tar.gz` & `tmp/antchain_twc-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_twc-1.8.8.tar", last modified: Wed Nov 23 09:00:03 2022, max compression
+gzip compressed data, was "dist/antchain_twc-1.8.9.tar", last modified: Fri Nov 25 06:09:07 2022, max compression
```

## Comparing `antchain_twc-1.8.8.tar` & `antchain_twc-1.8.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/
--rw-r--r--   0 root         (0) root         (0)      213 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2162 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/antchain_sdk_twc/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/antchain_sdk_twc/__init__.py
--rw-r--r--   0 root         (0) root         (0)   682400 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/antchain_sdk_twc/client.py
--rw-r--r--   0 root         (0) root         (0)  1823386 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/antchain_sdk_twc/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/antchain_twc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2162 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/antchain_twc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/antchain_twc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/antchain_twc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/antchain_twc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/antchain_twc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-23 09:00:03.000000 antchain_twc-1.8.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-23 09:00:01.000000 antchain_twc-1.8.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/
+-rw-r--r--   0 root         (0) root         (0)      213 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2162 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_sdk_twc/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/antchain_sdk_twc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   682400 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/antchain_sdk_twc/client.py
+-rw-r--r--   0 root         (0) root         (0)  1823714 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/antchain_sdk_twc/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2162 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/setup.py
```

### Comparing `antchain_twc-1.8.8/LICENSE` & `antchain_twc-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.8.8/PKG-INFO` & `antchain_twc-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_twc
-Version: 1.8.8
+Version: 1.8.9
 Summary: Ant Chain TWC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_twc-1.8.8/README-CN.md` & `antchain_twc-1.8.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.8.8/README.md` & `antchain_twc-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.8.8/antchain_sdk_twc/client.py` & `antchain_twc-1.8.9/antchain_sdk_twc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.8',
+                    'sdk_version': '1.8.9',
                     '_prod_code': 'TWC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'twc-openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.8',
+                    'sdk_version': '1.8.9',
                     '_prod_code': 'TWC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'twc-openapi.antchain.antgroup.com'),
```

### Comparing `antchain_twc-1.8.8/antchain_sdk_twc/models.py` & `antchain_twc-1.8.9/antchain_sdk_twc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -22001,46 +22001,54 @@
 
 class QueryContractTaskRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         task_id: str = None,
+        task_type: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 创建任务时，返回的任务id
         self.task_id = task_id
+        # 任务类型
+        self.task_type = task_type
 
     def validate(self):
         self.validate_required(self.task_id, 'task_id')
+        self.validate_required(self.task_type, 'task_type')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.task_id is not None:
             result['task_id'] = self.task_id
+        if self.task_type is not None:
+            result['task_type'] = self.task_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('task_id') is not None:
             self.task_id = m.get('task_id')
+        if m.get('task_type') is not None:
+            self.task_type = m.get('task_type')
         return self
 
 
 class QueryContractTaskResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_twc-1.8.8/antchain_twc.egg-info/PKG-INFO` & `antchain_twc-1.8.9/antchain_twc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-twc
-Version: 1.8.8
+Version: 1.8.9
 Summary: Ant Chain TWC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_twc-1.8.8/setup.py` & `antchain_twc-1.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_twc.
 
-Created on 23/11/2022
+Created on 25/11/2022
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_twc"
 NAME = "antchain_twc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain TWC SDK Library for Python"
```

