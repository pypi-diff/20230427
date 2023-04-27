# Comparing `tmp/cloudsnorkel.cdk-github-runners-0.9.6.tar.gz` & `tmp/cloudsnorkel.cdk-github-runners-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.6.tar", last modified: Sun Apr 23 18:13:16 2023, max compression
+gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.7.tar", last modified: Thu Apr 27 21:25:04 2023, max compression
```

## Comparing `cloudsnorkel.cdk-github-runners-0.9.6.tar` & `cloudsnorkel.cdk-github-runners-0.9.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.791942 cloudsnorkel.cdk-github-runners-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.791942 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/
--rw-r--r--   0 runner    (1001) docker     (123)   562399 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1997391 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:13:06.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:13:16.795943 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:13:16.000000 cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.204815 cloudsnorkel.cdk-github-runners-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-27 21:25:04.204815 cloudsnorkel.cdk-github-runners-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:25:04.204815 cloudsnorkel.cdk-github-runners-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.196815 cloudsnorkel.cdk-github-runners-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.196815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.200815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)   563192 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.200815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1998045 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:24:44.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:25:04.200815 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 21:25:04.000000 cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.6/LICENSE` & `cloudsnorkel.cdk-github-runners-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.6/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.6
+Version: 0.9.7
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.6/README.md` & `cloudsnorkel.cdk-github-runners-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.6/setup.py` & `cloudsnorkel.cdk-github-runners-0.9.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudsnorkel.cdk-github-runners",
-    "version": "0.9.6",
+    "version": "0.9.7",
     "description": "CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.",
     "license": "Apache-2.0",
     "url": "https://github.com/CloudSnorkel/cdk-github-runners.git",
     "long_description_content_type": "text/markdown",
     "author": "Amir Szekely<amir@cloudsnorkel.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudsnorkel.cdk_github_runners",
         "cloudsnorkel.cdk_github_runners._jsii"
     ],
     "package_data": {
         "cloudsnorkel.cdk_github_runners._jsii": [
-            "cdk-github-runners@0.9.6.jsii.tgz"
+            "cdk-github-runners@0.9.7.jsii.tgz"
         ],
         "cloudsnorkel.cdk_github_runners": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel/cdk_github_runners/__init__.py` & `cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel/cdk_github_runners/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7863,14 +7863,15 @@
         image_builder: typing.Optional[IRunnerImageBuilder] = None,
         instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
         labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         max_instances: typing.Optional[jsii.Number] = None,
         memory_limit_mib: typing.Optional[jsii.Number] = None,
         min_instances: typing.Optional[jsii.Number] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        spot: typing.Optional[builtins.bool] = None,
         spot_max_price: typing.Optional[builtins.str] = None,
         storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
         subnet_selection: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
         log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
         retry_options: typing.Optional[typing.Union[ProviderRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
@@ -7885,15 +7886,16 @@
         :param image_builder: (experimental) Runner image builder used to build Docker images containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: EcsRunnerProvider.imageBuilder()
         :param instance_type: (experimental) Instance type of ECS cluster instances. Only used when creating a new cluster. Default: m5.large or m6g.large
         :param labels: (experimental) GitHub Actions labels used for this provider. These labels are used to identify which provider should spawn a new on-demand runner. Every job sends a webhook with the labels it's looking for based on runs-on. We match the labels from the webhook with the labels specified here. If all the labels specified here are present in the job's labels, this provider will be chosen and spawn a new runner. Default: ['ecs']
         :param max_instances: (experimental) The maximum number of instances to run in the cluster. Only used when creating a new cluster. Default: 5
         :param memory_limit_mib: (experimental) The amount (in MiB) of memory used by the task. Default: 3500
         :param min_instances: (experimental) The minimum number of instances to run in the cluster. Only used when creating a new cluster. Default: 0
         :param security_groups: (experimental) Security groups to assign to the task. Default: a new security group
-        :param spot_max_price: (experimental) Use spot capacity and set a maximum price for spot instances. Default: no spot capacity
+        :param spot: (experimental) Use spot capacity. Default: false (true if spotMaxPrice is specified)
+        :param spot_max_price: (experimental) Maximum price for spot instances.
         :param storage_size: (experimental) Size of volume available for launched cluster instances. This modifies the boot volume size and doesn't add any additional volumes. Each instance can be used by multiple runners, so make sure there is enough space for all of them. Default: default size for AMI (usually 30GB for Linux and 50GB for Windows)
         :param subnet_selection: (experimental) Subnets to run the runners in. Default: ECS default
         :param vpc: (experimental) VPC to launch the runners in. Default: default account VPC
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param retry_options: (experimental) Options to retry operation in case of failure like missing capacity, or API quota issues. Default: retry 10 times up to about 45 minutes
 
         :stability: experimental
@@ -7911,14 +7913,15 @@
             image_builder=image_builder,
             instance_type=instance_type,
             labels=labels,
             max_instances=max_instances,
             memory_limit_mib=memory_limit_mib,
             min_instances=min_instances,
             security_groups=security_groups,
+            spot=spot,
             spot_max_price=spot_max_price,
             storage_size=storage_size,
             subnet_selection=subnet_selection,
             vpc=vpc,
             log_retention=log_retention,
             retry_options=retry_options,
         )
@@ -8162,14 +8165,15 @@
         "image_builder": "imageBuilder",
         "instance_type": "instanceType",
         "labels": "labels",
         "max_instances": "maxInstances",
         "memory_limit_mib": "memoryLimitMiB",
         "min_instances": "minInstances",
         "security_groups": "securityGroups",
+        "spot": "spot",
         "spot_max_price": "spotMaxPrice",
         "storage_size": "storageSize",
         "subnet_selection": "subnetSelection",
         "vpc": "vpc",
     },
 )
 class EcsRunnerProviderProps(RunnerProviderProps):
@@ -8186,14 +8190,15 @@
         image_builder: typing.Optional[IRunnerImageBuilder] = None,
         instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
         labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         max_instances: typing.Optional[jsii.Number] = None,
         memory_limit_mib: typing.Optional[jsii.Number] = None,
         min_instances: typing.Optional[jsii.Number] = None,
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        spot: typing.Optional[builtins.bool] = None,
         spot_max_price: typing.Optional[builtins.str] = None,
         storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
         subnet_selection: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Properties for EcsRunnerProvider.
 
@@ -8207,15 +8212,16 @@
         :param image_builder: (experimental) Runner image builder used to build Docker images containing GitHub Runner and all requirements. The image builder determines the OS and architecture of the runner. Default: EcsRunnerProvider.imageBuilder()
         :param instance_type: (experimental) Instance type of ECS cluster instances. Only used when creating a new cluster. Default: m5.large or m6g.large
         :param labels: (experimental) GitHub Actions labels used for this provider. These labels are used to identify which provider should spawn a new on-demand runner. Every job sends a webhook with the labels it's looking for based on runs-on. We match the labels from the webhook with the labels specified here. If all the labels specified here are present in the job's labels, this provider will be chosen and spawn a new runner. Default: ['ecs']
         :param max_instances: (experimental) The maximum number of instances to run in the cluster. Only used when creating a new cluster. Default: 5
         :param memory_limit_mib: (experimental) The amount (in MiB) of memory used by the task. Default: 3500
         :param min_instances: (experimental) The minimum number of instances to run in the cluster. Only used when creating a new cluster. Default: 0
         :param security_groups: (experimental) Security groups to assign to the task. Default: a new security group
-        :param spot_max_price: (experimental) Use spot capacity and set a maximum price for spot instances. Default: no spot capacity
+        :param spot: (experimental) Use spot capacity. Default: false (true if spotMaxPrice is specified)
+        :param spot_max_price: (experimental) Maximum price for spot instances.
         :param storage_size: (experimental) Size of volume available for launched cluster instances. This modifies the boot volume size and doesn't add any additional volumes. Each instance can be used by multiple runners, so make sure there is enough space for all of them. Default: default size for AMI (usually 30GB for Linux and 50GB for Windows)
         :param subnet_selection: (experimental) Subnets to run the runners in. Default: ECS default
         :param vpc: (experimental) VPC to launch the runners in. Default: default account VPC
 
         :stability: experimental
         '''
         if isinstance(retry_options, dict):
@@ -8234,14 +8240,15 @@
             check_type(argname="argument image_builder", value=image_builder, expected_type=type_hints["image_builder"])
             check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
             check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
             check_type(argname="argument max_instances", value=max_instances, expected_type=type_hints["max_instances"])
             check_type(argname="argument memory_limit_mib", value=memory_limit_mib, expected_type=type_hints["memory_limit_mib"])
             check_type(argname="argument min_instances", value=min_instances, expected_type=type_hints["min_instances"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
+            check_type(argname="argument spot", value=spot, expected_type=type_hints["spot"])
             check_type(argname="argument spot_max_price", value=spot_max_price, expected_type=type_hints["spot_max_price"])
             check_type(argname="argument storage_size", value=storage_size, expected_type=type_hints["storage_size"])
             check_type(argname="argument subnet_selection", value=subnet_selection, expected_type=type_hints["subnet_selection"])
             check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if log_retention is not None:
             self._values["log_retention"] = log_retention
@@ -8267,14 +8274,16 @@
             self._values["max_instances"] = max_instances
         if memory_limit_mib is not None:
             self._values["memory_limit_mib"] = memory_limit_mib
         if min_instances is not None:
             self._values["min_instances"] = min_instances
         if security_groups is not None:
             self._values["security_groups"] = security_groups
+        if spot is not None:
+            self._values["spot"] = spot
         if spot_max_price is not None:
             self._values["spot_max_price"] = spot_max_price
         if storage_size is not None:
             self._values["storage_size"] = storage_size
         if subnet_selection is not None:
             self._values["subnet_selection"] = subnet_selection
         if vpc is not None:
@@ -8460,18 +8469,27 @@
 
         :stability: experimental
         '''
         result = self._values.get("security_groups")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
 
     @builtins.property
-    def spot_max_price(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Use spot capacity and set a maximum price for spot instances.
+    def spot(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Use spot capacity.
 
-        :default: no spot capacity
+        :default: false (true if spotMaxPrice is specified)
+
+        :stability: experimental
+        '''
+        result = self._values.get("spot")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def spot_max_price(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Maximum price for spot instances.
 
         :stability: experimental
         '''
         result = self._values.get("spot_max_price")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
@@ -10960,14 +10978,15 @@
     image_builder: typing.Optional[IRunnerImageBuilder] = None,
     instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
     labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     max_instances: typing.Optional[jsii.Number] = None,
     memory_limit_mib: typing.Optional[jsii.Number] = None,
     min_instances: typing.Optional[jsii.Number] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    spot: typing.Optional[builtins.bool] = None,
     spot_max_price: typing.Optional[builtins.str] = None,
     storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
     subnet_selection: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
     vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
     retry_options: typing.Optional[typing.Union[ProviderRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
@@ -11036,14 +11055,15 @@
     image_builder: typing.Optional[IRunnerImageBuilder] = None,
     instance_type: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.InstanceType] = None,
     labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     max_instances: typing.Optional[jsii.Number] = None,
     memory_limit_mib: typing.Optional[jsii.Number] = None,
     min_instances: typing.Optional[jsii.Number] = None,
     security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    spot: typing.Optional[builtins.bool] = None,
     spot_max_price: typing.Optional[builtins.str] = None,
     storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
     subnet_selection: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
     vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.6
+Version: 0.9.7
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.6/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt` & `cloudsnorkel.cdk-github-runners-0.9.7/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
 src/cloudsnorkel/cdk_github_runners/__init__.py
 src/cloudsnorkel/cdk_github_runners/py.typed
 src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
-src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.6.jsii.tgz
+src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.7.jsii.tgz
```

