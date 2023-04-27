# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.882.tar", last modified: Wed Apr 26 03:37:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.883.tar", last modified: Thu Apr 27 00:36:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.882.tar` & `tencentcloud-sdk-python-lcic-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4332 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138236 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    47779 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:37:24.000000 tencentcloud-sdk-python-lcic-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139745 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    47779 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-27 00:36:20.000000 tencentcloud-sdk-python-lcic-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:36:21.000000 tencentcloud-sdk-python-lcic-3.0.883/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/README.rst` & `tencentcloud-sdk-python-lcic-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -969,14 +969,16 @@
         :type RTCAudienceNumber: int
         :param AudienceType: 观看类型。0未知，1互动，2cdn或直播。 目前仅支持互动类型
         :type AudienceType: int
         :param RecordLayout: 录制布局。录制模板枚举值参考：https://cloud.tencent.com/document/product/1639/89744
         :type RecordLayout: int
         :param GroupId: 房间绑定的群组ID,非空时限制组成员进入
         :type GroupId: str
+        :param EnableDirectControl: 打开学生麦克风/摄像头的授权开关
+        :type EnableDirectControl: int
         """
         self.Name = None
         self.StartTime = None
         self.EndTime = None
         self.SdkAppId = None
         self.Resolution = None
         self.MaxMicNumber = None
@@ -987,14 +989,15 @@
         self.AudioQuality = None
         self.DisableRecord = None
         self.Assistants = None
         self.RTCAudienceNumber = None
         self.AudienceType = None
         self.RecordLayout = None
         self.GroupId = None
+        self.EnableDirectControl = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.SdkAppId = params.get("SdkAppId")
@@ -1007,14 +1010,15 @@
         self.AudioQuality = params.get("AudioQuality")
         self.DisableRecord = params.get("DisableRecord")
         self.Assistants = params.get("Assistants")
         self.RTCAudienceNumber = params.get("RTCAudienceNumber")
         self.AudienceType = params.get("AudienceType")
         self.RecordLayout = params.get("RecordLayout")
         self.GroupId = params.get("GroupId")
+        self.EnableDirectControl = params.get("EnableDirectControl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2209,14 +2213,16 @@
         :type RecordUrl: str
         :param Status: 课堂状态。0为未开始，1为已开始，2为已结束，3为已过期。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         :param GroupId: 房间绑定的群组ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type GroupId: str
+        :param EnableDirectControl: 打开学生麦克风/摄像头的授权开关
+        :type EnableDirectControl: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Name = None
         self.StartTime = None
         self.EndTime = None
         self.TeacherId = None
@@ -2227,14 +2233,15 @@
         self.AudioQuality = None
         self.SubType = None
         self.DisableRecord = None
         self.Assistants = None
         self.RecordUrl = None
         self.Status = None
         self.GroupId = None
+        self.EnableDirectControl = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
@@ -2246,14 +2253,15 @@
         self.AudioQuality = params.get("AudioQuality")
         self.SubType = params.get("SubType")
         self.DisableRecord = params.get("DisableRecord")
         self.Assistants = params.get("Assistants")
         self.RecordUrl = params.get("RecordUrl")
         self.Status = params.get("Status")
         self.GroupId = params.get("GroupId")
+        self.EnableDirectControl = params.get("EnableDirectControl")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeRoomStatisticsRequest(AbstractModel):
     """DescribeRoomStatistics请求参数结构体
 
     """
@@ -3534,14 +3542,16 @@
 1 禁止录制
 直播开始后不允许修改。
         :type DisableRecord: int
         :param Assistants: 助教Id列表。直播开始后不允许修改。
         :type Assistants: list of str
         :param GroupId: 房间绑定的群组ID
         :type GroupId: str
+        :param EnableDirectControl: 打开学生麦克风/摄像头的授权开关
+        :type EnableDirectControl: int
         """
         self.RoomId = None
         self.SdkAppId = None
         self.StartTime = None
         self.EndTime = None
         self.TeacherId = None
         self.Name = None
@@ -3549,14 +3559,15 @@
         self.MaxMicNumber = None
         self.AutoMic = None
         self.AudioQuality = None
         self.SubType = None
         self.DisableRecord = None
         self.Assistants = None
         self.GroupId = None
+        self.EnableDirectControl = None
 
 
     def _deserialize(self, params):
         self.RoomId = params.get("RoomId")
         self.SdkAppId = params.get("SdkAppId")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
@@ -3566,14 +3577,15 @@
         self.MaxMicNumber = params.get("MaxMicNumber")
         self.AutoMic = params.get("AutoMic")
         self.AudioQuality = params.get("AudioQuality")
         self.SubType = params.get("SubType")
         self.DisableRecord = params.get("DisableRecord")
         self.Assistants = params.get("Assistants")
         self.GroupId = params.get("GroupId")
+        self.EnableDirectControl = params.get("EnableDirectControl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3787,14 +3799,16 @@
         :type RTCAudienceNumber: int
         :param AudienceType: 观看类型。
         :type AudienceType: int
         :param RecordLayout: 录制布局。
         :type RecordLayout: int
         :param GroupId: 房间绑定的群组ID
         :type GroupId: str
+        :param EnableDirectControl: 打开学生麦克风/摄像头的授权开关
+        :type EnableDirectControl: int
         """
         self.Name = None
         self.StartTime = None
         self.EndTime = None
         self.Resolution = None
         self.MaxMicNumber = None
         self.SubType = None
@@ -3804,14 +3818,15 @@
         self.AudioQuality = None
         self.DisableRecord = None
         self.Assistants = None
         self.RTCAudienceNumber = None
         self.AudienceType = None
         self.RecordLayout = None
         self.GroupId = None
+        self.EnableDirectControl = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.Resolution = params.get("Resolution")
@@ -3823,14 +3838,15 @@
         self.AudioQuality = params.get("AudioQuality")
         self.DisableRecord = params.get("DisableRecord")
         self.Assistants = params.get("Assistants")
         self.RTCAudienceNumber = params.get("RTCAudienceNumber")
         self.AudienceType = params.get("AudienceType")
         self.RecordLayout = params.get("RecordLayout")
         self.GroupId = params.get("GroupId")
+        self.EnableDirectControl = params.get("EnableDirectControl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3874,40 +3890,50 @@
         :type MaxRTCMember: int
         :param ReplayUrl: 房间录制地址。已废弃，使用新字段 RecordUrl
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReplayUrl: str
         :param RecordUrl: 录制地址（协议为https)。仅在房间结束后存在。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecordUrl: str
+        :param MaxMicNumber: 最高房间内人数（包括老师），0表示不限制，默认为0
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MaxMicNumber: int
+        :param EnableDirectControl: 打开学生麦克风/摄像头的授权开关 
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnableDirectControl: int
         """
         self.Name = None
         self.RoomId = None
         self.Status = None
         self.StartTime = None
         self.EndTime = None
         self.RealStartTime = None
         self.RealEndTime = None
         self.Resolution = None
         self.MaxRTCMember = None
         self.ReplayUrl = None
         self.RecordUrl = None
+        self.MaxMicNumber = None
+        self.EnableDirectControl = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.RoomId = params.get("RoomId")
         self.Status = params.get("Status")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.RealStartTime = params.get("RealStartTime")
         self.RealEndTime = params.get("RealEndTime")
         self.Resolution = params.get("Resolution")
         self.MaxRTCMember = params.get("MaxRTCMember")
         self.ReplayUrl = params.get("ReplayUrl")
         self.RecordUrl = params.get("RecordUrl")
+        self.MaxMicNumber = params.get("MaxMicNumber")
+        self.EnableDirectControl = params.get("EnableDirectControl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.883/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.883/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.882/setup.py` & `tencentcloud-sdk-python-lcic-3.0.883/setup.py`

 * *Files identical despite different names*

