# Comparing `tmp/alibabacloud_waf-openapi20211001_py2-2.0.1.tar.gz` & `tmp/alibabacloud_waf-openapi20211001_py2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_waf-openapi20211001_py2-2.0.1.tar", last modified: Mon Dec  5 12:16:21 2022, max compression
+gzip compressed data, was "dist/alibabacloud_waf-openapi20211001_py2-2.0.2.tar", last modified: Thu Apr 27 12:30:10 2023, max compression
```

## Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1.tar` & `alibabacloud_waf-openapi20211001_py2-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/
--rw-r--r--   0 root         (0) root         (0)       68 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67902 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001/client.py
--rw-r--r--   0 root         (0) root         (0)   280752 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2945 2022-12-05 12:16:21.000000 alibabacloud_waf-openapi20211001_py2-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86361 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001/client.py
+-rw-r--r--   0 root         (0) root         (0)   427194 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-27 12:30:10.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-04-27 12:30:09.000000 alibabacloud_waf-openapi20211001_py2-2.0.2/setup.py
```

### Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1/LICENSE` & `alibabacloud_waf-openapi20211001_py2-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1/PKG-INFO` & `alibabacloud_waf-openapi20211001_py2-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_waf-openapi20211001_py2
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1/README-CN.md` & `alibabacloud_waf-openapi20211001_py2-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1/README.md` & `alibabacloud_waf-openapi20211001_py2-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001/client.py` & `alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -57,14 +57,18 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def clear_major_protection_black_ip_with_options(self, request, runtime):
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
@@ -95,14 +99,18 @@
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
@@ -125,14 +133,18 @@
     def create_defense_rule_with_options(self, request, runtime):
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
@@ -161,14 +173,18 @@
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
@@ -197,30 +213,34 @@
         return self.create_defense_template_with_options(request, runtime)
 
     def create_domain_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = waf_openapi_20211001_models.CreateDomainShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.listen):
-            request.listen_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.listen), 'Listen', 'json')
+            request.listen_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.listen, 'Listen', 'json')
         if not UtilClient.is_unset(tmp_req.redirect):
-            request.redirect_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.redirect), 'Redirect', 'json')
+            request.redirect_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.redirect, 'Redirect', 'json')
         query = {}
         if not UtilClient.is_unset(request.access_type):
             query['AccessType'] = request.access_type
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_id):
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
@@ -237,24 +257,38 @@
         )
 
     def create_domain(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_domain_with_options(request, runtime)
 
     def create_major_protection_black_ip_with_options(self, request, runtime):
+        """
+        This operation is available only on the China site (aliyun.com).
+        
+
+        @param request: CreateMajorProtectionBlackIpRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
@@ -271,24 +305,36 @@
         )
         return TeaCore.from_map(
             waf_openapi_20211001_models.CreateMajorProtectionBlackIpResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_major_protection_black_ip(self, request):
+        """
+        This operation is available only on the China site (aliyun.com).
+        
+
+        @param request: CreateMajorProtectionBlackIpRequest
+
+        @return: CreateMajorProtectionBlackIpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_major_protection_black_ip_with_options(request, runtime)
 
     def delete_defense_resource_group_with_options(self, request, runtime):
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
@@ -309,14 +355,18 @@
         return self.delete_defense_resource_group_with_options(request, runtime)
 
     def delete_defense_rule_with_options(self, request, runtime):
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
@@ -341,14 +391,18 @@
         return self.delete_defense_rule_with_options(request, runtime)
 
     def delete_defense_template_with_options(self, request, runtime):
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
@@ -373,18 +427,22 @@
     def delete_domain_with_options(self, request, runtime):
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
@@ -407,14 +465,18 @@
     def delete_major_protection_black_ip_with_options(self, request, runtime):
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
@@ -441,14 +503,18 @@
     def describe_defense_resource_group_with_options(self, request, runtime):
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
@@ -475,14 +541,22 @@
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
@@ -503,14 +577,18 @@
         return self.describe_defense_resources_with_options(request, runtime)
 
     def describe_defense_rule_with_options(self, request, runtime):
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
@@ -541,14 +619,18 @@
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
@@ -571,14 +653,18 @@
         return self.describe_defense_rules_with_options(request, runtime)
 
     def describe_defense_template_with_options(self, request, runtime):
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
@@ -603,14 +689,18 @@
     def describe_domain_detail_with_options(self, request, runtime):
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
@@ -639,14 +729,22 @@
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
@@ -671,16 +769,20 @@
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
@@ -705,14 +807,18 @@
     def describe_flow_top_resource_with_options(self, request, runtime):
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
@@ -737,16 +843,20 @@
     def describe_flow_top_url_with_options(self, request, runtime):
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
@@ -764,21 +874,141 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_flow_top_url(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_flow_top_url_with_options(request, runtime)
 
+    def describe_hybrid_cloud_groups_with_options(self, request, runtime):
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
+    def describe_hybrid_cloud_groups(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_hybrid_cloud_groups_with_options(request, runtime)
+
+    def describe_hybrid_cloud_resources_with_options(self, request, runtime):
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
+    def describe_hybrid_cloud_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_hybrid_cloud_resources_with_options(request, runtime)
+
+    def describe_hybrid_cloud_user_with_options(self, request, runtime):
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
+    def describe_hybrid_cloud_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_hybrid_cloud_user_with_options(request, runtime)
+
     def describe_instance_with_options(self, request, runtime):
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
@@ -807,14 +1037,18 @@
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
@@ -843,16 +1077,20 @@
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
@@ -875,14 +1113,18 @@
         return self.describe_peak_trend_with_options(request, runtime)
 
     def describe_resource_log_status_with_options(self, request, runtime):
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
@@ -905,16 +1147,20 @@
         return self.describe_resource_log_status_with_options(request, runtime)
 
     def describe_resource_port_with_options(self, request, runtime):
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
@@ -939,16 +1185,20 @@
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
@@ -977,14 +1227,18 @@
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
@@ -1011,16 +1265,20 @@
     def describe_rule_hits_top_client_ip_with_options(self, request, runtime):
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
@@ -1047,14 +1305,18 @@
     def describe_rule_hits_top_resource_with_options(self, request, runtime):
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
@@ -1081,16 +1343,20 @@
     def describe_rule_hits_top_rule_id_with_options(self, request, runtime):
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
@@ -1117,14 +1383,16 @@
     def describe_rule_hits_top_tule_type_with_options(self, request, runtime):
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
@@ -1151,16 +1419,20 @@
     def describe_rule_hits_top_ua_with_options(self, request, runtime):
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
@@ -1185,16 +1457,20 @@
     def describe_rule_hits_top_url_with_options(self, request, runtime):
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
@@ -1219,14 +1495,18 @@
         return self.describe_rule_hits_top_url_with_options(request, runtime)
 
     def describe_template_resources_with_options(self, request, runtime):
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
@@ -1253,16 +1533,20 @@
     def describe_visit_top_ip_with_options(self, request, runtime):
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
@@ -1287,14 +1571,16 @@
     def describe_visit_uas_with_options(self, request, runtime):
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
@@ -1319,14 +1605,18 @@
         return self.describe_visit_uas_with_options(request, runtime)
 
     def describe_waf_source_ip_segment_with_options(self, request, runtime):
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
@@ -1355,14 +1645,18 @@
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
@@ -1385,14 +1679,18 @@
     def modify_defense_rule_with_options(self, request, runtime):
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
@@ -1417,14 +1715,18 @@
         return self.modify_defense_rule_with_options(request, runtime)
 
     def modify_defense_rule_status_with_options(self, request, runtime):
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
@@ -1453,14 +1755,18 @@
     def modify_defense_template_with_options(self, request, runtime):
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
@@ -1485,14 +1791,18 @@
         return self.modify_defense_template_with_options(request, runtime)
 
     def modify_defense_template_status_with_options(self, request, runtime):
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
@@ -1517,30 +1827,32 @@
         return self.modify_defense_template_status_with_options(request, runtime)
 
     def modify_domain_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = waf_openapi_20211001_models.ModifyDomainShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.listen):
-            request.listen_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.listen), 'Listen', 'json')
+            request.listen_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.listen, 'Listen', 'json')
         if not UtilClient.is_unset(tmp_req.redirect):
-            request.redirect_shrink = OpenApiUtilClient.array_to_string_with_specified_style(TeaCore.to_map(tmp_req.redirect), 'Redirect', 'json')
+            request.redirect_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.redirect, 'Redirect', 'json')
         query = {}
         if not UtilClient.is_unset(request.access_type):
             query['AccessType'] = request.access_type
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_id):
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
@@ -1567,14 +1879,18 @@
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
@@ -1599,16 +1915,20 @@
         return self.modify_major_protection_black_ip_with_options(request, runtime)
 
     def modify_resource_log_status_with_options(self, request, runtime):
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
@@ -1635,14 +1955,18 @@
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

### Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO` & `alibabacloud_waf-openapi20211001_py2-2.0.2/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-waf-openapi20211001-py2
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-2.0.1/setup.py` & `alibabacloud_waf-openapi20211001_py2-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_waf-openapi20211001_py2.
 
-Created on 05/12/2022
+Created on 27/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_waf_openapi20211001"
 NAME = "alibabacloud_waf-openapi20211001_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud waf-openapi (20211001) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

