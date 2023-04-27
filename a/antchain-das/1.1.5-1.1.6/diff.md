# Comparing `tmp/antchain_das-1.1.5.tar.gz` & `tmp/antchain_das-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_das-1.1.5.tar", last modified: Fri Sep  3 04:13:44 2021, max compression
+gzip compressed data, was "dist/antchain_das-1.1.6.tar", last modified: Tue Sep 14 03:46:09 2021, max compression
```

## Comparing `antchain_das-1.1.5.tar` & `antchain_das-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-03 04:13:44.000000 antchain_das-1.1.5/
--rw-r--r--   0 root         (0) root         (0)      600 2021-09-03 04:13:43.000000 antchain_das-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-09-03 04:13:43.000000 antchain_das-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2170 2021-09-03 04:13:44.000000 antchain_das-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      812 2021-09-03 04:13:43.000000 antchain_das-1.1.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      998 2021-09-03 04:13:43.000000 antchain_das-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-03 04:13:44.000000 antchain_das-1.1.5/antchain_das.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2170 2021-09-03 04:13:44.000000 antchain_das-1.1.5/antchain_das.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2021-09-03 04:13:44.000000 antchain_das-1.1.5/antchain_das.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-03 04:13:44.000000 antchain_das-1.1.5/antchain_das.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2021-09-03 04:13:44.000000 antchain_das-1.1.5/antchain_das.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-09-03 04:13:44.000000 antchain_das-1.1.5/antchain_das.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-03 04:13:44.000000 antchain_das-1.1.5/antchain_sdk_das/
--rw-r--r--   0 root         (0) root         (0)       21 2021-09-03 04:13:43.000000 antchain_das-1.1.5/antchain_sdk_das/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38842 2021-09-03 04:13:43.000000 antchain_das-1.1.5/antchain_sdk_das/client.py
--rw-r--r--   0 root         (0) root         (0)    75258 2021-09-03 04:13:43.000000 antchain_das-1.1.5/antchain_sdk_das/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2021-09-03 04:13:44.000000 antchain_das-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2021-09-03 04:13:43.000000 antchain_das-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-14 03:46:09.000000 antchain_das-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2021-09-14 03:46:09.000000 antchain_das-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-09-14 03:46:09.000000 antchain_das-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2170 2021-09-14 03:46:09.000000 antchain_das-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      812 2021-09-14 03:46:09.000000 antchain_das-1.1.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      998 2021-09-14 03:46:09.000000 antchain_das-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2170 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38842 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/client.py
+-rw-r--r--   0 root         (0) root         (0)    75009 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2021-09-14 03:46:09.000000 antchain_das-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2021-09-14 03:46:09.000000 antchain_das-1.1.6/setup.py
```

### Comparing `antchain_das-1.1.5/LICENSE` & `antchain_das-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_das-1.1.5/PKG-INFO` & `antchain_das-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_das
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ant Chain DAS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_das-1.1.5/README-CN.md` & `antchain_das-1.1.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_das-1.1.5/README.md` & `antchain_das-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_das-1.1.5/antchain_das.egg-info/PKG-INFO` & `antchain_das-1.1.6/antchain_das.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-das
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ant Chain DAS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_das-1.1.5/antchain_sdk_das/client.py` & `antchain_das-1.1.6/antchain_sdk_das/client.py`

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
-                    'sdk_version': '1.1.5'
+                    'sdk_version': '1.1.6'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.5'
+                    'sdk_version': '1.1.6'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
```

### Comparing `antchain_das-1.1.5/antchain_sdk_das/models.py` & `antchain_das-1.1.6/antchain_sdk_das/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -350,62 +350,62 @@
             self.individual_phone_num = m.get('individual_phone_num')
         return self
 
 
 class DataSourceInfo(TeaModel):
     def __init__(
         self,
-        id: str = None,
+        biz_uuid: str = None,
         name: str = None,
         provider: str = None,
         data_owner_type: str = None,
         data_source_interface_info: DataSourceInterface = None,
     ):
-        # 数据源ID
-        self.id = id
+        # 数据源biz_uuid
+        self.biz_uuid = biz_uuid
         # 数据源名称
         self.name = name
         # 数据提供方
         self.provider = provider
         # 枚举值：ENTERPRISE、INDIVIDUAL
         self.data_owner_type = data_owner_type
         # 数据源接口信息
         self.data_source_interface_info = data_source_interface_info
 
     def validate(self):
-        self.validate_required(self.id, 'id')
+        self.validate_required(self.biz_uuid, 'biz_uuid')
         self.validate_required(self.name, 'name')
         if self.name is not None:
             self.validate_max_length(self.name, 'name', 20)
         self.validate_required(self.provider, 'provider')
         if self.provider is not None:
             self.validate_max_length(self.provider, 'provider', 30)
         self.validate_required(self.data_owner_type, 'data_owner_type')
         self.validate_required(self.data_source_interface_info, 'data_source_interface_info')
         if self.data_source_interface_info:
             self.data_source_interface_info.validate()
 
     def to_map(self):
         result = dict()
-        if self.id is not None:
-            result['id'] = self.id
+        if self.biz_uuid is not None:
+            result['biz_uuid'] = self.biz_uuid
         if self.name is not None:
             result['name'] = self.name
         if self.provider is not None:
             result['provider'] = self.provider
         if self.data_owner_type is not None:
             result['data_owner_type'] = self.data_owner_type
         if self.data_source_interface_info is not None:
             result['data_source_interface_info'] = self.data_source_interface_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('id') is not None:
-            self.id = m.get('id')
+        if m.get('biz_uuid') is not None:
+            self.biz_uuid = m.get('biz_uuid')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('provider') is not None:
             self.provider = m.get('provider')
         if m.get('data_owner_type') is not None:
             self.data_owner_type = m.get('data_owner_type')
         if m.get('data_source_interface_info') is not None:
@@ -551,43 +551,43 @@
 
 
 class GetDasLinkRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        be_authed_person_app_id: str = None,
+        be_authed_person_app_biz_uuid: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 被授权人接入应用id
-        self.be_authed_person_app_id = be_authed_person_app_id
+        # 被授权人接入应用biz_uuid
+        self.be_authed_person_app_biz_uuid = be_authed_person_app_biz_uuid
 
     def validate(self):
-        self.validate_required(self.be_authed_person_app_id, 'be_authed_person_app_id')
+        self.validate_required(self.be_authed_person_app_biz_uuid, 'be_authed_person_app_biz_uuid')
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.be_authed_person_app_id is not None:
-            result['be_authed_person_app_id'] = self.be_authed_person_app_id
+        if self.be_authed_person_app_biz_uuid is not None:
+            result['be_authed_person_app_biz_uuid'] = self.be_authed_person_app_biz_uuid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('be_authed_person_app_id') is not None:
-            self.be_authed_person_app_id = m.get('be_authed_person_app_id')
+        if m.get('be_authed_person_app_biz_uuid') is not None:
+            self.be_authed_person_app_biz_uuid = m.get('be_authed_person_app_biz_uuid')
         return self
 
 
 class GetDasLinkResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -640,51 +640,51 @@
 
 
 class GetDasEnterprisevcRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        auth_instance_id: str = None,
+        auth_instance_biz_uuid: str = None,
         auth_person_enterprise_info: AuthPersonEnterpriseInfo = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 授权实例ID
-        self.auth_instance_id = auth_instance_id
+        # 授权实例biz_uuid
+        self.auth_instance_biz_uuid = auth_instance_biz_uuid
         # 授权企业信息
         self.auth_person_enterprise_info = auth_person_enterprise_info
 
     def validate(self):
-        self.validate_required(self.auth_instance_id, 'auth_instance_id')
+        self.validate_required(self.auth_instance_biz_uuid, 'auth_instance_biz_uuid')
         self.validate_required(self.auth_person_enterprise_info, 'auth_person_enterprise_info')
         if self.auth_person_enterprise_info:
             self.auth_person_enterprise_info.validate()
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.auth_instance_id is not None:
-            result['auth_instance_id'] = self.auth_instance_id
+        if self.auth_instance_biz_uuid is not None:
+            result['auth_instance_biz_uuid'] = self.auth_instance_biz_uuid
         if self.auth_person_enterprise_info is not None:
             result['auth_person_enterprise_info'] = self.auth_person_enterprise_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('auth_instance_id') is not None:
-            self.auth_instance_id = m.get('auth_instance_id')
+        if m.get('auth_instance_biz_uuid') is not None:
+            self.auth_instance_biz_uuid = m.get('auth_instance_biz_uuid')
         if m.get('auth_person_enterprise_info') is not None:
             temp_model = AuthPersonEnterpriseInfo()
             self.auth_person_enterprise_info = temp_model.from_map(m['auth_person_enterprise_info'])
         return self
 
 
 class GetDasEnterprisevcResponse(TeaModel):
@@ -733,51 +733,51 @@
 
 
 class GetDasIndividualvcRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        auth_instance_id: str = None,
+        auth_instance_biz_uuid: str = None,
         authed_person_individual_info: AuthPersonIndividualInfo = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 授权实例ID
-        self.auth_instance_id = auth_instance_id
+        # 授权实例biz_uuid
+        self.auth_instance_biz_uuid = auth_instance_biz_uuid
         # 授权人个人信息
         self.authed_person_individual_info = authed_person_individual_info
 
     def validate(self):
-        self.validate_required(self.auth_instance_id, 'auth_instance_id')
+        self.validate_required(self.auth_instance_biz_uuid, 'auth_instance_biz_uuid')
         self.validate_required(self.authed_person_individual_info, 'authed_person_individual_info')
         if self.authed_person_individual_info:
             self.authed_person_individual_info.validate()
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.auth_instance_id is not None:
-            result['auth_instance_id'] = self.auth_instance_id
+        if self.auth_instance_biz_uuid is not None:
+            result['auth_instance_biz_uuid'] = self.auth_instance_biz_uuid
         if self.authed_person_individual_info is not None:
             result['authed_person_individual_info'] = self.authed_person_individual_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('auth_instance_id') is not None:
-            self.auth_instance_id = m.get('auth_instance_id')
+        if m.get('auth_instance_biz_uuid') is not None:
+            self.auth_instance_biz_uuid = m.get('auth_instance_biz_uuid')
         if m.get('authed_person_individual_info') is not None:
             temp_model = AuthPersonIndividualInfo()
             self.authed_person_individual_info = temp_model.from_map(m['authed_person_individual_info'])
         return self
 
 
 class GetDasIndividualvcResponse(TeaModel):
@@ -827,50 +827,50 @@
 
 class SendDasSmsRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         receive_phone_num: int = None,
-        auth_instance_id: str = None,
+        auth_instance_biz_uuid: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 接收方电话号码
         self.receive_phone_num = receive_phone_num
-        # 授权实例ID
-        self.auth_instance_id = auth_instance_id
+        # 授权实例biz_uuid
+        self.auth_instance_biz_uuid = auth_instance_biz_uuid
 
     def validate(self):
         self.validate_required(self.receive_phone_num, 'receive_phone_num')
-        self.validate_required(self.auth_instance_id, 'auth_instance_id')
+        self.validate_required(self.auth_instance_biz_uuid, 'auth_instance_biz_uuid')
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.receive_phone_num is not None:
             result['receive_phone_num'] = self.receive_phone_num
-        if self.auth_instance_id is not None:
-            result['auth_instance_id'] = self.auth_instance_id
+        if self.auth_instance_biz_uuid is not None:
+            result['auth_instance_biz_uuid'] = self.auth_instance_biz_uuid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('receive_phone_num') is not None:
             self.receive_phone_num = m.get('receive_phone_num')
-        if m.get('auth_instance_id') is not None:
-            self.auth_instance_id = m.get('auth_instance_id')
+        if m.get('auth_instance_biz_uuid') is not None:
+            self.auth_instance_biz_uuid = m.get('auth_instance_biz_uuid')
         return self
 
 
 class SendDasSmsResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -910,72 +910,64 @@
 
 class AuthDasSmsRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         verification_code: str = None,
-        auth_instance_id: str = None,
-        be_authed_person_app_id: str = None,
+        auth_instance_biz_uuid: str = None,
         auth_person_enterprise_info: AuthPersonEnterpriseInfo = None,
         auth_person_individual_info: AuthPersonIndividualInfo = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 手机验证码
         self.verification_code = verification_code
-        # 授权实例ID
-        self.auth_instance_id = auth_instance_id
-        # 被授权企业接入应用ID
-        self.be_authed_person_app_id = be_authed_person_app_id
+        # 授权实例biz_uuid
+        self.auth_instance_biz_uuid = auth_instance_biz_uuid
         # 授权企业信息
         self.auth_person_enterprise_info = auth_person_enterprise_info
         # 授权人个人信息
         self.auth_person_individual_info = auth_person_individual_info
 
     def validate(self):
         self.validate_required(self.verification_code, 'verification_code')
-        self.validate_required(self.auth_instance_id, 'auth_instance_id')
-        self.validate_required(self.be_authed_person_app_id, 'be_authed_person_app_id')
+        self.validate_required(self.auth_instance_biz_uuid, 'auth_instance_biz_uuid')
         if self.auth_person_enterprise_info:
             self.auth_person_enterprise_info.validate()
         if self.auth_person_individual_info:
             self.auth_person_individual_info.validate()
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.verification_code is not None:
             result['verification_code'] = self.verification_code
-        if self.auth_instance_id is not None:
-            result['auth_instance_id'] = self.auth_instance_id
-        if self.be_authed_person_app_id is not None:
-            result['be_authed_person_app_id'] = self.be_authed_person_app_id
+        if self.auth_instance_biz_uuid is not None:
+            result['auth_instance_biz_uuid'] = self.auth_instance_biz_uuid
         if self.auth_person_enterprise_info is not None:
             result['auth_person_enterprise_info'] = self.auth_person_enterprise_info.to_map()
         if self.auth_person_individual_info is not None:
             result['auth_person_individual_info'] = self.auth_person_individual_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('verification_code') is not None:
             self.verification_code = m.get('verification_code')
-        if m.get('auth_instance_id') is not None:
-            self.auth_instance_id = m.get('auth_instance_id')
-        if m.get('be_authed_person_app_id') is not None:
-            self.be_authed_person_app_id = m.get('be_authed_person_app_id')
+        if m.get('auth_instance_biz_uuid') is not None:
+            self.auth_instance_biz_uuid = m.get('auth_instance_biz_uuid')
         if m.get('auth_person_enterprise_info') is not None:
             temp_model = AuthPersonEnterpriseInfo()
             self.auth_person_enterprise_info = temp_model.from_map(m['auth_person_enterprise_info'])
         if m.get('auth_person_individual_info') is not None:
             temp_model = AuthPersonIndividualInfo()
             self.auth_person_individual_info = temp_model.from_map(m['auth_person_individual_info'])
         return self
@@ -1034,36 +1026,36 @@
 
 
 class VerifyDasEnterpriseRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        auth_instance_id: str = None,
+        auth_instance_biz_uuid: str = None,
         vc: str = None,
         be_authed_person_info: BeAuthedPersonInfo = None,
         auth_person_enterprise_info: AuthPersonEnterpriseInfo = None,
         data_source_info: List[DataSource] = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 被授权企业接入应用ID
-        self.auth_instance_id = auth_instance_id
+        self.auth_instance_biz_uuid = auth_instance_biz_uuid
         # VC完整内容
         self.vc = vc
         # 被授权企业信息
         self.be_authed_person_info = be_authed_person_info
         # 授权人企业信息
         self.auth_person_enterprise_info = auth_person_enterprise_info
         # 需要访问的数据源信息列表
         self.data_source_info = data_source_info
 
     def validate(self):
-        self.validate_required(self.auth_instance_id, 'auth_instance_id')
+        self.validate_required(self.auth_instance_biz_uuid, 'auth_instance_biz_uuid')
         self.validate_required(self.vc, 'vc')
         self.validate_required(self.be_authed_person_info, 'be_authed_person_info')
         if self.be_authed_person_info:
             self.be_authed_person_info.validate()
         self.validate_required(self.auth_person_enterprise_info, 'auth_person_enterprise_info')
         if self.auth_person_enterprise_info:
             self.auth_person_enterprise_info.validate()
@@ -1075,16 +1067,16 @@
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.auth_instance_id is not None:
-            result['auth_instance_id'] = self.auth_instance_id
+        if self.auth_instance_biz_uuid is not None:
+            result['auth_instance_biz_uuid'] = self.auth_instance_biz_uuid
         if self.vc is not None:
             result['vc'] = self.vc
         if self.be_authed_person_info is not None:
             result['be_authed_person_info'] = self.be_authed_person_info.to_map()
         if self.auth_person_enterprise_info is not None:
             result['auth_person_enterprise_info'] = self.auth_person_enterprise_info.to_map()
         result['data_source_info'] = []
@@ -1095,16 +1087,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('auth_instance_id') is not None:
-            self.auth_instance_id = m.get('auth_instance_id')
+        if m.get('auth_instance_biz_uuid') is not None:
+            self.auth_instance_biz_uuid = m.get('auth_instance_biz_uuid')
         if m.get('vc') is not None:
             self.vc = m.get('vc')
         if m.get('be_authed_person_info') is not None:
             temp_model = BeAuthedPersonInfo()
             self.be_authed_person_info = temp_model.from_map(m['be_authed_person_info'])
         if m.get('auth_person_enterprise_info') is not None:
             temp_model = AuthPersonEnterpriseInfo()
@@ -1170,36 +1162,36 @@
 
 
 class VerifyDasIndividualRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        auth_instance_id: str = None,
+        auth_instance_biz_uuid: str = None,
         vc: str = None,
         be_authed_person_info: BeAuthedPersonInfo = None,
         auth_person_individual_info: AuthPersonIndividualInfo = None,
         data_source_info: List[DataSource] = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 被授权企业接入应用ID
-        self.auth_instance_id = auth_instance_id
+        # 授权实例biz_uuid
+        self.auth_instance_biz_uuid = auth_instance_biz_uuid
         # VC完整内容
         self.vc = vc
         # 被授权企业信息
         self.be_authed_person_info = be_authed_person_info
         # 授权人个人信息
         self.auth_person_individual_info = auth_person_individual_info
         # 需要访问的数据源信息列表
         self.data_source_info = data_source_info
 
     def validate(self):
-        self.validate_required(self.auth_instance_id, 'auth_instance_id')
+        self.validate_required(self.auth_instance_biz_uuid, 'auth_instance_biz_uuid')
         self.validate_required(self.vc, 'vc')
         self.validate_required(self.be_authed_person_info, 'be_authed_person_info')
         if self.be_authed_person_info:
             self.be_authed_person_info.validate()
         self.validate_required(self.auth_person_individual_info, 'auth_person_individual_info')
         if self.auth_person_individual_info:
             self.auth_person_individual_info.validate()
@@ -1211,16 +1203,16 @@
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.auth_instance_id is not None:
-            result['auth_instance_id'] = self.auth_instance_id
+        if self.auth_instance_biz_uuid is not None:
+            result['auth_instance_biz_uuid'] = self.auth_instance_biz_uuid
         if self.vc is not None:
             result['vc'] = self.vc
         if self.be_authed_person_info is not None:
             result['be_authed_person_info'] = self.be_authed_person_info.to_map()
         if self.auth_person_individual_info is not None:
             result['auth_person_individual_info'] = self.auth_person_individual_info.to_map()
         result['data_source_info'] = []
@@ -1231,16 +1223,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('auth_instance_id') is not None:
-            self.auth_instance_id = m.get('auth_instance_id')
+        if m.get('auth_instance_biz_uuid') is not None:
+            self.auth_instance_biz_uuid = m.get('auth_instance_biz_uuid')
         if m.get('vc') is not None:
             self.vc = m.get('vc')
         if m.get('be_authed_person_info') is not None:
             temp_model = BeAuthedPersonInfo()
             self.be_authed_person_info = temp_model.from_map(m['be_authed_person_info'])
         if m.get('auth_person_individual_info') is not None:
             temp_model = AuthPersonIndividualInfo()
@@ -1375,80 +1367,80 @@
 
 class CreateDasDatasourceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        id: str = None,
+        biz_uuid: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 数据源ID
-        self.id = id
+        # 数据源 biz_uuid
+        self.biz_uuid = biz_uuid
 
     def validate(self):
         pass
 
     def to_map(self):
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.id is not None:
-            result['id'] = self.id
+        if self.biz_uuid is not None:
+            result['biz_uuid'] = self.biz_uuid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('id') is not None:
-            self.id = m.get('id')
+        if m.get('biz_uuid') is not None:
+            self.biz_uuid = m.get('biz_uuid')
         return self
 
 
 class UpdateDasDatasourceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        id: str = None,
+        biz_uuid: str = None,
         name: str = None,
         provider: str = None,
         data_owner_type: str = None,
         data_source_interface: DataSourceInterface = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 要修改的数据源ID
-        self.id = id
+        # 要修改的数据源biz_uuid
+        self.biz_uuid = biz_uuid
         # 数据源名称
         self.name = name
         # 数据源提供方
         self.provider = provider
         # 枚举值：ENTERPRISE、INDIVIDUAL
         self.data_owner_type = data_owner_type
         # 数据源接口定义
         self.data_source_interface = data_source_interface
 
     def validate(self):
-        self.validate_required(self.id, 'id')
+        self.validate_required(self.biz_uuid, 'biz_uuid')
         self.validate_required(self.name, 'name')
         if self.name is not None:
             self.validate_max_length(self.name, 'name', 20)
         self.validate_required(self.provider, 'provider')
         if self.provider is not None:
             self.validate_max_length(self.provider, 'provider', 30)
         self.validate_required(self.data_owner_type, 'data_owner_type')
@@ -1458,16 +1450,16 @@
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.id is not None:
-            result['id'] = self.id
+        if self.biz_uuid is not None:
+            result['biz_uuid'] = self.biz_uuid
         if self.name is not None:
             result['name'] = self.name
         if self.provider is not None:
             result['provider'] = self.provider
         if self.data_owner_type is not None:
             result['data_owner_type'] = self.data_owner_type
         if self.data_source_interface is not None:
@@ -1476,16 +1468,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('id') is not None:
-            self.id = m.get('id')
+        if m.get('biz_uuid') is not None:
+            self.biz_uuid = m.get('biz_uuid')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('provider') is not None:
             self.provider = m.get('provider')
         if m.get('data_owner_type') is not None:
             self.data_owner_type = m.get('data_owner_type')
         if m.get('data_source_interface') is not None:
@@ -1533,43 +1525,43 @@
 
 
 class DeleteDasDatasourceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        id: str = None,
+        biz_uuid: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 要删除的数据源ID
-        self.id = id
+        # 要删除的数据源biz_uuid
+        self.biz_uuid = biz_uuid
 
     def validate(self):
-        self.validate_required(self.id, 'id')
+        self.validate_required(self.biz_uuid, 'biz_uuid')
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.id is not None:
-            result['id'] = self.id
+        if self.biz_uuid is not None:
+            result['biz_uuid'] = self.biz_uuid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('id') is not None:
-            self.id = m.get('id')
+        if m.get('biz_uuid') is not None:
+            self.biz_uuid = m.get('biz_uuid')
         return self
 
 
 class DeleteDasDatasourceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -1725,55 +1717,55 @@
 
 
 class VerifyDasAuthresultRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        data_source_ids: List[str] = None,
+        data_source_biz_uuids: List[str] = None,
         be_authed_person_app_name: str = None,
         auth_person_enterprise_credit_num: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 数据源ID列表
-        self.data_source_ids = data_source_ids
+        # 数据源biz_uuid列表
+        self.data_source_biz_uuids = data_source_biz_uuids
         # 被授权企业接入应用名称
         self.be_authed_person_app_name = be_authed_person_app_name
         # 授权企业统一社会信用码
         self.auth_person_enterprise_credit_num = auth_person_enterprise_credit_num
 
     def validate(self):
-        self.validate_required(self.data_source_ids, 'data_source_ids')
+        self.validate_required(self.data_source_biz_uuids, 'data_source_biz_uuids')
         self.validate_required(self.be_authed_person_app_name, 'be_authed_person_app_name')
         self.validate_required(self.auth_person_enterprise_credit_num, 'auth_person_enterprise_credit_num')
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.data_source_ids is not None:
-            result['data_source_ids'] = self.data_source_ids
+        if self.data_source_biz_uuids is not None:
+            result['data_source_biz_uuids'] = self.data_source_biz_uuids
         if self.be_authed_person_app_name is not None:
             result['be_authed_person_app_name'] = self.be_authed_person_app_name
         if self.auth_person_enterprise_credit_num is not None:
             result['auth_person_enterprise_credit_num'] = self.auth_person_enterprise_credit_num
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('data_source_ids') is not None:
-            self.data_source_ids = m.get('data_source_ids')
+        if m.get('data_source_biz_uuids') is not None:
+            self.data_source_biz_uuids = m.get('data_source_biz_uuids')
         if m.get('be_authed_person_app_name') is not None:
             self.be_authed_person_app_name = m.get('be_authed_person_app_name')
         if m.get('auth_person_enterprise_credit_num') is not None:
             self.auth_person_enterprise_credit_num = m.get('auth_person_enterprise_credit_num')
         return self
 
 
@@ -1823,63 +1815,63 @@
 
 
 class AuthDasAuthresultRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        data_source_ids: List[str] = None,
+        data_source_biz_uuids: List[str] = None,
         be_authed_person_app_name: str = None,
         auth_person_enterprise_info: AuthPersonEnterpriseInfo = None,
         auth_person_individual_info: AuthPersonIndividualInfo = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 数据源ID列表
-        self.data_source_ids = data_source_ids
+        # 数据源biz_uuid列表
+        self.data_source_biz_uuids = data_source_biz_uuids
         # 被授权企业接入应用名称
         self.be_authed_person_app_name = be_authed_person_app_name
         # 授权企业信息
         self.auth_person_enterprise_info = auth_person_enterprise_info
         # 授权人信息
         self.auth_person_individual_info = auth_person_individual_info
 
     def validate(self):
-        self.validate_required(self.data_source_ids, 'data_source_ids')
+        self.validate_required(self.data_source_biz_uuids, 'data_source_biz_uuids')
         self.validate_required(self.be_authed_person_app_name, 'be_authed_person_app_name')
         if self.auth_person_enterprise_info:
             self.auth_person_enterprise_info.validate()
         if self.auth_person_individual_info:
             self.auth_person_individual_info.validate()
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.data_source_ids is not None:
-            result['data_source_ids'] = self.data_source_ids
+        if self.data_source_biz_uuids is not None:
+            result['data_source_biz_uuids'] = self.data_source_biz_uuids
         if self.be_authed_person_app_name is not None:
             result['be_authed_person_app_name'] = self.be_authed_person_app_name
         if self.auth_person_enterprise_info is not None:
             result['auth_person_enterprise_info'] = self.auth_person_enterprise_info.to_map()
         if self.auth_person_individual_info is not None:
             result['auth_person_individual_info'] = self.auth_person_individual_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('data_source_ids') is not None:
-            self.data_source_ids = m.get('data_source_ids')
+        if m.get('data_source_biz_uuids') is not None:
+            self.data_source_biz_uuids = m.get('data_source_biz_uuids')
         if m.get('be_authed_person_app_name') is not None:
             self.be_authed_person_app_name = m.get('be_authed_person_app_name')
         if m.get('auth_person_enterprise_info') is not None:
             temp_model = AuthPersonEnterpriseInfo()
             self.auth_person_enterprise_info = temp_model.from_map(m['auth_person_enterprise_info'])
         if m.get('auth_person_individual_info') is not None:
             temp_model = AuthPersonIndividualInfo()
@@ -1889,74 +1881,60 @@
 
 class AuthDasAuthresultResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        be_authed_person_id: str = None,
-        be_authed_person_app_id: str = None,
-        auth_instance_id: str = None,
-        auth_result_id: str = None,
+        auth_instance_biz_uuid: str = None,
+        auth_result_biz_uuid: str = None,
         vc: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 被授权企业ID
-        self.be_authed_person_id = be_authed_person_id
-        # 被授权企业接入应用ID
-        self.be_authed_person_app_id = be_authed_person_app_id
-        # 授权实例ID
-        self.auth_instance_id = auth_instance_id
-        # 授权详情ID
-        self.auth_result_id = auth_result_id
+        # 授权实例biz_uuid
+        self.auth_instance_biz_uuid = auth_instance_biz_uuid
+        # 授权详情biz_uuid
+        self.auth_result_biz_uuid = auth_result_biz_uuid
         # VC 完整信息
         self.vc = vc
 
     def validate(self):
         pass
 
     def to_map(self):
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.be_authed_person_id is not None:
-            result['be_authed_person_id'] = self.be_authed_person_id
-        if self.be_authed_person_app_id is not None:
-            result['be_authed_person_app_id'] = self.be_authed_person_app_id
-        if self.auth_instance_id is not None:
-            result['auth_instance_id'] = self.auth_instance_id
-        if self.auth_result_id is not None:
-            result['auth_result_id'] = self.auth_result_id
+        if self.auth_instance_biz_uuid is not None:
+            result['auth_instance_biz_uuid'] = self.auth_instance_biz_uuid
+        if self.auth_result_biz_uuid is not None:
+            result['auth_result_biz_uuid'] = self.auth_result_biz_uuid
         if self.vc is not None:
             result['vc'] = self.vc
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('be_authed_person_id') is not None:
-            self.be_authed_person_id = m.get('be_authed_person_id')
-        if m.get('be_authed_person_app_id') is not None:
-            self.be_authed_person_app_id = m.get('be_authed_person_app_id')
-        if m.get('auth_instance_id') is not None:
-            self.auth_instance_id = m.get('auth_instance_id')
-        if m.get('auth_result_id') is not None:
-            self.auth_result_id = m.get('auth_result_id')
+        if m.get('auth_instance_biz_uuid') is not None:
+            self.auth_instance_biz_uuid = m.get('auth_instance_biz_uuid')
+        if m.get('auth_result_biz_uuid') is not None:
+            self.auth_result_biz_uuid = m.get('auth_result_biz_uuid')
         if m.get('vc') is not None:
             self.vc = m.get('vc')
         return self
```

### Comparing `antchain_das-1.1.5/setup.py` & `antchain_das-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_das.
 
-Created on 03/09/2021
+Created on 14/09/2021
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_das"
 NAME = "antchain_das" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain DAS SDK Library for Python"
```

