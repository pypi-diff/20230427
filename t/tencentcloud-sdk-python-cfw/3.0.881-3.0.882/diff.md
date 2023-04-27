# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.881.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.881.tar", last modified: Tue Apr 25 00:29:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.882.tar", last modified: Wed Apr 26 03:04:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.881.tar` & `tencentcloud-sdk-python-cfw-3.0.882.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65621 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   215473 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:29:22.000000 tencentcloud-sdk-python-cfw-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65621 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   215473 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-26 03:04:52.000000 tencentcloud-sdk-python-cfw-3.0.882/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/README.rst` & `tencentcloud-sdk-python-cfw-3.0.882/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/cfw/v20190904/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.882/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.882/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.882/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.881
+Version: 3.0.882
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.881/setup.py` & `tencentcloud-sdk-python-cfw-3.0.882/setup.py`

 * *Files identical despite different names*
