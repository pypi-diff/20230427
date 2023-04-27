# Comparing `tmp/citros-23.17.3.tar.gz` & `tmp/citros-23.17.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.17.3.tar", last modified: Thu Apr 27 13:02:03 2023, max compression
+gzip compressed data, was "citros-23.17.4.tar", last modified: Thu Apr 27 13:23:49 2023, max compression
```

## Comparing `citros-23.17.3.tar` & `citros-23.17.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.846699 citros-23.17.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 13:01:47.000000 citros-23.17.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 13:02:03.842699 citros-23.17.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 13:01:47.000000 citros-23.17.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-27 13:01:47.000000 citros-23.17.3/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 13:01:47.000000 citros-23.17.3/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 13:01:47.000000 citros-23.17.3/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 13:01:47.000000 citros-23.17.3/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 13:01:47.000000 citros-23.17.3/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 13:01:47.000000 citros-23.17.3/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 13:01:47.000000 citros-23.17.3/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 13:01:47.000000 citros-23.17.3/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:01:47.000000 citros-23.17.3/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 13:01:47.000000 citros-23.17.3/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 13:01:47.000000 citros-23.17.3/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:02:03.846699 citros-23.17.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 13:01:47.000000 citros-23.17.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:47.000000 citros-23.17.3/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:47.000000 citros-23.17.3/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 13:23:31.000000 citros-23.17.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 13:23:49.161410 citros-23.17.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 13:23:31.000000 citros-23.17.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.157410 citros-23.17.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-27 13:23:31.000000 citros-23.17.4/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 13:23:31.000000 citros-23.17.4/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 13:23:31.000000 citros-23.17.4/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-27 13:23:31.000000 citros-23.17.4/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 13:23:31.000000 citros-23.17.4/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 13:23:31.000000 citros-23.17.4/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 13:23:31.000000 citros-23.17.4/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-27 13:23:31.000000 citros-23.17.4/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 13:23:31.000000 citros-23.17.4/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 13:23:31.000000 citros-23.17.4/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 13:23:31.000000 citros-23.17.4/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 13:23:31.000000 citros-23.17.4/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 13:23:31.000000 citros-23.17.4/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 13:23:31.000000 citros-23.17.4/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 13:23:31.000000 citros-23.17.4/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:23:31.000000 citros-23.17.4/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 13:23:31.000000 citros-23.17.4/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 13:23:31.000000 citros-23.17.4/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 13:23:31.000000 citros-23.17.4/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 13:23:31.000000 citros-23.17.4/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 13:23:31.000000 citros-23.17.4/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 13:23:49.000000 citros-23.17.4/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 13:23:49.000000 citros-23.17.4/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:23:49.000000 citros-23.17.4/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 13:23:49.000000 citros-23.17.4/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:23:49.000000 citros-23.17.4/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 13:23:31.000000 citros-23.17.4/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:23:49.161410 citros-23.17.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 13:23:31.000000 citros-23.17.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:49.161410 citros-23.17.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:31.000000 citros-23.17.4/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:23:31.000000 citros-23.17.4/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.17.3/LICENSE` & `citros-23.17.4/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/PKG-INFO` & `citros-23.17.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.3
+Version: 23.17.4
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.3/README.md` & `citros-23.17.4/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/bin/citros` & `citros-23.17.4/bin/citros`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 def logout(args, argv):
     citros = Citros()  
     citros.logout()        
 
 def sync_project(args, argv):             
     citros = Citros()   
     if not citros.isAuthenticated():
-        print("please log in first!")
+        print("sync_project: please log in first!")
         return
     project_data = citros.parser_ros2.parse(args.dir, args.name, args.ws)
     # print("sync_project:project: ", json.dumps(project_data, indent=2))
     citros.integration.sync_project(project_data)
 
 def run_simulation(simulation_id, repeats):    
     # TODO: create new batch for this simulation
@@ -104,18 +104,18 @@
     """
     print_citros()
     
     citros = Citros()
     if args.key:
         loggedin = citros.authenticate_with_key(args.key)
         if not loggedin:
-            sys.exit("please log in first!")            
+            sys.exit("run_ros2_project.authenticate_with_key: please log in first!")            
         
     if not citros.isAuthenticated():
-        sys.exit("please log in first!")             
+        sys.exit("run_ros2_project: please log in first!")             
     
     # k8s indexed batch job is passing the index with JOB_COMPLETION_INDEX env variable.
     if args.sid == "JOB_COMPLETION_INDEX":
         args.sid = config("JOB_COMPLETION_INDEX", "bad-value-from-k8s")
         print(f"got JOB_COMPLETION_INDEX={args.sid} from k8s.")
     
     if (args.sid == ''):
@@ -128,25 +128,25 @@
     run_simulation_run(args.batch_run_id, args.sid, str(args.timeout))
     sys.exit(0)
     
 # experimental:
 def load_params(args, argv):
     citros = Citros()
     if not citros.isAuthenticated():
-        print("please log in first!")
+        print("load_params: please log in first!")
         return
     # TODO: source the ros project to env terminal
     citros.params.init_params(args.batch_run_id, args.sid)
 
 # experimental:
 def upload_bag(args, argv): 
     # print("upload_bag")
     citros = Citros()
     if not citros.isAuthenticated():
-        print("please log in first!")
+        print("upload_bag: please log in first!")
         return
     bag_resp, batch_text, resp_json = citros.bag.emit(args.bag, args.batch_run_id, args.sid)        
     print("bag_resp, ", bag_resp)
     print("batch_text", batch_text)
     print("resp_json", resp_json)
     
 def docker_login(argx, argv):
@@ -171,15 +171,15 @@
     args.runs - how many query's to send,
     args.sleep - how much sleep between sends. 
     """      
     print("Starting stress test for citros.")
     
     citros = Citros(batch_run_id=args.batch_run_id, simulation_run_id=args.sid)    
     if not citros.isAuthenticated():
-        print("please log in first!")
+        print("stress_user_db: please log in first!")
         return
     
     print(f"sending {args.runs} log messages.")
     for i in range(1, int(args.runs) + 1):
         # print(f"sending {i} message.")
         citros.events.creating("72311c81-5992-431a-9373-81aa2bdb3fe1", "2", "vova", "stress test", "")
         # citros.log.debug(f"{i} - sending message.")
```

### Comparing `citros-23.17.3/citros/__init__.py` & `citros-23.17.4/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/citros.py` & `citros-23.17.4/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/citros_bag.py` & `citros-23.17.4/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/citros_batch.py` & `citros-23.17.4/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/citros_events.py` & `citros-23.17.4/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/citros_integration.py` & `citros-23.17.4/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/citros_params.py` & `citros-23.17.4/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/citros_utils.py` & `citros-23.17.4/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/launches/__init__.py` & `citros-23.17.4/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/launches/launch.py` & `citros-23.17.4/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/logger/__init__.py` & `citros-23.17.4/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/logger/logger.py` & `citros-23.17.4/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/logger/logger_pg_handler.py` & `citros-23.17.4/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/parsers/__init__.py` & `citros-23.17.4/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/parsers/parser_ros2.py` & `citros-23.17.4/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/rosbag/__init__.py` & `citros-23.17.4/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/rosbag/reader_base.py` & `citros-23.17.4/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/rosbag/reader_mcap.py` & `citros-23.17.4/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros/rosbag/reader_sqlite.py` & `citros-23.17.4/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/citros.egg-info/PKG-INFO` & `citros-23.17.4/citros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.3
+Version: 23.17.4
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.3/citros.egg-info/SOURCES.txt` & `citros-23.17.4/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.17.3/setup.py` & `citros-23.17.4/setup.py`

 * *Files identical despite different names*

