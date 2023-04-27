# Comparing `tmp/sumocr-2023.1.tar.gz` & `tmp/sumocr-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumocr-2023.1.tar", last modified: Mon Jan  9 12:42:53 2023, max compression
+gzip compressed data, was "sumocr-2023.2.tar", last modified: Thu Apr 27 08:09:19 2023, max compression
```

## Comparing `sumocr-2023.1.tar` & `sumocr-2023.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/
--rw-rw-r--   0 florian   (1000) florian   (1000)     1569 2023-01-09 12:35:59.000000 sumocr-2023.1/LICENSE.txt
--rw-rw-r--   0 florian   (1000) florian   (1000)       50 2023-01-09 12:35:59.000000 sumocr-2023.1/MANIFEST.in
--rw-rw-r--   0 florian   (1000) florian   (1000)     1896 2023-01-09 12:42:53.008168 sumocr-2023.1/PKG-INFO
--rw-rw-r--   0 florian   (1000) florian   (1000)      973 2023-01-09 12:35:59.000000 sumocr-2023.1/README.md
--rw-rw-r--   0 florian   (1000) florian   (1000)       38 2023-01-09 12:42:53.008168 sumocr-2023.1/setup.cfg
--rw-rw-r--   0 florian   (1000) florian   (1000)     2062 2023-01-09 12:36:39.000000 sumocr-2023.1/setup.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumo_interface_tests/
--rw-rw-r--   0 florian   (1000) florian   (1000)       53 2023-01-09 12:35:59.000000 sumocr-2023.1/sumo_interface_tests/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     3762 2023-01-09 12:35:59.000000 sumocr-2023.1/sumo_interface_tests/conftest.py
--rw-rw-r--   0 florian   (1000) florian   (1000)      723 2023-01-09 12:35:59.000000 sumocr-2023.1/sumo_interface_tests/test_package.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/
--rw-rw-r--   0 florian   (1000) florian   (1000)      343 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/__init__.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/interface/
--rw-rw-r--   0 florian   (1000) florian   (1000)      217 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/interface/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     9146 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/interface/ego_vehicle.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     2894 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/interface/params.py
--rw-rw-r--   0 florian   (1000) florian   (1000)    50199 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/interface/sumo_simulation.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     8817 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/interface/util.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/maps/
--rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/maps/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     1758 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/maps/scenario_wrapper.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     6243 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/maps/sumo_scenario.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     8402 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/maps/util.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/sumo_config/
--rw-rw-r--   0 florian   (1000) florian   (1000)      642 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_config/.sumo.cfg
--rw-rw-r--   0 florian   (1000) florian   (1000)      166 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_config/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     8591 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_config/default.py
--rw-rw-r--   0 florian   (1000) florian   (1000)      679 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_config/pathConfig.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     1562 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_config/plot_params.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/sumo_docker/
--rw-rw-r--   0 florian   (1000) florian   (1000)      123 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/__init__.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/sumo_docker/interface/
--rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/interface/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     2494 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/interface/docker_interface.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/sumo_docker/rpc/
--rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/rpc/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     1605 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/rpc/messaging.py
--rw-rw-r--   0 florian   (1000) florian   (1000)    32095 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/rpc/sumo_client.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/sumo_docker/utils/
--rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/utils/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)    15371 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/sumo_docker/utils/docker_runner.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr/visualization/
--rw-rw-r--   0 florian   (1000) florian   (1000)       64 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/visualization/__init__.py
--rw-rw-r--   0 florian   (1000) florian   (1000)     7980 2023-01-09 12:35:59.000000 sumocr-2023.1/sumocr/visualization/video.py
-drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-01-09 12:42:53.008168 sumocr-2023.1/sumocr.egg-info/
--rw-rw-r--   0 florian   (1000) florian   (1000)     1896 2023-01-09 12:42:52.000000 sumocr-2023.1/sumocr.egg-info/PKG-INFO
--rw-rw-r--   0 florian   (1000) florian   (1000)     1096 2023-01-09 12:42:52.000000 sumocr-2023.1/sumocr.egg-info/SOURCES.txt
--rw-rw-r--   0 florian   (1000) florian   (1000)        1 2023-01-09 12:42:52.000000 sumocr-2023.1/sumocr.egg-info/dependency_links.txt
--rw-rw-r--   0 florian   (1000) florian   (1000)      337 2023-01-09 12:42:52.000000 sumocr-2023.1/sumocr.egg-info/requires.txt
--rw-rw-r--   0 florian   (1000) florian   (1000)       28 2023-01-09 12:42:52.000000 sumocr-2023.1/sumocr.egg-info/top_level.txt
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/
+-rw-rw-r--   0 florian   (1000) florian   (1000)     1569 2023-04-27 08:05:33.000000 sumocr-2023.2/LICENSE.txt
+-rw-rw-r--   0 florian   (1000) florian   (1000)       50 2023-04-27 08:05:33.000000 sumocr-2023.2/MANIFEST.in
+-rw-rw-r--   0 florian   (1000) florian   (1000)     1896 2023-04-27 08:09:19.516589 sumocr-2023.2/PKG-INFO
+-rw-rw-r--   0 florian   (1000) florian   (1000)      973 2023-04-27 08:05:33.000000 sumocr-2023.2/README.md
+-rw-rw-r--   0 florian   (1000) florian   (1000)       38 2023-04-27 08:09:19.516589 sumocr-2023.2/setup.cfg
+-rw-rw-r--   0 florian   (1000) florian   (1000)     2062 2023-04-27 08:06:42.000000 sumocr-2023.2/setup.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumo_interface_tests/
+-rw-rw-r--   0 florian   (1000) florian   (1000)       53 2023-04-27 08:05:33.000000 sumocr-2023.2/sumo_interface_tests/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     3762 2023-04-27 08:05:33.000000 sumocr-2023.2/sumo_interface_tests/conftest.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)      723 2023-04-27 08:05:33.000000 sumocr-2023.2/sumo_interface_tests/test_package.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/
+-rw-rw-r--   0 florian   (1000) florian   (1000)      343 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/__init__.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/interface/
+-rw-rw-r--   0 florian   (1000) florian   (1000)      217 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/interface/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     9146 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/interface/ego_vehicle.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     2894 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/interface/params.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)    50199 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/interface/sumo_simulation.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     8817 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/interface/util.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/maps/
+-rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/maps/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     1758 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/maps/scenario_wrapper.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     6243 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/maps/sumo_scenario.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     8402 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/maps/util.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/sumo_config/
+-rw-rw-r--   0 florian   (1000) florian   (1000)      642 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_config/.sumo.cfg
+-rw-rw-r--   0 florian   (1000) florian   (1000)      166 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_config/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     8591 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_config/default.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)      679 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_config/pathConfig.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     1562 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_config/plot_params.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/sumo_docker/
+-rw-rw-r--   0 florian   (1000) florian   (1000)      123 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/__init__.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/sumo_docker/interface/
+-rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/interface/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     2494 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/interface/docker_interface.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/sumo_docker/rpc/
+-rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/rpc/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     1605 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/rpc/messaging.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)    32095 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/rpc/sumo_client.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/sumo_docker/utils/
+-rw-rw-r--   0 florian   (1000) florian   (1000)        0 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/utils/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)    15371 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/sumo_docker/utils/docker_runner.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr/visualization/
+-rw-rw-r--   0 florian   (1000) florian   (1000)       64 2023-04-27 08:05:33.000000 sumocr-2023.2/sumocr/visualization/__init__.py
+-rw-rw-r--   0 florian   (1000) florian   (1000)     8342 2023-04-27 07:58:36.000000 sumocr-2023.2/sumocr/visualization/video.py
+drwxrwxr-x   0 florian   (1000) florian   (1000)        0 2023-04-27 08:09:19.516589 sumocr-2023.2/sumocr.egg-info/
+-rw-rw-r--   0 florian   (1000) florian   (1000)     1896 2023-04-27 08:09:19.000000 sumocr-2023.2/sumocr.egg-info/PKG-INFO
+-rw-rw-r--   0 florian   (1000) florian   (1000)     1096 2023-04-27 08:09:19.000000 sumocr-2023.2/sumocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 florian   (1000) florian   (1000)        1 2023-04-27 08:09:19.000000 sumocr-2023.2/sumocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 florian   (1000) florian   (1000)      337 2023-04-27 08:09:19.000000 sumocr-2023.2/sumocr.egg-info/requires.txt
+-rw-rw-r--   0 florian   (1000) florian   (1000)       28 2023-04-27 08:09:19.000000 sumocr-2023.2/sumocr.egg-info/top_level.txt
```

### Comparing `sumocr-2023.1/LICENSE.txt` & `sumocr-2023.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/PKG-INFO` & `sumocr-2023.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumocr
-Version: 2023.1
+Version: 2023.2
 Summary: Python tool to interface with the SUMO traffic simulator
 Home-page: https://commonroad.in.tum.de/sumo-interface
 Author: Cyber-Physical Systems Group, Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 License: BSD License
 Project-URL: Documentation, https://commonroad.in.tum.de/sumo-interface
 Project-URL: Forum, https://commonroad.in.tum.de/forum/c/sumo-interface
```

### Comparing `sumocr-2023.1/README.md` & `sumocr-2023.2/README.md`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/setup.py` & `sumocr-2023.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='sumocr',
-    version='2023.1',
+    version='2023.2',
     description='Python tool to interface with the SUMO traffic simulator',
     keywords='autonomous automated vehicles driving motion planning',
     url='https://commonroad.in.tum.de/sumo-interface',
     project_urls={
         'Documentation': 'https://commonroad.in.tum.de/sumo-interface',
         'Forum': 'https://commonroad.in.tum.de/forum/c/sumo-interface',
         'Source': 'https://gitlab.lrz.de/tum-cps/commonroad-sumo-interface',
```

### Comparing `sumocr-2023.1/sumo_interface_tests/conftest.py` & `sumocr-2023.2/sumo_interface_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumo_interface_tests/test_package.py` & `sumocr-2023.2/sumo_interface_tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/interface/ego_vehicle.py` & `sumocr-2023.2/sumocr/interface/ego_vehicle.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/interface/params.py` & `sumocr-2023.2/sumocr/interface/params.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/interface/sumo_simulation.py` & `sumocr-2023.2/sumocr/interface/sumo_simulation.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/interface/util.py` & `sumocr-2023.2/sumocr/interface/util.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/maps/scenario_wrapper.py` & `sumocr-2023.2/sumocr/maps/scenario_wrapper.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/maps/sumo_scenario.py` & `sumocr-2023.2/sumocr/maps/sumo_scenario.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/maps/util.py` & `sumocr-2023.2/sumocr/maps/util.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_config/.sumo.cfg` & `sumocr-2023.2/sumocr/sumo_config/.sumo.cfg`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_config/default.py` & `sumocr-2023.2/sumocr/sumo_config/default.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_config/pathConfig.py` & `sumocr-2023.2/sumocr/sumo_config/pathConfig.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_config/plot_params.py` & `sumocr-2023.2/sumocr/sumo_config/plot_params.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_docker/interface/docker_interface.py` & `sumocr-2023.2/sumocr/sumo_docker/interface/docker_interface.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_docker/rpc/messaging.py` & `sumocr-2023.2/sumocr/sumo_docker/rpc/messaging.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_docker/rpc/sumo_client.py` & `sumocr-2023.2/sumocr/sumo_docker/rpc/sumo_client.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/sumo_docker/utils/docker_runner.py` & `sumocr-2023.2/sumocr/sumo_docker/utils/docker_runner.py`

 * *Files identical despite different names*

### Comparing `sumocr-2023.1/sumocr/visualization/video.py` & `sumocr-2023.2/sumocr/visualization/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.prediction.prediction import TrajectoryPrediction
 from commonroad.scenario.obstacle import ObstacleType, DynamicObstacle
 from commonroad.scenario.scenario import Scenario
 from commonroad.visualization.mp_renderer import MPRenderer
+from commonroad.visualization.draw_params import MPDrawParams
 from matplotlib.animation import FuncAnimation
 
 __author__ = "Peter Kocsis, Daniel Tar, Edmond Irani Liu"
 __copyright__ = "TUM Cyber-Physical System Group"
 __credits__ = []
 __version__ = "0.1"
 __maintainer__ = "Moritz Klischat"
@@ -82,58 +83,64 @@
 
     interval = (
             1000 * scenario.dt
     )  # delay between frames in milliseconds, 1 second * dt to get actual time in ms
 
     dpi = 150
     figsize = (5, 5)
-    rnd = MPRenderer(figsize=figsize)
-    rnd.draw_params.axis_visible = False
+    draw_params = MPDrawParams()
+    draw_params.axis_visible = False
+    rnd = MPRenderer(figsize=figsize, draw_params=draw_params)
     rnd.ax.axes.get_xaxis().set_visible(False)
     (ln,) = plt.plot([], [], animated=True)
 
     def init_plot():
         plt.cla()
         if planning_problem_set is not None:
             planning_problem_set.draw(rnd)
 
         if dynamic_obstacles_ego is not None:
-            rnd.draw_params.time_begin = 0
-            rnd.draw_params.time_end = 0
-            rnd.draw_params.axis_visible = False
-            rnd.draw_params.dynamic_obstacle.vehicle_shape.occupancy.shape.facecolor = "green"
-            rnd.draw_list(dynamic_obstacles_ego)
-
-        rnd.draw_params.time_begin = 0
-        rnd.draw_params.time_end = 0
-        scenario.draw(renderer=rnd)
+            draw_params = MPDrawParams()
+            draw_params.time_begin = 0
+            draw_params.time_end = 0
+            draw_params.axis_visible = False
+            draw_params.dynamic_obstacle.vehicle_shape.occupancy.shape.facecolor = "green"
+            rnd.draw_list(dynamic_obstacles_ego, draw_params)
+
+        draw_params = MPDrawParams()
+        draw_params.time_begin = 0
+        draw_params.time_end = 0
+        scenario.draw(renderer=rnd, draw_params=draw_params)
         rnd.plot_limits = dict_plot_limits[0]
         rnd.render()
         plt.draw()
         rnd.f.tight_layout()
         return (ln,)
 
     def animate_plot(frame):
         rnd.clear(keep_static_artists=False)
         if planning_problem_set is not None:
             planning_problem_set.draw(rnd)
 
-        rnd.draw_params.time_begin = frame
-        rnd.draw_params.time_end = frame
-        rnd.draw_list(scenario.dynamic_obstacles)
+        draw_params = MPDrawParams()
+        draw_params.time_begin = frame
+        draw_params.time_end = frame
+        rnd.draw_list(scenario.dynamic_obstacles, draw_params=draw_params)
 
         if dynamic_obstacles_ego is not None:
-            rnd.draw_params.time_begin = frame
-            rnd.draw_params.time_end = frame
-            rnd.draw_params.dynamic_obstacle.vehicle_shape.occupancy.shape.facecolor = "green"
-            rnd.draw_list(dynamic_obstacles_ego)
-        
-        rnd.draw_params.time_begin = 0
-        rnd.draw_params.time_end = 0
-        scenario.lanelet_network.draw(renderer=rnd)
+            draw_params = MPDrawParams()
+            draw_params.time_begin = frame
+            draw_params.time_end = frame
+            draw_params.dynamic_obstacle.vehicle_shape.occupancy.shape.facecolor = "green"
+            rnd.draw_list(dynamic_obstacles_ego, draw_params=draw_params)
+
+        draw_params = MPDrawParams()
+        draw_params.time_begin = 0
+        draw_params.time_end = 0
+        scenario.lanelet_network.draw(renderer=rnd, draw_params=draw_params)
 
         rnd.plot_limits = dict_plot_limits[frame]
         rnd.f.tight_layout()
         rnd.render()
         return (ln,)
 
     anim = FuncAnimation(rnd.f, animate_plot, frames=frame_count, init_func=init_plot, blit=True, interval=interval)
```

### Comparing `sumocr-2023.1/sumocr.egg-info/PKG-INFO` & `sumocr-2023.2/sumocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumocr
-Version: 2023.1
+Version: 2023.2
 Summary: Python tool to interface with the SUMO traffic simulator
 Home-page: https://commonroad.in.tum.de/sumo-interface
 Author: Cyber-Physical Systems Group, Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 License: BSD License
 Project-URL: Documentation, https://commonroad.in.tum.de/sumo-interface
 Project-URL: Forum, https://commonroad.in.tum.de/forum/c/sumo-interface
```

### Comparing `sumocr-2023.1/sumocr.egg-info/SOURCES.txt` & `sumocr-2023.2/sumocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

