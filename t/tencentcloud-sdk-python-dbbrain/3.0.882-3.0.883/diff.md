# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.882.tar", last modified: Wed Apr 26 03:17:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.883.tar", last modified: Thu Apr 27 00:27:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.882.tar` & `tencentcloud-sdk-python-dbbrain-3.0.883.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    48612 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   182383 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111297 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:17:32.000000 tencentcloud-sdk-python-dbbrain-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    48612 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   182325 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111297 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-27 00:27:24.000000 tencentcloud-sdk-python-dbbrain-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:27:25.000000 tencentcloud-sdk-python-dbbrain-3.0.883/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -890,16 +890,15 @@
 
     def __init__(self):
         r"""
         :param AsyncRequestIds: 需要删除的任务id列表
         :type AsyncRequestIds: list of int
         :param InstanceId: 实例ID
         :type InstanceId: str
-        :param Product: 服务产品类型，支持值包括： "mysql" - 云数据库 MySQL， "cynosdb" - 云数据库 CynosDB for MySQL， "mongodb" - 云数据库 CynosDB for MySQL，
-默认值为"mysql"。
+        :param Product: 服务产品类型，支持值："mysql" - 云数据库 MySQL；"cynosdb" - 云数据库 TDSQL-C for MySQL，默认为"mysql"。
         :type Product: str
         """
         self.AsyncRequestIds = None
         self.InstanceId = None
         self.Product = None
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.883/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.883/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.882/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.883/setup.py`

 * *Files identical despite different names*

