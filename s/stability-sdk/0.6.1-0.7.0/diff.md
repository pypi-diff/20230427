# Comparing `tmp/stability-sdk-0.6.1.tar.gz` & `tmp/stability-sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.6.1.tar", last modified: Tue Apr 18 22:30:22 2023, max compression
+gzip compressed data, was "stability-sdk-0.7.0.tar", last modified: Thu Apr 27 17:02:42 2023, max compression
```

## Comparing `stability-sdk-0.6.1.tar` & `stability-sdk-0.7.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/stability_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/src/stability_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/src/stability_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/src/stability_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/stability_sdk/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37463 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/project/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-18 22:30:04.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:05.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-18 22:30:05.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-18 22:30:05.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:05.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-18 22:30:05.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-18 22:30:05.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-18 22:30:05.000000 stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/src/stability_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.627613 stability-sdk-0.6.1/src/stability_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-18 22:30:22.000000 stability-sdk-0.6.1/src/stability_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-18 22:30:22.000000 stability-sdk-0.6.1/src/stability_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:30:22.000000 stability-sdk-0.6.1/src/stability_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 22:30:22.000000 stability-sdk-0.6.1/src/stability_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 22:30:22.000000 stability-sdk-0.6.1/src/stability_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:30:22.631613 stability-sdk-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-18 22:30:01.000000 stability-sdk-0.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.228326 stability-sdk-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37463 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.228326 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/tests/test_utils.py
```

### Comparing `stability-sdk-0.6.1/LICENSE` & `stability-sdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/PKG-INFO` & `stability-sdk-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
@@ -121,30 +121,39 @@
 ```
 usage: client.py upscale
        [-h]
        --init_image INIT_IMAGE
        [--height HEIGHT] [--width WIDTH] [--prefix PREFIX] [--artifact_types ARTIFACT_TYPES]
        [--no-store] [--show] [--engine ENGINE]
 
+positional arguments:
+  prompt (ignored in esrgan engines)
+
 options:
   -h, --help            show this help message and exit
   --init_image INIT_IMAGE, -i INIT_IMAGE
                         Init image
   --height HEIGHT, -H HEIGHT
                         height of upscaled image in pixels
   --width WIDTH, -W WIDTH
                         width of upscaled image in pixels
+  --steps STEPS, -s STEPS
+                        [auto] number of steps (ignored in esrgan engines)
+  --seed SEED, -S SEED  random seed to use (ignored in esrgan engines)
+  --cfg_scale CFG_SCALE, -C CFG_SCALE
+                        [7.0] CFG scale factor (ignored in esrgan engines)
   --prefix PREFIX, -p PREFIX
                         output prefixes for artifacts
   --artifact_types ARTIFACT_TYPES, -t ARTIFACT_TYPES
                         filter artifacts by type (ARTIFACT_IMAGE, ARTIFACT_TEXT, ARTIFACT_CLASSIFICATIONS, etc)
   --no-store            do not write out artifacts
   --show                open artifacts using PIL
   --engine ENGINE, -e ENGINE
                         engine to use for upscale
+  
 ```
 
 
 ## Connecting to the API using languages other than Python
 
 If a language you would like to connect to the API with is not currently documented on [Platform](https://platform.stability.ai) you can use the following
 protobuf definition to compile stubs for your language:
```

### Comparing `stability-sdk-0.6.1/README.md` & `stability-sdk-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -88,30 +88,39 @@
 ```
 usage: client.py upscale
        [-h]
        --init_image INIT_IMAGE
        [--height HEIGHT] [--width WIDTH] [--prefix PREFIX] [--artifact_types ARTIFACT_TYPES]
        [--no-store] [--show] [--engine ENGINE]
 
+positional arguments:
+  prompt (ignored in esrgan engines)
+
 options:
   -h, --help            show this help message and exit
   --init_image INIT_IMAGE, -i INIT_IMAGE
                         Init image
   --height HEIGHT, -H HEIGHT
                         height of upscaled image in pixels
   --width WIDTH, -W WIDTH
                         width of upscaled image in pixels
+  --steps STEPS, -s STEPS
+                        [auto] number of steps (ignored in esrgan engines)
+  --seed SEED, -S SEED  random seed to use (ignored in esrgan engines)
+  --cfg_scale CFG_SCALE, -C CFG_SCALE
+                        [7.0] CFG scale factor (ignored in esrgan engines)
   --prefix PREFIX, -p PREFIX
                         output prefixes for artifacts
   --artifact_types ARTIFACT_TYPES, -t ARTIFACT_TYPES
                         filter artifacts by type (ARTIFACT_IMAGE, ARTIFACT_TEXT, ARTIFACT_CLASSIFICATIONS, etc)
   --no-store            do not write out artifacts
   --show                open artifacts using PIL
   --engine ENGINE, -e ENGINE
                         engine to use for upscale
+  
 ```
 
 
 ## Connecting to the API using languages other than Python
 
 If a language you would like to connect to the API with is not currently documented on [Platform](https://platform.stability.ai) you can use the following
 protobuf definition to compile stubs for your language:
```

### Comparing `stability-sdk-0.6.1/setup.py` & `stability-sdk-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open('README.md','r') as f:
     README = f.read()
 
 setup(
     name='stability-sdk',
-    version='0.6.1',
+    version='0.7.0',
     author='Stability AI',
     author_email='support@stability.ai',
     maintainer='Stability AI',
     maintainer_email='support@stability.ai',
     url='https://beta.dreamstudio.ai/',
     download_url='https://github.com/Stability-AI/stability-sdk/',
```

### Comparing `stability-sdk-0.6.1/src/stability_sdk/client.py` & `stability-sdk-0.7.0/src/stability_sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import time
 import mimetypes
 
 import grpc
 from argparse import ArgumentParser, Namespace
 from typing import Dict, Generator, List, Optional, Union, Any, Sequence, Tuple
 from google.protobuf.json_format import MessageToJson
+from google.protobuf.struct_pb2 import Struct
 from PIL import Image
 
 try:
     from dotenv import load_dotenv
 except ModuleNotFoundError:
     pass
 else:
@@ -310,51 +311,91 @@
             width=width,
             seed=seed,
             steps=steps,
             samples=samples,
             parameters=[generation.StepParameter(**step_parameters)],
         )
 
-
         return self.emit_request(prompt=prompts, image_parameters=image_parameters)
     
     def upscale(
         self,
         init_image: Image.Image,
         height: int = None,
         width: int = None,
+        prompt: Union[str, generation.Prompt] = None,
+        steps: Optional[int] = 20,
+        cfg_scale: float = 7.0,
+        seed: int = 0
     ) -> Generator[generation.Answer, None, None]:
+        """
+        Upscale an image.
+
+        :param init_image: Image to upscale.
+
+        Optional parameters for upscale method:
+
+        :param height: Height of the output images.
+        :param width: Width of the output images.
+        :param prompt: Prompt used in text conditioned models
+        :param steps: Number of diffusion steps
+        :param cfg_scale: Intensity of the prompt, when a prompt is used
+        :param seed: Seed for the random number generator.
+
+        Some variables are not used for specific engines, but are included for consistency.
+
+        Variables ignored in ESRGAN engines: prompt, steps, cfg_scale, seed
+
+        :return: Tuple of (prompts, image_parameters)
+        """
+
+        step_parameters = dict(
+            sampler=generation.SamplerParameters(cfg_scale=cfg_scale)
+        )
+
         image_parameters=generation.ImageParameters(
             height=height,
             width=width,
+            seed=[seed],
+            steps=steps,
+            parameters=[generation.StepParameter(**step_parameters)],
         )
 
         prompts = [image_to_prompt(init_image, init=True)]
 
-        return self.emit_request(prompt=prompts, image_parameters=image_parameters, engine_id=self.upscale_engine)
+        if prompt:
+            if isinstance(prompt, str):
+                prompt = generation.Prompt(text=prompt)
+            elif not isinstance(prompt, generation.Prompt):
+                raise ValueError("prompt must be a string or Prompt object")
+            prompts.append(prompt)
 
+        return self.emit_request(prompt=prompts, image_parameters=image_parameters, engine_id=self.upscale_engine)
+    
 
     # The motivation here is to facilitate constructing requests by passing protobuf objects directly.
     def emit_request(
         self,
         prompt: generation.Prompt,
         image_parameters: generation.ImageParameters,
+        extra_parameters: Optional[Struct] = None,
         engine_id: str = None,
         request_id: str = None,
     ):
         if not request_id:
             request_id = str(uuid.uuid4())
         if not engine_id:
             engine_id = self.engine
 
         rq = generation.Request(
             engine_id=engine_id,
             request_id=request_id,
             prompt=prompt,
-            image=image_parameters
+            image=image_parameters,
+            extras=extra_parameters
         )
 
         if self.verbose:
             logger.info("Sending request.")
 
         start = time.time()
         for answer in self.stub.Generate(rq, **self.grpc_args):
@@ -373,32 +414,38 @@
                     logger.info(
                         f"Got keepalive {answer.answer_id} in " f"{duration:0.2f}s"
                     )
 
             yield answer
             start = time.time()
 
-
-if __name__ == "__main__":
-    # Set up logging for output to console.
-    fh = logging.StreamHandler()
-    fh_formatter = logging.Formatter(
-        "%(asctime)s %(levelname)s %(filename)s(%(process)d) - %(message)s"
-    )
-    fh.setFormatter(fh_formatter)
-    logger.addHandler(fh)
-
-    logger.warning(
-        "[Deprecation Warning] The method you have used to invoke the sdk will be deprecated shortly."
-        "[Deprecation Warning] Please modify your code to call the sdk without invoking the 'client' module instead."
-        "[Deprecation Warning] rather than:"
-        "[Deprecation Warning]    $ python -m stability_sdk.client ...  "
-        "[Deprecation Warning] instead do this:"
-        "[Deprecation Warning]    $ python -m stability_sdk ...  "
-    )
+def process_cli(logger: logging.Logger = None,
+                warn_client_call_deprecated: bool = True,
+                ):
+    if not logger:
+        logger = logging.getLogger(__name__)
+        logger.setLevel(level=logging.INFO)
+
+        # Set up logging for output to console.
+        fh = logging.StreamHandler()
+        fh_formatter = logging.Formatter(
+            "%(asctime)s %(levelname)s %(filename)s(%(process)d) - %(message)s"
+        )
+        fh.setFormatter(fh_formatter)
+        logger.addHandler(fh)
+    
+    if warn_client_call_deprecated:
+        logger.warning(
+            "[Deprecation Warning] The method you have used to invoke the sdk will be deprecated shortly."
+            "[Deprecation Warning] Please modify your code to call the sdk without invoking the 'client' module instead."
+            "[Deprecation Warning] rather than:"
+            "[Deprecation Warning]    $ python -m stability_sdk.client ...  "
+            "[Deprecation Warning] instead do this:"
+            "[Deprecation Warning]    $ python -m stability_sdk ...  "
+        )
 
     STABILITY_HOST = os.getenv("STABILITY_HOST", "grpc.stability.ai:443")
     STABILITY_KEY = os.getenv("STABILITY_KEY", "")
 
     if not STABILITY_HOST:
         logger.warning("STABILITY_HOST environment variable needs to be set.")
         sys.exit(1)
@@ -426,14 +473,23 @@
     parser_upscale.add_argument(
         "--height", "-H", type=int, default=None, help="height of upscaled image"
     )
     parser_upscale.add_argument(
         "--width", "-W", type=int, default=None, help="width of upscaled image"
     )
     parser_upscale.add_argument(
+        "--cfg_scale", "-C", type=float, default=7.0, help="[7.0] CFG scale factor (ignored in esrgan engines)"
+    )
+    parser_upscale.add_argument(
+        "--steps", "-s", type=int, default=None, help="[20] number of steps (ignored in esrgan engines)"
+    )
+    parser_upscale.add_argument(
+        "--seed", "-S", type=int, default=0, help="random seed to use (ignored in esrgan engines)"
+    )
+    parser_upscale.add_argument(
         "--prefix",
         "-p",
         type=str,
         default="upscale_",
         help="output prefixes for artifacts",
     )
     parser_upscale.add_argument(
@@ -442,22 +498,27 @@
         action='append',
         type=str,
         help="filter artifacts by type (ARTIFACT_IMAGE, ARTIFACT_TEXT, ARTIFACT_CLASSIFICATIONS, etc)"
     )
     parser_upscale.add_argument(
         "--no-store", action="store_true", help="do not write out artifacts"
     )
-    parser_upscale.add_argument("--show", action="store_true", help="open artifacts using PIL")
+    parser_upscale.add_argument(
+        "--show", action="store_true", help="open artifacts using PIL"
+    )
     parser_upscale.add_argument(
         "--engine",
         "-e",
         type=str,
         help="engine to use for upscale",
         default="esrgan-v1-x2plus",
     )
+    parser_upscale.add_argument(
+        "prompt", nargs="*"
+    )
     
 
     parser_generate = subparsers.add_parser('generate')
     parser_generate.add_argument(
         "--height", "-H", type=int, default=512, help="[512] height of image"
     )
     parser_generate.add_argument(
@@ -483,15 +544,16 @@
         "-A",
         type=str,        
         help="[auto-select] (" + ", ".join(SAMPLERS.keys()) + ")",
     )
     parser_generate.add_argument(
         "--steps", "-s", type=int, default=None, help="[auto] number of steps"
     )
-    parser_generate.add_argument("--seed", "-S", type=int, default=0, help="random seed to use")
+    parser_generate.add_argument(
+        "--seed", "-S", type=int, default=0, help="random seed to use")
     parser_generate.add_argument(
         "--prefix",
         "-p",
         type=str,
         default="generation_",
         help="output prefixes for artifacts",
     )
@@ -546,26 +608,33 @@
         )
         input_args = ['generate'] + input_args
       
     args = parser.parse_args(input_args)
     
     if args.command == "upscale":
         args.init_image = Image.open(args.init_image)
+        if not args.prompt:
+            args.prompt = [""]
+        args.prompt = " ".join(args.prompt)
 
         request =  {
-        "height": args.height,
-        "width": args.width,
-        "init_image": args.init_image,
+            "height": args.height,
+            "width": args.width,
+            "init_image": args.init_image,
+            "steps": args.steps,
+            "seed": args.seed,
+            "cfg_scale": args.cfg_scale,
+            "prompt": args.prompt,
             }
         stability_api = StabilityInference(
             STABILITY_HOST, STABILITY_KEY, upscale_engine=args.engine, verbose=True
         )
         answers = stability_api.upscale(**request)
         artifacts = process_artifacts_from_answers(
-            args.prefix, "", answers, write=not args.no_store, verbose=True,
+            args.prefix, args.prompt, answers, write=not args.no_store, verbose=True,
             filter_types=args.artifact_types,
         )
     elif args.command == "generate":
         if not args.prompt and not args.init_image:
             logger.warning("prompt or init image must be provided")
             parser.print_help()
             sys.exit(1)
@@ -607,7 +676,11 @@
     
     if args.show:
         for artifact in open_images(artifacts, verbose=True):
             pass
     else:
         for artifact in artifacts:
             pass
+
+
+if __name__ == "__main__":
+    process_cli(logger)
```

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/project/project_pb2.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/protobuf.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py` & `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk/utils.py` & `stability-sdk-0.7.0/src/stability_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/src/stability_sdk.egg-info/PKG-INFO` & `stability-sdk-0.7.0/src/stability_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
@@ -121,30 +121,39 @@
 ```
 usage: client.py upscale
        [-h]
        --init_image INIT_IMAGE
        [--height HEIGHT] [--width WIDTH] [--prefix PREFIX] [--artifact_types ARTIFACT_TYPES]
        [--no-store] [--show] [--engine ENGINE]
 
+positional arguments:
+  prompt (ignored in esrgan engines)
+
 options:
   -h, --help            show this help message and exit
   --init_image INIT_IMAGE, -i INIT_IMAGE
                         Init image
   --height HEIGHT, -H HEIGHT
                         height of upscaled image in pixels
   --width WIDTH, -W WIDTH
                         width of upscaled image in pixels
+  --steps STEPS, -s STEPS
+                        [auto] number of steps (ignored in esrgan engines)
+  --seed SEED, -S SEED  random seed to use (ignored in esrgan engines)
+  --cfg_scale CFG_SCALE, -C CFG_SCALE
+                        [7.0] CFG scale factor (ignored in esrgan engines)
   --prefix PREFIX, -p PREFIX
                         output prefixes for artifacts
   --artifact_types ARTIFACT_TYPES, -t ARTIFACT_TYPES
                         filter artifacts by type (ARTIFACT_IMAGE, ARTIFACT_TEXT, ARTIFACT_CLASSIFICATIONS, etc)
   --no-store            do not write out artifacts
   --show                open artifacts using PIL
   --engine ENGINE, -e ENGINE
                         engine to use for upscale
+  
 ```
 
 
 ## Connecting to the API using languages other than Python
 
 If a language you would like to connect to the API with is not currently documented on [Platform](https://platform.stability.ai) you can use the following
 protobuf definition to compile stubs for your language:
```

### Comparing `stability-sdk-0.6.1/src/stability_sdk.egg-info/SOURCES.txt` & `stability-sdk-0.7.0/src/stability_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/tests/test_client.py` & `stability-sdk-0.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.6.1/tests/test_utils.py` & `stability-sdk-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

