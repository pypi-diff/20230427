# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.882.tar", last modified: Wed Apr 26 03:37:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.883.tar", last modified: Thu Apr 27 00:36:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.882.tar` & `tencentcloud-sdk-python-lighthouse-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      758 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    23370 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    88751 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230902 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:37:30.000000 tencentcloud-sdk-python-lighthouse-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    24692 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    88751 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230902 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:36:27.000000 tencentcloud-sdk-python-lighthouse-3.0.883/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.882'
+__version__ = '3.0.883'
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # CAM签名/鉴权错误。
 AUTHFAILURE = 'AuthFailure'
 
+# 该地域尚未开放，请选择其他地域。
+AUTHFAILURE_INVALIDREGION = 'AuthFailure.InvalidRegion'
+
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
 # 创建镜像失败。
 FAILEDOPERATION_CREATEBLUEPRINTFAILED = 'FailedOperation.CreateBlueprintFailed'
 
 # 创建实例失败。
@@ -43,26 +46,32 @@
 
 # 查询实例退还错误。
 FAILEDOPERATION_DESCRIBEINSTANCESRETURNABLEERROR = 'FailedOperation.DescribeInstancesReturnableError'
 
 # 查询流量包失败。
 FAILEDOPERATION_DESCRIBEINSTANCESTRAFFICPACKAGESFAILED = 'FailedOperation.DescribeInstancesTrafficPackagesFailed'
 
+# 查询资源返回了不符合要求内容。
+FAILEDOPERATION_DESCRIBERESOURCESRETURNABLEERROR = 'FailedOperation.DescribeResourcesReturnableError'
+
 # 销毁资源失败，请稍后重新操作。
 FAILEDOPERATION_DESTROYRESOURCESFAILED = 'FailedOperation.DestroyResourcesFailed'
 
 # 对防火墙规则的操作失败。
 FAILEDOPERATION_FIREWALLRULESOPERATIONFAILED = 'FailedOperation.FirewallRulesOperationFailed'
 
 # 对密钥对的导入操作失败。
 FAILEDOPERATION_IMPORTKEYPAIRFAILED = 'FailedOperation.ImportKeyPairFailed'
 
 # 对实例的操作失败。
 FAILEDOPERATION_INSTANCEOPERATIONFAILED = 'FailedOperation.InstanceOperationFailed'
 
+# 命令无法找到。
+FAILEDOPERATION_INVALIDCOMMANDNOTFOUND = 'FailedOperation.InvalidCommandNotFound'
+
 # 退还资源失败。
 FAILEDOPERATION_ISOLATERESOURCESFAILED = 'FailedOperation.IsolateResourcesFailed'
 
 # 变更实例套餐失败。
 FAILEDOPERATION_MODIFYINSTANCESBUNDLEFAILED = 'FailedOperation.ModifyInstancesBundleFailed'
 
 # 变更资源属性失败，请稍后重新操作。
@@ -73,14 +82,17 @@
 
 # 请求错误。
 FAILEDOPERATION_REQUESTERROR = 'FailedOperation.RequestError'
 
 # 快照操作失败。
 FAILEDOPERATION_SNAPSHOTOPERATIONFAILED = 'FailedOperation.SnapshotOperationFailed'
 
+# 调用计费网关服务失败，请稍后重新操作操作。
+FAILEDOPERATION_TRADECALLBILLINGGATEWAYFAILED = 'FailedOperation.TradeCallBillingGatewayFailed'
+
 # 计费询价失败。
 FAILEDOPERATION_TRADEGETPRICEFAILED = 'FailedOperation.TradeGetPriceFailed'
 
 # 操作失败，不能创建自定义镜像。
 FAILEDOPERATION_UNABLETOCREATEBLUEPRINT = 'FailedOperation.UnableToCreateBlueprint'
 
 # 无法创建实例。
@@ -136,14 +148,17 @@
 
 # 套餐和镜像不匹配。
 INVALIDPARAMETER_BUNDLEANDBLUEPRINTNOTMATCH = 'InvalidParameter.BundleAndBlueprintNotMatch'
 
 # 产品未定义的套餐 ID。
 INVALIDPARAMETER_BUNDLEIDNOTFOUND = 'InvalidParameter.BundleIdNotFound'
 
+# 参数冲突。
+INVALIDPARAMETER_CONFLICT = 'InvalidParameter.Conflict'
+
 # 参数非法，Filter 参数中的 Values 取值数量超过允许的最大数量。
 INVALIDPARAMETER_FILTERVALUELIMITEXCEEDED = 'InvalidParameter.FilterValueLimitExceeded'
 
 # 参数非法，防火墙规则重复。
 INVALIDPARAMETER_FIREWALLRULESDUPLICATED = 'InvalidParameter.FirewallRulesDuplicated'
 
 # 参数非法，防火墙规则已存在。
@@ -163,14 +178,17 @@
 
 # 参数非法，Filter 参数不是字典。
 INVALIDPARAMETER_INVALIDFILTERNOTDICT = 'InvalidParameter.InvalidFilterNotDict'
 
 # 参数非法，Filter 参数中有不支持的 Name。
 INVALIDPARAMETER_INVALIDFILTERNOTSUPPORTEDNAME = 'InvalidParameter.InvalidFilterNotSupportedName'
 
+# 必须要指定一个要修改的属性。
+INVALIDPARAMETER_MUSTSPECIFYONEATTRIBUTETOMODIFY = 'InvalidParameter.MustSpecifyOneAttributeToModify'
+
 # 参数非法，每次只能修改一个属性。
 INVALIDPARAMETER_ONLYALLOWMODIFYONEATTRIBUTE = 'InvalidParameter.OnlyAllowModifyOneAttribute'
 
 # 参数非法，参数冲突。
 INVALIDPARAMETER_PARAMETERCONFLICT = 'InvalidParameter.ParameterConflict'
 
 # 参数取值错误。
@@ -187,17 +205,23 @@
 
 # 套餐和镜像不匹配。
 INVALIDPARAMETERVALUE_BUNDLEANDBLUEPRINTNOTMATCH = 'InvalidParameterValue.BundleAndBlueprintNotMatch'
 
 # 云联网实例ID格式非法。
 INVALIDPARAMETERVALUE_CCNIDMALFORMED = 'InvalidParameterValue.CcnIdMalformed'
 
+# 客户令牌长度超出限制。
+INVALIDPARAMETERVALUE_CLIENTTOKENTOOLONG = 'InvalidParameterValue.ClientTokenTooLong'
+
 # 参数值非法，云硬盘备份点 ID 格式非法。
 INVALIDPARAMETERVALUE_DISKBACKUPIDMALFORMED = 'InvalidParameterValue.DiskBackupIdMalformed'
 
+# 指定的云盘备份点名称不可大于最大长度。
+INVALIDPARAMETERVALUE_DISKBACKUPNAMETOOLONG = 'InvalidParameterValue.DiskBackupNameTooLong'
+
 # 磁盘名称长度超出限制。
 INVALIDPARAMETERVALUE_DISKNAMETOOLONG = 'InvalidParameterValue.DiskNameTooLong'
 
 # 磁盘大小发生改变。
 INVALIDPARAMETERVALUE_DISKSIZENOTMATCH = 'InvalidParameterValue.DiskSizeNotMatch'
 
 # 参数 `KeyName` 已经存在且重复。
@@ -313,14 +337,17 @@
 
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
 # 实例挂载数据盘配额不足，无法挂载磁盘。
 LIMITEXCEEDED_ATTACHDATADISKQUOTALIMITEXCEEDED = 'LimitExceeded.AttachDataDiskQuotaLimitExceeded'
 
+# 配额不足，当前自定义镜像配额不允许创建新的自定义镜像。
+LIMITEXCEEDED_BLUEPRINTQUOTALIMITEXCEEDED = 'LimitExceeded.BlueprintQuotaLimitExceeded'
+
 # 超过磁盘备份点配额限制。
 LIMITEXCEEDED_DISKBACKUPQUOTALIMITEXCEEDED = 'LimitExceeded.DiskBackupQuotaLimitExceeded'
 
 # 超过防火墙规则配额。
 LIMITEXCEEDED_FIREWALLRULESLIMITEXCEEDED = 'LimitExceeded.FirewallRulesLimitExceeded'
 
 # 超过实例配额。
@@ -361,14 +388,17 @@
 
 # 禁止对实例进行操作，实例在创建中，不允许进行该操作。
 OPERATIONDENIED_INSTANCECREATING = 'OperationDenied.InstanceCreating'
 
 # 禁止对实例进行操作，实例最近一次的操作尚在进行中。
 OPERATIONDENIED_INSTANCEOPERATIONINPROGRESS = 'OperationDenied.InstanceOperationInProgress'
 
+# 禁止创建快照。
+OPERATIONDENIED_OPERATIONDENIEDCREATESNAPSHOT = 'OperationDenied.OperationDeniedCreateSnapshot'
+
 # 使用存储型套餐的实例不支持创建快照。
 OPERATIONDENIED_OPERATIONDENIEDCREATESNAPSHOTFORSTORAGEBUNDLE = 'OperationDenied.OperationDeniedCreateSnapshotForStorageBundle'
 
 # 磁盘备份点正在使用中，不支持此操作。
 RESOURCEINUSE_DISKBACKUPINUSE = 'ResourceInUse.DiskBackupInUse'
 
 # 密钥对正在使用中。
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud/lighthouse/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.883/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.883/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.882/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.883/setup.py`

 * *Files identical despite different names*

