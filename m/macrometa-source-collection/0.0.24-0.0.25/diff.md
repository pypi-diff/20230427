# Comparing `tmp/macrometa-source-collection-0.0.24.tar.gz` & `tmp/macrometa-source-collection-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.24.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.25.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.24.tar` & `macrometa-source-collection-0.0.25.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8418 2023-04-24 12:31:10.829819 macrometa-source-collection-0.0.24/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     6396 2023-04-24 12:31:10.829819 macrometa-source-collection-0.0.24/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-04-24 12:31:11.081839 macrometa-source-collection-0.0.24/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.24/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.24/PKG-INFO
+-rw-r--r--   0        0        0     8346 2023-04-27 08:54:31.255945 macrometa-source-collection-0.0.25/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     7366 2023-04-27 08:54:31.255945 macrometa-source-collection-0.0.25/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-04-27 08:54:31.595942 macrometa-source-collection-0.0.25/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.25/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.25/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.24/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.25/macrometa_source_collection/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """GDN data connector source for GDN Collections."""
-from collections import Counter
+from collections import defaultdict
 
 import pkg_resources
 import singer
 from c8 import C8Client
 from c8connector import C8Connector, Sample, ConfigProperty, ConfigAttributeType, Schema, SchemaAttributeType, \
     SchemaAttribute
-from macrometa_source_collection.client import GDNCollectionClient
+from macrometa_source_collection.client import GDNCollectionClient, get_singer_data_type
 from singer import utils
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema as SingerSchema
 
 LOGGER = singer.get_logger('macrometa_source_collection')
 
 REQUIRED_CONFIG_KEYS = [
@@ -67,15 +67,16 @@
         config = self.get_config(integration)
         schema, data = get_schema_and_data(C8Client(
             "https",
             host=config["region"],
             port=443,
             geofabric=config["fabric"],
             apikey=config["api_key"]
-        ), config["source_collection"], 10)
+        ), config["source_collection"], 50)
+        data = data[:10]
         return [Sample(
             schema=Schema(config["source_collection"],
                           [SchemaAttribute(k, get_attribute_type(v)) for k, v in schema.items()]),
             data=data
         )]
 
     def schemas(self, integration: dict) -> list[Schema]:
@@ -131,51 +132,39 @@
         except KeyError as e:
             raise KeyError(f'Integration property `{e}` not found.')
 
 
 def get_schema_and_data(client: C8Client, collection: str, sample_size: int):
     cursor = client.execute_query(f"FOR d IN @@collection LIMIT 0, @count RETURN d",
                                   bind_vars={"@collection": collection, "count": sample_size})
-    schemas = []
-    schema_map = {}
-    data_map = {}
+    schema_counts = defaultdict(int)
+    records_by_schema = defaultdict(list)
     while not cursor.empty():
         rec = cursor.next()
         rec.pop('_id', None)
         rec.pop('_rev', None)
-        h = str(hash(rec.keys().__str__()))
-        schema_map[h] = rec.keys()
-        schemas.append(h)
-        if h in data_map:
-            data_map[h].append(rec)
-        else:
-            data_map[h] = [rec]
+        # Skip empty records or records with no keys
+        if not rec or not rec.keys():
+            continue
+
+        schema_keys = rec.keys()
+        schema = tuple((k, get_singer_data_type(rec[k])) for k in schema_keys)
+        schema_counts[schema] += 1
+        records_by_schema[schema].append(rec)
+
     schema = {"data": "object"}
     data = []
-    if len(schemas) > 0:
-        most_common, _ = Counter(schemas).most_common(1)[0]
-        schema_keys = schema_map[most_common]
-        data = data_map[most_common]
-        schema = {
-            k: get_singer_data_type(data[0][k]) for k in schema_keys
-        }
-    return schema, data
+    if schema_counts:
+        # Get the most common schema
+        most_common_schema = max(schema_counts, key=schema_counts.get)
+        schema = dict(most_common_schema)
 
-
-def get_singer_data_type(val):
-    if type(val) == str:
-        return "string"
-    elif type(val) == int:
-        return "integer"
-    elif type(val) == float:
-        return "number"
-    elif type(val) == bool:
-        return "boolean"
-    else:
-        return "object"
+        # Get the list of records associated with the most common schema
+        data = records_by_schema[most_common_schema]
+    return schema, data
 
 
 def get_attribute_type(source_type: str) -> SchemaAttributeType:
     if source_type == 'string':
         return SchemaAttributeType.STRING
     elif source_type == 'integer':
         return SchemaAttributeType.LONG
```

### Comparing `macrometa-source-collection-0.0.24/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.25/macrometa_source_collection/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 
         start_http_server(8000)
 
     def sync(self, stream):
         """Return documents in target GDN collection as records."""
         if self._c8_client.has_collection(self._collection):
             self.send_schema_message(stream)
-            self.load_existing_data(stream)
-            LOGGER.info(f"Full table sync completed")
-            meta_keys = ['_key', '_sdc_deleted_at']
+            columns = list(stream.schema.properties.keys())
+            columns.remove("_sdc_deleted_at")
+            schema_properties = stream.schema.properties
+            self.load_existing_data(stream, columns, schema_properties)
+            LOGGER.info("Full table sync completed.")
 
             # pulsar client throws some messages into stdout when subscribed to a topic. Meltano tap/target doesn't like
             # this and tries to process the pulsar log messages in stdout as input singer records. Therefore we are trying
             #  to turn off pulsar logging here. This is the best way I found with the current pulsar client API.
             _pulsar_logger = logging.getLogger("pulsar-logger")
             _pulsar_logger.setLevel(logging.CRITICAL)
             _pulsar_logger.addHandler(logging.NullHandler())
@@ -66,57 +68,70 @@
                 authentication=self._auth,
                 tls_allow_insecure_connection=False,
                 logger=_pulsar_logger,
             )
             _sub_name = self._wf_uuid if self._wf_uuid else f"cs_{uuid.uuid1()}"
             _topic = f"persistent://{self._tenant}/c8local.{self._fabric}/{self._collection}"
             _consumer: pulsar.Consumer = _pulsar_client.subscribe(_topic, _sub_name)
+
             while True:
                 try: 
                     msg = _consumer.receive()
-                    LOGGER.warn(f"Message recevied from stream: {msg}")
                     data = msg.data()
                     if data == None or not data:
                         continue
                     props = msg.properties()
                     j = json.loads(data.decode("utf8"))
-                    LOGGER.warn(f"Payload recevied from stream: {j}")
-                    j['_sdc_deleted_at'] = None
+                    j.pop('_id', None)
+                    j.pop('_rev', None)
+
                     if props["op"] == "INSERT" or props["op"] == "UPDATE":
-                        # skip inserts without data.
-                        if len(j.keys() ^ meta_keys) > 0:
+                        # skip inserts not having valid schema
+                        if len(j.keys() ^ columns) == 0 and all(
+                            get_singer_data_type(j[key]) == schema_properties[key].type
+                            for key in j.keys()
+                        ):
+                            j['_sdc_deleted_at'] = None
                             singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                             singer.write_message(singer_record)
                     elif props["op"] == "DELETE":
+                        # Currently, we don't have a way to validate schema here
                         j['_sdc_deleted_at'] = singer.utils.strftime(utils.now())
                         singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
                         singer.write_message(singer_record)
-                    #self.exported_bytes.inc(len(data))
-                    #self.exported_documents.inc()
-                    #time = datetime.fromtimestamp(msg.publish_timestamp()/1000)
-                    #event_time = datetime.strptime(time, "%Y-%m-%dT%H:%M:%S.%fZ")
-                    #self.export_lag.observe((utils.now() - event_time).total_seconds())
+                    self.exported_bytes.inc(len(data))
+                    self.exported_documents.inc()
+                    time = datetime.fromtimestamp(msg.publish_timestamp()/1000)
+                    time_str = time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+                    event_time = datetime.strptime(time_str, "%Y-%m-%dT%H:%M:%S.%fZ")
+                    self.export_lag.observe((utils.now() - event_time).total_seconds())
                     _consumer.acknowledge(msg.message_id())
                 except Exception as e:
                     LOGGER.warn(f"Exception received: {e}")
                     self.export_errors.inc()
         
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
-    def load_existing_data(self, stream):
+
+    def load_existing_data(self, stream, columns, schema_properties):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
                                                bind_vars={"@collection": self._collection},
                                                stream=True)
         while (not cursor.empty()) or cursor.has_more():
             rec = cursor.next()
             rec.pop('_id', None)
             rec.pop('_rev', None)
-            singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
-            singer.write_message(singer_record)
+            # skip existing data not having valid schema
+            if len(rec.keys() ^ columns) == 0 and all(
+                get_singer_data_type(rec[key]) == schema_properties[key].type
+                for key in rec.keys()
+            ):
+                singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
+                singer.write_message(singer_record)
 
     def send_schema_message(self, stream: CatalogEntry, bookmark_properties=[]):
         schema_message = singer.SchemaMessage(stream=stream.stream,
                                               schema=stream.schema.to_dict(),
                                               key_properties=stream.key_properties,
                                               bookmark_properties=bookmark_properties)
         singer.write_message(schema_message)
@@ -124,7 +139,20 @@
     def msg_to_singer_message(self, stream, msg, version, time_extracted):
         return singer.RecordMessage(
             stream=stream.stream,
             record=msg,
             version=version,
             time_extracted=time_extracted
         )
+
+
+def get_singer_data_type(val):
+    if type(val) == str:
+        return "string"
+    elif type(val) == int:
+        return "integer"
+    elif type(val) == float:
+        return "number"
+    elif type(val) == bool:
+        return "boolean"
+    else:
+        return "object"
```

### Comparing `macrometa-source-collection-0.0.24/pyproject.toml` & `macrometa-source-collection-0.0.25/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.24'
+version='0.0.25'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.24/setup.py` & `macrometa-source-collection-0.0.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.24',
+    'version': '0.0.25',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.24/PKG-INFO` & `macrometa-source-collection-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.24
+Version: 0.0.25
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

