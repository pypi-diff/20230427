# Comparing `tmp/async_paho_mqtt_client-0.3.3-py3-none-any.whl.zip` & `tmp/async_paho_mqtt_client-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3206 bytes, number of entries: 5
--rw-r--r--  2.0 unx     6835 b- defN 23-Apr-27 14:36 async_paho_mqtt_client.py
--rw-r--r--  2.0 unx      539 b- defN 23-Apr-27 14:37 async_paho_mqtt_client-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 14:37 async_paho_mqtt_client-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 23-Apr-27 14:37 async_paho_mqtt_client-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      439 b- defN 23-Apr-27 14:37 async_paho_mqtt_client-0.3.3.dist-info/RECORD
-5 files, 7928 bytes uncompressed, 2378 bytes compressed:  70.0%
+Zip file size: 3210 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     6843 b- defN 23-Apr-27 14:38 async_paho_mqtt_client.py
+-rw-r--r--  2.0 unx      539 b- defN 23-Apr-27 14:39 async_paho_mqtt_client-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 14:39 async_paho_mqtt_client-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Apr-27 14:39 async_paho_mqtt_client-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      439 b- defN 23-Apr-27 14:39 async_paho_mqtt_client-0.3.4.dist-info/RECORD
+5 files, 7936 bytes uncompressed, 2382 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: async_paho_mqtt_client.py
 Comment: 
 
-Filename: async_paho_mqtt_client-0.3.3.dist-info/METADATA
+Filename: async_paho_mqtt_client-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: async_paho_mqtt_client-0.3.3.dist-info/WHEEL
+Filename: async_paho_mqtt_client-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: async_paho_mqtt_client-0.3.3.dist-info/top_level.txt
+Filename: async_paho_mqtt_client-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: async_paho_mqtt_client-0.3.3.dist-info/RECORD
+Filename: async_paho_mqtt_client-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## async_paho_mqtt_client.py

```diff
@@ -136,15 +136,15 @@
                 break
             except:
                 self.logger.warning('MQTT connect failed, sleeping %s',self.reconnect_interval)
                 await asyncio.sleep(self.reconnect_interval)
         self.logger.info('MQTT finished reconnect loop')
    
     async def start(self):
-        self.loop = get_running_loop()
+        self.loop = asyncio.get_running_loop()
         if self._reconnector_loop is None or self._reconnector_loop.done():
             self._reconnector_loop = self.loop.create_task(self.reconnect_loop())
 
     async def wait_started(self):
         if self._reconnector_loop is not None and not self._reconnector_loop.done():
             await asyncio.wait_for(self._reconnector_loop,None)
```

## Comparing `async_paho_mqtt_client-0.3.3.dist-info/METADATA` & `async_paho_mqtt_client-0.3.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-paho-mqtt-client
-Version: 0.3.3
+Version: 0.3.4
 Home-page: https://github.com/mortbauer/async-paho-mqtt-client
 Author: Martin Ortbauer
 Author-email: martin@villagefarmer.net
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: paho-mqtt
```

