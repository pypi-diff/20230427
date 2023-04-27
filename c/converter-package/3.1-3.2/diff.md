# Comparing `tmp/converter_package-3.1.tar.gz` & `tmp/converter_package-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/converter_package-3.1.tar", last modified: Thu Apr 27 10:10:18 2023, max compression
+gzip compressed data, was "dist/converter_package-3.2.tar", last modified: Thu Apr 27 10:14:43 2023, max compression
```

## Comparing `converter_package-3.1.tar` & `converter_package-3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:10:18.000000 converter_package-3.1/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 10:10:18.000000 converter_package-3.1/PKG-INFO
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      696 2023-04-27 10:10:17.000000 converter_package-3.1/setup.py
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:10:18.000000 converter_package-3.1/converter_package/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     7027 2023-01-23 08:59:17.000000 converter_package-3.1/converter_package/MatchingModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     1305 2022-01-25 08:53:27.000000 converter_package-3.1/converter_package/CloudFramework.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     3428 2022-11-17 10:24:26.000000 converter_package-3.1/converter_package/ComputeNode.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      666 2022-11-24 13:31:15.000000 converter_package-3.1/converter_package/ActionModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      438 2022-01-25 08:53:27.000000 converter_package-3.1/converter_package/Workflows.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      242 2022-01-25 08:53:27.000000 converter_package-3.1/converter_package/Action.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      565 2022-11-24 13:33:47.000000 converter_package-3.1/converter_package/ID.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)    92055 2023-04-27 10:09:28.000000 converter_package-3.1/converter_package/Converter.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)    11636 2023-02-01 11:10:18.000000 converter_package-3.1/converter_package/Parser.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        0 2022-07-28 09:30:38.000000 converter_package-3.1/converter_package/__init__.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     3816 2023-01-19 14:51:16.000000 converter_package-3.1/converter_package/Container.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      514 2022-01-26 10:33:29.000000 converter_package-3.1/converter_package/Image.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     1385 2022-11-24 13:33:47.000000 converter_package-3.1/converter_package/WorkflowModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      733 2022-01-25 08:53:27.000000 converter_package-3.1/converter_package/Repository.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      622 2022-10-13 11:01:53.000000 converter_package-3.1/converter_package/Kafka_Producer.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2369 2023-03-30 13:41:33.000000 converter_package-3.1/README.md
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:10:18.000000 converter_package-3.1/converter_package.egg-info/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2022-09-13 13:10:54.000000 converter_package-3.1/converter_package.egg-info/not-zip-safe
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 10:10:18.000000 converter_package-3.1/converter_package.egg-info/PKG-INFO
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2023-04-27 10:10:18.000000 converter_package-3.1/converter_package.egg-info/dependency_links.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       18 2023-04-27 10:10:18.000000 converter_package-3.1/converter_package.egg-info/top_level.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      732 2023-04-27 10:10:18.000000 converter_package-3.1/converter_package.egg-info/SOURCES.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       58 2023-04-27 10:10:18.000000 converter_package-3.1/converter_package.egg-info/requires.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       38 2023-04-27 10:10:18.000000 converter_package-3.1/setup.cfg
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:14:43.000000 converter_package-3.2/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 10:14:43.000000 converter_package-3.2/PKG-INFO
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      696 2023-04-27 10:14:39.000000 converter_package-3.2/setup.py
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     7027 2023-01-23 08:59:17.000000 converter_package-3.2/converter_package/MatchingModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     1305 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/CloudFramework.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     3428 2022-11-17 10:24:26.000000 converter_package-3.2/converter_package/ComputeNode.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      666 2022-11-24 13:31:15.000000 converter_package-3.2/converter_package/ActionModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      438 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/Workflows.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      242 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/Action.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      565 2022-11-24 13:33:47.000000 converter_package-3.2/converter_package/ID.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)    91997 2023-04-27 10:14:19.000000 converter_package-3.2/converter_package/Converter.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)    11636 2023-02-01 11:10:18.000000 converter_package-3.2/converter_package/Parser.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        0 2022-07-28 09:30:38.000000 converter_package-3.2/converter_package/__init__.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     3816 2023-01-19 14:51:16.000000 converter_package-3.2/converter_package/Container.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      514 2022-01-26 10:33:29.000000 converter_package-3.2/converter_package/Image.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     1385 2022-11-24 13:33:47.000000 converter_package-3.2/converter_package/WorkflowModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      733 2022-01-25 08:53:27.000000 converter_package-3.2/converter_package/Repository.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      622 2022-10-13 11:01:53.000000 converter_package-3.2/converter_package/Kafka_Producer.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     2369 2023-03-30 13:41:33.000000 converter_package-3.2/README.md
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2022-09-13 13:10:54.000000 converter_package-3.2/converter_package.egg-info/not-zip-safe
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/PKG-INFO
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       18 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/top_level.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      732 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       58 2023-04-27 10:14:43.000000 converter_package-3.2/converter_package.egg-info/requires.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       38 2023-04-27 10:14:43.000000 converter_package-3.2/setup.cfg
```

### Comparing `converter_package-3.1/PKG-INFO` & `converter_package-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: converter_package
-Version: 3.1
+Version: 3.2
 Summary: This converter library is able to transform the ACCORDION application model to K3s configuration files
 Home-page: UNKNOWN
 Author: Giannis Korontanis
 Author-email: gkorod2@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `converter_package-3.1/setup.py` & `converter_package-3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(name='converter_package',
-      version='3.1',
+      version='3.2',
       description='This converter library is able to transform the ACCORDION application model to K3s configuration files',
       author='Giannis Korontanis',
       author_email='gkorod2@gmail.com',
       license='MIT',
       packages=['converter_package'],
       long_description=long_description,
       long_description_content_type='text/markdown',
```

### Comparing `converter_package-3.1/converter_package/MatchingModel.py` & `converter_package-3.2/converter_package/MatchingModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/CloudFramework.py` & `converter_package-3.2/converter_package/CloudFramework.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/ComputeNode.py` & `converter_package-3.2/converter_package/ComputeNode.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/ActionModel.py` & `converter_package-3.2/converter_package/ActionModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/ID.py` & `converter_package-3.2/converter_package/ID.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/Converter.py` & `converter_package-3.2/converter_package/Converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1132,30 +1132,30 @@
                                                                 'disk': {
                                                                     'bus': 'sata'},
                                                                 'name': 'disk0'},
                                                                 {'cdrom': {
                                                                     'bus': 'sata'},
                                                                     'name': 'virtiocontainerdisk'}
 
-                                                            ]}, 'networks': [{'name': 'default', 'pod': {}}],
+                                                            ]},
                                                         'machine': {
                                                             'type': 'q35'},
                                                         'resources': {
                                                             'requests': {
                                                                 'memory': resource.get_mem()}}},
                                                     'volumes': [
                                                         {
                                                             'name': 'disk0',
                                                             'persistentVolumeClaim': {
                                                                 'claimName': dv}},
                                                         {
                                                             'name': 'virtiocontainerdisk',
                                                             'containerDisk': {
                                                                 'image': 'kubevirt/virtio-container-disk'}},
-                                                    ]}}}}}
+                                                    ],'networks': [{'name': 'default', 'pod': {}}]}}}}}
                                 deployment = extra_labels(deployment, resource.get_gpu_brand(),
                                                           resource.get_gpu_dedicated(), resource.get_wifi_antenna())
                             else:
                                 gpu_model = gpu.get('gpu_model')
                                 deployment = {
                                     application_instance + "-" + x.get_name() + "-" + minicloud: {
                                         'apiVersion': 'kubevirt.io/v1',
@@ -1191,30 +1191,29 @@
                                                                 'name': 'disk0'},
                                                                 {'cdrom': {
                                                                     'bus': 'sata'},
                                                                     'name': 'virtiocontainerdisk'}
 
                                                             ], 'gpus': [
                                                                 {'name': 'gpu1', 'deviceName': gpu_model}]},
-                                                        'networks': [{'name': 'default', 'pod': {}}],
                                                         'machine': {
                                                             'type': 'q35'},
                                                         'resources': {
                                                             'requests': {
                                                                 'memory': resource.get_mem()}}},
                                                     'volumes': [
                                                         {
                                                             'name': 'disk0',
                                                             'persistentVolumeClaim': {
                                                                 'claimName': dv}},
                                                         {
                                                             'name': 'virtiocontainerdisk',
                                                             'containerDisk': {
                                                                 'image': 'kubevirt/virtio-container-disk'}},
-                                                    ]}}}}}
+                                                    ],'networks': [{'name': 'default', 'pod': {}}]}}}}}
 
                                 deployment = extra_labels(deployment, resource.get_gpu_brand(),
                                                           resource.get_gpu_dedicated(), resource.get_wifi_antenna())
                         deployment_files.append(deployment)
     if vm_flag:
         exporter_service = {
             application_instance + "-" + x.get_name() + "-" + minicloud + "-exporter-service": {
```

### Comparing `converter_package-3.1/converter_package/Parser.py` & `converter_package-3.2/converter_package/Parser.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/Container.py` & `converter_package-3.2/converter_package/Container.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/Image.py` & `converter_package-3.2/converter_package/Image.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/WorkflowModel.py` & `converter_package-3.2/converter_package/WorkflowModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/Repository.py` & `converter_package-3.2/converter_package/Repository.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package/Kafka_Producer.py` & `converter_package-3.2/converter_package/Kafka_Producer.py`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/README.md` & `converter_package-3.2/README.md`

 * *Files identical despite different names*

### Comparing `converter_package-3.1/converter_package.egg-info/PKG-INFO` & `converter_package-3.2/converter_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: converter-package
-Version: 3.1
+Version: 3.2
 Summary: This converter library is able to transform the ACCORDION application model to K3s configuration files
 Home-page: UNKNOWN
 Author: Giannis Korontanis
 Author-email: gkorod2@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `converter_package-3.1/converter_package.egg-info/SOURCES.txt` & `converter_package-3.2/converter_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

