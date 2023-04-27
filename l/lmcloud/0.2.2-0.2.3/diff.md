# Comparing `tmp/lmcloud-0.2.2.tar.gz` & `tmp/lmcloud-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.2.2.tar", last modified: Wed Apr 26 08:49:39 2023, max compression
+gzip compressed data, was "lmcloud-0.2.3.tar", last modified: Thu Apr 27 06:16:08 2023, max compression
```

## Comparing `lmcloud-0.2.2.tar` & `lmcloud-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:49:39.488324 lmcloud-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 08:49:25.000000 lmcloud-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 08:49:39.488324 lmcloud-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-26 08:49:25.000000 lmcloud-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:49:39.484324 lmcloud-0.2.2/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:49:39.488324 lmcloud-0.2.2/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:49:39.488324 lmcloud-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-26 08:49:25.000000 lmcloud-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:16:08.068407 lmcloud-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 06:15:47.000000 lmcloud-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-27 06:16:08.068407 lmcloud-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-27 06:15:47.000000 lmcloud-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:16:08.068407 lmcloud-0.2.3/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-27 06:15:47.000000 lmcloud-0.2.3/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:16:08.068407 lmcloud-0.2.3/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 06:16:08.000000 lmcloud-0.2.3/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:16:08.068407 lmcloud-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-27 06:15:47.000000 lmcloud-0.2.3/setup.py
```

### Comparing `lmcloud-0.2.2/LICENSE` & `lmcloud-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.2/PKG-INFO` & `lmcloud-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -82,7 +82,18 @@
 
 ### Websockets
 The local API initiates a websocket connection to
 ```
 http://{IP}:8081/api/v1/streaming
 ```
 The packets which are received on that WebSocket are documented in [websockets](docs/websockets.md)
+
+If WebSockets are enabled the shot timer becomes available to use, however as long as the library is running in WebSocket mode, the App will no longer be able to connect.
+
+To use WebSockets start the integration with
+```python
+lm = await LMCloud.create_with_local_api(creds, <IP>, port=8081, use_websockets=True)
+
+while True:
+    print(lm._lm_local_api.active_brew) # is a brew running at the moment
+    print(lm._lm_local_api.active_brew_duration) # the current shot timer returned by the machine
+```
```

### Comparing `lmcloud-0.2.2/README.md` & `lmcloud-0.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -63,8 +63,19 @@
 ```
 
 ### Websockets
 The local API initiates a websocket connection to
 ```
 http://{IP}:8081/api/v1/streaming
 ```
-The packets which are received on that WebSocket are documented in [websockets](docs/websockets.md)
+The packets which are received on that WebSocket are documented in [websockets](docs/websockets.md)
+
+If WebSockets are enabled the shot timer becomes available to use, however as long as the library is running in WebSocket mode, the App will no longer be able to connect.
+
+To use WebSockets start the integration with
+```python
+lm = await LMCloud.create_with_local_api(creds, <IP>, port=8081, use_websockets=True)
+
+while True:
+    print(lm._lm_local_api.active_brew) # is a brew running at the moment
+    print(lm._lm_local_api.active_brew_duration) # the current shot timer returned by the machine
+```
```

### Comparing `lmcloud-0.2.2/lmcloud/const.py` & `lmcloud-0.2.3/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.2/lmcloud/helpers.py` & `lmcloud-0.2.3/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.2/lmcloud/lmcloud.py` & `lmcloud-0.2.3/lmcloud/lmcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         await self.update_local_machine_status()
         return self
 
     '''
     Also initialize a local API client
     '''
     @classmethod
-    async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=True):
+    async def create_with_local_api(cls, credentials, ip, port=8081, use_websocket=False):
         self = cls()
         self.client = await self._connect(credentials)
         self._machine_info = await self._get_machine_info()
         self._lm_local_api = LMLocalAPI(local_ip=ip, local_port=port, local_bearer=self.machine_info[KEY])
         self._gw_url_with_serial = GW_MACHINE_BASE_URL + "/" + self.machine_info[SERIAL_NUMBER]
         self._firmware = await self.get_firmware()
         if use_websocket:
@@ -243,15 +243,15 @@
             if self._lm_local_api._timestamp_last_websocket_msg == None or (datetime.now() - self._lm_local_api._timestamp_last_websocket_msg).total_seconds() > 30: 
                 if self._use_websocket and not in_init: # during init we don't want to log this warning
                     _logger.warn("Could not get local machine status. Falling back to cloud status.")
                 await self._update_status_obj()
                 self._status[ACTIVE_BREW] = False
             else:
                 # Get local status from WebSockets
-                print("Using local status")
+                _logger.info("Using local status")
                 self._status = self._lm_local_api._status # reference to the same object tp get websocket updates
         else:
             await self._update_config_obj()     
             await self._update_status_obj()
 
         await self._update_statistics_obj()
```

### Comparing `lmcloud-0.2.2/lmcloud/lmlocalapi.py` & `lmcloud-0.2.3/lmcloud/lmlocalapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,8 +108,8 @@
                 elif message[0]["name"] in ["BrewingStartedGroup1StopType", "BrewingStartedGroup1DoseIndex"]:
                     # started active brew
                     self._status[ACTIVE_BREW] = True
                 elif message[0]["name"] in ["BrewingSnapshotGroup1", "FlushStoppedGroup1DoseIndex", "FlushStoppedGroup1Time"]:
                     # stopped active brew
                     self._status[ACTIVE_BREW] = False
         except Exception as e:
-            print(f"Error during handling of websocket message: {e}")
+            _logger.error(f"Error during handling of websocket message: {e}")
```

### Comparing `lmcloud-0.2.2/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.2.3/lmcloud.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -82,7 +82,18 @@
 
 ### Websockets
 The local API initiates a websocket connection to
 ```
 http://{IP}:8081/api/v1/streaming
 ```
 The packets which are received on that WebSocket are documented in [websockets](docs/websockets.md)
+
+If WebSockets are enabled the shot timer becomes available to use, however as long as the library is running in WebSocket mode, the App will no longer be able to connect.
+
+To use WebSockets start the integration with
+```python
+lm = await LMCloud.create_with_local_api(creds, <IP>, port=8081, use_websockets=True)
+
+while True:
+    print(lm._lm_local_api.active_brew) # is a brew running at the moment
+    print(lm._lm_local_api.active_brew_duration) # the current shot timer returned by the machine
+```
```

### Comparing `lmcloud-0.2.2/setup.py` & `lmcloud-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.2.2",
+    version="0.2.3",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

