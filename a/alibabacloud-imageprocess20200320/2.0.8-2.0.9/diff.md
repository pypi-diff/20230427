# Comparing `tmp/alibabacloud_imageprocess20200320-2.0.8.tar.gz` & `tmp/alibabacloud_imageprocess20200320-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_imageprocess20200320-2.0.8.tar", last modified: Wed Apr  6 10:27:01 2022, max compression
+gzip compressed data, was "dist/alibabacloud_imageprocess20200320-2.0.9.tar", last modified: Fri Apr  8 02:12:10 2022, max compression
```

## Comparing `alibabacloud_imageprocess20200320-2.0.8.tar` & `alibabacloud_imageprocess20200320-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/
--rw-r--r--   0 root         (0) root         (0)     1005 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2382 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320/
--rw-r--r--   0 root         (0) root         (0)       21 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91609 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320/client.py
--rw-r--r--   0 root         (0) root         (0)   138762 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2382 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      492 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      350 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2889 2022-04-06 10:27:01.000000 alibabacloud_imageprocess20200320-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1059 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2382 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94429 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320/client.py
+-rw-r--r--   0 root         (0) root         (0)   142225 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2382 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      350 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2889 2022-04-08 02:12:10.000000 alibabacloud_imageprocess20200320-2.0.9/setup.py
```

### Comparing `alibabacloud_imageprocess20200320-2.0.8/ChangeLog.md` & `alibabacloud_imageprocess20200320-2.0.9/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-04-06 Version: 2.0.8
+- Release FeedbackSession.
+
 2021-07-19 Version: 2.0.7
 - Update ScreenChestCT.
 
 2021-07-02 Version: 2.0.6
 - Release AnalyzeChestVessel.
 
 2021-05-14 Version: 2.0.5
```

### Comparing `alibabacloud_imageprocess20200320-2.0.8/LICENSE` & `alibabacloud_imageprocess20200320-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_imageprocess20200320-2.0.8/PKG-INFO` & `alibabacloud_imageprocess20200320-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_imageprocess20200320
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud imageprocess (20200320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_imageprocess20200320-2.0.8/README-CN.md` & `alibabacloud_imageprocess20200320-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_imageprocess20200320-2.0.8/README.md` & `alibabacloud_imageprocess20200320-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320/client.py` & `alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1680,14 +1680,88 @@
     async def detect_spine_mri_async(
         self,
         request: imageprocess_20200320_models.DetectSpineMRIRequest,
     ) -> imageprocess_20200320_models.DetectSpineMRIResponse:
         runtime = util_models.RuntimeOptions()
         return await self.detect_spine_mriwith_options_async(request, runtime)
 
+    def feedback_session_with_options(
+        self,
+        request: imageprocess_20200320_models.FeedbackSessionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> imageprocess_20200320_models.FeedbackSessionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.feedback):
+            body['Feedback'] = request.feedback
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='FeedbackSession',
+            version='2020-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            imageprocess_20200320_models.FeedbackSessionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def feedback_session_with_options_async(
+        self,
+        request: imageprocess_20200320_models.FeedbackSessionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> imageprocess_20200320_models.FeedbackSessionResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.feedback):
+            body['Feedback'] = request.feedback
+        if not UtilClient.is_unset(request.session_id):
+            body['SessionId'] = request.session_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='FeedbackSession',
+            version='2020-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            imageprocess_20200320_models.FeedbackSessionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def feedback_session(
+        self,
+        request: imageprocess_20200320_models.FeedbackSessionRequest,
+    ) -> imageprocess_20200320_models.FeedbackSessionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.feedback_session_with_options(request, runtime)
+
+    async def feedback_session_async(
+        self,
+        request: imageprocess_20200320_models.FeedbackSessionRequest,
+    ) -> imageprocess_20200320_models.FeedbackSessionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.feedback_session_with_options_async(request, runtime)
+
     def get_async_job_result_with_options(
         self,
         request: imageprocess_20200320_models.GetAsyncJobResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> imageprocess_20200320_models.GetAsyncJobResultResponse:
         UtilClient.validate_model(request)
         body = {}
```

### Comparing `alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320/models.py` & `alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2926,14 +2926,147 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DetectSpineMRIResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class FeedbackSessionRequest(TeaModel):
+    def __init__(
+        self,
+        feedback: str = None,
+        session_id: str = None,
+    ):
+        self.feedback = feedback
+        self.session_id = session_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.feedback is not None:
+            result['Feedback'] = self.feedback
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Feedback') is not None:
+            self.feedback = m.get('Feedback')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        return self
+
+
+class FeedbackSessionResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        data: str = None,
+    ):
+        self.data = data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        return self
+
+
+class FeedbackSessionResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: FeedbackSessionResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        # Id of the request
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = FeedbackSessionResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class FeedbackSessionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: FeedbackSessionResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = FeedbackSessionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetAsyncJobResultRequest(TeaModel):
     def __init__(
         self,
         job_id: str = None,
     ):
         self.job_id = job_id
```

### Comparing `alibabacloud_imageprocess20200320-2.0.8/alibabacloud_imageprocess20200320.egg-info/PKG-INFO` & `alibabacloud_imageprocess20200320-2.0.9/alibabacloud_imageprocess20200320.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-imageprocess20200320
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud imageprocess (20200320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_imageprocess20200320-2.0.8/setup.py` & `alibabacloud_imageprocess20200320-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_imageprocess20200320.
 
-Created on 06/04/2022
+Created on 08/04/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_imageprocess20200320"
 NAME = "alibabacloud_imageprocess20200320" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud imageprocess (20200320) SDK Library for Python"
```

