# Comparing `tmp/citros-23.17.1.tar.gz` & `tmp/citros-23.17.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.17.1.tar", last modified: Thu Apr 27 06:01:28 2023, max compression
+gzip compressed data, was "citros-23.17.3.tar", last modified: Thu Apr 27 13:02:03 2023, max compression
```

## Comparing `citros-23.17.1.tar` & `citros-23.17.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.560340 citros-23.17.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 06:01:12.000000 citros-23.17.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 06:01:28.560340 citros-23.17.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 06:01:12.000000 citros-23.17.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-27 06:01:12.000000 citros-23.17.1/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 06:01:12.000000 citros-23.17.1/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 06:01:12.000000 citros-23.17.1/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 06:01:12.000000 citros-23.17.1/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 06:01:12.000000 citros-23.17.1/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 06:01:12.000000 citros-23.17.1/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 06:01:12.000000 citros-23.17.1/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 06:01:12.000000 citros-23.17.1/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 06:01:12.000000 citros-23.17.1/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 06:01:12.000000 citros-23.17.1/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 06:01:12.000000 citros-23.17.1/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.560340 citros-23.17.1/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 06:01:12.000000 citros-23.17.1/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.556340 citros-23.17.1/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 06:01:28.000000 citros-23.17.1/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 06:01:12.000000 citros-23.17.1/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:01:28.560340 citros-23.17.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 06:01:12.000000 citros-23.17.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:28.560340 citros-23.17.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:12.000000 citros-23.17.1/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:01:12.000000 citros-23.17.1/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.846699 citros-23.17.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 13:01:47.000000 citros-23.17.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 13:02:03.842699 citros-23.17.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 13:01:47.000000 citros-23.17.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-27 13:01:47.000000 citros-23.17.3/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-27 13:01:47.000000 citros-23.17.3/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-27 13:01:47.000000 citros-23.17.3/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 13:01:47.000000 citros-23.17.3/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 13:01:47.000000 citros-23.17.3/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 13:01:47.000000 citros-23.17.3/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-27 13:01:47.000000 citros-23.17.3/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-27 13:01:47.000000 citros-23.17.3/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 13:01:47.000000 citros-23.17.3/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:01:47.000000 citros-23.17.3/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-27 13:01:47.000000 citros-23.17.3/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 13:01:47.000000 citros-23.17.3/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:02:03.000000 citros-23.17.3/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 13:01:47.000000 citros-23.17.3/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:02:03.846699 citros-23.17.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 13:01:47.000000 citros-23.17.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:02:03.842699 citros-23.17.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:47.000000 citros-23.17.3/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:47.000000 citros-23.17.3/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.17.1/LICENSE` & `citros-23.17.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/PKG-INFO` & `citros-23.17.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.1
+Version: 23.17.3
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.1/README.md` & `citros-23.17.3/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/bin/citros` & `citros-23.17.3/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/__init__.py` & `citros-23.17.3/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/citros.py` & `citros-23.17.3/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/citros_bag.py` & `citros-23.17.3/citros/citros_bag.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,30 +30,30 @@
         self.CONFIG_FOLDER = config("CONFIG_FOLDER", 'tmp/config')
         # if not self.CITROS_DATA_HOST:
         #     raise Exception("env variable CITROS_DATA_HOST is None, the simulation will not be able to upload the data to DB.")            
     
     # get token to upload the bag to GCP bucket.
     def get_bag_access_token(self):
         if not self.citros.isAuthenticated():
-            print("user is not logged in. please log in first.")
+            self.log.error("User is not logged in. please log in first.")
             return None
         
         rest_data = None
         import requests      
         try:
             resp = requests.post(self.CITROS_BAG_TOKEN, headers={
                 "Authorization": f"Bearer {self.citros._get_token()}"
             })
             if resp.status_code == 404:      
-                print("[ERROR] cant find [{self.CITROS_BAG_TOKEN}] url.")
+                self.log.error("cant find [{self.CITROS_BAG_TOKEN}] url.")
                 return 
             rest_data = resp.json()
         except Exception as err:
-            print("[ERROR] cant get access token at this moment... check google json file that may is currapt (sa-api-secret)")
-            print(err)
+            self.log.error("Cant get access token at this moment... check google json file that may is currapt (sa-api-secret)")
+            self.log.error(err)
             return    
                                 
         try:
             # token = rest_data
             token = rest_data["access_token"]            
             expires_in = rest_data["expires_in"]
             token_type = rest_data["token_type"]
@@ -78,25 +78,24 @@
         return self.sync_bag_pgdb(batch_run_id, simulation_run_id, path_to_metadata, path_to_bag)
     
     ################################################################################################
     ### sync BAG to Postgres DB
     ################################################################################################
     def sync_bag_pgdb(self, batch_run_id, simulation_run_id, path_to_metadata, path_to_bag):        
         import psycopg2
-        print("------------------------------------------------------------------------------------")
-        print(f"[{datetime.datetime.now()}] uploading bag to PGDB")
+        self.log.debug("------------------------------------------------------------------------------------")
+        self.log.debug(f"uploading bag to PGDB")
         
         connection = None
         # get data-token from citros to access data DB.             
         user = self.citros.getUser()      
         
         if user is None or user["username"] is None or user["id"] is None:
-            error_text = f"[{datetime.datetime.now()}] [ERROR] at sync_bag, failed to get user from CITROS."
-            self.log.error(error_text)            
-            print(error_text)            
+            error_text = f"Error at sync_bag, failed to get user from CITROS."
+            self.log.error(error_text)                                 
             return False, error_text, None
         
         if not self.CITROS_DATA_HOST:
             raise Exception(f"[{datetime.datetime.now()}] ENV variable [CITROS_DATA_HOST] is None, the simulation will not be able to upload the data to DB.")            
         
         connection = psycopg2.connect(user=user["username"],
                                     password=user["id"],
@@ -112,19 +111,19 @@
         
         try:                                       
             #####################
             # Uploads configs    
             #####################
             import glob
             rid_counter = 0
-            print(f"[{datetime.datetime.now()}] + uploading config")
+            self.log.debug(f"uploading config")
             for config_file in glob.glob(self.CONFIG_FOLDER + "/*"):                
                 with open(f"{config_file}", 'r') as file:                                                     
                     config_dict = yaml.load(file, Loader=yaml.FullLoader) 
-                    print(f"[{datetime.datetime.now()}] - uploading config [{config_file}]")
+                    self.log.debug(f"uploading config [{config_file}]")
                     
                     record_to_insert = {
                         "sid": simulation_run_id,
                         "rid": rid_counter,
                         "time": 0,
                         "topic": '/config',
                         "type": 'params',
@@ -136,100 +135,100 @@
                     cursor.execute(postgres_insert_query, record_to_insert)                                                        
                     connection.commit()                
                       
             
             #####################
             # Uploads metadata
             #####################
-            print(f"[{datetime.datetime.now()}] + uploading metadata")
+            self.log.debug(f" + uploading metadata")
             with open(path_to_metadata, 'r') as file:                                                     
                 metadata_dict = yaml.load(file, Loader=yaml.FullLoader) 
-                print(f"[{datetime.datetime.now()}] - uploading metadata")
+                self.log.debug(f" - uploading metadata")
                 
                 record_to_insert = {
                     "sid": simulation_run_id,
                     "rid": 0,
                     "time": 0,
                     "topic": '/metadata',
                     "type": 'metadata',
                     "data": json.dumps(metadata_dict)
                 }
                 
-                # print("metadata record_to_insert:", record_to_insert)
+                # self.log.debug("metadata record_to_insert:", record_to_insert)
                 # record_to_insert = (simulation_run_id, 0, 0, '/metadata', 'metadata', json.dumps(metadata_dict))                
-                # print(postgres_insert_query, record_to_insert)
+                # self.log.debug(postgres_insert_query, record_to_insert)
                 
                 cursor.execute(postgres_insert_query, record_to_insert)                                                        
                 connection.commit()                                 
             
             #####################
             # Uploading data
             #####################  
-            print(f"[{datetime.datetime.now()}] +++ uploading bag to PG", flush=True)
+            self.log.debug(f" +++ uploading bag to PG")
             bagReader = BagReaderSQL()
             total_size = 0
             for buffer in bagReader.read_messages(path_to_bag, simulation_run_id):
-                # print(f"[{datetime.datetime.now()}] + read_messages", flush=True)
+                # self.log.debug(f" + read_messages")
                 size = buffer.seek(0, os.SEEK_END)
                 size = buffer.tell()
                 total_size = total_size + size
                 buffer.seek(0)                
-                print(f"[{datetime.datetime.now()}] \tinserting buffer size: { (size / 1024 ) / 1024 } MB", flush=True)
+                self.log.debug(f" \tinserting buffer size: { (size / 1024 ) / 1024 } MB")
                 if size == 0:
                     continue
                 cursor.execute(f'SET search_path TO data_bucket')
                 try:           
                     cursor.copy_from(buffer, batch_run_id, sep=chr(0x1E), null="", columns=['sid', 'rid', 'time', 'topic', 'type', 'data'])                
                 except (Exception, psycopg2.Error) as error:
                     buffer.seek(0)                      
-                    print(f"[{datetime.datetime.now()}] Failed to insert record into table, aboring uploading to PG DB.", error) 
-                    print(traceback.format_exc())
-                    # print("===============================================================================================")
-                    # print(buffer.getvalue())
-                    # print("===============================================================================================")
+                    self.log.error(f" Failed to insert record into table, aboring uploading to PG DB.", error) 
+                    # self.log.error(traceback.format_exc())
+                    self.log.exception(error)     
+                    # self.log.debug("===============================================================================================")
+                    # self.log.debug(buffer.getvalue())
+                    # self.log.debug("===============================================================================================")
                     return False, "got exception from pgdb", str(error)
                 # buffer.truncate(0)
                 # buffer.seek(0)
                 # buffer.close()
                 connection.commit()
-            print(f"[{datetime.datetime.now()}] --- done uploading to PG", flush=True)
+            self.log.debug(f" --- done uploading to PG")
             return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}] to Postgres. [size: {(total_size / 1024)/1024} MB]", None
         except (Exception, psycopg2.Error) as error:
-            print(f"[{datetime.datetime.now()}] Failed to insert record into table, aboring uploading to PG DB.", error) 
-            print(traceback.format_exc())
+            self.log.exception(f" Failed to insert record into table, aboring uploading to PG DB.", error) 
+            self.log.exception(traceback.format_exc())
             return False, "got exception from pgdb", str(error)
         finally:
             # closing database connection.
             if connection:
                 cursor.close()
                 connection.close()
-                print(f"[{datetime.datetime.now()}] PostgreSQL connection is closed")  
+                self.log.debug(f"PostgreSQL connection is closed")  
                 
     ################################################################################################
     ### sync BAG to Google Bucket
     ################################################################################################
     def sync_bag_google_bucket(self, batch_run_id, simulation_run_id, path_to_metadata, path_to_bag):
-        print("------------------------------------------------------------------------------------")
-        print("uploading bag to google bucket")
+        self.log.debug("------------------------------------------------------------------------------------")
+        self.log.debug("uploading bag to google bucket")
         if not self.citros.isAuthenticated():
-            print("not authenticated. please login first.")
+            self.log.debug("not authenticated. please login first.")
             return False, "not authenticated. please login first." , None       
         
         bag_file_name = path_to_bag.split('/')[-1]            
         data_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={batch_run_id + "/sid-" + simulation_run_id + "/" + bag_file_name}'        
         
         metadata_name = path_to_metadata.split('/')[-1]  
         metadata_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={batch_run_id + "/sid-" + simulation_run_id + "/" + metadata_name}'        
 
         google_token = self.get_bag_access_token()
-        # print("google_token", google_token)
+        # self.log.debug("google_token", google_token)
         if google_token is None:
             error_text = f"[ERROR] at sync_bag, failed to get google token from CITROS."
-            self.log.error(error_text)            
-            print(error_text)            
+            self.log.error(error_text)                                  
             return False, error_text, None  
         
         import requests  
         # uploading metadata first, assuming much smaller file. 
         with open(path_to_metadata, 'rb') as data:
             # metadata = yaml.safe_load(data)
             metadata_resp = requests.post(metadata_url,
@@ -237,37 +236,34 @@
                                 headers={
                                     "Authorization": f"Bearer {google_token}",
                                     "Content-Type" : "application/octet-stream"
                                 }
                             ) 
         if metadata_resp.status_code != 200:                        
             error_text = f"[ERROR] from sync_bag: [{metadata_resp.status_code}]:[{metadata_resp.reason}]"
-            self.log.error(error_text)            
-            print(error_text)            
+            self.log.error(error_text)
             return False, error_text, None  
         
         self.log.info(f"done updating metadata to: [{batch_run_id}],[{simulation_run_id}] - [{metadata_resp.text}]")
         
         # uploading the bag
         with open(path_to_bag, 'rb') as data:            
             bag_resp = requests.post(data_url,
                                 data=data,
                                 headers={
                                     "Authorization": f"Bearer {google_token}",
                                     "Content-Type" : "application/octet-stream"
                                 }
                             ) 
-            # print("bag_resp", bag_resp)
+            # self.log.debug("bag_resp", bag_resp)
             
         if bag_resp.status_code != 200:                        
             error_text = f"[ERROR] from sync_bag: [{bag_resp.status_code}]:[{bag_resp.reason}]"
             self.log.error(error_text)            
-            print(error_text)
-            # print("sync_bag", CITROS_BAG, request_json)
+            # self.log.debug("sync_bag", CITROS_BAG, request_json)
             return False, error_text, None  
         
-        # print("resp", json.loads(bag_resp.text))
+        # self.log.debug("resp", json.loads(bag_resp.text))
         
-        self.log.info(f"done updating bag to: [{batch_run_id}],[{simulation_run_id}] - [{bag_resp.text}] ")
-        print(f"done updating bag to: [{batch_run_id}],[{simulation_run_id}] - [{bag_resp.text}] ")
+        self.log.info(f"done updating bag to: [{batch_run_id}],[{simulation_run_id}] - [{bag_resp.text}] ")        
         return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}]", bag_resp.text
```

### Comparing `citros-23.17.1/citros/citros_batch.py` & `citros-23.17.3/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/citros_events.py` & `citros-23.17.3/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/citros_integration.py` & `citros-23.17.3/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/citros_params.py` & `citros-23.17.3/citros/citros_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # from pkg_resources import Distribution
 from soupsieve import match
 import yaml
+import json
 from pathlib import Path
 from decouple import config
 
 class citros_params():
     def __init__(self, citros):
         self.citros = citros
         self.log = citros.log
@@ -160,15 +161,15 @@
             os.makedirs(self.CONFIG_FOLDER)
         except FileExistsError:
             # directory already exists
             pass
                 
         from ament_index_python.packages import get_package_share_directory
         for package_name, citros_config in config.items():     
-            self.log.debug(f"Saving config for {package_name}")                               
+            self.log.debug(f"Saving config for [{package_name}]")                               
             # TODO: add other method to get the package path
             path_to_package = None
             try:
                 path_to_package = get_package_share_directory(package_name) # get the path to the package install directory - the project must be sourced for it to work            
             except Exception as e:
                 self.log.exception(e)
                 continue                
@@ -188,37 +189,39 @@
             path = path + "params.yaml"
             
             # check if file exists?
             if not Path(path).exists():
                 self.log.debug(f"No config file {path} exits for pack:{package_name}. passing.") 
                 continue
             
-            self.log.debug(f"Loading default config from {path}") 
+            # self.log.debug(f"Loading default config from {path}") 
             with open(path, "r") as stream:
                 try:    
                     default_config = yaml.safe_load(stream)
                 except yaml.YAMLError as exc:
                     print(exc)
             
-            self.log.debug(f"Merging configuration files.") 
+            # self.log.debug(f"Merging configuration files.") 
             merged_config = {key: value for (key, value) in (list(default_config.items()) + list(citros_config.items()))}
             
+            # self.log.debug(f"config file for {package_name}:")
+            self.log.debug(json.dumps(merged_config, indent=4))
+            
             with open(path, 'w') as file:
                 yaml.dump(merged_config, file)  
                 
             # save for metadata
             with open(f"{self.CONFIG_FOLDER}/{package_name}.yaml", 'w') as file:                                     
-                yaml.dump(merged_config, file) 
-        self.log.debug("Saved config to project") 
+                yaml.dump(merged_config, file)         
     
     def init_params(self, batch_run_id, sid):                
-        self.log.debug("Getting parameters from CITROS.") 
+        self.log.info("Getting parameters from CITROS.") 
         config = self.get_config(batch_run_id, sid)
         if not config:
             # if there is no config, cant init anything...
             self.log.warning("If there is no config, cant init anything...") 
             return
-        self.log.debug("Saving parameters to files. ")
-        
-        self.save_config(config)                        
+        self.log.debug("Saving parameters to files. ")        
+        self.save_config(config)     
+        self.log.debug("Done saving config files.")                    
         return config
```

### Comparing `citros-23.17.1/citros/citros_utils.py` & `citros-23.17.3/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/launches/__init__.py` & `citros-23.17.3/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/launches/launch.py` & `citros-23.17.3/citros/launches/launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 ################################
 # Entrypoint        
 ################################
 def generate_launch_description(batch_run_id, simulation_run_id, timeout):  
     batch_run_id = str(batch_run_id)    
     simulation_run_id = str(simulation_run_id)    
     timeout = str(timeout)    
-    citros.log.debug("+ generate_launch_description()")
-    citros.log.debug("batch_run_id: ", batch_run_id)
-    citros.log.debug("simulation_run_id: ", simulation_run_id)
-    citros.log.debug("timeout: ", timeout)
     
     citros = Citros(batch_run_id, simulation_run_id)
+    citros.log.debug("+ generate_launch_description()")
+    citros.log.debug(f"batch_run_id: {batch_run_id}")
+    citros.log.debug(f"simulation_run_id: {simulation_run_id}")
+    citros.log.debug(f"timeout: {timeout}")
+    
     resp = citros.checkStatus()
     if not resp:        
         return 
     citros.log.debug("Health-check: OK")
     citros.events.init(batch_run_id=batch_run_id, sid=simulation_run_id, tag="INIT", message="updated config", metadata=None)
     
     ld = LaunchDescription([
@@ -153,20 +154,20 @@
     
     ################################
     # STD LOG on ros events. 
     ################################   
     # Setup a custom event handler for all stdout/stderr from processes.
     # Later, this will be a configurable, but always present, extension to the LaunchService.
     def on_output(event: Event) -> None:                
-        citros.log.info(f"[ROS] [{cast(process.ProcessIO, event).process_name}] {event.text.decode()}")
+        # citros.log.info(f"[ROS][{cast(process.ProcessIO, event).process_name}]{event.text.decode()}")
         
         # cast(process.ProcessIO, event).process_name
-        # for line in event.text.decode().splitlines():
-        #     # citros.log.debug('[{}] {}'.format(cast(process.ProcessIO, event).process_name, line))
-        #     citros.log.info(f"[ROS] [{cast(process.ProcessIO, event).process_name}] {line}")
+        for line in event.text.decode().splitlines():
+            # citros.log.debug('[{}] {}'.format(cast(process.ProcessIO, event).process_name, line))
+            citros.log.info(f"[ROS][{cast(process.ProcessIO, event).process_name}]{line}")
 
     ld.add_action(RegisterEventHandler(
         OnProcessIO(                
                 on_stdout=on_output,
                 on_stderr=on_output,
             )
         )
```

### Comparing `citros-23.17.1/citros/logger/__init__.py` & `citros-23.17.3/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/logger/logger.py` & `citros-23.17.3/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/logger/logger_pg_handler.py` & `citros-23.17.3/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/parsers/__init__.py` & `citros-23.17.3/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/parsers/parser_ros2.py` & `citros-23.17.3/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/rosbag/__init__.py` & `citros-23.17.3/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/rosbag/reader_base.py` & `citros-23.17.3/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/rosbag/reader_mcap.py` & `citros-23.17.3/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros/rosbag/reader_sqlite.py` & `citros-23.17.3/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/citros.egg-info/PKG-INFO` & `citros-23.17.3/citros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.17.1
+Version: 23.17.3
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.17.1/citros.egg-info/SOURCES.txt` & `citros-23.17.3/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.17.1/setup.py` & `citros-23.17.3/setup.py`

 * *Files identical despite different names*

