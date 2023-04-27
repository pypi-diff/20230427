# Comparing `tmp/tencentcloud-sdk-python-bsca-3.0.882.tar.gz` & `tmp/tencentcloud-sdk-python-bsca-3.0.883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bsca-3.0.882.tar", last modified: Wed Apr 26 02:53:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bsca-3.0.883.tar", last modified: Thu Apr 27 00:19:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bsca-3.0.882.tar` & `tencentcloud-sdk-python-bsca-3.0.883.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/
--rw-r--r--   0 root         (0) root         (0)     1057 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5955 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/bsca_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32074 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud_sdk_python_bsca.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud_sdk_python_bsca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud_sdk_python_bsca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/tencentcloud_sdk_python_bsca.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 02:53:56.000000 tencentcloud-sdk-python-bsca-3.0.882/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5955 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/bsca_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32074 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud_sdk_python_bsca.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud_sdk_python_bsca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud_sdk_python_bsca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/tencentcloud_sdk_python_bsca.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:19:02.000000 tencentcloud-sdk-python-bsca-3.0.883/setup.cfg
```

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/README.rst` & `tencentcloud-sdk-python-bsca-3.0.883/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/errorcodes.py` & `tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/bsca_client.py` & `tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/bsca_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/bsca/v20210811/models.py` & `tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/bsca/v20210811/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bsca-3.0.883/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bsca-3.0.883/tencentcloud_sdk_python_bsca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bsca
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Bsca SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/PKG-INFO` & `tencentcloud-sdk-python-bsca-3.0.883/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bsca
-Version: 3.0.882
+Version: 3.0.883
 Summary: Tencent Cloud Bsca SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bsca-3.0.882/setup.py` & `tencentcloud-sdk-python-bsca-3.0.883/setup.py`

 * *Files identical despite different names*
