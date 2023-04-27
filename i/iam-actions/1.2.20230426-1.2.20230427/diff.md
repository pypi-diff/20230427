# Comparing `tmp/iam_actions-1.2.20230426.tar.gz` & `tmp/iam_actions-1.2.20230427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230426.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230427.tar", max compression
```

## Comparing `iam_actions-1.2.20230426.tar` & `iam_actions-1.2.20230427.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/README.md
--rw-r--r--   0        0        0      228 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/iam_actions/__init__.py
--rw-r--r--   0        0        0  4224370 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-26 02:30:56.313800 iam_actions-1.2.20230426/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-26 02:30:56.317800 iam_actions-1.2.20230426/iam_actions/generate/services.py
--rw-r--r--   0        0        0   543474 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/policies.json
--rw-r--r--   0        0        0   190303 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   527056 2023-04-26 02:32:19.336893 iam_actions-1.2.20230426/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-26 02:32:20.132886 iam_actions-1.2.20230426/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230426/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230426/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/README.md
+-rw-r--r--   0        0        0      228 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4228268 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-27 02:26:10.775297 iam_actions-1.2.20230427/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   544282 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/policies.json
+-rw-r--r--   0        0        0   190316 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   527862 2023-04-27 02:28:37.745116 iam_actions-1.2.20230427/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-27 02:28:38.853130 iam_actions-1.2.20230427/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230427/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230427/PKG-INFO
```

### Comparing `iam_actions-1.2.20230426/LICENSE` & `iam_actions-1.2.20230427/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/README.md` & `iam_actions-1.2.20230427/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/iam_actions/actions.json` & `iam_actions-1.2.20230427/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970654928638122%*

 * *Differences: {"'fms'": "{'ListAdminsManagingAccount': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *          "'ListAdminsManagingAccount'), ('condition_keys', []), ('description', 'Not Documented "*

 * *          "by AWS'), ('orphan', False), ('resources', [])]), 'PutAdminAccount': "*

 * *          "OrderedDict([('access_level', 'Undocumented'), ('action', 'PutAdminAccount'), "*

 * *          "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', False), "*

 * *          "('resources', [])]), 'GetAdmin […]*

```diff
@@ -59626,14 +59626,22 @@
             "access_level": "Read",
             "action": "GetAdminAccount",
             "condition_keys": [],
             "description": "Grants permission to return the AWS Organizations account that is associated with AWS Firewall Manager as the AWS Firewall Manager administrator",
             "orphan": false,
             "resources": []
         },
+        "GetAdminScope": {
+            "access_level": "Undocumented",
+            "action": "GetAdminScope",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetAppsList": {
             "access_level": "Read",
             "action": "GetAppsList",
             "condition_keys": [],
             "description": "Grants permission to return information about the specified AWS Firewall Manager applications list",
             "orphan": false,
             "resources": [
@@ -59712,14 +59720,30 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve violations for a resource based on the specified AWS Firewall Manager policy and AWS account",
             "orphan": false,
             "resources": [
                 "policy"
             ]
         },
+        "ListAdminAccountsForOrganization": {
+            "access_level": "Undocumented",
+            "action": "ListAdminAccountsForOrganization",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListAdminsManagingAccount": {
+            "access_level": "Undocumented",
+            "action": "ListAdminsManagingAccount",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAppsLists": {
             "access_level": "List",
             "action": "ListAppsLists",
             "condition_keys": [],
             "description": "Grants permission to return an array of AppsListDataSummary objects",
             "orphan": false,
             "resources": []
@@ -59798,14 +59822,22 @@
             "access_level": "List",
             "action": "ListThirdPartyFirewallFirewallPolicies",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of all of the third-party firewall policies that are associated with the third-party firewall administrator's account",
             "orphan": false,
             "resources": []
         },
+        "PutAdminAccount": {
+            "access_level": "Undocumented",
+            "action": "PutAdminAccount",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PutAppsList": {
             "access_level": "Write",
             "action": "PutAppsList",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -103572,14 +103604,136 @@
             "description": "Grants permission to update an existing policy with a new name, description, or content",
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
+    "osis": {
+        "CreatePipeline": {
+            "access_level": "Undocumented",
+            "action": "CreatePipeline",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeletePipeline": {
+            "access_level": "Undocumented",
+            "action": "DeletePipeline",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPipeline": {
+            "access_level": "Undocumented",
+            "action": "GetPipeline",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPipelineBlueprint": {
+            "access_level": "Undocumented",
+            "action": "GetPipelineBlueprint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPipelineChangeProgress": {
+            "access_level": "Undocumented",
+            "action": "GetPipelineChangeProgress",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "Ingest": {
+            "access_level": "Undocumented",
+            "action": "Ingest",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListPipelineBlueprints": {
+            "access_level": "Undocumented",
+            "action": "ListPipelineBlueprints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListPipelines": {
+            "access_level": "Undocumented",
+            "action": "ListPipelines",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartPipeline": {
+            "access_level": "Undocumented",
+            "action": "StartPipeline",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StopPipeline": {
+            "access_level": "Undocumented",
+            "action": "StopPipeline",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePipeline": {
+            "access_level": "Undocumented",
+            "action": "UpdatePipeline",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ValidatePipeline": {
+            "access_level": "Undocumented",
+            "action": "ValidatePipeline",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "outposts": {
         "CancelOrder": {
             "access_level": "Write",
             "action": "CancelOrder",
             "condition_keys": [],
             "description": "Grants permission to cancel an order",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230426/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230427/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230427/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/iam_actions/generate/generate.py` & `iam_actions-1.2.20230427/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230427/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230427/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/iam_actions/generate/services.py` & `iam_actions-1.2.20230427/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230426/iam_actions/policies.json` & `iam_actions-1.2.20230427/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997315592903828%*

 * *Differences: {"'serviceMap'": "{'AWS Firewall Manager': {'Actions': {insert: [(12, 'GetAdminScope'), (22, "*

 * *                 "'ListAdminAccountsForOrganization'), (23, 'ListAdminsManagingAccount'), (34, "*

 * *                 "'PutAdminAccount')]}}, 'Amazon OpenSearch Ingestion': "*

 * *                 "OrderedDict([('StringPrefix', 'osis'), ('Actions', ['CreatePipeline', "*

 * *                 "'DeletePipeline', 'GetPipeline', 'GetPipelineBlueprint', "*

 * *                 "'GetPipelineChangeProgress', 'Ingest', 'ListPipelineBlueprint […]*

```diff
@@ -3758,33 +3758,37 @@
                 "DeleteNotificationChannel",
                 "DeletePolicy",
                 "DeleteProtocolsList",
                 "DeleteResourceSet",
                 "DisassociateAdminAccount",
                 "DisassociateThirdPartyFirewall",
                 "GetAdminAccount",
+                "GetAdminScope",
                 "GetAppsList",
                 "GetComplianceDetail",
                 "GetNotificationChannel",
                 "GetPolicy",
                 "GetProtectionStatus",
                 "GetProtocolsList",
                 "GetResourceSet",
                 "GetThirdPartyFirewallAssociationStatus",
                 "GetViolationDetails",
+                "ListAdminAccountsForOrganization",
+                "ListAdminsManagingAccount",
                 "ListAppsLists",
                 "ListComplianceStatus",
                 "ListDiscoveredResources",
                 "ListMemberAccounts",
                 "ListPolicies",
                 "ListProtocolsLists",
                 "ListResourceSetResources",
                 "ListResourceSets",
                 "ListTagsForResource",
                 "ListThirdPartyFirewallFirewallPolicies",
+                "PutAdminAccount",
                 "PutAppsList",
                 "PutNotificationChannel",
                 "PutPolicy",
                 "PutProtocolsList",
                 "PutResourceSet",
                 "TagResource",
                 "UntagResource"
@@ -15909,14 +15913,42 @@
                 "aws:TagKeys",
                 "omics:AnnotationImportJobJobId",
                 "omics:AnnotationStoreName",
                 "omics:VariantImportJobJobId",
                 "omics:VariantStoreName"
             ]
         },
+        "Amazon OpenSearch Ingestion": {
+            "ARNFormat": "arn:aws:osis:${Region}:${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:aws:osis:.+:.+:.+",
+            "Actions": [
+                "CreatePipeline",
+                "DeletePipeline",
+                "GetPipeline",
+                "GetPipelineBlueprint",
+                "GetPipelineChangeProgress",
+                "Ingest",
+                "ListPipelineBlueprints",
+                "ListPipelines",
+                "ListTagsForResource",
+                "StartPipeline",
+                "StopPipeline",
+                "TagResource",
+                "UntagResource",
+                "UpdatePipeline",
+                "ValidatePipeline"
+            ],
+            "HasResource": true,
+            "StringPrefix": "osis",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "Amazon OpenSearch Serverless": {
             "ARNFormat": "arn:aws:aoss:${Region}:${Account}:${Resource}",
             "ARNRegex": "^arn:aws:aoss:.+",
             "Actions": [
                 "BatchGetCollection",
                 "BatchGetVpcEndpoint",
                 "CreateAccessPolicy",
```

### Comparing `iam_actions-1.2.20230426/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230427/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971988795518207%*

 * *Differences: {"'osis'": 'OrderedDict()'}*

```diff
@@ -4526,14 +4526,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "root": {
             "arn_pattern": "arn:*:organizations::*:root/o-*/r-*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
+    "osis": {},
     "outposts": {
         "outpost": {
             "arn_pattern": "arn:*:outposts:*:*:outpost:*",
             "condition_keys": null
         },
         "site": {
             "arn_pattern": "arn:*:outposts:*:*:site/*",
```

### Comparing `iam_actions-1.2.20230426/iam_actions/services.json` & `iam_actions-1.2.20230427/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971877639944867%*

 * *Differences: {"'fms'": "{'Actions': {insert: [(12, 'GetAdminScope'), (22, 'ListAdminAccountsForOrganization'), "*

 * *          "(23, 'ListAdminsManagingAccount'), (34, 'PutAdminAccount')]}}",*

 * * "'osis'": "OrderedDict([('Actions', ['CreatePipeline', 'DeletePipeline', 'GetPipeline', "*

 * *           "'GetPipelineBlueprint', 'GetPipelineChangeProgress', 'Ingest', "*

 * *           "'ListPipelineBlueprints', 'ListPipelines', 'ListTagsForResource', 'StartPipeline', "*

 * *           "'StopPipeline', 'TagResource', 'UntagResource', 'UpdatePipel […]*

```diff
@@ -8242,33 +8242,37 @@
             "DeleteNotificationChannel",
             "DeletePolicy",
             "DeleteProtocolsList",
             "DeleteResourceSet",
             "DisassociateAdminAccount",
             "DisassociateThirdPartyFirewall",
             "GetAdminAccount",
+            "GetAdminScope",
             "GetAppsList",
             "GetComplianceDetail",
             "GetNotificationChannel",
             "GetPolicy",
             "GetProtectionStatus",
             "GetProtocolsList",
             "GetResourceSet",
             "GetThirdPartyFirewallAssociationStatus",
             "GetViolationDetails",
+            "ListAdminAccountsForOrganization",
+            "ListAdminsManagingAccount",
             "ListAppsLists",
             "ListComplianceStatus",
             "ListDiscoveredResources",
             "ListMemberAccounts",
             "ListPolicies",
             "ListProtocolsLists",
             "ListResourceSetResources",
             "ListResourceSets",
             "ListTagsForResource",
             "ListThirdPartyFirewallFirewallPolicies",
+            "PutAdminAccount",
             "PutAppsList",
             "PutNotificationChannel",
             "PutPolicy",
             "PutProtocolsList",
             "PutResourceSet",
             "TagResource",
             "UntagResource"
@@ -14543,14 +14547,48 @@
             "organizations:ServicePrincipal"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Organizations"
         ]
     },
+    "osis": {
+        "ARNFormats": [
+            "arn:aws:osis:${Region}:${Account}:${ResourceType}/${ResourceName}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:osis:.+:.+:.+"
+        ],
+        "Actions": [
+            "CreatePipeline",
+            "DeletePipeline",
+            "GetPipeline",
+            "GetPipelineBlueprint",
+            "GetPipelineChangeProgress",
+            "Ingest",
+            "ListPipelineBlueprints",
+            "ListPipelines",
+            "ListTagsForResource",
+            "StartPipeline",
+            "StopPipeline",
+            "TagResource",
+            "UntagResource",
+            "UpdatePipeline",
+            "ValidatePipeline"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "Amazon OpenSearch Ingestion"
+        ]
+    },
     "outposts": {
         "ARNFormats": [
             "arn:aws:outposts:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:outposts:.+:.+:.+"
         ],
```

### Comparing `iam_actions-1.2.20230426/pyproject.toml` & `iam_actions-1.2.20230427/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230426"
+version = "1.2.20230427"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230426/setup.py` & `iam_actions-1.2.20230427/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230426',
+    'version': '1.2.20230427',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230426/PKG-INFO` & `iam_actions-1.2.20230427/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230426
+Version: 1.2.20230427
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

