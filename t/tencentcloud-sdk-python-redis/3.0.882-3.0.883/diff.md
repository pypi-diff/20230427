# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.882.tar", last modified: Wed Apr 26 03:43:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.883.tar", last modified: Thu Apr 27 00:46:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.882.tar` & `tencentcloud-sdk-python-redis-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86631 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   291086 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 03:43:54.000000 tencentcloud-sdk-python-redis-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:43:55.000000 tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86664 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   291508 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-27 00:46:16.000000 tencentcloud-sdk-python-redis-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:46:17.000000 tencentcloud-sdk-python-redis-3.0.883/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.882/README.rst` & `tencentcloud-sdk-python-redis-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1495,15 +1495,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def KillMasterGroup(self, request):
-        """模拟故障
+        """本接口（KillMasterGroup）模拟故障。
 
         :param request: Request instance for KillMasterGroup.
         :type request: :class:`tencentcloud.redis.v20180412.models.KillMasterGroupRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.KillMasterGroupResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.883/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4662,39 +4662,46 @@
 class InstanceClusterNode(AbstractModel):
     """实例节点类型
 
     """
 
     def __init__(self):
         r"""
-        :param Name: 节点名称
+        :param Name: 节点名称。
         :type Name: str
-        :param RunId: 实例运行时节点Id
+        :param RunId: 实例运行时节点 ID。
         :type RunId: str
-        :param Role: 集群角色：0-master；1-slave
+        :param Role: 集群角色。
+- 0：master。
+- 1：slave。
         :type Role: int
-        :param Status: 节点状态：0-readwrite, 1-read, 2-backup
+        :param Status: 节点状态。
+- 0：readwrite,。
+- 1：read。
+- 2：backup。
         :type Status: int
-        :param Connected: 服务状态：0-down；1-on
+        :param Connected: 服务状态。
+0-down。
+1-on
         :type Connected: int
-        :param CreateTime: 节点创建时间
+        :param CreateTime: 节点创建时间。
         :type CreateTime: str
-        :param DownTime: 节点下线时间
+        :param DownTime: 节点下线时间。
         :type DownTime: str
-        :param Slots: 节点slot分布
+        :param Slots: 节点 Slot 分布区间。
         :type Slots: str
-        :param Keys: 节点key分布
+        :param Keys: 节点 Key分布。
         :type Keys: int
-        :param Qps: 节点qps
+        :param Qps: 节点 QPS。分片节点每秒执行次数。单位：次/秒。
         :type Qps: int
-        :param QpsSlope: 节点qps倾斜度
+        :param QpsSlope: 节点 QPS 倾斜度。
         :type QpsSlope: float
-        :param Storage: 节点存储
+        :param Storage: 节点存储。
         :type Storage: int
-        :param StorageSlope: 节点存储倾斜度
+        :param StorageSlope: 节点存储倾斜度。
         :type StorageSlope: float
         """
         self.Name = None
         self.RunId = None
         self.Role = None
         self.Status = None
         self.Connected = None
@@ -4959,17 +4966,17 @@
 class InstanceNode(AbstractModel):
     """实例节点
 
     """
 
     def __init__(self):
         r"""
-        :param Id: Id
+        :param Id: 实例 ID。
         :type Id: int
-        :param InstanceClusterNode: 节点详细信息
+        :param InstanceClusterNode: 节点详细信息。
         :type InstanceClusterNode: list of InstanceClusterNode
         """
         self.Id = None
         self.InstanceClusterNode = None
 
 
     def _deserialize(self, params):
@@ -5468,17 +5475,17 @@
 class InstanceTagInfo(AbstractModel):
     """实例标签信息
 
     """
 
     def __init__(self):
         r"""
-        :param TagKey: 标签键
+        :param TagKey: 标签键。
         :type TagKey: str
-        :param TagValue: 标签值
+        :param TagValue: 标签值。
         :type TagValue: str
         """
         self.TagKey = None
         self.TagValue = None
 
 
     def _deserialize(self, params):
@@ -5660,25 +5667,22 @@
 class KillMasterGroupRequest(AbstractModel):
     """KillMasterGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param Password: 1.长度8-30位,推荐使用12位以上的密码
-2.不能以"/"开头
-3.至少包含两项
-    a.小写字母a-z
-    b.大写字母A-Z
-    c.数字0-9
-    d.()`~!@#$%^&*-+=_|{}[]:;<>,.?/
+        :param Password: 该参数用于配置指定实例的访问密码。若为免密认证，该参数则无需配置。密码复杂度要求如下所示。
+- 长度8-30位,推荐使用12位以上的密码
+- 不能以"/"开头
+- 至少包含小写字母a-z、大写字母A-Z、数字0-9及其 ()`~!@#$%^&*-+=_|{}[]:;<>,.?/中的两项。
         :type Password: str
-        :param ShardIds: 单AZ实例节点信息
+        :param ShardIds: 分片集群的分片 ID。
         :type ShardIds: list of int
         """
         self.InstanceId = None
         self.Password = None
         self.ShardIds = None
 
 
@@ -5698,15 +5702,15 @@
 class KillMasterGroupResponse(AbstractModel):
     """KillMasterGroup返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TaskId: 异步任务ID
+        :param TaskId: 异步任务ID。
         :type TaskId: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TaskId = None
         self.RequestId = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.883/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.882/setup.py` & `tencentcloud-sdk-python-redis-3.0.883/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.882/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.883/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

