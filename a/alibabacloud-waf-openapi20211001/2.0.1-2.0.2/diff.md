# Comparing `tmp/alibabacloud_waf-openapi20211001-2.0.1.tar.gz` & `tmp/alibabacloud_waf-openapi20211001-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_waf-openapi20211001-2.0.1.tar", last modified: Mon Dec  5 12:17:04 2022, max compression
+gzip compressed data, was "dist/alibabacloud_waf-openapi20211001-2.0.2.tar", last modified: Thu Apr 27 12:30:45 2023, max compression
```

## Comparing `alibabacloud_waf-openapi20211001-2.0.1.tar` & `alibabacloud_waf-openapi20211001-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/
--rw-r--r--   0 root         (0) root         (0)       68 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165402 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001/client.py
--rw-r--r--   0 root         (0) root         (0)   278325 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2652 2022-12-05 12:17:04.000000 alibabacloud_waf-openapi20211001-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204606 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001/client.py
+-rw-r--r--   0 root         (0) root         (0)   423950 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-04-27 12:30:45.000000 alibabacloud_waf-openapi20211001-2.0.2/setup.py
```

### Comparing `alibabacloud_waf-openapi20211001-2.0.1/LICENSE` & `alibabacloud_waf-openapi20211001-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-2.0.1/PKG-INFO` & `alibabacloud_waf-openapi20211001-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_waf-openapi20211001
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001-2.0.1/README-CN.md` & `alibabacloud_waf-openapi20211001-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-2.0.1/README.md` & `alibabacloud_waf-openapi20211001-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001/client.py` & `alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         request: waf_openapi_20211001_models.ClearMajorProtectionBlackIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ClearMajorProtectionBlackIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -104,14 +108,18 @@
         request: waf_openapi_20211001_models.ClearMajorProtectionBlackIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ClearMajorProtectionBlackIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -156,14 +164,18 @@
             query['AddList'] = request.add_list
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -190,14 +202,18 @@
             query['AddList'] = request.add_list
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -234,14 +250,18 @@
     ) -> waf_openapi_20211001_models.CreateDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.defense_scene):
             query['DefenseScene'] = request.defense_scene
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rules):
             query['Rules'] = request.rules
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -268,14 +288,18 @@
     ) -> waf_openapi_20211001_models.CreateDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.defense_scene):
             query['DefenseScene'] = request.defense_scene
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rules):
             query['Rules'] = request.rules
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -318,14 +342,18 @@
         query = {}
         if not UtilClient.is_unset(request.defense_scene):
             query['DefenseScene'] = request.defense_scene
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_name):
             query['TemplateName'] = request.template_name
         if not UtilClient.is_unset(request.template_origin):
             query['TemplateOrigin'] = request.template_origin
         if not UtilClient.is_unset(request.template_status):
             query['TemplateStatus'] = request.template_status
         if not UtilClient.is_unset(request.template_type):
@@ -358,14 +386,18 @@
         query = {}
         if not UtilClient.is_unset(request.defense_scene):
             query['DefenseScene'] = request.defense_scene
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_name):
             query['TemplateName'] = request.template_name
         if not UtilClient.is_unset(request.template_origin):
             query['TemplateOrigin'] = request.template_origin
         if not UtilClient.is_unset(request.template_status):
             query['TemplateStatus'] = request.template_status
         if not UtilClient.is_unset(request.template_type):
@@ -424,14 +456,18 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.listen_shrink):
             query['Listen'] = request.listen_shrink
         if not UtilClient.is_unset(request.redirect_shrink):
             query['Redirect'] = request.redirect_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateDomain',
             version='2021-10-01',
             protocol='HTTPS',
@@ -468,14 +504,18 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.listen_shrink):
             query['Listen'] = request.listen_shrink
         if not UtilClient.is_unset(request.redirect_shrink):
             query['Redirect'] = request.redirect_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateDomain',
             version='2021-10-01',
             protocol='HTTPS',
@@ -506,24 +546,35 @@
         return await self.create_domain_with_options_async(request, runtime)
 
     def create_major_protection_black_ip_with_options(
         self,
         request: waf_openapi_20211001_models.CreateMajorProtectionBlackIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.CreateMajorProtectionBlackIpResponse:
+        """
+        This operation is available only on the China site (aliyun.com).
+        
+        @param request: CreateMajorProtectionBlackIpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMajorProtectionBlackIpResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.expired_time):
             query['ExpiredTime'] = request.expired_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.ip_list):
             query['IpList'] = request.ip_list
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -544,24 +595,35 @@
         )
 
     async def create_major_protection_black_ip_with_options_async(
         self,
         request: waf_openapi_20211001_models.CreateMajorProtectionBlackIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.CreateMajorProtectionBlackIpResponse:
+        """
+        This operation is available only on the China site (aliyun.com).
+        
+        @param request: CreateMajorProtectionBlackIpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMajorProtectionBlackIpResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.expired_time):
             query['ExpiredTime'] = request.expired_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.ip_list):
             query['IpList'] = request.ip_list
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -581,35 +643,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_major_protection_black_ip(
         self,
         request: waf_openapi_20211001_models.CreateMajorProtectionBlackIpRequest,
     ) -> waf_openapi_20211001_models.CreateMajorProtectionBlackIpResponse:
+        """
+        This operation is available only on the China site (aliyun.com).
+        
+        @param request: CreateMajorProtectionBlackIpRequest
+        @return: CreateMajorProtectionBlackIpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_major_protection_black_ip_with_options(request, runtime)
 
     async def create_major_protection_black_ip_async(
         self,
         request: waf_openapi_20211001_models.CreateMajorProtectionBlackIpRequest,
     ) -> waf_openapi_20211001_models.CreateMajorProtectionBlackIpResponse:
+        """
+        This operation is available only on the China site (aliyun.com).
+        
+        @param request: CreateMajorProtectionBlackIpRequest
+        @return: CreateMajorProtectionBlackIpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_major_protection_black_ip_with_options_async(request, runtime)
 
     def delete_defense_resource_group_with_options(
         self,
         request: waf_openapi_20211001_models.DeleteDefenseResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DeleteDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -632,14 +710,18 @@
     ) -> waf_openapi_20211001_models.DeleteDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -674,14 +756,18 @@
         request: waf_openapi_20211001_models.DeleteDefenseRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DeleteDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_ids):
             query['RuleIds'] = request.rule_ids
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -706,14 +792,18 @@
         request: waf_openapi_20211001_models.DeleteDefenseRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DeleteDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_ids):
             query['RuleIds'] = request.rule_ids
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -752,14 +842,18 @@
         request: waf_openapi_20211001_models.DeleteDefenseTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DeleteDefenseTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteDefenseTemplate',
@@ -782,14 +876,18 @@
         request: waf_openapi_20211001_models.DeleteDefenseTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DeleteDefenseTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteDefenseTemplate',
@@ -828,18 +926,22 @@
     ) -> waf_openapi_20211001_models.DeleteDomainResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.access_type):
             query['AccessType'] = request.access_type
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.domain_id):
+            query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteDomain',
             version='2021-10-01',
             protocol='HTTPS',
@@ -862,18 +964,22 @@
     ) -> waf_openapi_20211001_models.DeleteDomainResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.access_type):
             query['AccessType'] = request.access_type
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.domain_id):
+            query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteDomain',
             version='2021-10-01',
             protocol='HTTPS',
@@ -910,14 +1016,18 @@
     ) -> waf_openapi_20211001_models.DeleteMajorProtectionBlackIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.ip_list):
             query['IpList'] = request.ip_list
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -944,14 +1054,18 @@
     ) -> waf_openapi_20211001_models.DeleteMajorProtectionBlackIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.ip_list):
             query['IpList'] = request.ip_list
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -992,14 +1106,18 @@
     ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1022,14 +1140,18 @@
     ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1070,14 +1192,22 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.query):
             query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseResources',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1104,14 +1234,22 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.query):
             query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseResources',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1146,14 +1284,18 @@
         request: waf_openapi_20211001_models.DescribeDefenseRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1178,14 +1320,18 @@
         request: waf_openapi_20211001_models.DescribeDefenseRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1230,14 +1376,18 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.query):
             query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseRules',
@@ -1266,14 +1416,18 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.query):
             query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseRules',
@@ -1310,14 +1464,18 @@
         request: waf_openapi_20211001_models.DescribeDefenseTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseTemplate',
@@ -1340,14 +1498,18 @@
         request: waf_openapi_20211001_models.DescribeDefenseTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDefenseTemplate',
@@ -1386,14 +1548,18 @@
     ) -> waf_openapi_20211001_models.DescribeDomainDetailResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDomainDetail',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1416,14 +1582,18 @@
     ) -> waf_openapi_20211001_models.DescribeDomainDetailResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDomainDetail',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1466,14 +1636,22 @@
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDomains',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1502,14 +1680,22 @@
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDomains',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1548,16 +1734,20 @@
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeFlowChart',
@@ -1584,16 +1774,20 @@
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeFlowChart',
@@ -1632,14 +1826,18 @@
     ) -> waf_openapi_20211001_models.DescribeFlowTopResourceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeFlowTopResource',
@@ -1664,14 +1862,18 @@
     ) -> waf_openapi_20211001_models.DescribeFlowTopResourceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeFlowTopResource',
@@ -1710,16 +1912,20 @@
     ) -> waf_openapi_20211001_models.DescribeFlowTopUrlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeFlowTopUrl',
@@ -1744,16 +1950,20 @@
     ) -> waf_openapi_20211001_models.DescribeFlowTopUrlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeFlowTopUrl',
@@ -1781,25 +1991,307 @@
     async def describe_flow_top_url_async(
         self,
         request: waf_openapi_20211001_models.DescribeFlowTopUrlRequest,
     ) -> waf_openapi_20211001_models.DescribeFlowTopUrlResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_flow_top_url_with_options_async(request, runtime)
 
+    def describe_hybrid_cloud_groups_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudGroupsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.cluster_proxy_type):
+            query['ClusterProxyType'] = request.cluster_proxy_type
+        if not UtilClient.is_unset(request.group_name):
+            query['GroupName'] = request.group_name
+        if not UtilClient.is_unset(request.group_type):
+            query['GroupType'] = request.group_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHybridCloudGroups',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeHybridCloudGroupsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_hybrid_cloud_groups_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudGroupsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.cluster_proxy_type):
+            query['ClusterProxyType'] = request.cluster_proxy_type
+        if not UtilClient.is_unset(request.group_name):
+            query['GroupName'] = request.group_name
+        if not UtilClient.is_unset(request.group_type):
+            query['GroupType'] = request.group_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHybridCloudGroups',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeHybridCloudGroupsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_hybrid_cloud_groups(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudGroupsRequest,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_hybrid_cloud_groups_with_options(request, runtime)
+
+    async def describe_hybrid_cloud_groups_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudGroupsRequest,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_hybrid_cloud_groups_with_options_async(request, runtime)
+
+    def describe_hybrid_cloud_resources_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.backend):
+            query['Backend'] = request.backend
+        if not UtilClient.is_unset(request.cname_enabled):
+            query['CnameEnabled'] = request.cname_enabled
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHybridCloudResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeHybridCloudResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_hybrid_cloud_resources_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.backend):
+            query['Backend'] = request.backend
+        if not UtilClient.is_unset(request.cname_enabled):
+            query['CnameEnabled'] = request.cname_enabled
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHybridCloudResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeHybridCloudResourcesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_hybrid_cloud_resources(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudResourcesRequest,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_hybrid_cloud_resources_with_options(request, runtime)
+
+    async def describe_hybrid_cloud_resources_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudResourcesRequest,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_hybrid_cloud_resources_with_options_async(request, runtime)
+
+    def describe_hybrid_cloud_user_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHybridCloudUser',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeHybridCloudUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_hybrid_cloud_user_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHybridCloudUser',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeHybridCloudUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_hybrid_cloud_user(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudUserRequest,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_hybrid_cloud_user_with_options(request, runtime)
+
+    async def describe_hybrid_cloud_user_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeHybridCloudUserRequest,
+    ) -> waf_openapi_20211001_models.DescribeHybridCloudUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_hybrid_cloud_user_with_options_async(request, runtime)
+
     def describe_instance_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_group_id):
-            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeInstance',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1820,16 +2312,16 @@
         request: waf_openapi_20211001_models.DescribeInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.resource_group_id):
-            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeInstance',
             version='2021-10-01',
             protocol='HTTPS',
@@ -1872,14 +2364,18 @@
             query['IpLike'] = request.ip_like
         if not UtilClient.is_unset(request.order_by):
             query['OrderBy'] = request.order_by
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1912,14 +2408,18 @@
             query['IpLike'] = request.ip_like
         if not UtilClient.is_unset(request.order_by):
             query['OrderBy'] = request.order_by
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1962,16 +2462,20 @@
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePeakTrend',
@@ -1998,16 +2502,20 @@
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePeakTrend',
@@ -2044,14 +2552,18 @@
         request: waf_openapi_20211001_models.DescribeResourceLogStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeResourceLogStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.resources):
             query['Resources'] = request.resources
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeResourceLogStatus',
@@ -2074,14 +2586,18 @@
         request: waf_openapi_20211001_models.DescribeResourceLogStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeResourceLogStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.resources):
             query['Resources'] = request.resources
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeResourceLogStatus',
@@ -2118,16 +2634,20 @@
         request: waf_openapi_20211001_models.DescribeResourcePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeResourcePortResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_instance_id):
             query['ResourceInstanceId'] = request.resource_instance_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeResourcePort',
             version='2021-10-01',
             protocol='HTTPS',
@@ -2148,16 +2668,20 @@
         request: waf_openapi_20211001_models.DescribeResourcePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeResourcePortResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_instance_id):
             query['ResourceInstanceId'] = request.resource_instance_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeResourcePort',
             version='2021-10-01',
             protocol='HTTPS',
@@ -2196,16 +2720,20 @@
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2234,16 +2762,20 @@
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.interval):
             query['Interval'] = request.interval
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2286,14 +2818,18 @@
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.search_type):
             query['SearchType'] = request.search_type
         if not UtilClient.is_unset(request.search_value):
             query['SearchValue'] = request.search_value
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2322,14 +2858,18 @@
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.search_type):
             query['SearchType'] = request.search_type
         if not UtilClient.is_unset(request.search_value):
             query['SearchValue'] = request.search_value
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2370,16 +2910,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopClientIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2406,16 +2950,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopClientIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2456,14 +3004,18 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopResourceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2490,14 +3042,18 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopResourceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2538,16 +3094,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopRuleIdResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2574,16 +3134,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopRuleIdResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2624,14 +3188,16 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopTuleTypeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2658,14 +3224,16 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopTuleTypeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2706,16 +3274,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopUaResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRuleHitsTopUa',
@@ -2740,16 +3312,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopUaResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRuleHitsTopUa',
@@ -2788,16 +3364,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopUrlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2824,16 +3404,20 @@
     ) -> waf_openapi_20211001_models.DescribeRuleHitsTopUrlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2872,14 +3456,18 @@
         request: waf_openapi_20211001_models.DescribeTemplateResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeTemplateResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2904,14 +3492,18 @@
         request: waf_openapi_20211001_models.DescribeTemplateResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeTemplateResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2952,16 +3544,20 @@
     ) -> waf_openapi_20211001_models.DescribeVisitTopIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeVisitTopIp',
@@ -2986,16 +3582,20 @@
     ) -> waf_openapi_20211001_models.DescribeVisitTopIpResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeVisitTopIp',
@@ -3034,14 +3634,16 @@
     ) -> waf_openapi_20211001_models.DescribeVisitUasResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3068,14 +3670,16 @@
     ) -> waf_openapi_20211001_models.DescribeVisitUasResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_timestamp):
             query['EndTimestamp'] = request.end_timestamp
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
         if not UtilClient.is_unset(request.start_timestamp):
             query['StartTimestamp'] = request.start_timestamp
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3114,14 +3718,18 @@
         request: waf_openapi_20211001_models.DescribeWafSourceIpSegmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeWafSourceIpSegmentResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeWafSourceIpSegment',
             version='2021-10-01',
             protocol='HTTPS',
@@ -3142,14 +3750,18 @@
         request: waf_openapi_20211001_models.DescribeWafSourceIpSegmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeWafSourceIpSegmentResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeWafSourceIpSegment',
             version='2021-10-01',
             protocol='HTTPS',
@@ -3192,14 +3804,18 @@
             query['DeleteList'] = request.delete_list
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -3228,14 +3844,18 @@
             query['DeleteList'] = request.delete_list
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDefenseResourceGroup',
             version='2021-10-01',
             protocol='HTTPS',
@@ -3272,14 +3892,18 @@
     ) -> waf_openapi_20211001_models.ModifyDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.defense_scene):
             query['DefenseScene'] = request.defense_scene
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rules):
             query['Rules'] = request.rules
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3306,14 +3930,18 @@
     ) -> waf_openapi_20211001_models.ModifyDefenseRuleResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.defense_scene):
             query['DefenseScene'] = request.defense_scene
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rules):
             query['Rules'] = request.rules
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3352,14 +3980,18 @@
         request: waf_openapi_20211001_models.ModifyDefenseRuleStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyDefenseRuleStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.rule_status):
             query['RuleStatus'] = request.rule_status
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
@@ -3386,14 +4018,18 @@
         request: waf_openapi_20211001_models.ModifyDefenseRuleStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyDefenseRuleStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.rule_status):
             query['RuleStatus'] = request.rule_status
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
@@ -3436,14 +4072,18 @@
     ) -> waf_openapi_20211001_models.ModifyDefenseTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         if not UtilClient.is_unset(request.template_name):
             query['TemplateName'] = request.template_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3470,14 +4110,18 @@
     ) -> waf_openapi_20211001_models.ModifyDefenseTemplateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         if not UtilClient.is_unset(request.template_name):
             query['TemplateName'] = request.template_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3516,14 +4160,18 @@
         request: waf_openapi_20211001_models.ModifyDefenseTemplateStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyDefenseTemplateStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         if not UtilClient.is_unset(request.template_status):
             query['TemplateStatus'] = request.template_status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3548,14 +4196,18 @@
         request: waf_openapi_20211001_models.ModifyDefenseTemplateStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyDefenseTemplateStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         if not UtilClient.is_unset(request.template_status):
             query['TemplateStatus'] = request.template_status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3610,14 +4262,16 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.listen_shrink):
             query['Listen'] = request.listen_shrink
         if not UtilClient.is_unset(request.redirect_shrink):
             query['Redirect'] = request.redirect_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDomain',
             version='2021-10-01',
             protocol='HTTPS',
@@ -3654,14 +4308,16 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.listen_shrink):
             query['Listen'] = request.listen_shrink
         if not UtilClient.is_unset(request.redirect_shrink):
             query['Redirect'] = request.redirect_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_ip):
+            query['SourceIp'] = request.source_ip
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDomain',
             version='2021-10-01',
             protocol='HTTPS',
@@ -3702,14 +4358,18 @@
             query['Description'] = request.description
         if not UtilClient.is_unset(request.expired_time):
             query['ExpiredTime'] = request.expired_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.ip_list):
             query['IpList'] = request.ip_list
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3740,14 +4400,18 @@
             query['Description'] = request.description
         if not UtilClient.is_unset(request.expired_time):
             query['ExpiredTime'] = request.expired_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.ip_list):
             query['IpList'] = request.ip_list
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.rule_id):
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3786,16 +4450,20 @@
         request: waf_openapi_20211001_models.ModifyResourceLogStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyResourceLogStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyResourceLogStatus',
@@ -3818,16 +4486,20 @@
         request: waf_openapi_20211001_models.ModifyResourceLogStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyResourceLogStatusResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyResourceLogStatus',
@@ -3868,14 +4540,18 @@
         query = {}
         if not UtilClient.is_unset(request.bind_resource_groups):
             query['BindResourceGroups'] = request.bind_resource_groups
         if not UtilClient.is_unset(request.bind_resources):
             query['BindResources'] = request.bind_resources
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         if not UtilClient.is_unset(request.unbind_resource_groups):
             query['UnbindResourceGroups'] = request.unbind_resource_groups
         if not UtilClient.is_unset(request.unbind_resources):
             query['UnbindResources'] = request.unbind_resources
         req = open_api_models.OpenApiRequest(
@@ -3906,14 +4582,18 @@
         query = {}
         if not UtilClient.is_unset(request.bind_resource_groups):
             query['BindResourceGroups'] = request.bind_resource_groups
         if not UtilClient.is_unset(request.bind_resources):
             query['BindResources'] = request.bind_resources
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
         if not UtilClient.is_unset(request.template_id):
             query['TemplateId'] = request.template_id
         if not UtilClient.is_unset(request.unbind_resource_groups):
             query['UnbindResourceGroups'] = request.unbind_resource_groups
         if not UtilClient.is_unset(request.unbind_resources):
             query['UnbindResources'] = request.unbind_resources
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_waf-openapi20211001-2.0.1/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO` & `alibabacloud_waf-openapi20211001-2.0.2/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-waf-openapi20211001
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001-2.0.1/setup.py` & `alibabacloud_waf-openapi20211001-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_waf-openapi20211001.
 
-Created on 05/12/2022
+Created on 27/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_waf_openapi20211001"
 NAME = "alibabacloud_waf-openapi20211001" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud waf-openapi (20211001) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

