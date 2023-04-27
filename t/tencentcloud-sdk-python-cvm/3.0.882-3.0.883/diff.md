# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.882.tar", last modified: Wed Apr 26 03:09:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.883.tar", last modified: Thu Apr 27 00:26:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.882.tar` & `tencentcloud-sdk-python-cvm-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119282 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    42810 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   429673 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:09:19.000000 tencentcloud-sdk-python-cvm-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:09:20.000000 tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119282 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    42810 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   429673 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:26:32.000000 tencentcloud-sdk-python-cvm-3.0.883/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/README.rst` & `tencentcloud-sdk-python-cvm-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/cvm/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1659,15 +1659,15 @@
     """DescribeAccountQuota返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param AppId: 用户appid
-        :type AppId: str
+        :type AppId: int
         :param AccountQuotaOverview: 配额数据
         :type AccountQuotaOverview: :class:`tencentcloud.cvm.v20170312.models.AccountQuotaOverview`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.AppId = None
         self.AccountQuotaOverview = None
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.883/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/setup.py` & `tencentcloud-sdk-python-cvm-3.0.883/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.882/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.883/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

