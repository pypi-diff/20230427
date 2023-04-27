# Comparing `tmp/python_roborock-0.8.0.tar.gz` & `tmp/python_roborock-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.8.0.tar", max compression
+gzip compressed data, was "python_roborock-0.8.1.tar", max compression
```

## Comparing `python_roborock-0.8.0.tar` & `python_roborock-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-27 14:49:37.960720 python_roborock-0.8.0/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-27 14:49:37.960720 python_roborock-0.8.0/README.md
--rw-r--r--   0        0        0     1370 2023-04-27 14:49:38.732733 python_roborock-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/__init__.py
--rw-r--r--   0        0        0    20172 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/cli.py
--rw-r--r--   0        0        0     8241 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/cloud_api.py
--rw-r--r--   0        0        0     4329 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/code_mappings.py
--rw-r--r--   0        0        0      209 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/const.py
--rw-r--r--   0        0        0    10730 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/containers.py
--rw-r--r--   0        0        0     1487 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/exceptions.py
--rw-r--r--   0        0        0     6416 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/roborock_future.py
--rw-r--r--   0        0        0     6232 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/roborock_message.py
--rw-r--r--   0        0        0    12651 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/typing.py
--rw-r--r--   0        0        0      783 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 14:59:40.335621 python_roborock-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-27 14:59:40.335621 python_roborock-0.8.1/README.md
+-rw-r--r--   0        0        0     1370 2023-04-27 14:59:41.427633 python_roborock-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/__init__.py
+-rw-r--r--   0        0        0    20956 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/cli.py
+-rw-r--r--   0        0        0     7649 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4329 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/code_mappings.py
+-rw-r--r--   0        0        0      209 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/const.py
+-rw-r--r--   0        0        0    10730 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/containers.py
+-rw-r--r--   0        0        0     1483 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/exceptions.py
+-rw-r--r--   0        0        0     6578 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6232 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12651 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/typing.py
+-rw-r--r--   0        0        0      783 2023-04-27 14:59:40.335621 python_roborock-0.8.1/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.8.1/PKG-INFO
```

### Comparing `python_roborock-0.8.0/LICENSE` & `python_roborock-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/README.md` & `python_roborock-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/pyproject.toml` & `python_roborock-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.8.0"
+version = "0.8.1"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.8.0/roborock/api.py` & `python_roborock-0.8.1/roborock/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 )
 from .roborock_future import RoborockFuture
 from .roborock_message import RoborockMessage
 from .typing import DeviceProp, DockSummary, RoborockCommand
 from .util import unpack_list
 
 _LOGGER = logging.getLogger(__name__)
+KEEPALIVE = 60
 QUEUE_TIMEOUT = 4
 SPECIAL_COMMANDS = [
     RoborockCommand.GET_MAP_V1,
 ]
 
 
 def md5hex(message: str) -> str:
@@ -85,24 +86,33 @@
 
 class RoborockClient:
     def __init__(self, endpoint: str, devices_info: Mapping[str, RoborockDeviceInfo]) -> None:
         self.devices_info = devices_info
         self._endpoint = endpoint
         self._nonce = secrets.token_bytes(16)
         self._waiting_queue: dict[int, RoborockFuture] = {}
-        self._status_listeners: list[Callable[[int, str], None]] = []
+        self._last_device_msg_in = self.time_func()
+        self._last_disconnection = self.time_func()
+        self.keep_alive = KEEPALIVE
 
-    def add_status_listener(self, callback: Callable[[int, str], None]):
-        self._status_listeners.append(callback)
+    @property
+    def time_func(self) -> Callable[[], float]:
+        try:
+            # Use monotonic clock if available
+            time_func = time.monotonic
+        except AttributeError:
+            time_func = time.time
+        return time_func
 
     async def async_disconnect(self) -> Any:
         raise NotImplementedError
 
     def on_message(self, messages: list[RoborockMessage]) -> None:
         try:
+            self._last_device_msg_in = self.time_func()
             for data in messages:
                 protocol = data.protocol
                 if protocol == 102 or protocol == 4:
                     payload = json.loads(data.payload.decode())
                     for data_point_number, data_point in payload.get("dps").items():
                         if data_point_number == "102":
                             data_point_response = json.loads(data_point)
@@ -138,14 +148,27 @@
                         if queue:
                             if isinstance(decrypted, list):
                                 decrypted = decrypted[0]
                             queue.resolve((decrypted, None))
         except Exception as ex:
             _LOGGER.exception(ex)
 
+    def on_disconnect(self, exc: Optional[Exception]) -> None:
+        self._last_disconnection = self.time_func()
+        _LOGGER.warning("Roborock client disconnected")
+        if exc is not None:
+            _LOGGER.warning(exc)
+
+    def should_keepalive(self) -> bool:
+        now = self.time_func()
+        # noinspection PyUnresolvedReferences
+        if now - self._last_disconnection > self.keep_alive**2 and now - self._last_device_msg_in > self.keep_alive:
+            return False
+        return True
+
     async def _async_response(self, request_id: int, protocol_id: int = 0) -> tuple[Any, VacuumError | None]:
         try:
             queue = RoborockFuture(protocol_id)
             self._waiting_queue[request_id] = queue
             (response, err) = await queue.async_get(QUEUE_TIMEOUT)
             return response, err
         except (asyncio.TimeoutError, asyncio.CancelledError):
```

### Comparing `python_roborock-0.8.0/roborock/cli.py` & `python_roborock-0.8.1/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/roborock/cloud_api.py` & `python_roborock-0.8.1/roborock/cloud_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 import uuid
 from asyncio import Lock
 from typing import Mapping, Optional
 from urllib.parse import urlparse
 
 import paho.mqtt.client as mqtt
 
-from .api import SPECIAL_COMMANDS, RoborockClient, md5hex
+from .api import SPECIAL_COMMANDS, RoborockClient, md5hex, KEEPALIVE
 from .containers import RoborockDeviceInfo, UserData
 from .exceptions import CommandVacuumError, RoborockException, VacuumError
 from .roborock_future import RoborockFuture
 from .roborock_message import RoborockMessage, RoborockParser, md5bin
 from .typing import RoborockCommand
 
 _LOGGER = logging.getLogger(__name__)
-MQTT_KEEPALIVE = 60
 CONNECT_REQUEST_ID = 0
 DISCONNECT_REQUEST_ID = 1
 
 
 class RoborockMqttClient(RoborockClient, mqtt.Client):
     _thread: threading.Thread
 
@@ -45,16 +44,14 @@
             super().tls_set()
         self._mqtt_password = rriot.s
         self._hashed_password = md5hex(self._mqtt_password + ":" + rriot.k)[16:]
         super().username_pw_set(self._hashed_user, self._hashed_password)
         self._endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
         self._waiting_queue: dict[int, RoborockFuture] = {}
         self._mutex = Lock()
-        self._last_device_msg_in = mqtt.time_func()
-        self._last_disconnection = mqtt.time_func()
         self.update_client_id()
 
     def __del__(self) -> None:
         self.sync_disconnect()
 
     def on_connect(self, *args, **kwargs) -> None:
         _, __, ___, rc, ____ = args
@@ -76,48 +73,37 @@
             return
         _LOGGER.info(f"Subscribed to topic {topic}")
         if connection_queue:
             connection_queue.resolve((True, None))
 
     def on_message(self, *args, **kwargs) -> None:
         _, __, msg = args
-        self._last_device_msg_in = mqtt.time_func()
         device_id = msg.topic.split("/").pop()
         messages, _ = RoborockParser.decode(msg.payload, self.devices_info[device_id].device.local_key)
         super().on_message(messages)
 
     def on_disconnect(self, *args, **kwargs) -> None:
         try:
             _, __, rc, ___ = args
-            self._last_disconnection = mqtt.time_func()
-            message = f"Roborock mqtt client disconnected (rc: {rc})"
+            super().on_disconnect(RoborockException(f"(rc: {rc})"))
             if rc == mqtt.MQTT_ERR_PROTOCOL:
                 self.update_client_id()
-            _LOGGER.warning(message)
             connection_queue = self._waiting_queue.get(DISCONNECT_REQUEST_ID)
             if connection_queue:
                 connection_queue.resolve((True, None))
         except Exception as ex:
             _LOGGER.exception(ex)
 
     def update_client_id(self):
         self._client_id = mqtt.base62(uuid.uuid4().int, padding=22)
 
-    def _async_check_keepalive(self) -> None:
-        now = mqtt.time_func()
-        # noinspection PyUnresolvedReferences
-        if (
-            now - self._last_disconnection > self._keepalive**2  # type: ignore[attr-defined]
-            and now - self._last_device_msg_in > self._keepalive  # type: ignore[attr-defined]
-        ):
-            self._ping_t = self._last_device_msg_in
-
     def _check_keepalive(self) -> None:
-        self._async_check_keepalive()
-        # noinspection PyUnresolvedReferences
+        if not self.should_keepalive():
+            self._ping_t = self.time_func() - KEEPALIVE
+            # noinspection PyUnresolvedReferences
         super()._check_keepalive()  # type: ignore[misc]
 
     def sync_stop_loop(self) -> None:
         if self._thread:
             _LOGGER.info("Stopping mqtt loop")
             super().loop_stop()
 
@@ -138,15 +124,15 @@
 
     def sync_connect(self) -> bool:
         self.sync_start_loop()
         if not self.is_connected():
             if self._mqtt_port is None or self._mqtt_host is None:
                 raise RoborockException("Mqtt information was not entered. Cannot connect.")
             _LOGGER.info("Connecting to mqtt")
-            super().connect_async(host=self._mqtt_host, port=self._mqtt_port, keepalive=MQTT_KEEPALIVE)
+            super().connect_async(host=self._mqtt_host, port=self._mqtt_port, keepalive=KEEPALIVE)
             return True
         return False
 
     async def async_disconnect(self) -> None:
         async with self._mutex:
             disconnecting = self.sync_disconnect()
             if disconnecting:
```

### Comparing `python_roborock-0.8.0/roborock/code_mappings.py` & `python_roborock-0.8.1/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/roborock/containers.py` & `python_roborock-0.8.1/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/roborock/exceptions.py` & `python_roborock-0.8.1/roborock/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Roborock exceptions."""
 
 
-class RoborockException(BaseException):
+class RoborockException(Exception):
     """Class for Roborock exceptions."""
 
 
 class RoborockTimeout(RoborockException):
     """Class for Roborock timeout exceptions."""
```

### Comparing `python_roborock-0.8.0/roborock/local_api.py` & `python_roborock-0.8.1/roborock/local_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
 class RoborockLocalClient(RoborockClient):
     def __init__(self, devices_info: Mapping[str, RoborockLocalDeviceInfo]):
         super().__init__("abc", devices_info)
         self.loop = get_running_loop_or_create_one()
         self.device_listener: dict[str, RoborockSocketListener] = {
             device_id: RoborockSocketListener(
-                device_info.network_info.ip,
-                device_info.device.local_key,
-                self.on_message,
+                device_info.network_info.ip, device_info.device.local_key, self.on_message, self.on_disconnect
             )
             for device_id, device_info in devices_info.items()
         }
         self._batch_structs: list[RoborockMessage] = []
         self._executing = False
 
     async def async_connect(self) -> None:
@@ -79,14 +77,17 @@
             roborock_messages = [roborock_messages]
         local_key = self.devices_info[device_id].device.local_key
         msg = RoborockParser.encode(roborock_messages, local_key)
         # Send the command to the Roborock device
         listener = self.device_listener.get(device_id)
         if listener is None:
             raise RoborockException(f"No device listener for {device_id}")
+        if not self.should_keepalive():
+            listener.disconnect()
+
         _LOGGER.debug(f"Requesting device with {roborock_messages}")
         await listener.send_message(msg)
 
         responses = await asyncio.gather(
             *[self.async_local_response(roborock_message) for roborock_message in roborock_messages],
             return_exceptions=True,
         )
@@ -109,35 +110,37 @@
     roborock_port = 58867
 
     def __init__(
         self,
         ip: str,
         local_key: str,
         on_message: Callable[[list[RoborockMessage]], None],
+        on_disconnect: Callable[[Optional[Exception]], None],
         timeout: float | int = QUEUE_TIMEOUT,
     ):
         self.ip = ip
         self.local_key = local_key
         self.loop = get_running_loop_or_create_one()
         self.on_message = on_message
+        self.on_disconnect = on_disconnect
         self.timeout = timeout
         self.remaining = b""
         self.transport: Transport | None = None
         self._mutex = Lock()
 
     def data_received(self, message):
         if self.remaining:
             message = self.remaining + message
             self.remaining = b""
         (parser_msg, remaining) = RoborockParser.decode(message, self.local_key)
         self.remaining = remaining
         self.on_message(parser_msg)
 
-    def connection_lost(self, exc):
-        _LOGGER.debug("The server closed the connection")
+    def connection_lost(self, exc: Optional[Exception]):
+        self.on_disconnect(exc)
 
     def is_connected(self):
         return self.transport and self.transport.is_reading()
 
     async def connect(self):
         try:
             if not self.is_connected():
```

### Comparing `python_roborock-0.8.0/roborock/roborock_future.py` & `python_roborock-0.8.1/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/roborock/roborock_message.py` & `python_roborock-0.8.1/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/roborock/typing.py` & `python_roborock-0.8.1/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/roborock/util.py` & `python_roborock-0.8.1/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.8.0/PKG-INFO` & `python_roborock-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.8.0 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.8.1 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

