# Comparing `tmp/aliyun-python-sdk-imageprocess-2.0.4.tar.gz` & `tmp/aliyun-python-sdk-imageprocess-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-imageprocess-2.0.4.tar", last modified: Mon Apr  3 02:58:48 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-imageprocess-2.0.5.tar", last modified: Thu Apr 27 09:25:37 2023, max compression
```

## Comparing `aliyun-python-sdk-imageprocess-2.0.4.tar` & `aliyun-python-sdk-imageprocess-2.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1582 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      545 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1582 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2041 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/
--rw-r--r--   0 root         (0) root         (0)     2357 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/AnalyzeChestVesselRequest.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/CalcBMDRequest.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/CalcCACSRequest.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/ClassifyFNFRequest.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectCovid19CadRequest.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectHipKeypointXRayRequest.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectKneeKeypointXRayRequest.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectKneeXRayRequest.py
--rw-r--r--   0 root         (0) root         (0)     2321 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectLungNoduleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectLymphRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectPancRequest.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectRibFractureRequest.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectSkinDiseaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2135 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectSpineMRIRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/FeedbackSessionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/GetAsyncJobResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/RunCTRegistrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/RunMedQARequest.py
--rw-r--r--   0 root         (0) root         (0)     2451 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/ScreenChestCTRequest.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/ScreenECRequest.py
--rw-r--r--   0 root         (0) root         (0)     2317 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/SegmentLymphNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/SegmentOARRequest.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/TargetVolumeSegmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/TranslateMedRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2497 2023-04-03 02:58:48.000000 aliyun-python-sdk-imageprocess-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      545 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/AnalyzeChestVesselRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/CalcBMDRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/CalcCACSRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/ClassifyFNFRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectCovid19CadRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectHipKeypointXRayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectKneeKeypointXRayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectKneeXRayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectLungNoduleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectLymphRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectPancRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectRibFractureRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectSkinDiseaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectSpineMRIRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/FeedbackSessionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/GetAsyncJobResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/RunCTRegistrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/RunMedQARequest.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/ScreenChestCTRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/ScreenECRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/SegmentLymphNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/SegmentOARRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/TargetVolumeSegmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/TranslateMedRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-04-27 09:25:37.000000 aliyun-python-sdk-imageprocess-2.0.5/setup.py
```

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/LICENSE` & `aliyun-python-sdk-imageprocess-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/PKG-INFO` & `aliyun-python-sdk-imageprocess-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-imageprocess
-Version: 2.0.4
+Version: 2.0.5
 Summary: The imageprocess module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-imageprocess
```

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/README.rst` & `aliyun-python-sdk-imageprocess-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/PKG-INFO` & `aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-imageprocess
-Version: 2.0.4
+Version: 2.0.5
 Summary: The imageprocess module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-imageprocess
```

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyun_python_sdk_imageprocess.egg-info/SOURCES.txt` & `aliyun-python-sdk-imageprocess-2.0.5/aliyun_python_sdk_imageprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/endpoint.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/AnalyzeChestVesselRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/AnalyzeChestVesselRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/CalcBMDRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/CalcBMDRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/CalcCACSRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/CalcCACSRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/ClassifyFNFRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/ClassifyFNFRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectCovid19CadRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectCovid19CadRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectHipKeypointXRayRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectHipKeypointXRayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectKneeKeypointXRayRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectKneeKeypointXRayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectKneeXRayRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectKneeXRayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectLungNoduleRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectLungNoduleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectLymphRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectLymphRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectPancRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectPancRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectRibFractureRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectRibFractureRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectSkinDiseaseRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectSkinDiseaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/DetectSpineMRIRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/DetectSpineMRIRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/FeedbackSessionRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/FeedbackSessionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/GetAsyncJobResultRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/GetAsyncJobResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/RunCTRegistrationRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/RunCTRegistrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/RunMedQARequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/RunMedQARequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/ScreenChestCTRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/ScreenChestCTRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/ScreenECRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/ScreenECRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/SegmentLymphNodeRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/SegmentLymphNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/SegmentOARRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/SegmentOARRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/TargetVolumeSegmentRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/TargetVolumeSegmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/aliyunsdkimageprocess/request/v20200320/TranslateMedRequest.py` & `aliyun-python-sdk-imageprocess-2.0.5/aliyunsdkimageprocess/request/v20200320/TranslateMedRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imageprocess-2.0.4/setup.py` & `aliyun-python-sdk-imageprocess-2.0.5/setup.py`

 * *Files identical despite different names*

