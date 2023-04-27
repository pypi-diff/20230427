# Comparing `tmp/citros-23.14.9.tar.gz` & `tmp/citros-23.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.14.9.tar", last modified: Sun Apr  9 17:05:07 2023, max compression
+gzip compressed data, was "citros-23.17.1.tar", last modified: Thu Apr 27 06:01:28 2023, max compression
```

## Comparing `citros-23.14.9.tar` & `citros-23.17.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 17:04:53.000000 citros-23.14.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 17:05:07.648701 citros-23.14.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-09 17:04:53.000000 citros-23.14.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.644701 citros-23.14.9/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 17:04:53.000000 citros-23.14.9/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 17:04:53.000000 citros-23.14.9/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 17:04:53.000000 citros-23.14.9/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-04-09 17:04:53.000000 citros-23.14.9/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 17:04:53.000000 citros-23.14.9/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-09 17:04:53.000000 citros-23.14.9/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 17:04:53.000000 citros-23.14.9/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 17:04:53.000000 citros-23.14.9/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 17:04:53.000000 citros-23.14.9/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 17:04:53.000000 citros-23.14.9/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 17:04:53.000000 citros-23.14.9/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 17:04:53.000000 citros-23.14.9/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 17:04:53.000000 citros-23.14.9/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 17:04:53.000000 citros-23.14.9/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 17:04:53.000000 citros-23.14.9/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 17:04:53.000000 citros-23.14.9/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-09 17:04:53.000000 citros-23.14.9/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 17:04:53.000000 citros-23.14.9/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 17:04:53.000000 citros-23.14.9/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 17:04:53.000000 citros-23.14.9/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 17:04:53.000000 citros-23.14.9/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 17:05:07.000000 citros-23.14.9/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 17:05:07.000000 citros-23.14.9/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:05:07.000000 citros-23.14.9/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 17:05:07.000000 citros-23.14.9/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 17:05:07.000000 citros-23.14.9/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 17:04:53.000000 citros-23.14.9/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:05:07.648701 citros-23.14.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 17:04:53.000000 citros-23.14.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:05:07.648701 citros-23.14.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:53.000000 citros-23.14.9/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:04:53.000000 citros-23.14.9/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.560340 citros-23.17.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 06:01:12.000000 citros-23.17.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 06:01:28.560340 citros-23.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 06:01:12.000000 citros-23.17.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-27 06:01:12.000000 citros-23.17.1/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 06:01:12.000000 citros-23.17.1/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 06:01:12.000000 citros-23.17.1/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 06:01:12.000000 citros-23.17.1/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 06:01:12.000000 citros-23.17.1/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 06:01:12.000000 citros-23.17.1/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 06:01:12.000000 citros-23.17.1/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 06:01:12.000000 citros-23.17.1/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 06:01:12.000000 citros-23.17.1/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 06:01:12.000000 citros-23.17.1/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.560340 citros-23.17.1/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 06:01:12.000000 citros-23.17.1/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:01:28.560340 citros-23.17.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 06:01:12.000000 citros-23.17.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.560340 citros-23.17.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:12.000000 citros-23.17.1/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:12.000000 citros-23.17.1/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.14.9/LICENSE` & `citros-23.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/PKG-INFO` & `citros-23.17.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.9
+Version: 23.17.1
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.9/README.md` & `citros-23.17.1/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/bin/citros` & `citros-23.17.1/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/__init__.py` & `citros-23.17.1/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/citros.py` & `citros-23.17.1/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/citros_bag.py` & `citros-23.17.1/citros/citros_bag.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
                     print(f"[{datetime.datetime.now()}] - uploading config [{config_file}]")
                     
                     record_to_insert = {
                         "sid": simulation_run_id,
                         "rid": rid_counter,
                         "time": 0,
                         "topic": '/config',
-                        "type": config_file.split('.')[0],
+                        "type": 'params',
+                        # "type": config_file.split('.')[0],
                         "data": json.dumps(config_dict)
                     }
                     rid_counter = rid_counter + 1
                     
                     cursor.execute(postgres_insert_query, record_to_insert)                                                        
                     connection.commit()                
                       
@@ -171,26 +172,35 @@
                 size = buffer.seek(0, os.SEEK_END)
                 size = buffer.tell()
                 total_size = total_size + size
                 buffer.seek(0)                
                 print(f"[{datetime.datetime.now()}] \tinserting buffer size: { (size / 1024 ) / 1024 } MB", flush=True)
                 if size == 0:
                     continue
-                cursor.execute(f'SET search_path TO data_bucket')                
-                cursor.copy_from(buffer, batch_run_id, sep=chr(0x1E), columns=['sid', 'rid', 'time', 'topic', 'type', 'data'])                
+                cursor.execute(f'SET search_path TO data_bucket')
+                try:           
+                    cursor.copy_from(buffer, batch_run_id, sep=chr(0x1E), null="", columns=['sid', 'rid', 'time', 'topic', 'type', 'data'])                
+                except (Exception, psycopg2.Error) as error:
+                    buffer.seek(0)                      
+                    print(f"[{datetime.datetime.now()}] Failed to insert record into table, aboring uploading to PG DB.", error) 
+                    print(traceback.format_exc())
+                    # print("===============================================================================================")
+                    # print(buffer.getvalue())
+                    # print("===============================================================================================")
+                    return False, "got exception from pgdb", str(error)
                 # buffer.truncate(0)
                 # buffer.seek(0)
                 # buffer.close()
                 connection.commit()
             print(f"[{datetime.datetime.now()}] --- done uploading to PG", flush=True)
             return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}] to Postgres. [size: {(total_size / 1024)/1024} MB]", None
         except (Exception, psycopg2.Error) as error:
             print(f"[{datetime.datetime.now()}] Failed to insert record into table, aboring uploading to PG DB.", error) 
             print(traceback.format_exc())
-            return False, "go exception from pgdb", str(error)
+            return False, "got exception from pgdb", str(error)
         finally:
             # closing database connection.
             if connection:
                 cursor.close()
                 connection.close()
                 print(f"[{datetime.datetime.now()}] PostgreSQL connection is closed")
```

### Comparing `citros-23.14.9/citros/citros_batch.py` & `citros-23.17.1/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/citros_events.py` & `citros-23.17.1/citros/citros_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,16 +116,21 @@
         :param batch_run_id: batch run id
         :param sid: sequence-id of the simulation 
         :param event: event type
         :param tag: tag - can be any string
         :param message: a message for the event
         :param metadata: some dict object containing metadata.
         
-        
         """
+        try:
+            if type(metadata) == dict:
+                metadata = json.dumps(metadata)
+        except Exception as e:
+            print(e)
+                                    
         event = {
             "batch_run_id":batch_run_id, 
             "sid": sid, 
             "event":event_type, 
             "tag":tag, 
             "message":message,
             "metadata":metadata,
```

### Comparing `citros-23.14.9/citros/citros_integration.py` & `citros-23.17.1/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/citros_params.py` & `citros-23.17.1/citros/citros_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,34 +167,34 @@
             self.log.debug(f"Saving config for {package_name}")                               
             # TODO: add other method to get the package path
             path_to_package = None
             try:
                 path_to_package = get_package_share_directory(package_name) # get the path to the package install directory - the project must be sourced for it to work            
             except Exception as e:
                 self.log.exception(e)
-                return 
+                continue                
 
             if not path_to_package:
-                return
+                continue
                 
             path = f"{path_to_package}/config/"    
             
             # check if folder exists
             if not Path(path).exists():
                 self.log.debug(f"No config file {path} exits for pack:{package_name}. passing.") 
-                return
+                continue
                                                 
             # path = f"install/{package_name}/share/{package_name}/config/"
             Path(path).mkdir(parents=True, exist_ok=True)
             path = path + "params.yaml"
             
             # check if file exists?
             if not Path(path).exists():
                 self.log.debug(f"No config file {path} exits for pack:{package_name}. passing.") 
-                return
+                continue
             
             self.log.debug(f"Loading default config from {path}") 
             with open(path, "r") as stream:
                 try:    
                     default_config = yaml.safe_load(stream)
                 except yaml.YAMLError as exc:
                     print(exc)
@@ -206,20 +206,19 @@
                 yaml.dump(merged_config, file)  
                 
             # save for metadata
             with open(f"{self.CONFIG_FOLDER}/{package_name}.yaml", 'w') as file:                                     
                 yaml.dump(merged_config, file) 
         self.log.debug("Saved config to project") 
     
-    def init_params(self, batch_run_id, sid):
-        # TODO:[ ] if rerunning existing simulation- load last generated params from DB.
-        
+    def init_params(self, batch_run_id, sid):                
         self.log.debug("Getting parameters from CITROS.") 
         config = self.get_config(batch_run_id, sid)
         if not config:
-            # if there is no config cant init anything...
+            # if there is no config, cant init anything...
+            self.log.warning("If there is no config, cant init anything...") 
             return
-        self.log.debug("Saving parameters to files. ") 
+        self.log.debug("Saving parameters to files. ")
         
         self.save_config(config)                        
         return config
```

### Comparing `citros-23.14.9/citros/citros_utils.py` & `citros-23.17.1/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/launches/__init__.py` & `citros-23.17.1/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/launches/launch.py` & `citros-23.17.1/citros/launches/launch.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,42 +16,40 @@
 ################################
 # Entrypoint        
 ################################
 def generate_launch_description(batch_run_id, simulation_run_id, timeout):  
     batch_run_id = str(batch_run_id)    
     simulation_run_id = str(simulation_run_id)    
     timeout = str(timeout)    
-    print("[DEBUG] + generate_launch_description()")
-    print("[DEBUG] batch_run_id: ", batch_run_id)
-    print("[DEBUG] simulation_run_id: ", simulation_run_id)
-    print("[DEBUG] timeout: ", timeout)
+    citros.log.debug("+ generate_launch_description()")
+    citros.log.debug("batch_run_id: ", batch_run_id)
+    citros.log.debug("simulation_run_id: ", simulation_run_id)
+    citros.log.debug("timeout: ", timeout)
     
     citros = Citros(batch_run_id, simulation_run_id)
     resp = citros.checkStatus()
     if not resp:        
         return 
-    print("[DEBUG] Health-check: OK")
-    citros.events.init(batch_run_id=batch_run_id, sid=simulation_run_id, tag="INIT", message="updated config", metadata={})
+    citros.log.debug("Health-check: OK")
+    citros.events.init(batch_run_id=batch_run_id, sid=simulation_run_id, tag="INIT", message="updated config", metadata=None)
     
     ld = LaunchDescription([
         LogInfo(msg='CITROS launch file!')
     ])
     ld.add_action(SetLaunchConfiguration('batch_run_id', batch_run_id))
     ld.add_action(SetLaunchConfiguration('simulation_run_id', simulation_run_id))
     
     batch = citros.batch.get_batch(batch_run_id) 
     # overide TIMEOUT setting.
     timeout_from_client = batch['batchRun']['simulation']['timeout']            
     if (float(timeout_from_client) > 1):
         timeout = str(timeout_from_client)
     ld.add_action(SetLaunchConfiguration('timeout', timeout))  
-    
-    log_msg = f"initializing simulation batch_run_id: {batch_run_id}, simulation_run_id: {simulation_run_id}, timeout: {timeout}"  
-    citros.log.info(log_msg)             
-    print(log_msg)
+        
+    citros.log.info(f"initializing simulation batch_run_id: {batch_run_id}, simulation_run_id: {simulation_run_id}, timeout: {timeout}")
     
     ################################
     # Arguments        
     ################################
     ld.add_action(DeclareLaunchArgument(
         "log_level",
         default_value=["debug"],
@@ -87,15 +85,15 @@
     bag_folder = 'tmp/bag' 
     bag_name = 'bag_0.db3'  # default to sqlite3
     
     # delete folder if exists
     try:
         shutil.rmtree(bag_folder)
     except Exception as e:
-        # print(e)
+        # citros.log.exception(e)
         pass
 
     bag_cmd = ['ros2', 'bag', 'record', '-a', '-o', bag_folder]
     mcap = False
     if mcap:
         bag_cmd.append('-s')
         bag_cmd.append('mcap')
@@ -105,21 +103,19 @@
         cmd=bag_cmd,
         output='screen', 
         log_cmd=True
     )
     ld.add_action(record_proccess)
     
     def handle_done_recording(context, *args, **kwargs):    
-        citros.log.debug("handle_done_recording")
-        print("handle_done_recording")
+        citros.log.debug("handle_done_recording")        
         
         batch_run_id = LaunchConfiguration("batch_run_id").perform(context)  
         simulation_run_id = LaunchConfiguration("simulation_run_id").perform(context)     
-        
-        print("start uploading bag")
+                
         citros.log.info("start uploading bag")
         citros.events.stopping(batch_run_id, simulation_run_id, tag="BAG", message="uploading bag", metadata=None)
                 
         # send bag to DB        
         bag_resp, batch_text, resp = citros.bag.emit(f"{bag_folder}/{bag_name}", batch_run_id, simulation_run_id, 'google')        
         if bag_resp:
             citros.events.stopping(batch_run_id, simulation_run_id, tag="BAG", message=batch_text, metadata=resp)
@@ -130,15 +126,14 @@
         if bag_resp:
             citros.events.stopping(batch_run_id, simulation_run_id, tag="BAG", message=batch_text, metadata=resp)
         else:
             citros.events.error(batch_run_id, simulation_run_id, tag="BAG", message=batch_text, metadata=None)
             
         citros.events.done(batch_run_id, simulation_run_id, tag="DONE", message='done', metadata=resp)    
             
-        print("done uploading bag")
         citros.log.info("done uploading bag")
         
     ld.add_action(RegisterEventHandler(
         OnExecutionComplete(
             target_action=record_proccess,
             on_completion=[
                 LogInfo(msg='OnExecutionComplete: Done Recording event'),                    
@@ -157,21 +152,20 @@
     
     
     ################################
     # STD LOG on ros events. 
     ################################   
     # Setup a custom event handler for all stdout/stderr from processes.
     # Later, this will be a configurable, but always present, extension to the LaunchService.
-    def on_output(event: Event) -> None:        
-        # citros.log.info(f"[ROS] {event.text.decode()}")
+    def on_output(event: Event) -> None:                
         citros.log.info(f"[ROS] [{cast(process.ProcessIO, event).process_name}] {event.text.decode()}")
         
         # cast(process.ProcessIO, event).process_name
         # for line in event.text.decode().splitlines():
-        #     # print('[{}] {}'.format(cast(process.ProcessIO, event).process_name, line))
+        #     # citros.log.debug('[{}] {}'.format(cast(process.ProcessIO, event).process_name, line))
         #     citros.log.info(f"[ROS] [{cast(process.ProcessIO, event).process_name}] {line}")
 
     ld.add_action(RegisterEventHandler(
         OnProcessIO(                
                 on_stdout=on_output,
                 on_stderr=on_output,
             )
@@ -220,51 +214,50 @@
             client_launch
         ]
 
         # second option. add actions for nodes. 
         # client_launch
         listeners = []
         sub_entities = client_launch.get_sub_entities()
-        # print("sub_entities", sub_entities)
+        # citros.log.debug("sub_entities", sub_entities)
         for launchDescription in sub_entities:
             eps = launchDescription.entities         
             for ep in eps:                        
                 if type(ep) in [Node, ExecuteProcess]:
-                    # print("adding event OnProcessStart")
+                    # citros.log.debug("adding event OnProcessStart")
                     listeners.append(ep)
                     listeners.append(RegisterEventHandler(
                         OnProcessStart(
                             target_action=ep,
                             on_start=[
-                                # print(' +++++++++++ OnProcessStart'),
+                                # citros.log.debug(' +++++++++++ OnProcessStart'),
                                 LogInfo(msg=" +++++++++++ OnProcessStart")                    
                             ]
                         )
                     ))
                     
                     listeners.append(RegisterEventHandler(
                         OnProcessExit(
                             target_action=ep,
                             on_exit=[
                                 LogInfo(msg=" ----------- OnProcessExit")                    
                             ]
                         )
                     ))
 
-        print(f"running {len(listeners)} entities")
+        citros.log.debug(f"running {len(listeners)} entities")
         return listeners
       
     ld.add_action(OpaqueFunction(function=launch_setup))
                 
     ################################
     # Timeout Events
     ################################  
     def handle_timeout(context, *args, **kwargs):   
-        citros.log.debug("handle_timeout")
-        print(args)
+        citros.log.debug("handle_timeout")        
         batch_run_id = LaunchConfiguration("batch_run_id").perform(context)  
         simulation_run_id = LaunchConfiguration("simulation_run_id").perform(context)       
         timeout = LaunchConfiguration("timeout").perform(context)
         citros.events.terminating(batch_run_id, simulation_run_id, tag="TIMOUT", message=f"Reached timeout of: { timeout } sec", metadata=None)            
                  
     ld.add_action(
         TimerAction(
```

### Comparing `citros-23.14.9/citros/logger/__init__.py` & `citros-23.17.1/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/logger/logger.py` & `citros-23.17.1/citros/logger/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # create DIR if not exists
 if not os.path.isdir(".citros"):
    os.makedirs(".citros")
 
 # log to console
 def get_console_handler():
    console_handler = logging.StreamHandler(sys.stdout)
-   console_handler.setLevel(logging.ERROR)
+   # console_handler.setLevel(logging.ERROR)
    console_handler.setFormatter(FORMATTER)
    return console_handler
 
 # log to file
 def get_file_handler():
    file_handler = TimedRotatingFileHandler(LOG_FILE, when='midnight')   
    file_handler.setFormatter(FORMATTER)
    return file_handler
 
 # log to postgres
 def get_gql_handler(sync_logs, batch_run_id, simulation_run_id):
    gql_handler = PGHandler(sync_logs, batch_run_id, simulation_run_id)
-   FORMATTER = logging.Formatter("%(name)s.%(funcName)s:%(lineno)d — %(message)s")
+   FORMATTER = logging.Formatter("%(message)s")
    gql_handler.setFormatter(FORMATTER)   
    return gql_handler
 
 # def get_logger(logger_name, citros):
 #    # print(f"****** get_logger {logger_name}")
 #    log_queue = queue.Queue(-1)
 #    queue_handler = QueueHandler(log_queue)
@@ -67,15 +67,15 @@
    queue_handler = QueueHandler(log_queue)
    
    loggers[logger_name]["logger"] = logging.getLogger(logger_name)
    loggers[logger_name]["logger"].setLevel(logging.DEBUG)   
    loggers[logger_name]["logger"].addHandler(queue_handler)
    
    loggers[logger_name]["listener"] = QueueListener(log_queue, 
-                                                   #  get_console_handler(), 
+                                                    get_console_handler(), 
                                                     get_file_handler(), 
                                                     get_gql_handler(sync_func, batch_run_id, simulation_run_id),
                                                     respect_handler_level=True
                                                 )      
    loggers[logger_name]["listener"].start()   
    
 #    loggers[logger_name]["logger"].propagate = False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `citros-23.14.9/citros/logger/logger_pg_handler.py` & `citros-23.17.1/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/parsers/__init__.py` & `citros-23.17.1/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/parsers/parser_ros2.py` & `citros-23.17.1/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/rosbag/__init__.py` & `citros-23.17.1/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/rosbag/reader_base.py` & `citros-23.17.1/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/rosbag/reader_mcap.py` & `citros-23.17.1/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/citros/rosbag/reader_sqlite.py` & `citros-23.17.1/citros/rosbag/reader_sqlite.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 
         topics_data = self.cursor.execute("SELECT id, name, type FROM topics").fetchall()
         self.topics = {name_of:{'type':type_of, 'id':id_of, 'message':get_message(type_of) } for id_of,name_of,type_of in topics_data}
         
         buffer = StringIO()
         size = 0
         for topic_name in self.topics.keys():
+            if topic_name in ["/rosout", "/client_count", "/connected_clients"]:
+                continue
             rows = self.cursor.execute(f"select id, timestamp, data from messages where topic_id = {self.topics[topic_name]['id']}").fetchall()            
             rid = 0
             for id, timestamp, data in rows:
                 d_data = deserialize_message(data, self.topics[topic_name]["message"])
                 msg_dict = message_to_ordereddict(d_data)
                 json_data = json.dumps(msg_dict)
                 
-                row = chr(0x1E).join([f"{simulation_run_id}", f"{rid}", f"{timestamp}", f"{topic_name}", f"{self.topics[topic_name]['type']}", f"{json_data}\n"])            
+                row = chr(0x1E).join([f"{simulation_run_id}", f"{rid}", f"{timestamp}", f"{topic_name}", f"{self.topics[topic_name]['type']}", json_data])
                 rid = rid + 1
-                bytes_wrote = buffer.write(row)
+                bytes_wrote = buffer.write(row + '\n')
                 size = size + bytes_wrote
                 # 10MB chunks max
                 if size >= CHUNK_SIZE:                    
                     yield buffer
                     buffer, size = StringIO(), 0
         # return the rest of the file.
         yield buffer
```

### Comparing `citros-23.14.9/citros.egg-info/PKG-INFO` & `citros-23.17.1/citros.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.9
+Version: 23.17.1
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.9/citros.egg-info/SOURCES.txt` & `citros-23.17.1/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.14.9/setup.py` & `citros-23.17.1/setup.py`

 * *Files identical despite different names*

