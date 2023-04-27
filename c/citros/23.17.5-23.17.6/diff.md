# Comparing `tmp/citros-23.17.5.tar.gz` & `tmp/citros-23.17.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.17.5.tar", last modified: Thu Apr 27 14:04:46 2023, max compression
+gzip compressed data, was "citros-23.17.6.tar", last modified: Thu Apr 27 14:17:28 2023, max compression
```

## Comparing `citros-23.17.5.tar` & `citros-23.17.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.881673 citros-23.17.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 14:04:26.000000 citros-23.17.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 14:04:46.881673 citros-23.17.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 14:04:26.000000 citros-23.17.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.877673 citros-23.17.5/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-04-27 14:04:26.000000 citros-23.17.5/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.877673 citros-23.17.5/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 14:04:26.000000 citros-23.17.5/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 14:04:26.000000 citros-23.17.5/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-27 14:04:26.000000 citros-23.17.5/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 14:04:26.000000 citros-23.17.5/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 14:04:26.000000 citros-23.17.5/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 14:04:26.000000 citros-23.17.5/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-27 14:04:26.000000 citros-23.17.5/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 14:04:26.000000 citros-23.17.5/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.881673 citros-23.17.5/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 14:04:26.000000 citros-23.17.5/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 14:04:26.000000 citros-23.17.5/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.881673 citros-23.17.5/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 14:04:26.000000 citros-23.17.5/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 14:04:26.000000 citros-23.17.5/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 14:04:26.000000 citros-23.17.5/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.881673 citros-23.17.5/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 14:04:26.000000 citros-23.17.5/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 14:04:26.000000 citros-23.17.5/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 14:04:26.000000 citros-23.17.5/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.881673 citros-23.17.5/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 14:04:26.000000 citros-23.17.5/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 14:04:26.000000 citros-23.17.5/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 14:04:26.000000 citros-23.17.5/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 14:04:26.000000 citros-23.17.5/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.881673 citros-23.17.5/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 14:04:46.000000 citros-23.17.5/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 14:04:46.000000 citros-23.17.5/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:04:46.000000 citros-23.17.5/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 14:04:46.000000 citros-23.17.5/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 14:04:46.000000 citros-23.17.5/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 14:04:26.000000 citros-23.17.5/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:04:46.881673 citros-23.17.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 14:04:26.000000 citros-23.17.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:46.881673 citros-23.17.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:26.000000 citros-23.17.5/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:04:26.000000 citros-23.17.5/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.237180 citros-23.17.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 14:17:11.000000 citros-23.17.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 14:17:28.237180 citros-23.17.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 14:17:11.000000 citros-23.17.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.233180 citros-23.17.6/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-04-27 14:17:11.000000 citros-23.17.6/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.233180 citros-23.17.6/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 14:17:11.000000 citros-23.17.6/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 14:17:11.000000 citros-23.17.6/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-27 14:17:11.000000 citros-23.17.6/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 14:17:11.000000 citros-23.17.6/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 14:17:11.000000 citros-23.17.6/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 14:17:11.000000 citros-23.17.6/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-04-27 14:17:11.000000 citros-23.17.6/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 14:17:11.000000 citros-23.17.6/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.237180 citros-23.17.6/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 14:17:11.000000 citros-23.17.6/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 14:17:11.000000 citros-23.17.6/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.237180 citros-23.17.6/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 14:17:11.000000 citros-23.17.6/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 14:17:11.000000 citros-23.17.6/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 14:17:11.000000 citros-23.17.6/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.237180 citros-23.17.6/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 14:17:11.000000 citros-23.17.6/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 14:17:11.000000 citros-23.17.6/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 14:17:11.000000 citros-23.17.6/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.237180 citros-23.17.6/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 14:17:11.000000 citros-23.17.6/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 14:17:11.000000 citros-23.17.6/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 14:17:11.000000 citros-23.17.6/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 14:17:11.000000 citros-23.17.6/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.237180 citros-23.17.6/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 14:17:28.000000 citros-23.17.6/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 14:17:28.000000 citros-23.17.6/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:17:28.000000 citros-23.17.6/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 14:17:28.000000 citros-23.17.6/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 14:17:28.000000 citros-23.17.6/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 14:17:11.000000 citros-23.17.6/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:17:28.237180 citros-23.17.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 14:17:11.000000 citros-23.17.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:28.237180 citros-23.17.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:11.000000 citros-23.17.6/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:11.000000 citros-23.17.6/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.17.5/LICENSE` & `citros-23.17.6/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/PKG-INFO` & `citros-23.17.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.5
+Version: 23.17.6
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.5/README.md` & `citros-23.17.6/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/bin/citros` & `citros-23.17.6/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/__init__.py` & `citros-23.17.6/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/citros.py` & `citros-23.17.6/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/citros_bag.py` & `citros-23.17.6/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/citros_batch.py` & `citros-23.17.6/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/citros_events.py` & `citros-23.17.6/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/citros_integration.py` & `citros-23.17.6/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/citros_params.py` & `citros-23.17.6/citros/citros_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         }
         """
         result = self.citros.gql_execute(query, variable_values={"batchRunId": batch_run_id, "sid": sid})        
         return result
    
     def _coercion(self, value, type):
         if type == "FLOAT":
-            return float(value)                                                
+            return float(value)
         return value
         
     def _eval_distribution(self, parameter_setting):
         import numpy as np
 
         distribution_type = parameter_setting["distType"]
         param1 = parameter_setting["param1"]
@@ -131,15 +131,20 @@
             self.log.error("ERROR! Cant get parameters from CiTROS. There is no simulation attached to batch.")  
             return     
               
         # users parametre setup
         parameter_settings_list = data["batchRun"]["simulation"]["parameterSetup"]["parameterSettingsList"]        
         paramValues = {} 
         for ps in parameter_settings_list:
-            paramValues[str(ps["nodeParameterId"])] = self._eval_distribution(ps)
+            try:
+                paramValues[str(ps["nodeParameterId"])] = self._eval_distribution(ps)
+            except Exception as e:
+                self.log.error(f"Error in _eval_distribution, parameter_settings_list: [{json.dumps(ps, indent=4)}]")
+                # self.log.excption(e)
+                raise e
         
         # load defaults from ros nodes. 
         ros_packages_list = data["batchRun"]["simulation"]["project"]["rosPackagesList"]
         config = {}   
         for package in ros_packages_list:
             config[package["name"]] = {}
             for node in package["rosNodesByPackageIdList"]:
```

### Comparing `citros-23.17.5/citros/citros_utils.py` & `citros-23.17.6/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/launches/__init__.py` & `citros-23.17.6/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/launches/launch.py` & `citros-23.17.6/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/logger/__init__.py` & `citros-23.17.6/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/logger/logger.py` & `citros-23.17.6/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/logger/logger_pg_handler.py` & `citros-23.17.6/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/parsers/__init__.py` & `citros-23.17.6/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/parsers/parser_ros2.py` & `citros-23.17.6/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/rosbag/__init__.py` & `citros-23.17.6/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/rosbag/reader_base.py` & `citros-23.17.6/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/rosbag/reader_mcap.py` & `citros-23.17.6/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros/rosbag/reader_sqlite.py` & `citros-23.17.6/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/citros.egg-info/PKG-INFO` & `citros-23.17.6/citros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.5
+Version: 23.17.6
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.5/citros.egg-info/SOURCES.txt` & `citros-23.17.6/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.17.5/setup.py` & `citros-23.17.6/setup.py`

 * *Files identical despite different names*

