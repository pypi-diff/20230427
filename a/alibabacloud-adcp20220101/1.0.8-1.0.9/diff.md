# Comparing `tmp/alibabacloud_adcp20220101-1.0.8.tar.gz` & `tmp/alibabacloud_adcp20220101-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adcp20220101-1.0.8.tar", last modified: Thu Mar 16 01:42:41 2023, max compression
+gzip compressed data, was "dist/alibabacloud_adcp20220101-1.0.9.tar", last modified: Thu Apr 27 03:10:37 2023, max compression
```

## Comparing `alibabacloud_adcp20220101-1.0.8.tar` & `alibabacloud_adcp20220101-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      665 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46522 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101/client.py
--rw-r--r--   0 root         (0) root         (0)   115400 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2615 2023-03-16 01:42:40.000000 alibabacloud_adcp20220101-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      736 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77604 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)   186682 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-27 03:10:37.000000 alibabacloud_adcp20220101-1.0.9/setup.py
```

### Comparing `alibabacloud_adcp20220101-1.0.8/ChangeLog.md` & `alibabacloud_adcp20220101-1.0.9/ChangeLog.md`

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

### Comparing `alibabacloud_adcp20220101-1.0.8/LICENSE` & `alibabacloud_adcp20220101-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101-1.0.8/PKG-INFO` & `alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_adcp20220101
-Version: 1.0.8
+Name: alibabacloud-adcp20220101
+Version: 1.0.9
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101-1.0.8/README-CN.md` & `alibabacloud_adcp20220101-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101-1.0.8/README.md` & `alibabacloud_adcp20220101-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101/client.py` & `alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -341,14 +341,272 @@
     async def delete_hub_cluster_async(
         self,
         request: adcp_20220101_models.DeleteHubClusterRequest,
     ) -> adcp_20220101_models.DeleteHubClusterResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_hub_cluster_with_options_async(request, runtime)
 
+    def delete_policy_instance_with_options(
+        self,
+        tmp_req: adcp_20220101_models.DeletePolicyInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DeletePolicyInstanceResponse:
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
+    async def delete_policy_instance_with_options_async(
+        self,
+        tmp_req: adcp_20220101_models.DeletePolicyInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DeletePolicyInstanceResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_policy_instance(
+        self,
+        request: adcp_20220101_models.DeletePolicyInstanceRequest,
+    ) -> adcp_20220101_models.DeletePolicyInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_policy_instance_with_options(request, runtime)
+
+    async def delete_policy_instance_async(
+        self,
+        request: adcp_20220101_models.DeletePolicyInstanceRequest,
+    ) -> adcp_20220101_models.DeletePolicyInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_policy_instance_with_options_async(request, runtime)
+
+    def delete_user_permission_with_options(
+        self,
+        request: adcp_20220101_models.DeleteUserPermissionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DeleteUserPermissionResponse:
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
+    async def delete_user_permission_with_options_async(
+        self,
+        request: adcp_20220101_models.DeleteUserPermissionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DeleteUserPermissionResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_user_permission(
+        self,
+        request: adcp_20220101_models.DeleteUserPermissionRequest,
+    ) -> adcp_20220101_models.DeleteUserPermissionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_user_permission_with_options(request, runtime)
+
+    async def delete_user_permission_async(
+        self,
+        request: adcp_20220101_models.DeleteUserPermissionRequest,
+    ) -> adcp_20220101_models.DeleteUserPermissionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_user_permission_with_options_async(request, runtime)
+
+    def deploy_policy_instance_with_options(
+        self,
+        tmp_req: adcp_20220101_models.DeployPolicyInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DeployPolicyInstanceResponse:
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
+    async def deploy_policy_instance_with_options_async(
+        self,
+        tmp_req: adcp_20220101_models.DeployPolicyInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DeployPolicyInstanceResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def deploy_policy_instance(
+        self,
+        request: adcp_20220101_models.DeployPolicyInstanceRequest,
+    ) -> adcp_20220101_models.DeployPolicyInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.deploy_policy_instance_with_options(request, runtime)
+
+    async def deploy_policy_instance_async(
+        self,
+        request: adcp_20220101_models.DeployPolicyInstanceRequest,
+    ) -> adcp_20220101_models.DeployPolicyInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.deploy_policy_instance_with_options_async(request, runtime)
+
     def describe_hub_cluster_details_with_options(
         self,
         request: adcp_20220101_models.DescribeHubClusterDetailsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adcp_20220101_models.DescribeHubClusterDetailsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -695,14 +953,348 @@
     async def describe_managed_clusters_async(
         self,
         request: adcp_20220101_models.DescribeManagedClustersRequest,
     ) -> adcp_20220101_models.DescribeManagedClustersResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_managed_clusters_with_options_async(request, runtime)
 
+    def describe_policies_with_options(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePoliciesResponse:
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
+    async def describe_policies_with_options_async(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePoliciesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_policies(self) -> adcp_20220101_models.DescribePoliciesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policies_with_options(runtime)
+
+    async def describe_policies_async(self) -> adcp_20220101_models.DescribePoliciesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_policies_with_options_async(runtime)
+
+    def describe_policy_details_with_options(
+        self,
+        request: adcp_20220101_models.DescribePolicyDetailsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyDetailsResponse:
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
+    async def describe_policy_details_with_options_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyDetailsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyDetailsResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_policy_details(
+        self,
+        request: adcp_20220101_models.DescribePolicyDetailsRequest,
+    ) -> adcp_20220101_models.DescribePolicyDetailsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_details_with_options(request, runtime)
+
+    async def describe_policy_details_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyDetailsRequest,
+    ) -> adcp_20220101_models.DescribePolicyDetailsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_policy_details_with_options_async(request, runtime)
+
+    def describe_policy_governance_in_cluster_with_options(
+        self,
+        request: adcp_20220101_models.DescribePolicyGovernanceInClusterRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyGovernanceInClusterResponse:
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
+    async def describe_policy_governance_in_cluster_with_options_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyGovernanceInClusterRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyGovernanceInClusterResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_policy_governance_in_cluster(
+        self,
+        request: adcp_20220101_models.DescribePolicyGovernanceInClusterRequest,
+    ) -> adcp_20220101_models.DescribePolicyGovernanceInClusterResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_governance_in_cluster_with_options(request, runtime)
+
+    async def describe_policy_governance_in_cluster_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyGovernanceInClusterRequest,
+    ) -> adcp_20220101_models.DescribePolicyGovernanceInClusterResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_policy_governance_in_cluster_with_options_async(request, runtime)
+
+    def describe_policy_instances_with_options(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyInstancesResponse:
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
+    async def describe_policy_instances_with_options_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyInstancesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_policy_instances(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesRequest,
+    ) -> adcp_20220101_models.DescribePolicyInstancesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_instances_with_options(request, runtime)
+
+    async def describe_policy_instances_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesRequest,
+    ) -> adcp_20220101_models.DescribePolicyInstancesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_policy_instances_with_options_async(request, runtime)
+
+    def describe_policy_instances_status_with_options(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyInstancesStatusResponse:
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
+    async def describe_policy_instances_status_with_options_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.DescribePolicyInstancesStatusResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_policy_instances_status(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesStatusRequest,
+    ) -> adcp_20220101_models.DescribePolicyInstancesStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_policy_instances_status_with_options(request, runtime)
+
+    async def describe_policy_instances_status_async(
+        self,
+        request: adcp_20220101_models.DescribePolicyInstancesStatusRequest,
+    ) -> adcp_20220101_models.DescribePolicyInstancesStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_policy_instances_status_with_options_async(request, runtime)
+
     def describe_regions_with_options(
         self,
         request: adcp_20220101_models.DescribeRegionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adcp_20220101_models.DescribeRegionsResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -913,14 +1505,100 @@
     async def detach_cluster_from_hub_async(
         self,
         request: adcp_20220101_models.DetachClusterFromHubRequest,
     ) -> adcp_20220101_models.DetachClusterFromHubResponse:
         runtime = util_models.RuntimeOptions()
         return await self.detach_cluster_from_hub_with_options_async(request, runtime)
 
+    def grant_user_permission_with_options(
+        self,
+        request: adcp_20220101_models.GrantUserPermissionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.GrantUserPermissionResponse:
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
+    async def grant_user_permission_with_options_async(
+        self,
+        request: adcp_20220101_models.GrantUserPermissionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.GrantUserPermissionResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def grant_user_permission(
+        self,
+        request: adcp_20220101_models.GrantUserPermissionRequest,
+    ) -> adcp_20220101_models.GrantUserPermissionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.grant_user_permission_with_options(request, runtime)
+
+    async def grant_user_permission_async(
+        self,
+        request: adcp_20220101_models.GrantUserPermissionRequest,
+    ) -> adcp_20220101_models.GrantUserPermissionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.grant_user_permission_with_options_async(request, runtime)
+
     def grant_user_permissions_with_options(
         self,
         tmp_req: adcp_20220101_models.GrantUserPermissionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adcp_20220101_models.GrantUserPermissionsResponse:
         UtilClient.validate_model(tmp_req)
         request = adcp_20220101_models.GrantUserPermissionsShrinkRequest()
@@ -1116,7 +1794,93 @@
 
     async def update_hub_cluster_feature_async(
         self,
         request: adcp_20220101_models.UpdateHubClusterFeatureRequest,
     ) -> adcp_20220101_models.UpdateHubClusterFeatureResponse:
         runtime = util_models.RuntimeOptions()
         return await self.update_hub_cluster_feature_with_options_async(request, runtime)
+
+    def update_user_permission_with_options(
+        self,
+        request: adcp_20220101_models.UpdateUserPermissionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.UpdateUserPermissionResponse:
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
+    async def update_user_permission_with_options_async(
+        self,
+        request: adcp_20220101_models.UpdateUserPermissionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> adcp_20220101_models.UpdateUserPermissionResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_user_permission(
+        self,
+        request: adcp_20220101_models.UpdateUserPermissionRequest,
+    ) -> adcp_20220101_models.UpdateUserPermissionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_user_permission_with_options(request, runtime)
+
+    async def update_user_permission_async(
+        self,
+        request: adcp_20220101_models.UpdateUserPermissionRequest,
+    ) -> adcp_20220101_models.UpdateUserPermissionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_user_permission_with_options_async(request, runtime)
```

### Comparing `alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101/models.py` & `alibabacloud_adcp20220101-1.0.9/alibabacloud_adcp20220101/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -150,30 +150,36 @@
         price_limit: str = None,
         profile: str = None,
         region_id: str = None,
         v_switches: str = None,
         vpc_id: str = None,
         workflow_schedule_mode: str = None,
     ):
-        # Specifies whether to use a public IP address to expose the API server. Valid values: - true: uses a public IP address to expose the API server. - true: uses an internal IP address to expose the API server.
+        # Specifies whether to expose the API server to the Internet. Valid values:
+        # 
+        # *   true: exposes the API server to the Internet.
+        # *   false: exposes the API server to the internal network.
         self.api_server_public_eip = api_server_public_eip
         self.argo_server_enabled = argo_server_enabled
-        # Specifies whether to enable audit logs. Valid values: - true: enables audit logs. - false: disables audit logs.
+        # Specifies whether to enable the audit log feature. Valid values:
+        # 
+        # *   true: enables the audit log feature.
+        # *   false: disables the audit log feature.
         self.audit_log_enabled = audit_log_enabled
-        # Specifies whether the security group is an advanced security group.
+        # Specifies whether to use an advanced security group.
         self.is_enterprise_security_group = is_enterprise_security_group
         # The name of the master instance.
         self.name = name
         self.price_limit = price_limit
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
         self.profile = profile
         # The ID of the region. You can call the DescribeRegions operation to query available regions.
         self.region_id = region_id
         # The ID of the vSwitch.
         self.v_switches = v_switches
         # The ID of the virtual private cloud (VPC) to which the master instance belongs. You can call the DescribeVpcs operation to query available VPCs.
         self.vpc_id = vpc_id
@@ -330,16 +336,22 @@
         self,
         cluster_id: str = None,
         force: bool = None,
         retain_resources: List[str] = None,
     ):
         # The ID of the master instance.
         self.cluster_id = cluster_id
-        # Specifies whether to forcefully delete the master instance. Valid values: - true: forcefully delete the master instance. - false: does not forcefully delete the master instance. Default value: false.
+        # Specifies whether to forcefully delete the master instance in ACK One. Valid values:
+        # 
+        # *   true: forcefully deletes the master instance in ACK One.
+        # *   false: does not forcibly delete the master instance in ACK One.
+        # 
+        # Default value: false.
         self.force = force
+        # The list of resources to retain.
         self.retain_resources = retain_resources
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -371,16 +383,22 @@
         self,
         cluster_id: str = None,
         force: bool = None,
         retain_resources_shrink: str = None,
     ):
         # The ID of the master instance.
         self.cluster_id = cluster_id
-        # Specifies whether to forcefully delete the master instance. Valid values: - true: forcefully delete the master instance. - false: does not forcefully delete the master instance. Default value: false.
+        # Specifies whether to forcefully delete the master instance in ACK One. Valid values:
+        # 
+        # *   true: forcefully deletes the master instance in ACK One.
+        # *   false: does not forcibly delete the master instance in ACK One.
+        # 
+        # Default value: false.
         self.force = force
+        # The list of resources to retain.
         self.retain_resources_shrink = retain_resources_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -410,19 +428,19 @@
 class DeleteHubClusterResponseBody(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         request_id: str = None,
         task_id: str = None,
     ):
-        # The ID of the master instance.
+        # The ID of the cluster.
         self.cluster_id = cluster_id
         # The ID of the request.
         self.request_id = request_id
-        # The ID of the master instance.
+        # The ID of the job.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -489,14 +507,443 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteHubClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeletePolicyInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        cluster_id: str = None,
+        cluster_ids: List[str] = None,
+        policy_name: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.cluster_ids = cluster_ids
+        self.policy_name = policy_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+        cluster_ids_shrink: str = None,
+        policy_name: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.cluster_ids_shrink = cluster_ids_shrink
+        self.policy_name = policy_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeletePolicyInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeletePolicyInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+        user_id: str = None,
+    ):
+        # The ID of the master instance.
+        self.cluster_id = cluster_id
+        # The ID of the RAM user.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class DeleteUserPermissionResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteUserPermissionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteUserPermissionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+        cluster_ids: List[str] = None,
+        namespaces: List[str] = None,
+        policy_action: str = None,
+        policy_name: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.cluster_ids = cluster_ids
+        self.namespaces = namespaces
+        self.policy_action = policy_action
+        self.policy_name = policy_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+        cluster_ids_shrink: str = None,
+        namespaces_shrink: str = None,
+        policy_action: str = None,
+        policy_name: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.cluster_ids_shrink = cluster_ids_shrink
+        self.namespaces_shrink = namespaces_shrink
+        self.policy_action = policy_action
+        self.policy_name = policy_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeployPolicyInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeployPolicyInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         cluster_id: str = None,
     ):
         # The ID of the master instance.
         self.cluster_id = cluster_id
@@ -526,15 +973,18 @@
         self,
         api_server_eip_id: str = None,
         enabled_public: bool = None,
         load_balancer_id: str = None,
     ):
         # The ID of the elastic IP address (EIP).
         self.api_server_eip_id = api_server_eip_id
-        # Indicates whether a public endpoint is used to expose the API server. Valid values: - true: a public endpoint is used to expose the API server. - false: no public endpoint is used to expose the API server.
+        # Indicates whether the API server is accessible over the Internet. Valid values:
+        # 
+        # *   true: The API server is accessible over the Internet.
+        # *   false: The API server is inaccessible over the Internet.
         self.enabled_public = enabled_public
         # The ID of the Server Load Balancer (SLB) instance.
         self.load_balancer_id = load_balancer_id
 
     def validate(self):
         pass
 
@@ -575,31 +1025,41 @@
         region_id: str = None,
         state: str = None,
         update_time: str = None,
         version: str = None,
     ):
         # The ID of the master instance.
         self.cluster_id = cluster_id
-        # The specification of the master instance. Valid values: - ack.pro.small: ACK Pro
+        # The specification of the master instance. Valid value:
+        # 
+        # *   ack.pro.small: ACK Pro cluster
         self.cluster_spec = cluster_spec
         # The time when the master instance was created.
         self.creation_time = creation_time
-        # The error message that is returned when the system fails to create the master instance.
+        # The error message returned when the master instance failed to be created.
         self.error_message = error_message
         # The name of the master instance.
         self.name = name
         # The configurations of the master instance.
         self.profile = profile
         # The ID of the region in which the master instance resides.
         self.region_id = region_id
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
         self.state = state
         # The time when the master instance was updated.
         self.update_time = update_time
-        # The Kubernetes version of the master instance.
+        # The version of the master instance.
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -658,22 +1118,23 @@
     def __init__(
         self,
         message: str = None,
         reason: str = None,
         status: str = None,
         type: str = None,
     ):
-        # The error message of the deletion condition.
+        # The error message returned.
         self.message = message
         # The reason for the deletion condition.
         self.reason = reason
-        # The status of the deletion condition. Valid values:
-        # - True: The master instance cannot be deleted.
-        # - False: The master instance can be deleted.
-        # - Unknow: Whether the master instance can be deleted is unknown.
+        # The status of the master instance that the deletion condition indicates. Valid values:
+        # 
+        # *   True: The master instance cannot be deleted.
+        # *   False: The master instance can be deleted.
+        # *   Unknow: Whether the master instance can be deleted is unknown.
         self.status = status
         # The type of deletion condition.
         self.type = type
 
     def validate(self):
         pass
 
@@ -708,17 +1169,17 @@
 
 class DescribeHubClusterDetailsResponseBodyClusterEndpoints(TeaModel):
     def __init__(
         self,
         intranet_api_server_endpoint: str = None,
         public_api_server_endpoint: str = None,
     ):
-        # The internal endpoint of the API server of the master instance.
+        # The endpoint that is used to access the API server over the internal network.
         self.intranet_api_server_endpoint = intranet_api_server_endpoint
-        # The public endpoint of the API server of the master instance.
+        # The endpoint that is used to access the API server over the Internet.
         self.public_api_server_endpoint = public_api_server_endpoint
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -744,19 +1205,22 @@
 class DescribeHubClusterDetailsResponseBodyClusterLogConfig(TeaModel):
     def __init__(
         self,
         enable_log: bool = None,
         log_project: str = None,
         log_store_ttl: str = None,
     ):
-        # Indicates whether audit logs are enabled. Valid values: - true: audit logs are enabled. - false: audit logs are disabled.
+        # Indicates whether the audit logging feature is enabled. Valid values:
+        # 
+        # *   true: Audit logging is enabled.
+        # *   false: Audit logging is disabled.
         self.enable_log = enable_log
-        # The name of the Log Service project.
+        # The name of the project of Log Service.
         self.log_project = log_project
-        # The retention period of the logs.
+        # The number of days that logs are retained by Log Service.
         self.log_store_ttl = log_store_ttl
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -785,17 +1249,20 @@
 
 class DescribeHubClusterDetailsResponseBodyClusterMeshConfig(TeaModel):
     def __init__(
         self,
         enable_mesh: bool = None,
         mesh_id: str = None,
     ):
-        # Indicates whether ASM is enabled. Valid values: - true: ASM is enabled. - false: ASM is disabled.
+        # Indicates whether ASM is enabled. Valid values:
+        # 
+        # *   true: ASM is enabled.
+        # *   false: ASM is disabled.
         self.enable_mesh = enable_mesh
-        # The ID of the ASM instance.
+        # service mesh (ASM) instance ID
         self.mesh_id = mesh_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -825,19 +1292,23 @@
         ipstack: str = None,
         security_group_ids: List[str] = None,
         v_switches: List[str] = None,
         vpc_id: str = None,
     ):
         # The domain name of the master instance.
         self.cluster_domain = cluster_domain
-        # The IP version that is supported by the master instance. Valid values: - ipv4: IPv4. - ipv6: IPv6. - dual: IPv4 and IPv6.
+        # The IP version that is supported by the master instance. Valid values:
+        # 
+        # *   ipv4: IPv4.
+        # *   ipv6: IPv6.
+        # *   dual: IPv4 and IPv6.
         self.ipstack = ipstack
-        # The ID of the associated security group.
+        # The IDs of the associated security groups.
         self.security_group_ids = security_group_ids
-        # A list of the vSwitches that are used by the master instance.
+        # The details of the vSwitches.
         self.v_switches = v_switches
         # The ID of the virtual private cloud (VPC) in which the master instance resides.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
@@ -1015,25 +1486,25 @@
         conditions: List[DescribeHubClusterDetailsResponseBodyClusterConditions] = None,
         endpoints: DescribeHubClusterDetailsResponseBodyClusterEndpoints = None,
         log_config: DescribeHubClusterDetailsResponseBodyClusterLogConfig = None,
         mesh_config: DescribeHubClusterDetailsResponseBodyClusterMeshConfig = None,
         network: DescribeHubClusterDetailsResponseBodyClusterNetwork = None,
         workflow_config: DescribeHubClusterDetailsResponseBodyClusterWorkflowConfig = None,
     ):
-        # Information about the API server of the master instance.
+        # The details of the API server of the master instance.
         self.api_server = api_server
-        # The details about the master instance.
+        # The details of the master instance.
         self.cluster_info = cluster_info
-        # The list of the deletion conditions of the master instance.
+        # The deletion conditions of the master instance.
         self.conditions = conditions
         # The endpoint of the master instance.
         self.endpoints = endpoints
         # The logging configuration.
         self.log_config = log_config
-        # The Service Mesh (ASM) configurations.
+        # The configurations of Alibaba Cloud Service Mesh (ASM).
         self.mesh_config = mesh_config
         # The network configurations of the master instance.
         self.network = network
         self.workflow_config = workflow_config
 
     def validate(self):
         if self.api_server:
@@ -1114,15 +1585,15 @@
 
 class DescribeHubClusterDetailsResponseBody(TeaModel):
     def __init__(
         self,
         cluster: DescribeHubClusterDetailsResponseBodyCluster = None,
         request_id: str = None,
     ):
-        # The details about the master instance.
+        # The details of the master instance.
         self.cluster = cluster
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.cluster:
             self.cluster.validate()
@@ -1197,15 +1668,20 @@
     def __init__(
         self,
         cluster_id: str = None,
         private_ip_address: bool = None,
     ):
         # The ID of the master instance.
         self.cluster_id = cluster_id
-        # Specifies whether to obtain the credential that is used to connect to the master instance over the internal network. Valid values: - `true`: obtains only the credential that is used to access the master instance over the internal network. - `false`: obtains only the credential that is used to access the master instance over the Internet. Default value: `false`.
+        # Specifies whether to obtain the kubeconfig file that is used to connect to the cluster over the internal network. Valid values:
+        # 
+        # *   `true`: obtains the kubeconfig file that is used to connect to the master instance over the internal network.
+        # *   `false`: obtains the kubeconfig file that is used to connect to the master instance over the Internet.
+        # 
+        # Default value: `false`
         self.private_ip_address = private_ip_address
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1230,15 +1706,15 @@
 
 class DescribeHubClusterKubeconfigResponseBody(TeaModel):
     def __init__(
         self,
         kubeconfig: str = None,
         request_id: str = None,
     ):
-        # The content of the kubeconfig file of the master instance.
+        # The content of the kubeconfig file.
         self.kubeconfig = kubeconfig
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -2396,14 +2872,1449 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeManagedClustersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePoliciesResponseBodyPolicies(TeaModel):
+    def __init__(
+        self,
+        category: str = None,
+        names: List[str] = None,
+    ):
+        self.category = category
+        self.names = names
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('Names') is not None:
+            self.names = m.get('Names')
+        return self
+
+
+class DescribePoliciesResponseBody(TeaModel):
+    def __init__(
+        self,
+        policies: List[DescribePoliciesResponseBodyPolicies] = None,
+        request_id: str = None,
+    ):
+        self.policies = policies
+        self.request_id = request_id
+
+    def validate(self):
+        if self.policies:
+            for k in self.policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePoliciesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        policy_name: str = None,
+    ):
+        self.policy_name = policy_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DescribePolicyDetailsResponseBodyPolicy(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        category: str = None,
+        created: str = None,
+        description: str = None,
+        name: str = None,
+        no_config: int = None,
+        severity: str = None,
+        template: str = None,
+        updated: str = None,
+    ):
+        self.action = action
+        self.category = category
+        self.created = created
+        self.description = description
+        self.name = name
+        self.no_config = no_config
+        self.severity = severity
+        self.template = template
+        self.updated = updated
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        policy: DescribePolicyDetailsResponseBodyPolicy = None,
+        request_id: str = None,
+    ):
+        self.policy = policy
+        self.request_id = request_id
+
+    def validate(self):
+        if self.policy:
+            self.policy.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePolicyDetailsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+    ):
+        self.cluster_id = cluster_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesCluster(TeaModel):
+    def __init__(
+        self,
+        cluster_id: str = None,
+        cluster_spec: str = None,
+        cluster_type: str = None,
+        name: str = None,
+        profile: str = None,
+        region_id: str = None,
+        state: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.cluster_spec = cluster_spec
+        self.cluster_type = cluster_type
+        self.name = name
+        self.profile = profile
+        self.region_id = region_id
+        self.state = state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        count: str = None,
+        log_project: str = None,
+        log_store: str = None,
+        logs: List[Dict[str, str]] = None,
+        progress: str = None,
+    ):
+        self.count = count
+        self.log_project = log_project
+        self.log_store = log_store
+        self.logs = logs
+        self.progress = progress
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        enabled_count: int = None,
+        severity: str = None,
+        total_count: int = None,
+    ):
+        self.enabled_count = enabled_count
+        self.severity = severity
+        self.total_count = total_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        severity: str = None,
+        violations: int = None,
+    ):
+        self.severity = severity
+        self.violations = violations
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Violations') is not None:
+            self.violations = m.get('Violations')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsWarn(TeaModel):
+    def __init__(
+        self,
+        severity: str = None,
+        violations: str = None,
+    ):
+        self.severity = severity
+        self.violations = violations
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Violations') is not None:
+            self.violations = m.get('Violations')
+        return self
+
+
+class DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolations(TeaModel):
+    def __init__(
+        self,
+        deny: List[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsDeny] = None,
+        warn: List[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolationsWarn] = None,
+    ):
+        self.deny = deny
+        self.warn = warn
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
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        policy_description: str = None,
+        policy_name: str = None,
+        severity: str = None,
+        violations: int = None,
+    ):
+        self.policy_description = policy_description
+        self.policy_name = policy_name
+        self.severity = severity
+        self.violations = violations
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        policy_description: str = None,
+        policy_name: str = None,
+        severity: str = None,
+        violations: int = None,
+    ):
+        self.policy_description = policy_description
+        self.policy_name = policy_name
+        self.severity = severity
+        self.violations = violations
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        deny: List[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsDeny] = None,
+        warn: List[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolationsWarn] = None,
+    ):
+        self.deny = deny
+        self.warn = warn
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
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        total_violations: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationTotalViolations = None,
+        violations: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolationViolations = None,
+    ):
+        self.total_violations = total_violations
+        self.violations = violations
+
+    def validate(self):
+        if self.total_violations:
+            self.total_violations.validate()
+        if self.violations:
+            self.violations.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        admit_log: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceAdmitLog = None,
+        on_state: List[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceOnState] = None,
+        violation: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernanceViolation = None,
+    ):
+        self.admit_log = admit_log
+        self.on_state = on_state
+        self.violation = violation
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
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesCluster = None,
+        policy_governance: DescribePolicyGovernanceInClusterResponseBodyPolicyGovernancesPolicyGovernance = None,
+    ):
+        self.cluster = cluster
+        self.policy_governance = policy_governance
+
+    def validate(self):
+        if self.cluster:
+            self.cluster.validate()
+        if self.policy_governance:
+            self.policy_governance.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        policy_governances: List[DescribePolicyGovernanceInClusterResponseBodyPolicyGovernances] = None,
+        request_id: str = None,
+    ):
+        self.policy_governances = policy_governances
+        self.request_id = request_id
+
+    def validate(self):
+        if self.policy_governances:
+            for k in self.policy_governances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePolicyGovernanceInClusterResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+        policy_name: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.policy_name = policy_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        return self
+
+
+class DescribePolicyInstancesResponseBodyPolicies(TeaModel):
+    def __init__(
+        self,
+        cluster_id: str = None,
+        instance_name: str = None,
+        policy_action: str = None,
+        policy_category: str = None,
+        policy_description: str = None,
+        policy_name: str = None,
+        policy_parameters: Dict[str, str] = None,
+        policy_scope: str = None,
+        policy_severity: str = None,
+        total_violations: int = None,
+    ):
+        self.cluster_id = cluster_id
+        self.instance_name = instance_name
+        self.policy_action = policy_action
+        self.policy_category = policy_category
+        self.policy_description = policy_description
+        self.policy_name = policy_name
+        self.policy_parameters = policy_parameters
+        self.policy_scope = policy_scope
+        self.policy_severity = policy_severity
+        self.total_violations = total_violations
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        policies: List[DescribePolicyInstancesResponseBodyPolicies] = None,
+        request_id: str = None,
+    ):
+        self.policies = policies
+        self.request_id = request_id
+
+    def validate(self):
+        if self.policies:
+            for k in self.policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePolicyInstancesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+    ):
+        self.cluster_id = cluster_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstancesPolicyClusters(TeaModel):
+    def __init__(
+        self,
+        cluster_id: str = None,
+        status: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstances(TeaModel):
+    def __init__(
+        self,
+        policy_category: str = None,
+        policy_clusters: List[DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstancesPolicyClusters] = None,
+        policy_description: str = None,
+        policy_instances_count: int = None,
+        policy_name: str = None,
+        policy_severity: str = None,
+    ):
+        self.policy_category = policy_category
+        self.policy_clusters = policy_clusters
+        self.policy_description = policy_description
+        self.policy_instances_count = policy_instances_count
+        self.policy_name = policy_name
+        self.policy_severity = policy_severity
+
+    def validate(self):
+        if self.policy_clusters:
+            for k in self.policy_clusters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        severity_count: str = None,
+        severity_type: str = None,
+    ):
+        self.severity_count = severity_count
+        self.severity_type = severity_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SeverityCount') is not None:
+            self.severity_count = m.get('SeverityCount')
+        if m.get('SeverityType') is not None:
+            self.severity_type = m.get('SeverityType')
+        return self
+
+
+class DescribePolicyInstancesStatusResponseBodyPolicies(TeaModel):
+    def __init__(
+        self,
+        policy_instances: List[DescribePolicyInstancesStatusResponseBodyPoliciesPolicyInstances] = None,
+        severity_info: List[DescribePolicyInstancesStatusResponseBodyPoliciesSeverityInfo] = None,
+    ):
+        self.policy_instances = policy_instances
+        self.severity_info = severity_info
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
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        policies: DescribePolicyInstancesStatusResponseBodyPolicies = None,
+        request_id: str = None,
+    ):
+        self.policies = policies
+        self.request_id = request_id
+
+    def validate(self):
+        if self.policies:
+            self.policies.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePolicyInstancesStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         language: str = None,
     ):
         # The language. Valid values: zh, en, and jp.
         self.language = language
@@ -2551,14 +4462,15 @@
 
 
 class DescribeUserPermissionsRequest(TeaModel):
     def __init__(
         self,
         user_id: str = None,
     ):
+        # The ID of the RAM user that you want to query.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2581,17 +4493,31 @@
     def __init__(
         self,
         resource_id: str = None,
         resource_type: str = None,
         role_name: str = None,
         role_type: str = None,
     ):
+        # The authorization setting. Valid values:
+        # 
+        # *   {cluster_id} is returned if the permissions are scoped to a cluster.
+        # *   {cluster_id}/{namespace} is returned if the permissions are scoped to a namespace of a cluster.
+        # *   all-clusters is returned if the permissions are scoped to all clusters.
         self.resource_id = resource_id
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: indicates that the permissions are scoped to a cluster.
+        # *   namespace: indicates that the permissions are scoped to a namespace of a cluster.
         self.resource_type = resource_type
+        # The name of the custom role. If a custom role is assigned, the value is the name of the assigned custom role.
         self.role_name = role_name
+        # The type of predefined role. Valid values:
+        # 
+        # *   admin: administrator
+        # *   dev: developer
         self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2624,15 +4550,17 @@
 
 class DescribeUserPermissionsResponseBody(TeaModel):
     def __init__(
         self,
         permissions: List[DescribeUserPermissionsResponseBodyPermissions] = None,
         request_id: str = None,
     ):
+        # The details about the permissions of the RAM user.
         self.permissions = permissions
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -2838,14 +4766,148 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DetachClusterFromHubResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GrantUserPermissionRequest(TeaModel):
+    def __init__(
+        self,
+        cluster_id: str = None,
+        namespace: str = None,
+        role_name: str = None,
+        role_type: str = None,
+        user_id: str = None,
+    ):
+        # The ID of the master instance.
+        self.cluster_id = cluster_id
+        # The namespace to which the permissions are scoped. By default, this parameter is empty when you set role_type to cluster.
+        self.namespace = namespace
+        # Specifies the predefined role that you want to assign. Valid values:
+        # 
+        # *   admin: the administrator role.
+        # *   dev: the developer role.
+        self.role_name = role_name
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: specifies that the permissions are scoped to a master instance.
+        # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
+        self.role_type = role_type
+        # The ID of the RAM user.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GrantUserPermissionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GrantUserPermissionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         cluster_id: str = None,
         namespace: str = None,
         role_name: str = None,
         role_type: str = None,
@@ -3048,26 +5110,38 @@
         v_switches: List[str] = None,
         workflow_schedule_mode: str = None,
     ):
         # The ID of the EIP.
         self.api_server_eip_id = api_server_eip_id
         self.argo_cdenabled = argo_cdenabled
         self.argo_server_enabled = argo_server_enabled
-        # Specifies whether to enable audit logs. Valid values: - true: enable audit logs. - false: disables audit logs.
+        # Specifies whether to enable the audit logging feature. Valid values:
+        # 
+        # *   true: enables the audit logging feature.
+        # *   false: disables the audit logging feature.
         self.audit_log_enabled = audit_log_enabled
-        # The ID of the master instance.
+        # The ID of the cluster.
         self.cluster_id = cluster_id
-        # Specifies whether to enable deletion protection for the master instance. After you enable deletion protection, you cannot delete the master instance in the console or by calling API operations. Valid values:
+        # Specifies whether to enable deletion protection for the cluster. After you enable deletion protection, you cannot delete the master instance in the console or by calling the DeleteHubCluster operation. Valid values:
+        # 
+        # *   true: enables deletion protection for the cluster.
+        # *   false: disables deletion protection for the cluster. This is the default value.
         self.deletion_protection = deletion_protection
-        # Specifies whether to enable Service Mesh (ASM). Valid values: true: enables ASM. false: disables ASM.
+        # Specifies whether to enable Alibaba Cloud Service Mesh (ASM). Valid values:
+        # 
+        # true: enables ASM. false: disables ASM.
         self.enable_mesh = enable_mesh
-        # The name of the master instance. The name must be 1 to 63 characters in length, and can contain letters and digits. The name must start with a letter. The name can contain letters, digits, underscores (_), and hyphens (-).
+        # The name of the cluster. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit
-        # Specifies whether to associate an elastic IP address (EIP) with the API server. Default value: false. To associate an EIP with the API server, set the value to true. You can use a custom EIP by setting the ApiServerEipId parameter. If you do not set the ApiServerEipId parameter, the system automatically creates an EIP.
+        # Specifies whether to associate an elastic IP address (EIP) with the API server. Valid values:
+        # 
+        # *   true: associates an EIP with the API server. You can specify the ApiServerEipId parameter. If you do not specify the ApiServerEipId parameter, the system automatically creates an EIP.
+        # *   false: disassociates an EIP from the API server.
         self.public_api_server_enabled = public_api_server_enabled
         self.v_switches = v_switches
         self.workflow_schedule_mode = workflow_schedule_mode
 
     def validate(self):
         pass
 
@@ -3148,26 +5222,38 @@
         v_switches_shrink: str = None,
         workflow_schedule_mode: str = None,
     ):
         # The ID of the EIP.
         self.api_server_eip_id = api_server_eip_id
         self.argo_cdenabled = argo_cdenabled
         self.argo_server_enabled = argo_server_enabled
-        # Specifies whether to enable audit logs. Valid values: - true: enable audit logs. - false: disables audit logs.
+        # Specifies whether to enable the audit logging feature. Valid values:
+        # 
+        # *   true: enables the audit logging feature.
+        # *   false: disables the audit logging feature.
         self.audit_log_enabled = audit_log_enabled
-        # The ID of the master instance.
+        # The ID of the cluster.
         self.cluster_id = cluster_id
-        # Specifies whether to enable deletion protection for the master instance. After you enable deletion protection, you cannot delete the master instance in the console or by calling API operations. Valid values:
+        # Specifies whether to enable deletion protection for the cluster. After you enable deletion protection, you cannot delete the master instance in the console or by calling the DeleteHubCluster operation. Valid values:
+        # 
+        # *   true: enables deletion protection for the cluster.
+        # *   false: disables deletion protection for the cluster. This is the default value.
         self.deletion_protection = deletion_protection
-        # Specifies whether to enable Service Mesh (ASM). Valid values: true: enables ASM. false: disables ASM.
+        # Specifies whether to enable Alibaba Cloud Service Mesh (ASM). Valid values:
+        # 
+        # true: enables ASM. false: disables ASM.
         self.enable_mesh = enable_mesh
-        # The name of the master instance. The name must be 1 to 63 characters in length, and can contain letters and digits. The name must start with a letter. The name can contain letters, digits, underscores (_), and hyphens (-).
+        # The name of the cluster. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit
-        # Specifies whether to associate an elastic IP address (EIP) with the API server. Default value: false. To associate an EIP with the API server, set the value to true. You can use a custom EIP by setting the ApiServerEipId parameter. If you do not set the ApiServerEipId parameter, the system automatically creates an EIP.
+        # Specifies whether to associate an elastic IP address (EIP) with the API server. Valid values:
+        # 
+        # *   true: associates an EIP with the API server. You can specify the ApiServerEipId parameter. If you do not specify the ApiServerEipId parameter, the system automatically creates an EIP.
+        # *   false: disassociates an EIP from the API server.
         self.public_api_server_enabled = public_api_server_enabled
         self.v_switches_shrink = v_switches_shrink
         self.workflow_schedule_mode = workflow_schedule_mode
 
     def validate(self):
         pass
 
@@ -3300,7 +5386,141 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateHubClusterFeatureResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateUserPermissionRequest(TeaModel):
+    def __init__(
+        self,
+        cluster_id: str = None,
+        namespace: str = None,
+        role_name: str = None,
+        role_type: str = None,
+        user_id: str = None,
+    ):
+        # The ID of the master instance.
+        self.cluster_id = cluster_id
+        # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
+        self.namespace = namespace
+        # Specifies the predefined role that you want to assign. Valid values:
+        # 
+        # *   admin: the administrator role.
+        # *   dev: the developer role.
+        self.role_name = role_name
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: specifies that the permissions are scoped to a master instance.
+        # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
+        self.role_type = role_type
+        # The ID of the RAM user.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateUserPermissionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateUserPermissionResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_adcp20220101-1.0.8/alibabacloud_adcp20220101.egg-info/PKG-INFO` & `alibabacloud_adcp20220101-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-adcp20220101
-Version: 1.0.8
+Name: alibabacloud_adcp20220101
+Version: 1.0.9
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101-1.0.8/setup.py` & `alibabacloud_adcp20220101-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adcp20220101.
 
-Created on 16/03/2023
+Created on 27/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adcp20220101"
 NAME = "alibabacloud_adcp20220101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adcp (20220101) SDK Library for Python"
```

