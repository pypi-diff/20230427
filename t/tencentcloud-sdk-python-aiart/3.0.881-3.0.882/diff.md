# Comparing `tmp/tencentcloud-sdk-python-aiart-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-aiart-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.881.tar", last modified: Tue Apr 25 00:18:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.882.tar", last modified: Wed Apr 26 02:49:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-aiart-3.0.881.tar` & `tencentcloud-sdk-python-aiart-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/
--rw-r--r--   0 root         (0) root         (0)     3578 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3668 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/aiart_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11656 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud_sdk_python_aiart.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:18:50.000000 tencentcloud-sdk-python-aiart-3.0.881/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/
+-rw-r--r--   0 root         (0) root         (0)     3578 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/aiart_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11632 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud_sdk_python_aiart.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 02:49:36.000000 tencentcloud-sdk-python-aiart-3.0.882/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/README.rst` & `tencentcloud-sdk-python-aiart-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/errorcodes.py` & `tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/aiart_client.py` & `tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/aiart_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/tencentcloud/aiart/v20221229/models.py` & `tencentcloud-sdk-python-aiart-3.0.882/tencentcloud/aiart/v20221229/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     """返回结果配置
 
     """
 
     def __init__(self):
         r"""
         :param Resolution: 生成图分辨率
-支持生成以下不同分辨率的图片，对应1:1方图、3:4竖图、4:3横图三种尺寸规格，不传默认为"768:768"
+支持生成以下不同分辨率的图片，对应1:1方图、3:4竖图、4:3横图三种尺寸规格。
 取值：
 ● 768:768
 ● 768:1024
 ● 1024:768
         :type Resolution: str
         """
         self.Resolution = None
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.882/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/setup.py` & `tencentcloud-sdk-python-aiart-3.0.882/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.881/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.882/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

