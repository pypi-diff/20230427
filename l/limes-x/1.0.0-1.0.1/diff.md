# Comparing `tmp/limes_x-1.0.0-py3-none-any.whl.zip` & `tmp/limes_x-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 35555 bytes, number of entries: 21
+Zip file size: 35670 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      220 b- defN 23-Apr-19 01:42 limes_x/__init__.py
 -rw-rw-r--  2.0 unx       69 b- defN 23-Apr-19 01:42 limes_x/constants.py
 -rw-rw-r--  2.0 unx     2864 b- defN 23-Apr-19 01:42 limes_x/telemetry.py
 -rw-rw-r--  2.0 unx    38931 b- defN 23-Apr-19 01:42 limes_x/workflow.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/common/__init__.py
 -rw-rw-r--  2.0 unx     8098 b- defN 23-Apr-19 01:42 limes_x/common/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/environments/__init__.py
 -rw-rw-r--  2.0 unx     1202 b- defN 23-Apr-19 01:42 limes_x/environments/_setup.py
--rw-rw-r--  2.0 unx     5541 b- defN 23-Apr-19 01:42 limes_x/environments/hpc.py
+-rw-rw-r--  2.0 unx     6015 b- defN 23-Apr-27 17:28 limes_x/environments/hpc.py
 -rw-rw-r--  2.0 unx     3654 b- defN 23-Apr-19 01:42 limes_x/environments/local.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/execution/__init__.py
 -rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-19 01:42 limes_x/execution/comms.py
 -rw-rw-r--  2.0 unx     9436 b- defN 23-Apr-19 01:42 limes_x/execution/executors.py
 -rw-rw-r--  2.0 unx     5105 b- defN 23-Apr-19 01:42 limes_x/execution/instances.py
 -rw-rw-r--  2.0 unx    14052 b- defN 23-Apr-19 01:42 limes_x/execution/modules.py
 -rw-rw-r--  2.0 unx     4419 b- defN 23-Apr-19 01:42 limes_x/execution/solver.py
 -rw-rw-r--  2.0 unx      677 b- defN 23-Apr-19 01:42 limes_x/execution/template_module_definition.py
--rw-rw-r--  2.0 unx     9991 b- defN 23-Apr-19 01:48 limes_x-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 01:48 limes_x-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-19 01:48 limes_x-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1717 b- defN 23-Apr-19 01:48 limes_x-1.0.0.dist-info/RECORD
-21 files, 108890 bytes uncompressed, 32757 bytes compressed:  69.9%
+-rw-rw-r--  2.0 unx     9991 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1717 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/RECORD
+21 files, 109364 bytes uncompressed, 32872 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: limes_x/execution/solver.py
 Comment: 
 
 Filename: limes_x/execution/template_module_definition.py
 Comment: 
 
-Filename: limes_x-1.0.0.dist-info/METADATA
+Filename: limes_x-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: limes_x-1.0.0.dist-info/WHEEL
+Filename: limes_x-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: limes_x-1.0.0.dist-info/top_level.txt
+Filename: limes_x-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: limes_x-1.0.0.dist-info/RECORD
+Filename: limes_x-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## limes_x/environments/hpc.py

```diff
@@ -89,36 +89,46 @@
         cp -r -L {MODULE_PATH}/{ComputeModule.LIB_FOLDER} {HPC_LIB}/{module_name}
         cd {HPC_WS} && ls -lh
     """, is_child=False)
     _shell(f"ls -lh {HPC_LIB}", is_child=False)
 
     # get requirements
     requirements = [str(CONTEXT.params.reference_folder.joinpath(req)) for req in THIS_MODULE.requirements]
-    req_ok = False
-    for req in requirements:
-        if not os.path.exists(req):
+    req_ok = True
+    for req_path in requirements:
+        found = False
+        for cmd, req in [
+            # (f"cd {HPC_REF} && pigz -dc {req_path}.tar.gz | tar -", f"{req_path}.tar.gz"),
+            (f"cd {HPC_REF} && pigz -dc {req_path}.lx.tgz | tar -", f"{req_path}.lx.tgz"),
+            (f"cp -r {req_path} {HPC_REF}", req_path),
+        ]:
+            if not os.path.exists(req): continue
+            found = True
+            _shell(f"""\
+                echo "---- getting requirement: {req}"
+                {cmd}
+            """, is_child=False)
+            break
+
+        if not found:
             req_ok = False
-            _shell(f'!ERR: requirement [{req}] missing"', is_child=False)
+            _shell(f'echo "ERROR: requirement [{req_path}] missing"', is_child=False)
             break
-        _shell(f"""\
-            echo "---- getting requirement: {req}"
-            cp -r {req} {HPC_REF}
-        """, is_child=False)
     _shell(f"ls -lh {HPC_REF}", is_child=False)
     CONTEXT.params.reference_folder = HPC_REF
     CONTEXT.ref = HPC_LIB
     CONTEXT.Save(HPC_WS)
 
     # remove myself from list of io jobs
     with FileSyncedDictionary(WORKSPACE) as com:
         com.RemoveIoTask(CONTEXT.job_id)
 
     # run step if @req met
     if req_ok:
-        _shell("echo $(date) running...", is_child=False)
+        _shell("echo running...", is_child=False)
         _shell(f"""\
             python {env.__file__} {HPC_LIB}/{module_name} {HPC_WS} {RELATIVE_OUTPUT_PATH} {True}\
         """, is_child=True)
 
         # gather results
         BL = {
             'context.json',
@@ -134,14 +144,16 @@
                 cp -r {out} {LOCAL_OUT_PATH.joinpath(out)}
             """, is_child=False)
         _shell("""\
             echo "---- final workspace:"
             ls | xargs -I {} sh -c "echo {}/ && ls -lh {}"
             echo "---- done!"
         """, is_child=False)
+    else:
+        _shell('echo "terminating due to missing requirement', is_child=False)
 
     result_json = 'result.json'
     result_path = RELATIVE_OUTPUT_PATH.joinpath(result_json)
     def _get_result_json():
         if result_path.exists():
             with open(result_path) as j:
                 try:
```

## Comparing `limes_x-1.0.0.dist-info/METADATA` & `limes_x-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limes-x
-Version: 1.0.0
+Version: 1.0.1
 Summary: declarative workflow automation
 Home-page: https://github.com/hallamlab/limes-x
 Author: Tony Liu
 Author-email: contacttonyliu@gmail.com
 Project-URL: Bug Tracker, https://github.com/hallamlab/limes-x/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `limes_x-1.0.0.dist-info/RECORD` & `limes_x-1.0.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 limes_x/constants.py,sha256=yugKKsslkE48FwDWtzqkZ8EUK4XLX_NEh9cccmm_1IM,69
 limes_x/telemetry.py,sha256=6hUE1nxxKkPUGUNq0KlIbHQqa3pSqA0zZSjb57Wyngc,2864
 limes_x/workflow.py,sha256=taAErdX4P017ay4y8CJoeg9f43okaXjtlpSVpbnMBPU,38931
 limes_x/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/common/utils.py,sha256=83ayvyp9oieN9CFF9VNxjQQwK06EWzqXKaLDjhGqC_c,8098
 limes_x/environments/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/environments/_setup.py,sha256=rI9gTVt2VMXfeAsuxkTx3ucBp5kd_K-Z6xbJqybzEvg,1202
-limes_x/environments/hpc.py,sha256=Q0muocdDb_3NeNW2tjPQxH5nCQK3wxnddOrXedt7XRA,5541
+limes_x/environments/hpc.py,sha256=MKU6R8hJ7fhqd5Mx3TXQzJCQCLBMhY5Wd33bygAnB04,6015
 limes_x/environments/local.py,sha256=MF_-1XB4hiFUI9_0fhXCRrMshFSlc5hyO1rG1B35kik,3654
 limes_x/execution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/execution/comms.py,sha256=Yx_cIyvzuA7h_iKU4R3fyd1LvsKZzZx-NsVZh_MXHE4,2814
 limes_x/execution/executors.py,sha256=6O7uZqyAqFLS-lmQifanKc_8CUKPTFHACL0yDrYiQlY,9436
 limes_x/execution/instances.py,sha256=lT32W3nNSOrfovSNEl7ARY8Yt4SkhkA-1NjWUhBvOds,5105
 limes_x/execution/modules.py,sha256=AIEY-xyIDUhrQvw7qxJChTwXNTEtydKjrxHZCd4woWs,14052
 limes_x/execution/solver.py,sha256=y9XNSlZscAHxizN57PZTMphHw1PVWjFnEfHyrGN7SFU,4419
 limes_x/execution/template_module_definition.py,sha256=RxW4KsU1-iEScq_Y5GIafSfeXnQQeYGYr9FC9AZ8-VQ,677
-limes_x-1.0.0.dist-info/METADATA,sha256=b8Sh182Es93CUPx1hYm5nskt_yvEMM56VNnw-BkMIVc,9991
-limes_x-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-limes_x-1.0.0.dist-info/top_level.txt,sha256=r9RGajCrNNSpim7JI2bx3UHGzgXw2vRLTNuxMRwPRNQ,8
-limes_x-1.0.0.dist-info/RECORD,,
+limes_x-1.0.1.dist-info/METADATA,sha256=TP1mWoyP9Uv5yUOoaIMInZZeVv5pyXbg2sTSJhDRnY4,9991
+limes_x-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+limes_x-1.0.1.dist-info/top_level.txt,sha256=r9RGajCrNNSpim7JI2bx3UHGzgXw2vRLTNuxMRwPRNQ,8
+limes_x-1.0.1.dist-info/RECORD,,
```

