# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.881.tar", last modified: Tue Apr 25 00:30:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.882.tar", last modified: Wed Apr 26 03:07:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.881.tar` & `tencentcloud-sdk-python-clb-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89842 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)   328539 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:30:08.000000 tencentcloud-sdk-python-clb-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:30:09.000000 tencentcloud-sdk-python-clb-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89842 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   328567 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:07:56.000000 tencentcloud-sdk-python-clb-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:07:57.000000 tencentcloud-sdk-python-clb-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-clb-3.0.881/README.rst` & `tencentcloud-sdk-python-clb-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.881/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.882/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7545,15 +7545,15 @@
         :param HealthCheck: 健康检查信息。详情请参见：[健康检查](https://cloud.tencent.com/document/product/214/6097)
         :type HealthCheck: :class:`tencentcloud.clb.v20180317.models.HealthCheck`
         :param Certificate: 证书信息；此参数和MultiCertInfo不能同时传入。
         :type Certificate: :class:`tencentcloud.clb.v20180317.models.CertificateInput`
         :param Scheduler: 规则的请求转发方式，可选值：WRR、LEAST_CONN、IP_HASH
 分别表示按权重轮询、最小连接数、按IP哈希， 默认为 WRR。
         :type Scheduler: str
-        :param ForwardType: 负载均衡与后端服务之间的转发协议，目前支持 HTTP/HTTPS/TRPC
+        :param ForwardType: 负载均衡与后端服务之间的转发协议，目前支持 HTTP/HTTPS/TRPC，TRPC暂未对外开放。
         :type ForwardType: str
         :param DefaultServer: 是否将该域名设为默认域名，注意，一个监听器下只能设置一个默认域名。
         :type DefaultServer: bool
         :param Http2: 是否开启Http2，注意，只有HTTPS域名才能开启Http2。
         :type Http2: bool
         :param TargetType: 后端目标类型，NODE表示绑定普通节点，TARGETGROUP表示绑定目标组
         :type TargetType: str
```

### Comparing `tencentcloud-sdk-python-clb-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.881/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.882/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.882/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.881/setup.py` & `tencentcloud-sdk-python-clb-3.0.882/setup.py`

 * *Files identical despite different names*

