# Comparing `tmp/deepprofile-0.0.8.tar.gz` & `tmp/deepprofile-0.0.9.tar.gz`

## Comparing `deepprofile-0.0.8.tar` & `deepprofile-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepprofile-0.0.8/tmp.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/__about__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/__init__.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/dcgm.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 deepprofile-0.0.8/deepprofile/nsight.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 deepprofile-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepprofile-0.0.8/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 deepprofile-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 deepprofile-0.0.8/README.md
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deepprofile-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 deepprofile-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepprofile-0.0.9/tmp.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 deepprofile-0.0.9/deepprofile/__about__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 deepprofile-0.0.9/deepprofile/__init__.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deepprofile-0.0.9/deepprofile/dcgm.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 deepprofile-0.0.9/deepprofile/nsight.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 deepprofile-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepprofile-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 deepprofile-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 deepprofile-0.0.9/README.md
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 deepprofile-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 deepprofile-0.0.9/PKG-INFO
```

### Comparing `deepprofile-0.0.8/deepprofile/dcgm.py` & `deepprofile-0.0.9/deepprofile/dcgm.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,15 @@
     print("Unable to find DCGM python bindings, please refer to the exmaple below: ")
     print("DCGMPATH=/usr/local/dcgm python dcgm_example.py")
 
 
 DCGM_JOB_ID = "DCGM_JOB"
 
 
-SAMPLE_INTERVAL = 1  # in microseconds
-
-
-def init_hostengine(fieldIds):
+def init_hostengine(fieldIds, dcgmSamplingInterval):
     opMode = dcgm_structs.DCGM_OPERATION_MODE_AUTO
     dcgmHandle = pydcgm.DcgmHandle(opMode=opMode)
     dcgmGroup = pydcgm.DcgmGroup(
         dcgmHandle, groupName="one_gpu_group", groupType=dcgm_structs.DCGM_GROUP_EMPTY
     )
 
     ## Get a handle to the system level object for DCGM
@@ -53,15 +50,15 @@
         dcgmGroup.AddGpu(gpu)
 
     print("Running with supported GPUs", supportedGPUs)
 
     dcgmFieldGroup = pydcgm.DcgmFieldGroup(
         dcgmHandle, "profiling_metrics", fieldIds=fieldIds
     )
-    dcgmGroup.samples.WatchFields(dcgmFieldGroup, SAMPLE_INTERVAL, 3600, 0)
+    dcgmGroup.samples.WatchFields(dcgmFieldGroup, dcgmSamplingInterval, 3600, 0)
     dcgmSystem.profiling.Resume()
 
     dcgmSamples = dcgmGroup.samples
     dfvc = dcgmSamples.GetAllSinceLastCall(dfvc=None, fieldGroup=dcgmFieldGroup)
 
     return dcgmGroup, dcgmFieldGroup, dfvc, dcgmHandle
 
@@ -78,16 +75,18 @@
     return samples.values
 
 
 vals = []
 
 
 @contextmanager
-def dcgm_profiling_decorator(fieldIds=[1003, 1004]):
-    dcgmGroup, dcgmFieldGroup, dfvc, dcgmHandle = init_hostengine(fieldIds=fieldIds)
+def dcgm_profiling_decorator(fieldIds=[1003, 1004], dcgmSamplingInterval=1000):
+    dcgmGroup, dcgmFieldGroup, dfvc, dcgmHandle = init_hostengine(
+        fieldIds=fieldIds, dcgmSamplingInterval=dcgmSamplingInterval
+    )
     vals.append((dcgmGroup, dcgmFieldGroup, dfvc, dcgmHandle))
     try:
         yield partial(get_metrics, dcgmGroup, dcgmFieldGroup, dfvc, dcgmHandle)
     finally:
         dcgmSystem = dcgmHandle.GetSystem()
         dcgmSystem.profiling.Pause()
```

### Comparing `deepprofile-0.0.8/deepprofile/nsight.py` & `deepprofile-0.0.9/deepprofile/nsight.py`

 * *Files identical despite different names*

### Comparing `deepprofile-0.0.8/LICENSE.txt` & `deepprofile-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepprofile-0.0.8/README.md` & `deepprofile-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `deepprofile-0.0.8/pyproject.toml` & `deepprofile-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepprofile-0.0.8/PKG-INFO` & `deepprofile-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepprofile
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/unknown/deepprofile#readme
 Project-URL: Issues, https://github.com/unknown/deepprofile/issues
 Project-URL: Source, https://github.com/unknown/deepprofile
 Author-email: SamKG <samyak.k.gupta@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

