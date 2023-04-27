# Comparing `tmp/alibabacloud_adcp20220101_py2-1.0.8.tar.gz` & `tmp/alibabacloud_adcp20220101_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adcp20220101_py2-1.0.8.tar", last modified: Thu Mar 16 01:42:12 2023, max compression
+gzip compressed data, was "dist/alibabacloud_adcp20220101_py2-1.0.9.tar", last modified: Thu Apr 27 03:09:52 2023, max compression
```

## Comparing `alibabacloud_adcp20220101_py2-1.0.8.tar` & `alibabacloud_adcp20220101_py2-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      665 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20562 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101/client.py
--rw-r--r--   0 root         (0) root         (0)   116539 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-03-16 01:42:12.000000 alibabacloud_adcp20220101_py2-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      736 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33022 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)   189208 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-04-27 03:09:52.000000 alibabacloud_adcp20220101_py2-1.0.9/setup.py
```

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/ChangeLog.md` & `alibabacloud_adcp20220101_py2-1.0.9/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-03-16 Version: 1.0.8
+- DescribeUserPermissions Remove uid info.
+
+
 2023-03-09 Version: 1.0.7
 -  GrantUserPermissions Add new api.
 - DescribeUserPermissions Add new api.
 
 
 2023-02-07 Version: 1.0.6
 - UpdateHubClusterFeature VSwitches can be configured.
```

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/LICENSE` & `alibabacloud_adcp20220101_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/PKG-INFO` & `alibabacloud_adcp20220101_py2-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_adcp20220101_py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/README-CN.md` & `alibabacloud_adcp20220101_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/README.md` & `alibabacloud_adcp20220101_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101/client.py` & `alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -170,14 +170,122 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_hub_cluster(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_hub_cluster_with_options(request, runtime)
 
+    def delete_policy_instance_with_options(self, tmp_req, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = adcp_20220101_models.DeletePolicyInstanceShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.cluster_ids):
+            request.cluster_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.cluster_ids, 'ClusterIds', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.cluster_ids_shrink):
+            query['ClusterIds'] = request.cluster_ids_shrink
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeletePolicyInstance',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DeletePolicyInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_policy_instance(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_policy_instance_with_options(request, runtime)
+
+    def delete_user_permission_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteUserPermission',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DeleteUserPermissionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_user_permission(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_user_permission_with_options(request, runtime)
+
+    def deploy_policy_instance_with_options(self, tmp_req, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = adcp_20220101_models.DeployPolicyInstanceShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.cluster_ids):
+            request.cluster_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.cluster_ids, 'ClusterIds', 'json')
+        if not UtilClient.is_unset(tmp_req.namespaces):
+            request.namespaces_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.namespaces, 'Namespaces', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.cluster_ids_shrink):
+            query['ClusterIds'] = request.cluster_ids_shrink
+        if not UtilClient.is_unset(request.namespaces_shrink):
+            query['Namespaces'] = request.namespaces_shrink
+        if not UtilClient.is_unset(request.policy_action):
+            query['PolicyAction'] = request.policy_action
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeployPolicyInstance',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DeployPolicyInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def deploy_policy_instance(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.deploy_policy_instance_with_options(request, runtime)
+
     def describe_hub_cluster_details_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cluster_id):
             query['ClusterId'] = request.cluster_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
@@ -312,14 +420,150 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_managed_clusters(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_managed_clusters_with_options(request, runtime)
 
+    def describe_policies_with_options(self, runtime):
+        req = open_api_models.OpenApiRequest()
+        params = open_api_models.Params(
+            action='DescribePolicies',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DescribePoliciesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_policies(self):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policies_with_options(runtime)
+
+    def describe_policy_details_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePolicyDetails',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DescribePolicyDetailsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_policy_details(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_details_with_options(request, runtime)
+
+    def describe_policy_governance_in_cluster_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePolicyGovernanceInCluster',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DescribePolicyGovernanceInClusterResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_policy_governance_in_cluster(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_governance_in_cluster_with_options(request, runtime)
+
+    def describe_policy_instances_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePolicyInstances',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DescribePolicyInstancesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_policy_instances(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_instances_with_options(request, runtime)
+
+    def describe_policy_instances_status_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePolicyInstancesStatus',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.DescribePolicyInstancesStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_policy_instances_status(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_instances_status_with_options(request, runtime)
+
     def describe_regions_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -400,14 +644,50 @@
             self.call_api(params, req, runtime)
         )
 
     def detach_cluster_from_hub(self, request):
         runtime = util_models.RuntimeOptions()
         return self.detach_cluster_from_hub_with_options(request, runtime)
 
+    def grant_user_permission_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.role_name):
+            query['RoleName'] = request.role_name
+        if not UtilClient.is_unset(request.role_type):
+            query['RoleType'] = request.role_type
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GrantUserPermission',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.GrantUserPermissionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def grant_user_permission(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.grant_user_permission_with_options(request, runtime)
+
     def grant_user_permissions_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = adcp_20220101_models.GrantUserPermissionsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.permissions):
             request.permissions_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.permissions, 'Permissions', 'json')
         query = {}
@@ -487,7 +767,43 @@
             adcp_20220101_models.UpdateHubClusterFeatureResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_hub_cluster_feature(self, request):
         runtime = util_models.RuntimeOptions()
         return self.update_hub_cluster_feature_with_options(request, runtime)
+
+    def update_user_permission_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.namespace):
+            query['Namespace'] = request.namespace
+        if not UtilClient.is_unset(request.role_name):
+            query['RoleName'] = request.role_name
+        if not UtilClient.is_unset(request.role_type):
+            query['RoleType'] = request.role_type
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateUserPermission',
+            version='2022-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            adcp_20220101_models.UpdateUserPermissionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def update_user_permission(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.update_user_permission_with_options(request, runtime)
```

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101/models.py` & `alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -122,30 +122,36 @@
         return self
 
 
 class CreateHubClusterRequest(TeaModel):
     def __init__(self, api_server_public_eip=None, argo_server_enabled=None, audit_log_enabled=None,
                  is_enterprise_security_group=None, name=None, price_limit=None, profile=None, region_id=None, v_switches=None, vpc_id=None,
                  workflow_schedule_mode=None):
-        # Specifies whether to use a public IP address to expose the API server. Valid values: - true: uses a public IP address to expose the API server. - true: uses an internal IP address to expose the API server.
+        # Specifies whether to expose the API server to the Internet. Valid values:
+        # 
+        # *   true: exposes the API server to the Internet.
+        # *   false: exposes the API server to the internal network.
         self.api_server_public_eip = api_server_public_eip  # type: bool
         self.argo_server_enabled = argo_server_enabled  # type: bool
-        # Specifies whether to enable audit logs. Valid values: - true: enables audit logs. - false: disables audit logs.
+        # Specifies whether to enable the audit log feature. Valid values:
+        # 
+        # *   true: enables the audit log feature.
+        # *   false: disables the audit log feature.
         self.audit_log_enabled = audit_log_enabled  # type: bool
-        # Specifies whether the security group is an advanced security group.
+        # Specifies whether to use an advanced security group.
         self.is_enterprise_security_group = is_enterprise_security_group  # type: bool
         # The name of the master instance.
         self.name = name  # type: str
         self.price_limit = price_limit  # type: str
-        # Scenario-oriented master control type. The value can be:
+        # The type of scenario for which the master instance is suitable. Valid values:
         # 
-        # - `Default`: Standard scenario Master instance.
-        # - `XFlow`: Workflow scenario master instance.
+        # *   `Default`: The master instance is suitable for standard scenarios.
+        # *   `XFlow`: The master instance is suitable for workflow scenarios.
         # 
-        # Default Value: `Default`.
+        # Default value: `Default`.
         self.profile = profile  # type: str
         # The ID of the region. You can call the DescribeRegions operation to query available regions.
         self.region_id = region_id  # type: str
         # The ID of the vSwitch.
         self.v_switches = v_switches  # type: str
         # The ID of the virtual private cloud (VPC) to which the master instance belongs. You can call the DescribeVpcs operation to query available VPCs.
         self.vpc_id = vpc_id  # type: str
@@ -287,16 +293,22 @@
         return self
 
 
 class DeleteHubClusterRequest(TeaModel):
     def __init__(self, cluster_id=None, force=None, retain_resources=None):
         # The ID of the master instance.
         self.cluster_id = cluster_id  # type: str
-        # Specifies whether to forcefully delete the master instance. Valid values: - true: forcefully delete the master instance. - false: does not forcefully delete the master instance. Default value: false.
+        # Specifies whether to forcefully delete the master instance in ACK One. Valid values:
+        # 
+        # *   true: forcefully deletes the master instance in ACK One.
+        # *   false: does not forcibly delete the master instance in ACK One.
+        # 
+        # Default value: false.
         self.force = force  # type: bool
+        # The list of resources to retain.
         self.retain_resources = retain_resources  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteHubClusterRequest, self).to_map()
@@ -323,16 +335,22 @@
         return self
 
 
 class DeleteHubClusterShrinkRequest(TeaModel):
     def __init__(self, cluster_id=None, force=None, retain_resources_shrink=None):
         # The ID of the master instance.
         self.cluster_id = cluster_id  # type: str
-        # Specifies whether to forcefully delete the master instance. Valid values: - true: forcefully delete the master instance. - false: does not forcefully delete the master instance. Default value: false.
+        # Specifies whether to forcefully delete the master instance in ACK One. Valid values:
+        # 
+        # *   true: forcefully deletes the master instance in ACK One.
+        # *   false: does not forcibly delete the master instance in ACK One.
+        # 
+        # Default value: false.
         self.force = force  # type: bool
+        # The list of resources to retain.
         self.retain_resources_shrink = retain_resources_shrink  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteHubClusterShrinkRequest, self).to_map()
@@ -357,19 +375,19 @@
         if m.get('RetainResources') is not None:
             self.retain_resources_shrink = m.get('RetainResources')
         return self
 
 
 class DeleteHubClusterResponseBody(TeaModel):
     def __init__(self, cluster_id=None, request_id=None, task_id=None):
-        # The ID of the master instance.
+        # The ID of the cluster.
         self.cluster_id = cluster_id  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The ID of the master instance.
+        # The ID of the job.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteHubClusterResponseBody, self).to_map()
@@ -431,14 +449,392 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteHubClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeletePolicyInstanceRequest(TeaModel):
+    def __init__(self, cluster_id=None, cluster_ids=None, policy_name=None):
+        self.cluster_id = cluster_id  # type: str
+        self.cluster_ids = cluster_ids  # type: list[str]
+        self.policy_name = policy_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeletePolicyInstanceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.cluster_ids is not None:
+            result['ClusterIds'] = self.cluster_ids
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('ClusterIds') is not None:
+            self.cluster_ids = m.get('ClusterIds')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DeletePolicyInstanceShrinkRequest(TeaModel):
+    def __init__(self, cluster_id=None, cluster_ids_shrink=None, policy_name=None):
+        self.cluster_id = cluster_id  # type: str
+        self.cluster_ids_shrink = cluster_ids_shrink  # type: str
+        self.policy_name = policy_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeletePolicyInstanceShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.cluster_ids_shrink is not None:
+            result['ClusterIds'] = self.cluster_ids_shrink
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('ClusterIds') is not None:
+            self.cluster_ids_shrink = m.get('ClusterIds')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DeletePolicyInstanceResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeletePolicyInstanceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeletePolicyInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeletePolicyInstanceResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeletePolicyInstanceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeletePolicyInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteUserPermissionRequest(TeaModel):
+    def __init__(self, cluster_id=None, user_id=None):
+        # The ID of the master instance.
+        self.cluster_id = cluster_id  # type: str
+        # The ID of the RAM user.
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteUserPermissionRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class DeleteUserPermissionResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteUserPermissionResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteUserPermissionResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteUserPermissionResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteUserPermissionResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteUserPermissionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeployPolicyInstanceRequest(TeaModel):
+    def __init__(self, cluster_id=None, cluster_ids=None, namespaces=None, policy_action=None, policy_name=None):
+        self.cluster_id = cluster_id  # type: str
+        self.cluster_ids = cluster_ids  # type: list[str]
+        self.namespaces = namespaces  # type: list[str]
+        self.policy_action = policy_action  # type: str
+        self.policy_name = policy_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeployPolicyInstanceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.cluster_ids is not None:
+            result['ClusterIds'] = self.cluster_ids
+        if self.namespaces is not None:
+            result['Namespaces'] = self.namespaces
+        if self.policy_action is not None:
+            result['PolicyAction'] = self.policy_action
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('ClusterIds') is not None:
+            self.cluster_ids = m.get('ClusterIds')
+        if m.get('Namespaces') is not None:
+            self.namespaces = m.get('Namespaces')
+        if m.get('PolicyAction') is not None:
+            self.policy_action = m.get('PolicyAction')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DeployPolicyInstanceShrinkRequest(TeaModel):
+    def __init__(self, cluster_id=None, cluster_ids_shrink=None, namespaces_shrink=None, policy_action=None,
+                 policy_name=None):
+        self.cluster_id = cluster_id  # type: str
+        self.cluster_ids_shrink = cluster_ids_shrink  # type: str
+        self.namespaces_shrink = namespaces_shrink  # type: str
+        self.policy_action = policy_action  # type: str
+        self.policy_name = policy_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeployPolicyInstanceShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.cluster_ids_shrink is not None:
+            result['ClusterIds'] = self.cluster_ids_shrink
+        if self.namespaces_shrink is not None:
+            result['Namespaces'] = self.namespaces_shrink
+        if self.policy_action is not None:
+            result['PolicyAction'] = self.policy_action
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('ClusterIds') is not None:
+            self.cluster_ids_shrink = m.get('ClusterIds')
+        if m.get('Namespaces') is not None:
+            self.namespaces_shrink = m.get('Namespaces')
+        if m.get('PolicyAction') is not None:
+            self.policy_action = m.get('PolicyAction')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DeployPolicyInstanceResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeployPolicyInstanceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeployPolicyInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeployPolicyInstanceResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeployPolicyInstanceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeployPolicyInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeHubClusterDetailsRequest(TeaModel):
     def __init__(self, cluster_id=None):
         # The ID of the master instance.
         self.cluster_id = cluster_id  # type: str
 
     def validate(self):
         pass
@@ -460,15 +856,18 @@
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterApiServer(TeaModel):
     def __init__(self, api_server_eip_id=None, enabled_public=None, load_balancer_id=None):
         # The ID of the elastic IP address (EIP).
         self.api_server_eip_id = api_server_eip_id  # type: str
-        # Indicates whether a public endpoint is used to expose the API server. Valid values: - true: a public endpoint is used to expose the API server. - false: no public endpoint is used to expose the API server.
+        # Indicates whether the API server is accessible over the Internet. Valid values:
+        # 
+        # *   true: The API server is accessible over the Internet.
+        # *   false: The API server is inaccessible over the Internet.
         self.enabled_public = enabled_public  # type: bool
         # The ID of the Server Load Balancer (SLB) instance.
         self.load_balancer_id = load_balancer_id  # type: str
 
     def validate(self):
         pass
 
@@ -498,31 +897,41 @@
 
 
 class DescribeHubClusterDetailsResponseBodyClusterClusterInfo(TeaModel):
     def __init__(self, cluster_id=None, cluster_spec=None, creation_time=None, error_message=None, name=None,
                  profile=None, region_id=None, state=None, update_time=None, version=None):
         # The ID of the master instance.
         self.cluster_id = cluster_id  # type: str
-        # The specification of the master instance. Valid values: - ack.pro.small: ACK Pro
+        # The specification of the master instance. Valid value:
+        # 
+        # *   ack.pro.small: ACK Pro cluster
         self.cluster_spec = cluster_spec  # type: str
         # The time when the master instance was created.
         self.creation_time = creation_time  # type: str
-        # The error message that is returned when the system fails to create the master instance.
+        # The error message returned when the master instance failed to be created.
         self.error_message = error_message  # type: str
         # The name of the master instance.
         self.name = name  # type: str
         # The configurations of the master instance.
         self.profile = profile  # type: str
         # The ID of the region in which the master instance resides.
         self.region_id = region_id  # type: str
-        # The status of the master instance. Valid values: - initial: The master instance is being initialized. - failed: The master instance failed to be created. - running: The master instance is running. - inactive: The master instance is inactive. - deleting: The master instance is being deleted. - delete_failed: The master instance failed to be deleted. - deleted: The master instance is deleted.
+        # The status of the master instance. Valid values:
+        # 
+        # *   initial: The master instance is being initialized.
+        # *   failed: The master instance failed to be created.
+        # *   running: The master instance is running
+        # *   inactive: The master instance is pending.
+        # *   deleting: The master instance is being deleted.
+        # *   delete_failed: The master instance failed to be deleted.
+        # *   deleted: The master instance is deleted.
         self.state = state  # type: str
         # The time when the master instance was updated.
         self.update_time = update_time  # type: str
-        # The Kubernetes version of the master instance.
+        # The version of the master instance.
         self.version = version  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClusterDetailsResponseBodyClusterClusterInfo, self).to_map()
@@ -575,22 +984,23 @@
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterConditions(TeaModel):
     def __init__(self, message=None, reason=None, status=None, type=None):
-        # The error message of the deletion condition.
+        # The error message returned.
         self.message = message  # type: str
         # The reason for the deletion condition.
         self.reason = reason  # type: str
-        # The status of the deletion condition. Valid values:
-        # - True: The master instance cannot be deleted.
-        # - False: The master instance can be deleted.
-        # - Unknow: Whether the master instance can be deleted is unknown.
+        # The status of the master instance that the deletion condition indicates. Valid values:
+        # 
+        # *   True: The master instance cannot be deleted.
+        # *   False: The master instance can be deleted.
+        # *   Unknow: Whether the master instance can be deleted is unknown.
         self.status = status  # type: str
         # The type of deletion condition.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
@@ -621,17 +1031,17 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterEndpoints(TeaModel):
     def __init__(self, intranet_api_server_endpoint=None, public_api_server_endpoint=None):
-        # The internal endpoint of the API server of the master instance.
+        # The endpoint that is used to access the API server over the internal network.
         self.intranet_api_server_endpoint = intranet_api_server_endpoint  # type: str
-        # The public endpoint of the API server of the master instance.
+        # The endpoint that is used to access the API server over the Internet.
         self.public_api_server_endpoint = public_api_server_endpoint  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClusterDetailsResponseBodyClusterEndpoints, self).to_map()
@@ -652,19 +1062,22 @@
         if m.get('PublicApiServerEndpoint') is not None:
             self.public_api_server_endpoint = m.get('PublicApiServerEndpoint')
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterLogConfig(TeaModel):
     def __init__(self, enable_log=None, log_project=None, log_store_ttl=None):
-        # Indicates whether audit logs are enabled. Valid values: - true: audit logs are enabled. - false: audit logs are disabled.
+        # Indicates whether the audit logging feature is enabled. Valid values:
+        # 
+        # *   true: Audit logging is enabled.
+        # *   false: Audit logging is disabled.
         self.enable_log = enable_log  # type: bool
-        # The name of the Log Service project.
+        # The name of the project of Log Service.
         self.log_project = log_project  # type: str
-        # The retention period of the logs.
+        # The number of days that logs are retained by Log Service.
         self.log_store_ttl = log_store_ttl  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClusterDetailsResponseBodyClusterLogConfig, self).to_map()
@@ -689,17 +1102,20 @@
         if m.get('LogStoreTTL') is not None:
             self.log_store_ttl = m.get('LogStoreTTL')
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterMeshConfig(TeaModel):
     def __init__(self, enable_mesh=None, mesh_id=None):
-        # Indicates whether ASM is enabled. Valid values: - true: ASM is enabled. - false: ASM is disabled.
+        # Indicates whether ASM is enabled. Valid values:
+        # 
+        # *   true: ASM is enabled.
+        # *   false: ASM is disabled.
         self.enable_mesh = enable_mesh  # type: bool
-        # The ID of the ASM instance.
+        # service mesh (ASM) instance ID
         self.mesh_id = mesh_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClusterDetailsResponseBodyClusterMeshConfig, self).to_map()
@@ -722,19 +1138,23 @@
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterNetwork(TeaModel):
     def __init__(self, cluster_domain=None, ipstack=None, security_group_ids=None, v_switches=None, vpc_id=None):
         # The domain name of the master instance.
         self.cluster_domain = cluster_domain  # type: str
-        # The IP version that is supported by the master instance. Valid values: - ipv4: IPv4. - ipv6: IPv6. - dual: IPv4 and IPv6.
+        # The IP version that is supported by the master instance. Valid values:
+        # 
+        # *   ipv4: IPv4.
+        # *   ipv6: IPv6.
+        # *   dual: IPv4 and IPv6.
         self.ipstack = ipstack  # type: str
-        # The ID of the associated security group.
+        # The IDs of the associated security groups.
         self.security_group_ids = security_group_ids  # type: list[str]
-        # A list of the vSwitches that are used by the master instance.
+        # The details of the vSwitches.
         self.v_switches = v_switches  # type: list[str]
         # The ID of the virtual private cloud (VPC) in which the master instance resides.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         pass
 
@@ -889,25 +1309,25 @@
                 self.workflow_units.append(temp_model.from_map(k))
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyCluster(TeaModel):
     def __init__(self, api_server=None, cluster_info=None, conditions=None, endpoints=None, log_config=None,
                  mesh_config=None, network=None, workflow_config=None):
-        # Information about the API server of the master instance.
+        # The details of the API server of the master instance.
         self.api_server = api_server  # type: DescribeHubClusterDetailsResponseBodyClusterApiServer
-        # The details about the master instance.
+        # The details of the master instance.
         self.cluster_info = cluster_info  # type: DescribeHubClusterDetailsResponseBodyClusterClusterInfo
-        # The list of the deletion conditions of the master instance.
+        # The deletion conditions of the master instance.
         self.conditions = conditions  # type: list[DescribeHubClusterDetailsResponseBodyClusterConditions]
         # The endpoint of the master instance.
         self.endpoints = endpoints  # type: DescribeHubClusterDetailsResponseBodyClusterEndpoints
         # The logging configuration.
         self.log_config = log_config  # type: DescribeHubClusterDetailsResponseBodyClusterLogConfig
-        # The Service Mesh (ASM) configurations.
+        # The configurations of Alibaba Cloud Service Mesh (ASM).
         self.mesh_config = mesh_config  # type: DescribeHubClusterDetailsResponseBodyClusterMeshConfig
         # The network configurations of the master instance.
         self.network = network  # type: DescribeHubClusterDetailsResponseBodyClusterNetwork
         self.workflow_config = workflow_config  # type: DescribeHubClusterDetailsResponseBodyClusterWorkflowConfig
 
     def validate(self):
         if self.api_server:
@@ -984,15 +1404,15 @@
             temp_model = DescribeHubClusterDetailsResponseBodyClusterWorkflowConfig()
             self.workflow_config = temp_model.from_map(m['WorkflowConfig'])
         return self
 
 
 class DescribeHubClusterDetailsResponseBody(TeaModel):
     def __init__(self, cluster=None, request_id=None):
-        # The details about the master instance.
+        # The details of the master instance.
         self.cluster = cluster  # type: DescribeHubClusterDetailsResponseBodyCluster
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.cluster:
             self.cluster.validate()
@@ -1058,15 +1478,20 @@
         return self
 
 
 class DescribeHubClusterKubeconfigRequest(TeaModel):
     def __init__(self, cluster_id=None, private_ip_address=None):
         # The ID of the master instance.
         self.cluster_id = cluster_id  # type: str
-        # Specifies whether to obtain the credential that is used to connect to the master instance over the internal network. Valid values: - `true`: obtains only the credential that is used to access the master instance over the internal network. - `false`: obtains only the credential that is used to access the master instance over the Internet. Default value: `false`.
+        # Specifies whether to obtain the kubeconfig file that is used to connect to the cluster over the internal network. Valid values:
+        # 
+        # *   `true`: obtains the kubeconfig file that is used to connect to the master instance over the internal network.
+        # *   `false`: obtains the kubeconfig file that is used to connect to the master instance over the Internet.
+        # 
+        # Default value: `false`
         self.private_ip_address = private_ip_address  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClusterKubeconfigRequest, self).to_map()
@@ -1087,15 +1512,15 @@
         if m.get('PrivateIpAddress') is not None:
             self.private_ip_address = m.get('PrivateIpAddress')
         return self
 
 
 class DescribeHubClusterKubeconfigResponseBody(TeaModel):
     def __init__(self, kubeconfig=None, request_id=None):
-        # The content of the kubeconfig file of the master instance.
+        # The content of the kubeconfig file.
         self.kubeconfig = kubeconfig  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -2131,14 +2556,1287 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeManagedClustersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePoliciesResponseBodyPolicies(TeaModel):
+    def __init__(self, category=None, names=None):
+        self.category = category  # type: str
+        self.names = names  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePoliciesResponseBodyPolicies, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.category is not None:
+            result['Category'] = self.category
+        if self.names is not None:
+            result['Names'] = self.names
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('Names') is not None:
+            self.names = m.get('Names')
+        return self
+
+
+class DescribePoliciesResponseBody(TeaModel):
+    def __init__(self, policies=None, request_id=None):
+        self.policies = policies  # type: list[DescribePoliciesResponseBodyPolicies]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.policies:
+            for k in self.policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePoliciesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Policies'] = []
+        if self.policies is not None:
+            for k in self.policies:
+                result['Policies'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.policies = []
+        if m.get('Policies') is not None:
+            for k in m.get('Policies'):
+                temp_model = DescribePoliciesResponseBodyPolicies()
+                self.policies.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePoliciesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePoliciesResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePoliciesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribePoliciesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribePolicyDetailsRequest(TeaModel):
+    def __init__(self, policy_name=None):
+        self.policy_name = policy_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyDetailsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DescribePolicyDetailsResponseBodyPolicy(TeaModel):
+    def __init__(self, action=None, category=None, created=None, description=None, name=None, no_config=None,
+                 severity=None, template=None, updated=None):
+        self.action = action  # type: str
+        self.category = category  # type: str
+        self.created = created  # type: str
+        self.description = description  # type: str
+        self.name = name  # type: str
+        self.no_config = no_config  # type: int
+        self.severity = severity  # type: str
+        self.template = template  # type: str
+        self.updated = updated  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyDetailsResponseBodyPolicy, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action is not None:
+            result['Action'] = self.action
+        if self.category is not None:
+            result['Category'] = self.category
+        if self.created is not None:
+            result['Created'] = self.created
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.no_config is not None:
+            result['NoConfig'] = self.no_config
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.template is not None:
+            result['Template'] = self.template
+        if self.updated is not None:
+            result['Updated'] = self.updated
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Action') is not None:
+            self.action = m.get('Action')
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('Created') is not None:
+            self.created = m.get('Created')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('NoConfig') is not None:
+            self.no_config = m.get('NoConfig')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Template') is not None:
+            self.template = m.get('Template')
+        if m.get('Updated') is not None:
+            self.updated = m.get('Updated')
+        return self
+
+
+class DescribePolicyDetailsResponseBody(TeaModel):
+    def __init__(self, policy=None, request_id=None):
+        self.policy = policy  # type: DescribePolicyDetailsResponseBodyPolicy
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.policy:
+            self.policy.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyDetailsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy is not None:
+            result['Policy'] = self.policy.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Policy') is not None:
+            temp_model = DescribePolicyDetailsResponseBodyPolicy()
+            self.policy = temp_model.from_map(m['Policy'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePolicyDetailsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePolicyDetailsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyDetailsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribePolicyDetailsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribePolicyGovernanceInClusterRequest(TeaModel):
+    def __init__(self, cluster_id=None):
+        self.cluster_id = cluster_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesCluster(TeaModel):
+    def __init__(self, cluster_id=None, cluster_spec=None, cluster_type=None, name=None, profile=None,
+                 region_id=None, state=None):
+        self.cluster_id = cluster_id  # type: str
+        self.cluster_spec = cluster_spec  # type: str
+        self.cluster_type = cluster_type  # type: str
+        self.name = name  # type: str
+        self.profile = profile  # type: str
+        self.region_id = region_id  # type: str
+        self.state = state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesCluster, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.cluster_spec is not None:
+            result['ClusterSpec'] = self.cluster_spec
+        if self.cluster_type is not None:
+            result['ClusterType'] = self.cluster_type
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.profile is not None:
+            result['Profile'] = self.profile
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.state is not None:
+            result['State'] = self.state
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('ClusterSpec') is not None:
+            self.cluster_spec = m.get('ClusterSpec')
+        if m.get('ClusterType') is not None:
+            self.cluster_type = m.get('ClusterType')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Profile') is not None:
+            self.profile = m.get('Profile')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('State') is not None:
+            self.state = m.get('State')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceAdmitLog(TeaModel):
+    def __init__(self, count=None, log_project=None, log_store=None, logs=None, progress=None):
+        self.count = count  # type: str
+        self.log_project = log_project  # type: str
+        self.log_store = log_store  # type: str
+        self.logs = logs  # type: list[dict[str, str]]
+        self.progress = progress  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceAdmitLog, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.count is not None:
+            result['Count'] = self.count
+        if self.log_project is not None:
+            result['LogProject'] = self.log_project
+        if self.log_store is not None:
+            result['LogStore'] = self.log_store
+        if self.logs is not None:
+            result['Logs'] = self.logs
+        if self.progress is not None:
+            result['Progress'] = self.progress
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Count') is not None:
+            self.count = m.get('Count')
+        if m.get('LogProject') is not None:
+            self.log_project = m.get('LogProject')
+        if m.get('LogStore') is not None:
+            self.log_store = m.get('LogStore')
+        if m.get('Logs') is not None:
+            self.logs = m.get('Logs')
+        if m.get('Progress') is not None:
+            self.progress = m.get('Progress')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceOnState(TeaModel):
+    def __init__(self, enabled_count=None, severity=None, total_count=None):
+        self.enabled_count = enabled_count  # type: long
+        self.severity = severity  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceOnState, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enabled_count is not None:
+            result['EnabledCount'] = self.enabled_count
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EnabledCount') is not None:
+            self.enabled_count = m.get('EnabledCount')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsDeny(TeaModel):
+    def __init__(self, severity=None, violations=None):
+        self.severity = severity  # type: str
+        self.violations = violations  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsDeny, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.violations is not None:
+            result['Violations'] = self.violations
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Violations') is not None:
+            self.violations = m.get('Violations')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsWarn(TeaModel):
+    def __init__(self, severity=None, violations=None):
+        self.severity = severity  # type: str
+        self.violations = violations  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsWarn, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.violations is not None:
+            result['Violations'] = self.violations
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Violations') is not None:
+            self.violations = m.get('Violations')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolations(TeaModel):
+    def __init__(self, deny=None, warn=None):
+        self.deny = deny  # type: list[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsDeny]
+        self.warn = warn  # type: list[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsWarn]
+
+    def validate(self):
+        if self.deny:
+            for k in self.deny:
+                if k:
+                    k.validate()
+        if self.warn:
+            for k in self.warn:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolations, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Deny'] = []
+        if self.deny is not None:
+            for k in self.deny:
+                result['Deny'].append(k.to_map() if k else None)
+        result['Warn'] = []
+        if self.warn is not None:
+            for k in self.warn:
+                result['Warn'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.deny = []
+        if m.get('Deny') is not None:
+            for k in m.get('Deny'):
+                temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsDeny()
+                self.deny.append(temp_model.from_map(k))
+        self.warn = []
+        if m.get('Warn') is not None:
+            for k in m.get('Warn'):
+                temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsWarn()
+                self.warn.append(temp_model.from_map(k))
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsDeny(TeaModel):
+    def __init__(self, policy_description=None, policy_name=None, severity=None, violations=None):
+        self.policy_description = policy_description  # type: str
+        self.policy_name = policy_name  # type: str
+        self.severity = severity  # type: str
+        self.violations = violations  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsDeny, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy_description is not None:
+            result['PolicyDescription'] = self.policy_description
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.violations is not None:
+            result['Violations'] = self.violations
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PolicyDescription') is not None:
+            self.policy_description = m.get('PolicyDescription')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Violations') is not None:
+            self.violations = m.get('Violations')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsWarn(TeaModel):
+    def __init__(self, policy_description=None, policy_name=None, severity=None, violations=None):
+        self.policy_description = policy_description  # type: str
+        self.policy_name = policy_name  # type: str
+        self.severity = severity  # type: str
+        self.violations = violations  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsWarn, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy_description is not None:
+            result['PolicyDescription'] = self.policy_description
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.violations is not None:
+            result['Violations'] = self.violations
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PolicyDescription') is not None:
+            self.policy_description = m.get('PolicyDescription')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Violations') is not None:
+            self.violations = m.get('Violations')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolations(TeaModel):
+    def __init__(self, deny=None, warn=None):
+        self.deny = deny  # type: list[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsDeny]
+        self.warn = warn  # type: list[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsWarn]
+
+    def validate(self):
+        if self.deny:
+            for k in self.deny:
+                if k:
+                    k.validate()
+        if self.warn:
+            for k in self.warn:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolations, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Deny'] = []
+        if self.deny is not None:
+            for k in self.deny:
+                result['Deny'].append(k.to_map() if k else None)
+        result['Warn'] = []
+        if self.warn is not None:
+            for k in self.warn:
+                result['Warn'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.deny = []
+        if m.get('Deny') is not None:
+            for k in m.get('Deny'):
+                temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsDeny()
+                self.deny.append(temp_model.from_map(k))
+        self.warn = []
+        if m.get('Warn') is not None:
+            for k in m.get('Warn'):
+                temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsWarn()
+                self.warn.append(temp_model.from_map(k))
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolation(TeaModel):
+    def __init__(self, total_violations=None, violations=None):
+        self.total_violations = total_violations  # type: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolations
+        self.violations = violations  # type: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolations
+
+    def validate(self):
+        if self.total_violations:
+            self.total_violations.validate()
+        if self.violations:
+            self.violations.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolation, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.total_violations is not None:
+            result['TotalViolations'] = self.total_violations.to_map()
+        if self.violations is not None:
+            result['Violations'] = self.violations.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TotalViolations') is not None:
+            temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolations()
+            self.total_violations = temp_model.from_map(m['TotalViolations'])
+        if m.get('Violations') is not None:
+            temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolations()
+            self.violations = temp_model.from_map(m['Violations'])
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernance(TeaModel):
+    def __init__(self, admit_log=None, on_state=None, violation=None):
+        self.admit_log = admit_log  # type: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceAdmitLog
+        self.on_state = on_state  # type: list[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceOnState]
+        self.violation = violation  # type: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolation
+
+    def validate(self):
+        if self.admit_log:
+            self.admit_log.validate()
+        if self.on_state:
+            for k in self.on_state:
+                if k:
+                    k.validate()
+        if self.violation:
+            self.violation.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernance, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.admit_log is not None:
+            result['AdmitLog'] = self.admit_log.to_map()
+        result['OnState'] = []
+        if self.on_state is not None:
+            for k in self.on_state:
+                result['OnState'].append(k.to_map() if k else None)
+        if self.violation is not None:
+            result['Violation'] = self.violation.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AdmitLog') is not None:
+            temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceAdmitLog()
+            self.admit_log = temp_model.from_map(m['AdmitLog'])
+        self.on_state = []
+        if m.get('OnState') is not None:
+            for k in m.get('OnState'):
+                temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceOnState()
+                self.on_state.append(temp_model.from_map(k))
+        if m.get('Violation') is not None:
+            temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolation()
+            self.violation = temp_model.from_map(m['Violation'])
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernances(TeaModel):
+    def __init__(self, cluster=None, policy_governance=None):
+        self.cluster = cluster  # type: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesCluster
+        self.policy_governance = policy_governance  # type: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernance
+
+    def validate(self):
+        if self.cluster:
+            self.cluster.validate()
+        if self.policy_governance:
+            self.policy_governance.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBodyPolicyGovernances, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster is not None:
+            result['Cluster'] = self.cluster.to_map()
+        if self.policy_governance is not None:
+            result['PolicyGovernance'] = self.policy_governance.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Cluster') is not None:
+            temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesCluster()
+            self.cluster = temp_model.from_map(m['Cluster'])
+        if m.get('PolicyGovernance') is not None:
+            temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernance()
+            self.policy_governance = temp_model.from_map(m['PolicyGovernance'])
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBody(TeaModel):
+    def __init__(self, policy_governances=None, request_id=None):
+        self.policy_governances = policy_governances  # type: list[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernances]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.policy_governances:
+            for k in self.policy_governances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['PolicyGovernances'] = []
+        if self.policy_governances is not None:
+            for k in self.policy_governances:
+                result['PolicyGovernances'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.policy_governances = []
+        if m.get('PolicyGovernances') is not None:
+            for k in m.get('PolicyGovernances'):
+                temp_model = DescribePolicyGovernanceInClusterResponseBodyPolicyGovernances()
+                self.policy_governances.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePolicyGovernanceInClusterResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyGovernanceInClusterResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribePolicyGovernanceInClusterResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribePolicyInstancesRequest(TeaModel):
+    def __init__(self, cluster_id=None, policy_name=None):
+        self.cluster_id = cluster_id  # type: str
+        self.policy_name = policy_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DescribePolicyInstancesResponseBodyPolicies(TeaModel):
+    def __init__(self, cluster_id=None, instance_name=None, policy_action=None, policy_category=None,
+                 policy_description=None, policy_name=None, policy_parameters=None, policy_scope=None, policy_severity=None,
+                 total_violations=None):
+        self.cluster_id = cluster_id  # type: str
+        self.instance_name = instance_name  # type: str
+        self.policy_action = policy_action  # type: str
+        self.policy_category = policy_category  # type: str
+        self.policy_description = policy_description  # type: str
+        self.policy_name = policy_name  # type: str
+        self.policy_parameters = policy_parameters  # type: dict[str, str]
+        self.policy_scope = policy_scope  # type: str
+        self.policy_severity = policy_severity  # type: str
+        self.total_violations = total_violations  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesResponseBodyPolicies, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.policy_action is not None:
+            result['PolicyAction'] = self.policy_action
+        if self.policy_category is not None:
+            result['PolicyCategory'] = self.policy_category
+        if self.policy_description is not None:
+            result['PolicyDescription'] = self.policy_description
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.policy_parameters is not None:
+            result['PolicyParameters'] = self.policy_parameters
+        if self.policy_scope is not None:
+            result['PolicyScope'] = self.policy_scope
+        if self.policy_severity is not None:
+            result['PolicySeverity'] = self.policy_severity
+        if self.total_violations is not None:
+            result['TotalViolations'] = self.total_violations
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('PolicyAction') is not None:
+            self.policy_action = m.get('PolicyAction')
+        if m.get('PolicyCategory') is not None:
+            self.policy_category = m.get('PolicyCategory')
+        if m.get('PolicyDescription') is not None:
+            self.policy_description = m.get('PolicyDescription')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('PolicyParameters') is not None:
+            self.policy_parameters = m.get('PolicyParameters')
+        if m.get('PolicyScope') is not None:
+            self.policy_scope = m.get('PolicyScope')
+        if m.get('PolicySeverity') is not None:
+            self.policy_severity = m.get('PolicySeverity')
+        if m.get('TotalViolations') is not None:
+            self.total_violations = m.get('TotalViolations')
+        return self
+
+
+class DescribePolicyInstancesResponseBody(TeaModel):
+    def __init__(self, policies=None, request_id=None):
+        self.policies = policies  # type: list[DescribePolicyInstancesResponseBodyPolicies]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.policies:
+            for k in self.policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Policies'] = []
+        if self.policies is not None:
+            for k in self.policies:
+                result['Policies'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.policies = []
+        if m.get('Policies') is not None:
+            for k in m.get('Policies'):
+                temp_model = DescribePolicyInstancesResponseBodyPolicies()
+                self.policies.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePolicyInstancesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePolicyInstancesResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribePolicyInstancesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribePolicyInstancesStatusRequest(TeaModel):
+    def __init__(self, cluster_id=None):
+        self.cluster_id = cluster_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesStatusRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstancesPolicyClusters(TeaModel):
+    def __init__(self, cluster_id=None, status=None):
+        self.cluster_id = cluster_id  # type: str
+        self.status = status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstancesPolicyClusters, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstances(TeaModel):
+    def __init__(self, policy_category=None, policy_clusters=None, policy_description=None,
+                 policy_instances_count=None, policy_name=None, policy_severity=None):
+        self.policy_category = policy_category  # type: str
+        self.policy_clusters = policy_clusters  # type: list[DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstancesPolicyClusters]
+        self.policy_description = policy_description  # type: str
+        self.policy_instances_count = policy_instances_count  # type: long
+        self.policy_name = policy_name  # type: str
+        self.policy_severity = policy_severity  # type: str
+
+    def validate(self):
+        if self.policy_clusters:
+            for k in self.policy_clusters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstances, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy_category is not None:
+            result['PolicyCategory'] = self.policy_category
+        result['PolicyClusters'] = []
+        if self.policy_clusters is not None:
+            for k in self.policy_clusters:
+                result['PolicyClusters'].append(k.to_map() if k else None)
+        if self.policy_description is not None:
+            result['PolicyDescription'] = self.policy_description
+        if self.policy_instances_count is not None:
+            result['PolicyInstancesCount'] = self.policy_instances_count
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.policy_severity is not None:
+            result['PolicySeverity'] = self.policy_severity
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PolicyCategory') is not None:
+            self.policy_category = m.get('PolicyCategory')
+        self.policy_clusters = []
+        if m.get('PolicyClusters') is not None:
+            for k in m.get('PolicyClusters'):
+                temp_model = DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstancesPolicyClusters()
+                self.policy_clusters.append(temp_model.from_map(k))
+        if m.get('PolicyDescription') is not None:
+            self.policy_description = m.get('PolicyDescription')
+        if m.get('PolicyInstancesCount') is not None:
+            self.policy_instances_count = m.get('PolicyInstancesCount')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('PolicySeverity') is not None:
+            self.policy_severity = m.get('PolicySeverity')
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBodyPoliciesSeverityInfo(TeaModel):
+    def __init__(self, severity_count=None, severity_type=None):
+        self.severity_count = severity_count  # type: str
+        self.severity_type = severity_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesStatusResponseBodyPoliciesSeverityInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.severity_count is not None:
+            result['SeverityCount'] = self.severity_count
+        if self.severity_type is not None:
+            result['SeverityType'] = self.severity_type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('SeverityCount') is not None:
+            self.severity_count = m.get('SeverityCount')
+        if m.get('SeverityType') is not None:
+            self.severity_type = m.get('SeverityType')
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBodyPolicies(TeaModel):
+    def __init__(self, policy_instances=None, severity_info=None):
+        self.policy_instances = policy_instances  # type: list[DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstances]
+        self.severity_info = severity_info  # type: list[DescribePolicyInstancesStatusResponseBodyPoliciesSeverityInfo]
+
+    def validate(self):
+        if self.policy_instances:
+            for k in self.policy_instances:
+                if k:
+                    k.validate()
+        if self.severity_info:
+            for k in self.severity_info:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesStatusResponseBodyPolicies, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['PolicyInstances'] = []
+        if self.policy_instances is not None:
+            for k in self.policy_instances:
+                result['PolicyInstances'].append(k.to_map() if k else None)
+        result['SeverityInfo'] = []
+        if self.severity_info is not None:
+            for k in self.severity_info:
+                result['SeverityInfo'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.policy_instances = []
+        if m.get('PolicyInstances') is not None:
+            for k in m.get('PolicyInstances'):
+                temp_model = DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstances()
+                self.policy_instances.append(temp_model.from_map(k))
+        self.severity_info = []
+        if m.get('SeverityInfo') is not None:
+            for k in m.get('SeverityInfo'):
+                temp_model = DescribePolicyInstancesStatusResponseBodyPoliciesSeverityInfo()
+                self.severity_info.append(temp_model.from_map(k))
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBody(TeaModel):
+    def __init__(self, policies=None, request_id=None):
+        self.policies = policies  # type: DescribePolicyInstancesStatusResponseBodyPolicies
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.policies:
+            self.policies.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesStatusResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policies is not None:
+            result['Policies'] = self.policies.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Policies') is not None:
+            temp_model = DescribePolicyInstancesStatusResponseBodyPolicies()
+            self.policies = temp_model.from_map(m['Policies'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePolicyInstancesStatusResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePolicyInstancesStatusResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePolicyInstancesStatusResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribePolicyInstancesStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeRegionsRequest(TeaModel):
     def __init__(self, language=None):
         # The language. Valid values: zh, en, and jp.
         self.language = language  # type: str
 
     def validate(self):
         pass
@@ -2267,14 +3965,15 @@
             temp_model = DescribeRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserPermissionsRequest(TeaModel):
     def __init__(self, user_id=None):
+        # The ID of the RAM user that you want to query.
         self.user_id = user_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserPermissionsRequest, self).to_map()
@@ -2291,17 +3990,31 @@
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         return self
 
 
 class DescribeUserPermissionsResponseBodyPermissions(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, role_name=None, role_type=None):
+        # The authorization setting. Valid values:
+        # 
+        # *   {cluster_id} is returned if the permissions are scoped to a cluster.
+        # *   {cluster_id}/{namespace} is returned if the permissions are scoped to a namespace of a cluster.
+        # *   all-clusters is returned if the permissions are scoped to all clusters.
         self.resource_id = resource_id  # type: str
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: indicates that the permissions are scoped to a cluster.
+        # *   namespace: indicates that the permissions are scoped to a namespace of a cluster.
         self.resource_type = resource_type  # type: str
+        # The name of the custom role. If a custom role is assigned, the value is the name of the assigned custom role.
         self.role_name = role_name  # type: str
+        # The type of predefined role. Valid values:
+        # 
+        # *   admin: administrator
+        # *   dev: developer
         self.role_type = role_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserPermissionsResponseBodyPermissions, self).to_map()
@@ -2330,15 +4043,17 @@
         if m.get('RoleType') is not None:
             self.role_type = m.get('RoleType')
         return self
 
 
 class DescribeUserPermissionsResponseBody(TeaModel):
     def __init__(self, permissions=None, request_id=None):
+        # The details about the permissions of the RAM user.
         self.permissions = permissions  # type: list[DescribeUserPermissionsResponseBodyPermissions]
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -2523,14 +4238,133 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DetachClusterFromHubResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GrantUserPermissionRequest(TeaModel):
+    def __init__(self, cluster_id=None, namespace=None, role_name=None, role_type=None, user_id=None):
+        # The ID of the master instance.
+        self.cluster_id = cluster_id  # type: str
+        # The namespace to which the permissions are scoped. By default, this parameter is empty when you set role_type to cluster.
+        self.namespace = namespace  # type: str
+        # Specifies the predefined role that you want to assign. Valid values:
+        # 
+        # *   admin: the administrator role.
+        # *   dev: the developer role.
+        self.role_name = role_name  # type: str
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: specifies that the permissions are scoped to a master instance.
+        # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
+        self.role_type = role_type  # type: str
+        # The ID of the RAM user.
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GrantUserPermissionRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        if self.role_name is not None:
+            result['RoleName'] = self.role_name
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('RoleName') is not None:
+            self.role_name = m.get('RoleName')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class GrantUserPermissionResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GrantUserPermissionResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GrantUserPermissionResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GrantUserPermissionResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GrantUserPermissionResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GrantUserPermissionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GrantUserPermissionsRequestPermissions(TeaModel):
     def __init__(self, cluster_id=None, namespace=None, role_name=None, role_type=None):
         self.cluster_id = cluster_id  # type: str
         self.namespace = namespace  # type: str
         self.role_name = role_name  # type: str
         self.role_type = role_type  # type: str
 
@@ -2699,26 +4533,38 @@
     def __init__(self, api_server_eip_id=None, argo_cdenabled=None, argo_server_enabled=None,
                  audit_log_enabled=None, cluster_id=None, deletion_protection=None, enable_mesh=None, name=None, price_limit=None,
                  public_api_server_enabled=None, v_switches=None, workflow_schedule_mode=None):
         # The ID of the EIP.
         self.api_server_eip_id = api_server_eip_id  # type: str
         self.argo_cdenabled = argo_cdenabled  # type: bool
         self.argo_server_enabled = argo_server_enabled  # type: bool
-        # Specifies whether to enable audit logs. Valid values: - true: enable audit logs. - false: disables audit logs.
+        # Specifies whether to enable the audit logging feature. Valid values:
+        # 
+        # *   true: enables the audit logging feature.
+        # *   false: disables the audit logging feature.
         self.audit_log_enabled = audit_log_enabled  # type: bool
-        # The ID of the master instance.
+        # The ID of the cluster.
         self.cluster_id = cluster_id  # type: str
-        # Specifies whether to enable deletion protection for the master instance. After you enable deletion protection, you cannot delete the master instance in the console or by calling API operations. Valid values:
+        # Specifies whether to enable deletion protection for the cluster. After you enable deletion protection, you cannot delete the master instance in the console or by calling the DeleteHubCluster operation. Valid values:
+        # 
+        # *   true: enables deletion protection for the cluster.
+        # *   false: disables deletion protection for the cluster. This is the default value.
         self.deletion_protection = deletion_protection  # type: bool
-        # Specifies whether to enable Service Mesh (ASM). Valid values: true: enables ASM. false: disables ASM.
+        # Specifies whether to enable Alibaba Cloud Service Mesh (ASM). Valid values:
+        # 
+        # true: enables ASM. false: disables ASM.
         self.enable_mesh = enable_mesh  # type: bool
-        # The name of the master instance. The name must be 1 to 63 characters in length, and can contain letters and digits. The name must start with a letter. The name can contain letters, digits, underscores (_), and hyphens (-).
+        # The name of the cluster. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name  # type: str
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit  # type: str
-        # Specifies whether to associate an elastic IP address (EIP) with the API server. Default value: false. To associate an EIP with the API server, set the value to true. You can use a custom EIP by setting the ApiServerEipId parameter. If you do not set the ApiServerEipId parameter, the system automatically creates an EIP.
+        # Specifies whether to associate an elastic IP address (EIP) with the API server. Valid values:
+        # 
+        # *   true: associates an EIP with the API server. You can specify the ApiServerEipId parameter. If you do not specify the ApiServerEipId parameter, the system automatically creates an EIP.
+        # *   false: disassociates an EIP from the API server.
         self.public_api_server_enabled = public_api_server_enabled  # type: bool
         self.v_switches = v_switches  # type: list[str]
         self.workflow_schedule_mode = workflow_schedule_mode  # type: str
 
     def validate(self):
         pass
 
@@ -2787,26 +4633,38 @@
     def __init__(self, api_server_eip_id=None, argo_cdenabled=None, argo_server_enabled=None,
                  audit_log_enabled=None, cluster_id=None, deletion_protection=None, enable_mesh=None, name=None, price_limit=None,
                  public_api_server_enabled=None, v_switches_shrink=None, workflow_schedule_mode=None):
         # The ID of the EIP.
         self.api_server_eip_id = api_server_eip_id  # type: str
         self.argo_cdenabled = argo_cdenabled  # type: bool
         self.argo_server_enabled = argo_server_enabled  # type: bool
-        # Specifies whether to enable audit logs. Valid values: - true: enable audit logs. - false: disables audit logs.
+        # Specifies whether to enable the audit logging feature. Valid values:
+        # 
+        # *   true: enables the audit logging feature.
+        # *   false: disables the audit logging feature.
         self.audit_log_enabled = audit_log_enabled  # type: bool
-        # The ID of the master instance.
+        # The ID of the cluster.
         self.cluster_id = cluster_id  # type: str
-        # Specifies whether to enable deletion protection for the master instance. After you enable deletion protection, you cannot delete the master instance in the console or by calling API operations. Valid values:
+        # Specifies whether to enable deletion protection for the cluster. After you enable deletion protection, you cannot delete the master instance in the console or by calling the DeleteHubCluster operation. Valid values:
+        # 
+        # *   true: enables deletion protection for the cluster.
+        # *   false: disables deletion protection for the cluster. This is the default value.
         self.deletion_protection = deletion_protection  # type: bool
-        # Specifies whether to enable Service Mesh (ASM). Valid values: true: enables ASM. false: disables ASM.
+        # Specifies whether to enable Alibaba Cloud Service Mesh (ASM). Valid values:
+        # 
+        # true: enables ASM. false: disables ASM.
         self.enable_mesh = enable_mesh  # type: bool
-        # The name of the master instance. The name must be 1 to 63 characters in length, and can contain letters and digits. The name must start with a letter. The name can contain letters, digits, underscores (_), and hyphens (-).
+        # The name of the cluster. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name  # type: str
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit  # type: str
-        # Specifies whether to associate an elastic IP address (EIP) with the API server. Default value: false. To associate an EIP with the API server, set the value to true. You can use a custom EIP by setting the ApiServerEipId parameter. If you do not set the ApiServerEipId parameter, the system automatically creates an EIP.
+        # Specifies whether to associate an elastic IP address (EIP) with the API server. Valid values:
+        # 
+        # *   true: associates an EIP with the API server. You can specify the ApiServerEipId parameter. If you do not specify the ApiServerEipId parameter, the system automatically creates an EIP.
+        # *   false: disassociates an EIP from the API server.
         self.public_api_server_enabled = public_api_server_enabled  # type: bool
         self.v_switches_shrink = v_switches_shrink  # type: str
         self.workflow_schedule_mode = workflow_schedule_mode  # type: str
 
     def validate(self):
         pass
 
@@ -2931,7 +4789,126 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateHubClusterFeatureResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateUserPermissionRequest(TeaModel):
+    def __init__(self, cluster_id=None, namespace=None, role_name=None, role_type=None, user_id=None):
+        # The ID of the master instance.
+        self.cluster_id = cluster_id  # type: str
+        # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
+        self.namespace = namespace  # type: str
+        # Specifies the predefined role that you want to assign. Valid values:
+        # 
+        # *   admin: the administrator role.
+        # *   dev: the developer role.
+        self.role_name = role_name  # type: str
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: specifies that the permissions are scoped to a master instance.
+        # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
+        self.role_type = role_type  # type: str
+        # The ID of the RAM user.
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateUserPermissionRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        if self.role_name is not None:
+            result['RoleName'] = self.role_name
+        if self.role_type is not None:
+            result['RoleType'] = self.role_type
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('RoleName') is not None:
+            self.role_name = m.get('RoleName')
+        if m.get('RoleType') is not None:
+            self.role_type = m.get('RoleType')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class UpdateUserPermissionResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateUserPermissionResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateUserPermissionResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateUserPermissionResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateUserPermissionResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateUserPermissionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO` & `alibabacloud_adcp20220101_py2-1.0.9/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-adcp20220101-py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101_py2-1.0.8/setup.py` & `alibabacloud_adcp20220101_py2-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adcp20220101_py2.
 
-Created on 16/03/2023
+Created on 27/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adcp20220101"
 NAME = "alibabacloud_adcp20220101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adcp (20220101) SDK Library for Python2"
```

