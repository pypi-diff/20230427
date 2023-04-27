# Comparing `tmp/tencentcloud-sdk-python-ssm-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-ssm-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.882.tar", last modified: Wed Apr 26 03:45:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssm-3.0.883.tar", last modified: Thu Apr 27 00:48:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssm-3.0.882.tar` & `tencentcloud-sdk-python-ssm-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/
--rw-r--r--   0 root         (0) root         (0)    24513 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/ssm_client.py
--rw-r--r--   0 root         (0) root         (0)     3474 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62817 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud_sdk_python_ssm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:45:49.000000 tencentcloud-sdk-python-ssm-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/
+-rw-r--r--   0 root         (0) root         (0)    24513 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/ssm_client.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63662 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud_sdk_python_ssm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud_sdk_python_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud_sdk_python_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/tencentcloud_sdk_python_ssm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:48:32.000000 tencentcloud-sdk-python-ssm-3.0.883/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/README.rst` & `tencentcloud-sdk-python-ssm-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/ssm_client.py` & `tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/ssm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/errorcodes.py` & `tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/ssm/v20190923/models.py` & `tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/ssm/v20190923/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1445,14 +1445,23 @@
         :type ProjectID: int
         :param AssociatedInstanceIDs: 当凭据类型为SSH密钥对凭据时，此字段有效，用于表示SSH密钥对所关联的CVM实例ID。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AssociatedInstanceIDs: list of str
         :param TargetUin: 当凭据类型为云API密钥对凭据时，此字段有效，用于表示云API密钥对所属的用户UIN。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TargetUin: int
+        :param RotationFrequency: 轮转的频率，以天作为单位，在轮转开启状态下生效。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RotationFrequency: int
+        :param ResourceID: 云产品凭据对应的云产品实例 ID 号。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceID: str
+        :param RotationBeginTime: 用户指定的轮转开始时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RotationBeginTime: str
         """
         self.SecretName = None
         self.Description = None
         self.KmsKeyId = None
         self.CreateUin = None
         self.Status = None
         self.DeleteTime = None
@@ -1462,14 +1471,17 @@
         self.NextRotationTime = None
         self.SecretType = None
         self.ProductName = None
         self.ResourceName = None
         self.ProjectID = None
         self.AssociatedInstanceIDs = None
         self.TargetUin = None
+        self.RotationFrequency = None
+        self.ResourceID = None
+        self.RotationBeginTime = None
 
 
     def _deserialize(self, params):
         self.SecretName = params.get("SecretName")
         self.Description = params.get("Description")
         self.KmsKeyId = params.get("KmsKeyId")
         self.CreateUin = params.get("CreateUin")
@@ -1481,14 +1493,17 @@
         self.NextRotationTime = params.get("NextRotationTime")
         self.SecretType = params.get("SecretType")
         self.ProductName = params.get("ProductName")
         self.ResourceName = params.get("ResourceName")
         self.ProjectID = params.get("ProjectID")
         self.AssociatedInstanceIDs = params.get("AssociatedInstanceIDs")
         self.TargetUin = params.get("TargetUin")
+        self.RotationFrequency = params.get("RotationFrequency")
+        self.ResourceID = params.get("ResourceID")
+        self.RotationBeginTime = params.get("RotationBeginTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssm-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.883/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssm-3.0.883/tencentcloud_sdk_python_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssm
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Ssm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssm-3.0.882/setup.py` & `tencentcloud-sdk-python-ssm-3.0.883/setup.py`

 * *Files identical despite different names*

