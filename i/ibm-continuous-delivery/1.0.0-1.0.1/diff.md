# Comparing `tmp/ibm-continuous-delivery-1.0.0.tar.gz` & `tmp/ibm-continuous-delivery-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-continuous-delivery-1.0.0.tar", last modified: Tue Feb 21 17:06:22 2023, max compression
+gzip compressed data, was "dist/ibm-continuous-delivery-1.0.1.tar", last modified: Wed Apr 26 22:54:31 2023, max compression
```

## Comparing `ibm-continuous-delivery-1.0.0.tar` & `ibm-continuous-delivery-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4461 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3475 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/
--rw-rw-r--   0 travis    (2000) travis    (2000)      918 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   255549 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/cd_tekton_pipeline_v2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   133231 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/cd_toolchain_v2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      668 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4461 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      549 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-21 17:05:33.000000 ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      154 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-02-21 17:06:22.000000 ibm-continuous-delivery-1.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2023-02-21 17:05:07.000000 ibm-continuous-delivery-1.0.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4464 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      918 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   255549 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/cd_tekton_pipeline_v2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   133231 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/cd_toolchain_v2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      668 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4464 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      549 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-26 22:53:30.000000 ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      154 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-26 22:54:31.000000 ibm-continuous-delivery-1.0.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2646 2023-04-26 22:52:56.000000 ibm-continuous-delivery-1.0.1/setup.py
```

### Comparing `ibm-continuous-delivery-1.0.0/LICENSE` & `ibm-continuous-delivery-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-continuous-delivery-1.0.0/PKG-INFO` & `ibm-continuous-delivery-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-continuous-delivery
-Version: 1.0.0
+Version: 1.0.1
 Summary: IBM Cloud Continuous Delivery Python SDK
 Home-page: https://github.com/IBM/continuous-delivery-python-sdk
 Author: IBM
 Author-email: xinyij@ca.ibm.com
 License: Apache 2.0
 Keywords: ibm_continuous_delivery
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 License-File: LICENSE
 
 [![Build Status](https://travis-ci.com/IBM/continuous-delivery-python-sdk.svg?branch=main)](https://travis.ibm.com/IBM/continuous-delivery-python-sdk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-continuous-delivery)](https://pypi.org/project/ibm-continuous-delivery/)
 [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-continuous-delivery.svg)](https://pypi.python.org/pypi/ibm-continuous-delivery)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
 
-# IBM Cloud Continuous Delivery Python SDK v1.0.0
+# IBM Cloud Continuous Delivery Python SDK v1.0.1
  
 The Python client library to interact with the [IBM Cloud Continuous Delivery Toolchain and Tekton Pipeline APIs](https://cloud.ibm.com/docs?tab=api-docs&category=devops).
 
 # Python Version
 The current minimum Python version supported is 3.7.
 
 ## Table of Contents
@@ -44,15 +44,15 @@
   You should regenerate the TOC after making changes to this file.
 
       npx markdown-toc -i README.md
   -->
 
 <!-- toc -->
 
-- [IBM Cloud Continuous Delivery Python SDK v1.0.0](#ibm-cloud-continuous-delivery-python-sdk-v037)
+- [IBM Cloud Continuous Delivery Python SDK v1.0.1](#ibm-cloud-continuous-delivery-python-sdk-v037)
 - [Python Version](#python-version)
   - [Table of Contents](#table-of-contents)
   - [Overview](#overview)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
   - [Using the SDK](#using-the-sdk)
   - [Questions](#questions)
@@ -91,15 +91,15 @@
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
 
 If you are having difficulties using this SDK or have a question about the IBM Cloud services,
-please ask a question
+please ask a question at
 [Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-cloud).
 
 ## Issues
 If you encounter an issue with the project, you are welcome to submit a
 [bug report](https://github.com/IBM/continuous-delivery-python-sdk/issues).
 Before that, please search for similar issues. It's possible that someone has already reported the problem.
```

### Comparing `ibm-continuous-delivery-1.0.0/README.md` & `ibm-continuous-delivery-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Build Status](https://travis-ci.com/IBM/continuous-delivery-python-sdk.svg?branch=main)](https://travis.ibm.com/IBM/continuous-delivery-python-sdk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-continuous-delivery)](https://pypi.org/project/ibm-continuous-delivery/)
 [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-continuous-delivery.svg)](https://pypi.python.org/pypi/ibm-continuous-delivery)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
 
-# IBM Cloud Continuous Delivery Python SDK v1.0.0
+# IBM Cloud Continuous Delivery Python SDK v1.0.1
  
 The Python client library to interact with the [IBM Cloud Continuous Delivery Toolchain and Tekton Pipeline APIs](https://cloud.ibm.com/docs?tab=api-docs&category=devops).
 
 # Python Version
 The current minimum Python version supported is 3.7.
 
 ## Table of Contents
@@ -20,15 +20,15 @@
   You should regenerate the TOC after making changes to this file.
 
       npx markdown-toc -i README.md
   -->
 
 <!-- toc -->
 
-- [IBM Cloud Continuous Delivery Python SDK v1.0.0](#ibm-cloud-continuous-delivery-python-sdk-v037)
+- [IBM Cloud Continuous Delivery Python SDK v1.0.1](#ibm-cloud-continuous-delivery-python-sdk-v037)
 - [Python Version](#python-version)
   - [Table of Contents](#table-of-contents)
   - [Overview](#overview)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
   - [Using the SDK](#using-the-sdk)
   - [Questions](#questions)
@@ -67,15 +67,15 @@
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
 
 If you are having difficulties using this SDK or have a question about the IBM Cloud services,
-please ask a question
+please ask a question at
 [Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-cloud).
 
 ## Issues
 If you encounter an issue with the project, you are welcome to submit a
 [bug report](https://github.com/IBM/continuous-delivery-python-sdk/issues).
 Before that, please search for similar issues. It's possible that someone has already reported the problem.
```

### Comparing `ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/__init__.py` & `ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/cd_tekton_pipeline_v2.py` & `ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/cd_tekton_pipeline_v2.py`

 * *Files identical despite different names*

### Comparing `ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/cd_toolchain_v2.py` & `ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/cd_toolchain_v2.py`

 * *Files identical despite different names*

### Comparing `ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/common.py` & `ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/common.py`

 * *Files identical despite different names*

### Comparing `ibm-continuous-delivery-1.0.0/ibm_continuous_delivery/version.py` & `ibm-continuous-delivery-1.0.1/ibm_continuous_delivery/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_continuous_delivery
 """
-__version__ = '1.0.0'
+__version__ = '1.0.1'
```

### Comparing `ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/PKG-INFO` & `ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-continuous-delivery
-Version: 1.0.0
+Version: 1.0.1
 Summary: IBM Cloud Continuous Delivery Python SDK
 Home-page: https://github.com/IBM/continuous-delivery-python-sdk
 Author: IBM
 Author-email: xinyij@ca.ibm.com
 License: Apache 2.0
 Keywords: ibm_continuous_delivery
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 License-File: LICENSE
 
 [![Build Status](https://travis-ci.com/IBM/continuous-delivery-python-sdk.svg?branch=main)](https://travis.ibm.com/IBM/continuous-delivery-python-sdk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-continuous-delivery)](https://pypi.org/project/ibm-continuous-delivery/)
 [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-continuous-delivery.svg)](https://pypi.python.org/pypi/ibm-continuous-delivery)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
 
-# IBM Cloud Continuous Delivery Python SDK v1.0.0
+# IBM Cloud Continuous Delivery Python SDK v1.0.1
  
 The Python client library to interact with the [IBM Cloud Continuous Delivery Toolchain and Tekton Pipeline APIs](https://cloud.ibm.com/docs?tab=api-docs&category=devops).
 
 # Python Version
 The current minimum Python version supported is 3.7.
 
 ## Table of Contents
@@ -44,15 +44,15 @@
   You should regenerate the TOC after making changes to this file.
 
       npx markdown-toc -i README.md
   -->
 
 <!-- toc -->
 
-- [IBM Cloud Continuous Delivery Python SDK v1.0.0](#ibm-cloud-continuous-delivery-python-sdk-v037)
+- [IBM Cloud Continuous Delivery Python SDK v1.0.1](#ibm-cloud-continuous-delivery-python-sdk-v037)
 - [Python Version](#python-version)
   - [Table of Contents](#table-of-contents)
   - [Overview](#overview)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
   - [Using the SDK](#using-the-sdk)
   - [Questions](#questions)
@@ -91,15 +91,15 @@
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
 
 If you are having difficulties using this SDK or have a question about the IBM Cloud services,
-please ask a question
+please ask a question at
 [Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-cloud).
 
 ## Issues
 If you encounter an issue with the project, you are welcome to submit a
 [bug report](https://github.com/IBM/continuous-delivery-python-sdk/issues).
 Before that, please search for similar issues. It's possible that someone has already reported the problem.
```

### Comparing `ibm-continuous-delivery-1.0.0/ibm_continuous_delivery.egg-info/SOURCES.txt` & `ibm-continuous-delivery-1.0.1/ibm_continuous_delivery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-continuous-delivery-1.0.0/setup.py` & `ibm-continuous-delivery-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 PACKAGE_NAME = 'ibm_continuous_delivery'
 PACKAGE_DESC = 'IBM Cloud Continuous Delivery Python SDK'
 
 with open('requirements.txt') as f:
     install_requires = [
         str(req) for req in pkg_resources.parse_requirements(f)
     ]
```

