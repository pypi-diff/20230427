# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.882.tar", last modified: Wed Apr 26 03:08:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.883.tar", last modified: Thu Apr 27 00:25:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.882.tar` & `tencentcloud-sdk-python-cls-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248744 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67922 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:08:25.000000 tencentcloud-sdk-python-cls-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   251498 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67922 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:25:32.000000 tencentcloud-sdk-python-cls-3.0.883/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.882/README.rst` & `tencentcloud-sdk-python-cls-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1977,22 +1977,25 @@
         :type AutoUpdate: bool
         :param UpdateStartTime: 升级开始时间，建议业务低峰期升级LogListener
         :type UpdateStartTime: str
         :param UpdateEndTime: 升级结束时间，建议业务低峰期升级LogListener
         :type UpdateEndTime: str
         :param ServiceLogging: 是否开启服务日志，用于记录因Loglistener 服务自身产生的log，开启后，会创建内部日志集cls_service_logging和日志主题loglistener_status,loglistener_alarm,loglistener_business，不产生计费
         :type ServiceLogging: bool
+        :param MetaTags: 机器组元数据信息列表
+        :type MetaTags: list of MetaTagInfo
         """
         self.GroupName = None
         self.MachineGroupType = None
         self.Tags = None
         self.AutoUpdate = None
         self.UpdateStartTime = None
         self.UpdateEndTime = None
         self.ServiceLogging = None
+        self.MetaTags = None
 
 
     def _deserialize(self, params):
         self.GroupName = params.get("GroupName")
         if params.get("MachineGroupType") is not None:
             self.MachineGroupType = MachineGroupTypeInfo()
             self.MachineGroupType._deserialize(params.get("MachineGroupType"))
@@ -2002,14 +2005,20 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.AutoUpdate = params.get("AutoUpdate")
         self.UpdateStartTime = params.get("UpdateStartTime")
         self.UpdateEndTime = params.get("UpdateEndTime")
         self.ServiceLogging = params.get("ServiceLogging")
+        if params.get("MetaTags") is not None:
+            self.MetaTags = []
+            for item in params.get("MetaTags"):
+                obj = MetaTagInfo()
+                obj._deserialize(item)
+                self.MetaTags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4398,14 +4407,21 @@
         :type Address: str
         :param ParseProtocol: rfc3164：指定系统日志采集使用RFC3164协议解析日志。
 rfc5424：指定系统日志采集使用RFC5424协议解析日志。
 auto：自动匹配rfc3164或者rfc5424其中一种协议
 该字段适用于：创建采集规则配置、修改采集规则配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type ParseProtocol: str
+        :param MetadataType: 元数据类型，0: 不使用元数据信息，1:使用机器组元数据，2:使用用户自定义元数据，3:使用采集配置路径，
+        :type MetadataType: int
+        :param PathRegex: 采集配置路径正则表达式，MetadataType为1时必填
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PathRegex: str
+        :param MetaTags: 用户自定义元数据信息，MetadataType为2时必填
+        :type MetaTags: list of MetaTagInfo
         """
         self.TimeKey = None
         self.TimeFormat = None
         self.Delimiter = None
         self.LogRegex = None
         self.BeginRegex = None
         self.Keys = None
@@ -4414,14 +4430,17 @@
         self.UnMatchLogKey = None
         self.Backtracking = None
         self.IsGBK = None
         self.JsonStandard = None
         self.Protocol = None
         self.Address = None
         self.ParseProtocol = None
+        self.MetadataType = None
+        self.PathRegex = None
+        self.MetaTags = None
 
 
     def _deserialize(self, params):
         self.TimeKey = params.get("TimeKey")
         self.TimeFormat = params.get("TimeFormat")
         self.Delimiter = params.get("Delimiter")
         self.LogRegex = params.get("LogRegex")
@@ -4437,14 +4456,22 @@
         self.UnMatchLogKey = params.get("UnMatchLogKey")
         self.Backtracking = params.get("Backtracking")
         self.IsGBK = params.get("IsGBK")
         self.JsonStandard = params.get("JsonStandard")
         self.Protocol = params.get("Protocol")
         self.Address = params.get("Address")
         self.ParseProtocol = params.get("ParseProtocol")
+        self.MetadataType = params.get("MetadataType")
+        self.PathRegex = params.get("PathRegex")
+        if params.get("MetaTags") is not None:
+            self.MetaTags = []
+            for item in params.get("MetaTags"):
+                obj = MetaTagInfo()
+                obj._deserialize(item)
+                self.MetaTags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5109,24 +5136,27 @@
         :type UpdateStartTime: str
         :param UpdateEndTime: 升级结束时间，建议业务低峰期升级LogListener
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateEndTime: str
         :param ServiceLogging: 是否开启服务日志，用于记录因Loglistener 服务自身产生的log，开启后，会创建内部日志集cls_service_logging和日志主题loglistener_status,loglistener_alarm,loglistener_business，不产生计费
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServiceLogging: bool
+        :param MetaTags: 机器组元数据信息列表
+        :type MetaTags: list of MetaTagInfo
         """
         self.GroupId = None
         self.GroupName = None
         self.MachineGroupType = None
         self.CreateTime = None
         self.Tags = None
         self.AutoUpdate = None
         self.UpdateStartTime = None
         self.UpdateEndTime = None
         self.ServiceLogging = None
+        self.MetaTags = None
 
 
     def _deserialize(self, params):
         self.GroupId = params.get("GroupId")
         self.GroupName = params.get("GroupName")
         if params.get("MachineGroupType") is not None:
             self.MachineGroupType = MachineGroupTypeInfo()
@@ -5138,14 +5168,20 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.AutoUpdate = params.get("AutoUpdate")
         self.UpdateStartTime = params.get("UpdateStartTime")
         self.UpdateEndTime = params.get("UpdateEndTime")
         self.ServiceLogging = params.get("ServiceLogging")
+        if params.get("MetaTags") is not None:
+            self.MetaTags = []
+            for item in params.get("MetaTags"):
+                obj = MetaTagInfo()
+                obj._deserialize(item)
+                self.MetaTags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5281,14 +5317,42 @@
             for item in params.get("Partitions"):
                 obj = PartitionInfo()
                 obj._deserialize(item)
                 self.Partitions.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class MetaTagInfo(AbstractModel):
+    """元数据信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Key: 元数据key
+        :type Key: str
+        :param Value: 元数据value
+        :type Value: str
+        """
+        self.Key = None
+        self.Value = None
+
+
+    def _deserialize(self, params):
+        self.Key = params.get("Key")
+        self.Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ModifyAlarmNoticeRequest(AbstractModel):
     """ModifyAlarmNotice请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5903,23 +5967,26 @@
         :type AutoUpdate: bool
         :param UpdateStartTime: 升级开始时间，建议业务低峰期升级LogListener
         :type UpdateStartTime: str
         :param UpdateEndTime: 升级结束时间，建议业务低峰期升级LogListener
         :type UpdateEndTime: str
         :param ServiceLogging: 是否开启服务日志，用于记录因Loglistener 服务自身产生的log，开启后，会创建内部日志集cls_service_logging和日志主题loglistener_status,loglistener_alarm,loglistener_business，不产生计费
         :type ServiceLogging: bool
+        :param MetaTags: 机器组元数据信息列表
+        :type MetaTags: list of MetaTagInfo
         """
         self.GroupId = None
         self.GroupName = None
         self.MachineGroupType = None
         self.Tags = None
         self.AutoUpdate = None
         self.UpdateStartTime = None
         self.UpdateEndTime = None
         self.ServiceLogging = None
+        self.MetaTags = None
 
 
     def _deserialize(self, params):
         self.GroupId = params.get("GroupId")
         self.GroupName = params.get("GroupName")
         if params.get("MachineGroupType") is not None:
             self.MachineGroupType = MachineGroupTypeInfo()
@@ -5930,14 +5997,20 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.AutoUpdate = params.get("AutoUpdate")
         self.UpdateStartTime = params.get("UpdateStartTime")
         self.UpdateEndTime = params.get("UpdateEndTime")
         self.ServiceLogging = params.get("ServiceLogging")
+        if params.get("MetaTags") is not None:
+            self.MetaTags = []
+            for item in params.get("MetaTags"):
+                obj = MetaTagInfo()
+                obj._deserialize(item)
+                self.MetaTags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.882/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.883/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.882/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.883/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.883/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.882/setup.py` & `tencentcloud-sdk-python-cls-3.0.883/setup.py`

 * *Files identical despite different names*

