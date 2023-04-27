# Comparing `tmp/converter_package-2.9.tar.gz` & `tmp/converter_package-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/converter_package-2.9.tar", last modified: Thu Apr 27 09:50:33 2023, max compression
+gzip compressed data, was "dist/converter_package-3.0.tar", last modified: Thu Apr 27 09:57:21 2023, max compression
```

## Comparing `converter_package-2.9.tar` & `converter_package-3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 09:50:33.000000 converter_package-2.9/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 09:50:33.000000 converter_package-2.9/PKG-INFO
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      696 2023-04-27 09:50:31.000000 converter_package-2.9/setup.py
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 09:50:33.000000 converter_package-2.9/converter_package/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     7027 2023-01-23 08:59:17.000000 converter_package-2.9/converter_package/MatchingModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     1305 2022-01-25 08:53:27.000000 converter_package-2.9/converter_package/CloudFramework.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     3428 2022-11-17 10:24:26.000000 converter_package-2.9/converter_package/ComputeNode.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      666 2022-11-24 13:31:15.000000 converter_package-2.9/converter_package/ActionModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      438 2022-01-25 08:53:27.000000 converter_package-2.9/converter_package/Workflows.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      242 2022-01-25 08:53:27.000000 converter_package-2.9/converter_package/Action.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      565 2022-11-24 13:33:47.000000 converter_package-2.9/converter_package/ID.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)    91848 2023-04-27 09:50:08.000000 converter_package-2.9/converter_package/Converter.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)    11636 2023-02-01 11:10:18.000000 converter_package-2.9/converter_package/Parser.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        0 2022-07-28 09:30:38.000000 converter_package-2.9/converter_package/__init__.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     3816 2023-01-19 14:51:16.000000 converter_package-2.9/converter_package/Container.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      514 2022-01-26 10:33:29.000000 converter_package-2.9/converter_package/Image.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     1385 2022-11-24 13:33:47.000000 converter_package-2.9/converter_package/WorkflowModel.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      733 2022-01-25 08:53:27.000000 converter_package-2.9/converter_package/Repository.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      622 2022-10-13 11:01:53.000000 converter_package-2.9/converter_package/Kafka_Producer.py
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2369 2023-03-30 13:41:33.000000 converter_package-2.9/README.md
-drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 09:50:33.000000 converter_package-2.9/converter_package.egg-info/
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2022-09-13 13:10:54.000000 converter_package-2.9/converter_package.egg-info/not-zip-safe
--rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 09:50:33.000000 converter_package-2.9/converter_package.egg-info/PKG-INFO
--rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2023-04-27 09:50:33.000000 converter_package-2.9/converter_package.egg-info/dependency_links.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       18 2023-04-27 09:50:33.000000 converter_package-2.9/converter_package.egg-info/top_level.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)      732 2023-04-27 09:50:33.000000 converter_package-2.9/converter_package.egg-info/SOURCES.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       58 2023-04-27 09:50:33.000000 converter_package-2.9/converter_package.egg-info/requires.txt
--rw-rw-r--   0 giannis   (1000) giannis   (1000)       38 2023-04-27 09:50:33.000000 converter_package-2.9/setup.cfg
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 09:57:21.000000 converter_package-3.0/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 09:57:21.000000 converter_package-3.0/PKG-INFO
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      696 2023-04-27 09:57:18.000000 converter_package-3.0/setup.py
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 09:57:21.000000 converter_package-3.0/converter_package/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     7027 2023-01-23 08:59:17.000000 converter_package-3.0/converter_package/MatchingModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     1305 2022-01-25 08:53:27.000000 converter_package-3.0/converter_package/CloudFramework.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     3428 2022-11-17 10:24:26.000000 converter_package-3.0/converter_package/ComputeNode.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      666 2022-11-24 13:31:15.000000 converter_package-3.0/converter_package/ActionModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      438 2022-01-25 08:53:27.000000 converter_package-3.0/converter_package/Workflows.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      242 2022-01-25 08:53:27.000000 converter_package-3.0/converter_package/Action.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      565 2022-11-24 13:33:47.000000 converter_package-3.0/converter_package/ID.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)    91840 2023-04-27 09:57:18.000000 converter_package-3.0/converter_package/Converter.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)    11636 2023-02-01 11:10:18.000000 converter_package-3.0/converter_package/Parser.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        0 2022-07-28 09:30:38.000000 converter_package-3.0/converter_package/__init__.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     3816 2023-01-19 14:51:16.000000 converter_package-3.0/converter_package/Container.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      514 2022-01-26 10:33:29.000000 converter_package-3.0/converter_package/Image.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     1385 2022-11-24 13:33:47.000000 converter_package-3.0/converter_package/WorkflowModel.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      733 2022-01-25 08:53:27.000000 converter_package-3.0/converter_package/Repository.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      622 2022-10-13 11:01:53.000000 converter_package-3.0/converter_package/Kafka_Producer.py
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     2369 2023-03-30 13:41:33.000000 converter_package-3.0/README.md
+drwxrwxr-x   0 giannis   (1000) giannis   (1000)        0 2023-04-27 09:57:21.000000 converter_package-3.0/converter_package.egg-info/
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2022-09-13 13:10:54.000000 converter_package-3.0/converter_package.egg-info/not-zip-safe
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)     2692 2023-04-27 09:57:21.000000 converter_package-3.0/converter_package.egg-info/PKG-INFO
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)        1 2023-04-27 09:57:21.000000 converter_package-3.0/converter_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       18 2023-04-27 09:57:21.000000 converter_package-3.0/converter_package.egg-info/top_level.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)      732 2023-04-27 09:57:21.000000 converter_package-3.0/converter_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       58 2023-04-27 09:57:21.000000 converter_package-3.0/converter_package.egg-info/requires.txt
+-rw-rw-r--   0 giannis   (1000) giannis   (1000)       38 2023-04-27 09:57:21.000000 converter_package-3.0/setup.cfg
```

### Comparing `converter_package-2.9/PKG-INFO` & `converter_package-3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: converter_package
-Version: 2.9
+Version: 3.0
 Summary: This converter library is able to transform the ACCORDION application model to K3s configuration files
 Home-page: UNKNOWN
 Author: Giannis Korontanis
 Author-email: gkorod2@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `converter_package-2.9/setup.py` & `converter_package-3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(name='converter_package',
-      version='2.9',
+      version='3.0',
       description='This converter library is able to transform the ACCORDION application model to K3s configuration files',
       author='Giannis Korontanis',
       author_email='gkorod2@gmail.com',
       license='MIT',
       packages=['converter_package'],
       long_description=long_description,
       long_description_content_type='text/markdown',
```

### Comparing `converter_package-2.9/converter_package/MatchingModel.py` & `converter_package-3.0/converter_package/MatchingModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/CloudFramework.py` & `converter_package-3.0/converter_package/CloudFramework.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/ComputeNode.py` & `converter_package-3.0/converter_package/ComputeNode.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/ActionModel.py` & `converter_package-3.0/converter_package/ActionModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/ID.py` & `converter_package-3.0/converter_package/ID.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/Converter.py` & `converter_package-3.0/converter_package/Converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1178,17 +1178,17 @@
                                                 'spec': {'nodeSelector': {
                                                     'beta.kubernetes.io/os': resource.get_os(),
                                                     'beta.kubernetes.io/arch': resource.get_arch()},
                                                     'domain': {'cpu': {
                                                         'cores': int(
                                                             resource.get_cpu())},
                                                         'devices': {
+                                                            'interfaces': [{'name': 'default', 'masquerade': {},
+                                                                            'ports': ports}],
                                                             'disks': [{
-                                                                'interfaces': [{'name': 'default', 'masquerade': {},
-                                                                                'ports': ports}],
                                                                 'disk': {
                                                                     'bus': 'sata'},
                                                                 'name': 'disk0'},
                                                                 {'cdrom': {
                                                                     'bus': 'sata'},
                                                                     'name': 'virtiocontainerdisk'}
```

### Comparing `converter_package-2.9/converter_package/Parser.py` & `converter_package-3.0/converter_package/Parser.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/Container.py` & `converter_package-3.0/converter_package/Container.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/Image.py` & `converter_package-3.0/converter_package/Image.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/WorkflowModel.py` & `converter_package-3.0/converter_package/WorkflowModel.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/Repository.py` & `converter_package-3.0/converter_package/Repository.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package/Kafka_Producer.py` & `converter_package-3.0/converter_package/Kafka_Producer.py`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/README.md` & `converter_package-3.0/README.md`

 * *Files identical despite different names*

### Comparing `converter_package-2.9/converter_package.egg-info/PKG-INFO` & `converter_package-3.0/converter_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: converter-package
-Version: 2.9
+Version: 3.0
 Summary: This converter library is able to transform the ACCORDION application model to K3s configuration files
 Home-page: UNKNOWN
 Author: Giannis Korontanis
 Author-email: gkorod2@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `converter_package-2.9/converter_package.egg-info/SOURCES.txt` & `converter_package-3.0/converter_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

