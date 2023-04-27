# Comparing `tmp/gxabm-2.2.0.tar.gz` & `tmp/gxabm-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.2.0.tar", last modified: Mon Apr 24 20:25:34 2023, max compression
+gzip compressed data, was "gxabm-2.3.0.tar", last modified: Thu Apr 27 20:19:21 2023, max compression
```

## Comparing `gxabm-2.2.0.tar` & `gxabm-2.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.747554 gxabm-2.2.0/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.2.0/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-24 20:25:34.747338 gxabm-2.2.0/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.2.0/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.737892 gxabm-2.2.0/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-04-24 20:24:53.000000 gxabm-2.2.0/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.743372 gxabm-2.2.0/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    16622 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     5443 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     6229 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7433 2023-01-18 20:21:02.000000 gxabm-2.2.0/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.2.0/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)     9582 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     2342 2023-01-18 20:21:02.000000 gxabm-2.2.0/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.2.0/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    10513 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     5499 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.745358 gxabm-2.2.0/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-24 20:25:34.747617 gxabm-2.2.0/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.2.0/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.746857 gxabm-2.2.0/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.2.0/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.2.0/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.2.0/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.2.0/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.2.0/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.140571 gxabm-2.3.0/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.3.0/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-27 20:19:21.140352 gxabm-2.3.0/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.3.0/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.132981 gxabm-2.3.0/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        5 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.3.0/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.137822 gxabm-2.3.0/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.3.0/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5458 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.3.0/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7727 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.3.0/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     9582 2023-04-27 20:14:45.000000 gxabm-2.3.0/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     3382 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.3.0/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    11186 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.3.0/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6930 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.138692 gxabm-2.3.0/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-27 20:19:21.140628 gxabm-2.3.0/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.3.0/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.139894 gxabm-2.3.0/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.3.0/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.3.0/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.3.0/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.3.0/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.3.0/test/workflow.py
```

### Comparing `gxabm-2.2.0/PKG-INFO` & `gxabm-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.2.0
+Version: 2.3.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.2.0/README.md` & `gxabm-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/__main__.py` & `gxabm-2.3.0/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/benchmark.py` & `gxabm-2.3.0/abm/lib/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import json
 import yaml
 import logging
 import argparse
 from lib import Keys, INVOCATIONS_DIR, METRICS_DIR
-from lib.common import connect, Context
+from lib.common import connect, Context, print_json
 from bioblend.galaxy import GalaxyInstance
 
 log = logging.getLogger('abm')
 
 def run_cli(context: Context, args: list):
     """
     Runs a single workflow defined by *args[0]*
@@ -118,27 +118,45 @@
             if Keys.INPUTS in run and run[Keys.INPUTS] is not None:
                 for spec in run[Keys.INPUTS]:
                     input = gi.workflows.get_workflow_inputs(wfid, spec[Keys.NAME])
                     if input is None or len(input) == 0:
                         print(f'ERROR: Invalid input specification for {spec[Keys.NAME]}')
                         return False
 
-                    dsname = spec[Keys.DATASET_ID]
-                    input_names.append(dsname)
-                    #inputs.append(dsname)
-                    # dsid = find_dataset_id(gi, dsname)
-                    dsdata = _get_dataset_data(gi, dsname)
-                    if dsdata is None:
-                        raise  Exception(f"ERROR: unable to resolve {dsname} to a dataset.")
-                    dsid = dsdata['id']
-                    dssize = dsdata['size']
-                    input_data_size.append(dssize)
-                    print(f"Input dataset ID: {dsname} [{dsid}] {dssize}")
-                    inputs[input[0]] = {'id': dsid, 'src': 'hda', 'size': dssize}
-
+                    if 'value' in spec:
+                        inputs[input[0]] = spec['value']
+                        print(f"Input data value: {spec['value']}")
+                    elif 'collection' in spec:
+                        dsname = spec['collection']
+                        input_names.append(dsname)
+                        #inputs.append(dsname)
+                        # dsid = find_dataset_id(gi, dsname)
+                        dsdata = _get_dataset_data(gi, dsname)
+                        if dsdata is None:
+                            raise  Exception(f"ERROR: unable to resolve {dsname} to a dataset.")
+                        dsid = dsdata['id']
+                        dssize = dsdata['size']
+                        input_data_size.append(dssize)
+                        print(f"Input dataset ID: {dsname} [{dsid}] {dssize}")
+                        inputs[input[0]] = {'id': dsid, 'src': 'hdca', 'size': dssize}
+                    elif Keys.DATASET_ID in spec:
+                        dsname = spec[Keys.DATASET_ID]
+                        input_names.append(dsname)
+                        #inputs.append(dsname)
+                        # dsid = find_dataset_id(gi, dsname)
+                        dsdata = _get_dataset_data(gi, dsname)
+                        if dsdata is None:
+                            raise  Exception(f"ERROR: unable to resolve {dsname} to a dataset.")
+                        dsid = dsdata['id']
+                        dssize = dsdata['size']
+                        input_data_size.append(dssize)
+                        print(f"Input dataset ID: {dsname} [{dsid}] {dssize}")
+                        inputs[input[0]] = {'id': dsid, 'src': 'hda', 'size': dssize}
+                    else:
+                        raise Exception(f'Invalid input value')
             print(f"Running workflow {wfid}")
             new_history_name = output_history_name
             if history_prefix is not None:
                 new_history_name = f"{history_prefix} {output_history_name}"
             if experiment is not None:
                 new_history_name = f"{experiment} {new_history_name}"
             invocation = gi.workflows.invoke_workflow(wfid, inputs=inputs, history_name=new_history_name)
@@ -411,16 +429,37 @@
         return make_result(ds)
     except Exception as e:
         pass
 
     try:
         datasets = gi.datasets.get_datasets(name=name_or_id)  # , deleted=True, purged=True)
         for ds in datasets:
-            if ds['state'] == 'ok' and not ds['deleted'] and ds['visible']:
+            print_json(ds)
+            state = True
+            if 'state' in ds:
+                state = ds['state'] == 'ok'
+            if state and not ds['deleted'] and ds['visible']:
                 # The dict returned by get_datasets does not include the input
                 # file sizes so we need to make another call to show_datasets
                 return make_result(gi.datasets.show_dataset(ds['id']))
+            # if ds['state'] == 'ok':
+            #     print('state is ok')
+            # if ds['deleted']:
+            #     print('dataset deleted')
+            # else:
+            #     print('dataset not deleted')
+            # if ds['visible']:
+            #     print('dataset visible')
+            # else:
+            #     print('dataset not visible')
     except Exception as e:
-        print(e)
+        pass
 
     return None
 
+
+from pprint import pprint
+def test(context:Context, args:list):
+    id = 'c90fffcf98b31cd3'
+    gi = connect(context)
+    inputs = gi.workflows.get_workflow_inputs(id, 'PE fastq input')
+    pprint(inputs)
```

### Comparing `gxabm-2.2.0/abm/lib/cloudlaunch.py` & `gxabm-2.3.0/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/common.py` & `gxabm-2.3.0/abm/lib/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
             self.API_KEY = args[1]
             self.KUBECONFIG = args[2]
         else:
             raise Exception(f'Invalid args for Context. Expected one or three, found {len(args)}')
 
 
 
-def print_json(obj):
-    print(json.dumps(obj, indent=2))
+def print_json(obj, indent=2):
+    print(json.dumps(obj, indent=indent))
 
 
 def print_yaml(obj):
     get_yaml_parser().dump(obj, sys.stdout)
 
 
 def connect(context:Context):
```

### Comparing `gxabm-2.2.0/abm/lib/config.py` & `gxabm-2.3.0/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/dataset.py` & `gxabm-2.3.0/abm/lib/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from common import connect, Context
 from pprint import pprint
 from pathlib import Path
 
 import os
 import yaml
 
-
 def list(context: Context, args: list):
     gi = connect(context)
     kwargs = {
         'limit': 10000,
         'offset': 0
     }
     if len(args) > 0:
@@ -25,19 +24,18 @@
             return
     #datasets = gi.datasets.get_datasets(limit=10000, offset=0)  # , deleted=True, purged=True)
     datasets = gi.datasets.get_datasets(**kwargs)
     if len(datasets) == 0:
         print('No datasets found')
         return
     print(f'Found {len(datasets)} datasets')
-    print('ID\tHistory\tDeleted\tState\tName')
+    print('ID\tHistory\tType\tDeleted\tState\tName')
     for dataset in datasets:
         state = dataset['state'] if 'state' in dataset else 'unknown'
-        print(f"{dataset['id']}\t{dataset['history_id']}\t{dataset['deleted']}\t{state}\t{dataset['name']}")
-        #pprint(dataset)
+        print(f"{dataset['id']}\t{dataset['history_id']}\t{dataset['history_content_type']}\t{dataset['deleted']}\t{state}\t{dataset['name']}")
 
 
 def clean(context: Context, args: list):
     if len(args) == 0:
         invalid_states = ['error', 'discarded', 'unknown']
     else:
         invalid_states = args
@@ -58,14 +56,23 @@
         print("ERROR: no dataset ID provided")
         return
     gi = connect(context)
     result = gi.datasets.show_dataset(args[0])
     print(json.dumps(result, indent=4))
 
 
+def get(context: Context, args: list):
+    if len(args) == 0:
+        print("ERROR: no dataset ID provided")
+        return
+    gi = connect(context)
+    result = gi.datasets.get_datasets(args[0])
+    print(json.dumps(result, indent=4))
+
+
 def delete(context: Context, args: list):
     # gi = connect(context)
     print("dataset delete not implemented")
 
 
 def upload(context: Context, args: list):
     history = None
```

### Comparing `gxabm-2.2.0/abm/lib/experiment.py` & `gxabm-2.3.0/abm/lib/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import threading
 
 import yaml
 import json
 import helm
 import benchmark
 import logging
+import traceback
 from common import load_profiles, Context
 from time import perf_counter
 from datetime import timedelta
 
 INVOCATIONS_DIR = "invocations"
 METRICS_DIR = "metrics"
 
@@ -109,28 +110,32 @@
     make_row = make_table_row
     header_row = "Run,Cloud,Job Conf,Workflow,History,Inputs,Tool,Tool Version,State,Slots,Memory,Runtime (Sec),CPU,Memory Limit (Bytes),Memory Max usage (Bytes)"
     for arg in args:
         if arg in ['-t', '--tsv']:
             if separator is not None:
                 print('ERROR: The output format is specified more than once')
                 return
+            print('tsv')
             separator = '\t'
         elif arg in ['-c', '--csv']:
             if separator is not None:
                 print('ERROR: The output format is specified more than once')
                 return
             separator = ','
+            print('csv')
         elif arg in ['-m', '--model']:
             if separator is not None:
                 print('ERROR: The output format is specified more than once')
                 return
+            print('making a model')
             separator = ','
             make_row = make_model_row
             header_row = "job_id,tool_id,tool_version,state,memory.max_usage_in_bytes,cpuacct.usage,process_count,galaxy_slots,runtime_seconds,ref_data_size,input_data_size_1,input_data_size_2"
         else:
+            print(f"Input dir {arg}")
             input_dirs.append(arg)
 
     if len(input_dirs) == 0:
         input_dirs.append('metrics')
 
     if separator is None:
         separator = ','
@@ -138,40 +143,43 @@
     print(header_row)
     for input_dir in input_dirs:
         for file in os.listdir(input_dir):
             input_path = os.path.join(input_dir, file)
             if not os.path.isfile(input_path) or not input_path.endswith('.json'):
                 continue
             try:
+                print(f"Loading {input_path}")
                 with open(input_path, 'r') as f:
                     data = json.load(f)
-                if data['metrics']['tool_id'] == 'upload1':
+                if data['job_metrics']['tool_id'] == 'upload1':
+                    print('Ignoring upload tool')
                     continue
                 row = make_row(data)
                 print(separator.join([ str(x) for x in row]))
             except Exception as e:
                 # Silently fail to allow the remainder of the table to be generated.
-                # print(f"Unable to process {input_path}")
-                # print(e)
-                pass
+                print(f"Unable to process {input_path}")
+                print(e)
+                traceback.print_exc( )
+                #pass
 
 
 accept_metrics = ['galaxy_slots', 'galaxy_memory_mb', 'runtime_seconds', 'cpuacct.usage','memory.limit_in_bytes', 'memory.max_usage_in_bytes']  #,'memory.soft_limit_in_bytes']
 
 def make_table_row(data: dict):
     row = [ str(data[key]) for key in ['run', 'cloud', 'job_conf', 'workflow_id', 'history_id', 'inputs']]
-    row.append(parse_toolid(data['metrics']['tool_id']))
-    row.append(data['metrics']['state'])
-    for e in _get_metrics(data['metrics']['job_metrics']):
+    row.append(parse_toolid(data['job_metrics']['tool_id']))
+    row.append(data['job_metrics']['state'])
+    for e in _get_metrics(data['job_metrics']['job_metrics']):
         row.append(e)
     return row
 
 
 def make_model_row(data: dict):
-    metrics = data['metrics']
+    metrics = data['job_metrics']
     row = []
     row.append(metrics['id'])
     tool_id = metrics['tool_id']
     row.append(tool_id)
     row.append(tool_id.split('/')[-1])
     row.append(metrics['state'])
     job_metrics = parse_job_metrics(metrics['job_metrics'])
```

### Comparing `gxabm-2.2.0/abm/lib/folder.py` & `gxabm-2.3.0/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/helm.py` & `gxabm-2.3.0/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/history.py` & `gxabm-2.3.0/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/job.py` & `gxabm-2.3.0/abm/lib/job.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 import logging
 
 log = logging.getLogger('abm')
 
 
 def list(context: Context, args: list):
     state = ''
+    history_id = None
     log.debug('Processing args')
     log_state = False
     while len(args) > 0:
         arg = args.pop(0)
         if arg in ['-s', '--state', 'state']:
             if len(args) == 0:
                 print("ERROR: specify a state, eg 'ok', 'error'")
                 return
             state = args.pop(0)
             log_state = True
-
+        elif arg in ['-h', '--history']:
+            history_id = args.pop(0)
+            log.debug(f"Getting jobs from history {history_id}")
     log.debug('Connecting to the Galaxy server')
     gi = connect(context)
     if log_state:
         log.debug(f"Getting jobs with state {state}")
     else:
         log.debug("Getting job list")
-    job_list = gi.jobs.get_jobs(state=state)
+    job_list = gi.jobs.get_jobs(state=state, history_id=history_id)
     log.debug(f"Iterating over job list with {len(job_list)} items")
     for job in job_list:
         print(f"{job['id']}\t{job['state']}\t{job['update_time']}\t{job['tool_id']}")
 
 
 def show(context: Context, args: list):
     if len(args) != 1:
@@ -47,15 +50,38 @@
 
 
 def metrics(context: Context, args: list):
     if len(args) == 0:
         print("ERROR: no job ID provided")
         return
     gi = connect(context)
-    metrics = gi.jobs.get_metrics(args[0])
+    if len(args) > 1:
+        arg = args.pop(0)
+        if arg in ['-h', '--history']:
+            history_id = args.pop(0)
+            log.debug(f"Getting metrics for jobs from history {history_id}")
+            job_list = gi.jobs.get_jobs(history_id=history_id)
+            metrics = []
+            for job in job_list:
+                metrics.append({
+                    'job_id': job['id'],
+                    'job_state': job['state'],
+                    'tool_id': job['tool_id'],
+                    'job_metrics': gi.jobs.get_metrics(job['id'])
+                })
+        else:
+            print(f"ERROR: Unrecognized argument {arg}")
+    else:
+        job = gi.jobs.show_job(args[0])
+        metrics = [{
+            'job_id': job['id'],
+            'job_state': job['state'],
+            'tool_id': job['tool_id'],
+            'job_metrics': gi.jobs.get_metrics(args[0])
+        }]
     print(json.dumps(metrics, indent=4))
     # metrics = {}
     # for m in gi.jobs.get_metrics(args[0]):
     #     metrics[m['name']] = get_value(m)
     # try:
     #     print(f"{metrics['galaxy_slots']},{metrics['galaxy_memory_mb']},{metrics['runtime_seconds']}")
     # except:
@@ -74,8 +100,8 @@
 
 
 def problems(context: Context, args: list):
     if len(args) == 0:
         print('ERROR: no job ID provided.')
         return
     gi = connect(context)
-    pprint(gi.jobs.get_common_problems(args[0]))
+    pprint(gi.jobs.get_common_problems(args[0]))
```

### Comparing `gxabm-2.2.0/abm/lib/kubectl.py` & `gxabm-2.3.0/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/library.py` & `gxabm-2.3.0/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/abm/lib/menu.yml` & `gxabm-2.3.0/abm/lib/menu.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-- name: 
+- name:
     - benchmark
     - bench
   help: 'manage benchmarks'
   menu:
     - name: ['run']
       handler: benchmark.run_cli
       help: run one of the workflow configurations.  If specified the prefix will be prepended to the new history name.
@@ -11,14 +11,18 @@
       handler: benchmark.translate
       help: translate workflow and dataset ID values into names
       params: PATH
     - name: ['validate']
       handler: benchmark.validate
       help: validate that workflow and dataset names can be translated into IDs
       params: PATH
+    - name: [test]
+      handler: benchmark.test
+      help: experimental code
+      params: VARIES
 - name:
     - workflow
     - wf
   help: manage Galaxy workflows
   menu:
     - name: ['upload', 'up']
       handler: workflow.upload
@@ -51,14 +55,22 @@
       handler: workflow.publish
       help: publish a workflow
       params: ID
     - name: ['ren', 'rename']
       handler: workflow.rename
       params: "ID 'new workflow name'"
       help: "rename a workflow on the Galaxy server"
+    - name: ['invocation']
+      handler: workflow.invocation
+      params: "--workflow WORKFLOW_ID --invocation INVOCATION_ID"
+      help: show details about a specific workflow invocation
+    - name: ['inputs']
+      help: list inputs required by a workflow
+      params: WORKFLOW_ID
+      handler: workflow.inputs
     - name: ['test']
       handler: workflow.test
       help: run some test code
 - name:
     - dataset
     - ds
   help: manage datasets
@@ -82,14 +94,18 @@
       handler: dataset.find
       help: search for datasets by name
       params: NAME
     - name: ['show']
       handler: dataset.show
       params: ID
       help: show detailed information on a dataset
+    - name: ['get']
+      handler: dataset.get
+      params: NAME_OR_ID
+      help: show information for a given dataset name or ID
     - name: [cleanup, clean, clear]
       handler: dataset.clean
       params: "[STATE [STATE...]]"
       help: deletes and purges all datasets that are not 'ok'
     - name: [rename, ren]
       handler: dataset.rename
       help: rename a dataset
@@ -154,33 +170,33 @@
       params: STR
       help: delete all histories that contain STR in the name. Use * to purge all histories.
       handler: history.purge
 - name: [ jobs, job ]
   help: manage jobs on the server
   menu:
     - name: [ list, ls ]
-      help: list all jobs, or jobs in a particular state
+      help: list all jobs, or jobs in a particular state. Can filter by a history.
       handler: job.list
-      params: "[-s|--state ok|running|error|waiting]"
+      params: "[-s|--state ok|running|error|waiting] [-h|--history_id historyID]"
     - name: [ show ]
       help: show detailed information about a job
       handler: job.show
       params: ID
     - name: [problems, problem, prob]
       help: list common problems that may have caused a job to fail
       handler: job.problems
       params: ID
     - name: [cancel, kill]
       help: kills a job
       handler: job.cancel
       params: ID
     - name: [ metrics, stats ]
-      help: display runtime metrics for the job
+      help: display runtime metrics for the job, or a list of jobs contained in a history
       handler: job.metrics
-      params: ID
+      params: "[ID | -h|--history historyID]"
 - name: [users, user]
   help: manage users on the Galaxy instance
   menu:
     - name: [list, ls]
       help: list all users on the Galaxy instance
       handler: users.list
     - name: [api_key, apikey, key]
```

### Comparing `gxabm-2.2.0/abm/lib/users.py` & `gxabm-2.3.0/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/gxabm.egg-info/PKG-INFO` & `gxabm-2.3.0/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.2.0
+Version: 2.3.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.2.0/gxabm.egg-info/SOURCES.txt` & `gxabm-2.3.0/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/setup.py` & `gxabm-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/test/check_tools.py` & `gxabm-2.3.0/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.2.0/test/metrics.py` & `gxabm-2.3.0/test/metrics.py`

 * *Files identical despite different names*

