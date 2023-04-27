# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.882.tar", last modified: Wed Apr 26 02:50:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.883.tar", last modified: Thu Apr 27 00:17:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.882.tar` & `tencentcloud-sdk-python-asr-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)    23847 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62143 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 02:50:46.000000 tencentcloud-sdk-python-asr-3.0.882/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)    23847 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62142 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:17:03.000000 tencentcloud-sdk-python-asr-3.0.883/tencentcloud_sdk_python_asr.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-asr-3.0.882/README.rst` & `tencentcloud-sdk-python-asr-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.882/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.883/tencentcloud/asr/v20190614/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
         :type ResTextFormat: int
         :param SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
         :type SourceType: int
         :param SpeakerDiarization: 是否开启说话人分离，0：不开启，1：开启(仅支持8k_zh，16k_zh，16k_zh_video，单声道音频)，默认值为 0。
 注意：8k电话场景建议使用双声道来区分通话双方，设置ChannelNum=2即可，不用开启说话人分离。
         :type SpeakerDiarization: int
         :param SpeakerNumber: 说话人分离人数（需配合开启说话人分离使用），取值范围：0-10，0代表自动分离（目前仅支持≤6个人），1-10代表指定说话人数分离。默认值为 0。
-注：话者分离目前是beta版本，请根据您的需要谨慎使用
+注：此功能结果仅供参考，请根据您的需要谨慎使用。
         :type SpeakerNumber: int
         :param CallbackUrl: 回调 URL，用户自行搭建的用于接收识别结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。回调格式&内容详见：[录音识别回调说明](https://cloud.tencent.com/document/product/1093/52632)
         :type CallbackUrl: str
         :param Url: 语音的URL地址，需要公网环境浏览器可下载。当 SourceType 值为 0 时须填写该字段，为 1 时不需要填写。注意：请确保录音文件时长在5个小时之内，否则可能识别失败。请保证文件的下载速度，否则可能下载失败。
         :type Url: str
         :param Data: 语音数据base64编码，当SourceType 值为1时必须填写，为0可不写。音频数据要小于5MB。
         :type Data: str
```

### Comparing `tencentcloud-sdk-python-asr-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.883/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.882/setup.py` & `tencentcloud-sdk-python-asr-3.0.883/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.882/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.883/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

