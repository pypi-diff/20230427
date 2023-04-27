# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.881.tar", last modified: Tue Apr 25 00:59:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.882.tar", last modified: Wed Apr 26 03:58:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.881.tar` & `tencentcloud-sdk-python-trtc-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198942 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58535 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:59:54.000000 tencentcloud-sdk-python-trtc-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198959 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58535 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:58:47.000000 tencentcloud-sdk-python-trtc-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/README.rst` & `tencentcloud-sdk-python-trtc-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3189,15 +3189,15 @@
 class OutputParams(AbstractModel):
     """MCU混流的输出参数
 
     """
 
     def __init__(self):
         r"""
-        :param StreamId: 直播流 ID，由用户自定义设置，该流 ID 不能与用户旁路的流 ID 相同。
+        :param StreamId: 直播流 ID，由用户自定义设置，该流 ID 不能与用户旁路的流 ID 相同，限制64字节。
         :type StreamId: str
         :param PureAudioStream: 取值范围[0,1]， 填0：直播流为音视频(默认); 填1：直播流为纯音频
         :type PureAudioStream: int
         :param RecordId: 自定义录制文件名称前缀。请先在实时音视频控制台开通录制功能，https://cloud.tencent.com/document/product/647/50768。
 【注意】该方式仅对旧版云端录制功能的应用生效，新版云端录制功能的应用请用接口CreateCloudRecording发起录制。新、旧云端录制类型判断方式请见：https://cloud.tencent.com/document/product/647/50768#record
         :type RecordId: str
         :param RecordAudioOnly: 取值范围[0,1]，填0无实际含义; 填1：指定录制文件格式为mp3。此参数不建议使用，建议在实时音视频控制台配置纯音频录制模板。
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.882/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.882/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.881/setup.py` & `tencentcloud-sdk-python-trtc-3.0.882/setup.py`

 * *Files identical despite different names*

