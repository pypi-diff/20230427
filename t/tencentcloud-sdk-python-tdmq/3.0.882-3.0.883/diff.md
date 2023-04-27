# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.882.tar", last modified: Wed Apr 26 03:50:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.883.tar", last modified: Thu Apr 27 00:53:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.882.tar` & `tencentcloud-sdk-python-tdmq-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   101085 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   375961 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:50:59.000000 tencentcloud-sdk-python-tdmq-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   101085 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   375759 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:53:55.000000 tencentcloud-sdk-python-tdmq-3.0.883/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2317,17 +2317,17 @@
 
     def __init__(self):
         r"""
         :param ClusterId: 集群ID
         :type ClusterId: str
         :param NamespaceId: 命名空间名称，3-64个字符，只能包含字母、数字、“-”及“_”
         :type NamespaceId: str
-        :param Ttl: 未消费消息的保留时间，以毫秒为单位，60秒-15天
+        :param Ttl: 已废弃
         :type Ttl: int
-        :param RetentionTime: 消息持久化后保留的时间，以毫秒为单位
+        :param RetentionTime: 已废弃
         :type RetentionTime: int
         :param Remark: 说明，最大128个字符
         :type Remark: str
         """
         self.ClusterId = None
         self.NamespaceId = None
         self.Ttl = None
@@ -7560,17 +7560,17 @@
 
     def __init__(self):
         r"""
         :param ClusterId: 集群ID
         :type ClusterId: str
         :param NamespaceId: 命名空间名称，3-64个字符，只能包含字母、数字、“-”及“_”
         :type NamespaceId: str
-        :param Ttl: 未消费消息的保留时间，以毫秒为单位，60秒-15天
+        :param Ttl: 已废弃
         :type Ttl: int
-        :param RetentionTime: 消息持久化后保留的时间，以毫秒为单位
+        :param RetentionTime: 已废弃
         :type RetentionTime: int
         :param Remark: 说明，最大128个字符
         :type Remark: str
         """
         self.ClusterId = None
         self.NamespaceId = None
         self.Ttl = None
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.883/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.883/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.882/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.883/setup.py`

 * *Files identical despite different names*

