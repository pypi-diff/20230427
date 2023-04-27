# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.881.tar", last modified: Tue Apr 25 00:58:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.882.tar", last modified: Wed Apr 26 03:57:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.881.tar` & `tencentcloud-sdk-python-tke-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   180345 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19455 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   649069 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   180345 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   649612 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:57:49.000000 tencentcloud-sdk-python-tke-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.881/README.rst` & `tencentcloud-sdk-python-tke-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.882/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3917,14 +3917,16 @@
         :type AutoUpgradeClusterLevel: bool
         :param ChargeType: 集群计费方式
         :type ChargeType: str
         :param EdgeVersion: 边缘集群版本，此版本区别于k8s版本，是整个集群各组件版本集合
         :type EdgeVersion: str
         :param RegistryPrefix: 边缘组件镜像仓库前缀
         :type RegistryPrefix: str
+        :param TagSpecification: 集群绑定的云标签
+        :type TagSpecification: :class:`tencentcloud.tke.v20180525.models.TagSpecification`
         """
         self.K8SVersion = None
         self.VpcId = None
         self.ClusterName = None
         self.PodCIDR = None
         self.ServiceCIDR = None
         self.ClusterDesc = None
@@ -3932,14 +3934,15 @@
         self.MaxNodePodNum = None
         self.PublicLB = None
         self.ClusterLevel = None
         self.AutoUpgradeClusterLevel = None
         self.ChargeType = None
         self.EdgeVersion = None
         self.RegistryPrefix = None
+        self.TagSpecification = None
 
 
     def _deserialize(self, params):
         self.K8SVersion = params.get("K8SVersion")
         self.VpcId = params.get("VpcId")
         self.ClusterName = params.get("ClusterName")
         self.PodCIDR = params.get("PodCIDR")
@@ -3953,14 +3956,17 @@
             self.PublicLB = EdgeClusterPublicLB()
             self.PublicLB._deserialize(params.get("PublicLB"))
         self.ClusterLevel = params.get("ClusterLevel")
         self.AutoUpgradeClusterLevel = params.get("AutoUpgradeClusterLevel")
         self.ChargeType = params.get("ChargeType")
         self.EdgeVersion = params.get("EdgeVersion")
         self.RegistryPrefix = params.get("RegistryPrefix")
+        if params.get("TagSpecification") is not None:
+            self.TagSpecification = TagSpecification()
+            self.TagSpecification._deserialize(params.get("TagSpecification"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9767,25 +9773,28 @@
         :type CoreDns: str
         :param HealthRegion: 集群的健康检查多地域部署信息
         :type HealthRegion: str
         :param Health: 集群的健康检查部署信息
         :type Health: str
         :param GridDaemon: 是否部署GridDaemon以支持headless service
         :type GridDaemon: str
+        :param UnitCluster: 公网访问kins集群
+        :type UnitCluster: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Addresses = None
         self.Credential = None
         self.PublicLB = None
         self.InternalLB = None
         self.CoreDns = None
         self.HealthRegion = None
         self.Health = None
         self.GridDaemon = None
+        self.UnitCluster = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Addresses") is not None:
             self.Addresses = []
             for item in params.get("Addresses"):
@@ -9801,14 +9810,15 @@
         if params.get("InternalLB") is not None:
             self.InternalLB = EdgeClusterInternalLB()
             self.InternalLB._deserialize(params.get("InternalLB"))
         self.CoreDns = params.get("CoreDns")
         self.HealthRegion = params.get("HealthRegion")
         self.Health = params.get("Health")
         self.GridDaemon = params.get("GridDaemon")
+        self.UnitCluster = params.get("UnitCluster")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeTKEEdgeClusterStatusRequest(AbstractModel):
     """DescribeTKEEdgeClusterStatus请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.882/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.881'
+__version__ = '3.0.882'
```

### Comparing `tencentcloud-sdk-python-tke-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.882/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.882/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.881/setup.py` & `tencentcloud-sdk-python-tke-3.0.882/setup.py`

 * *Files identical despite different names*

