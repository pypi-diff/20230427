# Comparing `tmp/pydevice2mqtt-0.2.2.tar.gz` & `tmp/pydevice2mqtt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydevice2mqtt-0.2.2.tar", last modified: Tue Apr 25 18:19:25 2023, max compression
+gzip compressed data, was "pydevice2mqtt-0.2.3.tar", last modified: Thu Apr 27 15:35:49 2023, max compression
```

## Comparing `pydevice2mqtt-0.2.2.tar` & `pydevice2mqtt-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1759 2023-04-25 18:12:28.120988 pydevice2mqtt-0.2.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.2/.gitignore
--rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.2/LICENSE
--rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.2/README.md
--rw-r--r--   0        0        0     1019 2023-04-25 18:19:22.918913 pydevice2mqtt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.2/src/pydevice2mqtt/__init__.py
--rw-r--r--   0        0        0     8761 2023-04-25 18:12:28.124989 pydevice2mqtt-0.2.2/src/pydevice2mqtt/pydevice2mqtt.py
--rw-r--r--   0        0        0    18871 2023-04-25 18:12:28.125991 pydevice2mqtt-0.2.2/src/pydevice2mqtt/remote_devices.py
--rw-r--r--   0        0        0     6830 2023-04-25 18:12:28.127986 pydevice2mqtt-0.2.2/test/pydevice2mqtt_test.py
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1759 2023-04-25 18:12:28.120988 pydevice2mqtt-0.2.3/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.3/README.md
+-rw-r--r--   0        0        0     1019 2023-04-27 15:15:54.993960 pydevice2mqtt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.3/src/pydevice2mqtt/__init__.py
+-rw-r--r--   0        0        0     8729 2023-04-27 14:59:29.570632 pydevice2mqtt-0.2.3/src/pydevice2mqtt/pydevice2mqtt.py
+-rw-r--r--   0        0        0    19883 2023-04-27 15:32:24.789036 pydevice2mqtt-0.2.3/src/pydevice2mqtt/remote_devices.py
+-rw-r--r--   0        0        0     7258 2023-04-27 15:14:55.747429 pydevice2mqtt-0.2.3/test/pydevice2mqtt_test.py
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.3/PKG-INFO
```

### Comparing `pydevice2mqtt-0.2.2/.github/workflows/python-app.yml` & `pydevice2mqtt-0.2.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.2/.gitignore` & `pydevice2mqtt-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.2/LICENSE` & `pydevice2mqtt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.2/README.md` & `pydevice2mqtt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.2/pyproject.toml` & `pydevice2mqtt-0.2.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 2e0d 0a20 2020 2053 7570 706f 7274 7320  ...    Supports 
 00000090: 7468 6520 4861 7373 6f20 6175 746f 2063  the Hasso auto c
 000000a0: 6f6e 6669 6775 7261 7469 6f6e 2070 726f  onfiguration pro
 000000b0: 746f 636f 6c0d 0a20 2020 2027 2727 0d0a  tocol..    '''..
 000000c0: 2020 2020 6c69 6365 6e73 6520 3d20 7b66      license = {f
 000000d0: 696c 6520 3d20 224c 4943 454e 5345 227d  ile = "LICENSE"}
 000000e0: 0d0a 2020 2020 7665 7273 696f 6e20 3d20  ..    version = 
-000000f0: 2230 2e32 2e32 220d 0a20 2020 2072 6561  "0.2.2"..    rea
+000000f0: 2230 2e32 2e33 220d 0a20 2020 2072 6561  "0.2.3"..    rea
 00000100: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
 00000110: 220d 0a20 2020 2072 6571 7569 7265 732d  "..    requires-
 00000120: 7079 7468 6f6e 203d 2022 3e3d 332e 3722  python = ">=3.7"
 00000130: 0d0a 2020 2020 6175 7468 6f72 7320 3d20  ..    authors = 
 00000140: 5b7b 6e61 6d65 3d22 4869 6768 496d 7022  [{name="HighImp"
 00000150: 2c20 656d 6169 6c3d 2241 6e79 4869 6768  , email="AnyHigh
 00000160: 5a40 676d 6169 6c2e 636f 6d22 7d5d 0d0a  Z@gmail.com"}]..
```

### Comparing `pydevice2mqtt-0.2.2/src/pydevice2mqtt/pydevice2mqtt.py` & `pydevice2mqtt-0.2.3/src/pydevice2mqtt/pydevice2mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,15 @@
 
         assert set(remote_devices.keys()).issubset(set(self._supported_device_classes.keys()))
         for remote_device_class, devices in remote_devices.items():
             for object_id, device_settings in devices.items():
                 device_settings["object_id"] = object_id
                 new_device: RemoteDevice = self._supported_device_classes[remote_device_class](device_settings,
                                                                                                mqtt_settings)
-                new_device_uid = new_device.get_uid()
-                self._devices[new_device_uid] = new_device
+                self._devices[new_device.get_id()] = new_device
 
         self._subscribed_channels_dict = {}
         for topic_function_dict in [device.get_device_topics() for device in self._devices.values()]:
             self._subscribed_channels_dict.update(topic_function_dict)
 
         self._bridge_name = mqtt_settings["bridge_name"]
         self._node_channel = f'{mqtt_settings["operating_prefix"]}/{self._bridge_name}/#'
@@ -167,29 +166,29 @@
             logging.warning(f"Detect unsubscribed channel for this node: {msg.topic}")
         except Exception as error:
             logging.error(f"Catching unhandled error inside of an device: {error}")
 
     def configure_devices(self):
         """Register Bridge Devices by write the config in HASSIO style to the discovery channel
         """
-        for uid, device in self._devices.items():
-            logging.debug(f"Configure: {uid}")
+        for dev_id, device in self._devices.items():
+            logging.debug(f"Configure: {dev_id}")
             discover_info = device.get_discovery()
             self._mqtt_client.publish(topic=discover_info[0],
                                       payload=json.dumps(discover_info[1]),
                                       retain=True,
                                       qos=1)
             logging.debug(f'{discover_info[0]}: "{discover_info[1]}"')
 
     def delete_devices(self):
         """Unregister all devices by flushing the Discovery Channel
         """
-        for uid, device in self._devices.items():  # type: RemoteDevice
-            logging.debug(f"Unlink: {uid}")
+        for dev_id, device in self._devices.items():  # type: RemoteDevice
+            logging.debug(f"Unlink: {dev_id}")
             discover_info = device.get_discovery()
             self._mqtt_client.publish(topic=discover_info[0],
                                       payload="")
 
     def get_devices(self) -> Dict[str, RemoteDevice]:
         """Return a dict with all registered devices
         """
-        return {uid: device for uid, device in self._devices.items()}
+        return {dev_id: device for dev_id, device in self._devices.items()}
```

### Comparing `pydevice2mqtt-0.2.2/src/pydevice2mqtt/remote_devices.py` & `pydevice2mqtt-0.2.3/src/pydevice2mqtt/remote_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import json
 import logging
 import time
 from collections import namedtuple, defaultdict
 
 try:
     import espeak
@@ -20,56 +21,70 @@
     _BASE_CONFIG_REQ = {
         "name": str,  # Display Name
     }
 
     _CONFIG_REQ = {}
 
     def __init__(self, device_settings: dict, mqtt_settings: dict):
-        self._operation_topics = defaultdict(MQTTChannel)
 
-        self._config: dict = {}
-        self._config["object_id"] = device_settings["object_id"]
-        self._discovery_prefix = f"{mqtt_settings['discovery_prefix']}/" \
-                                 f"{device_settings['device_class']}/" \
-                                 f"{mqtt_settings['bridge_name']}/" \
-                                 f"{self.get_uid()}/"
+        uid_string = f"{mqtt_settings['operating_prefix']}_" \
+                     f"{mqtt_settings['bridge_name']}_" \
+                     f"{self.__class__.__name__}_" \
+                     f"{device_settings['object_id']}"
 
-        self._operating_prefix = f"{mqtt_settings['operating_prefix']}/" \
-                                 f"{mqtt_settings['bridge_name']}/" \
-                                 f"{self.get_uid()}/"
-
-        self._logging_channel = None
-        if mqtt_settings["logging"]:
-            self._logging_channel = f"{mqtt_settings['operating_prefix']}/" \
-                                    f"{mqtt_settings['bridge_name']}/" \
-                                    f"{self.get_uid()}/" \
-                                    f"log"
-
-        self._config["topic"] = f"{self._discovery_prefix}config"
-
-        self._add_channel(channel_name="state_topic",
-                          sub_topic="state",
-                          on_message=None)
+        uid_hash = hashlib.new("sha1", data=uid_string.encode(), usedforsecurity=False)
+        self._uid = uid_hash.hexdigest()[:16]
 
         self._device_class = device_settings['device_class']
-        self._config["name"] = device_settings["name"]
+
+        # prepare auto config dict
+        self._config: dict = {"device": {"identifiers": [f"{mqtt_settings['operating_prefix']}_"
+                                                         f"{mqtt_settings['bridge_name']}"],
+                                         "name": mqtt_settings['bridge_name']}, "name": device_settings["name"],
+                              "unique_id": self._uid,
+                              "object_id": device_settings["object_id"]}
 
         # some devices may need special attributes to appear in a special manner in hassio,
         # there are too many to handle all of them, so add them via generic dict from config on demand
         if "opt_attr" in device_settings.keys():
             attribute = None
             try:
                 for attribute, value in device_settings["opt_attr"].items():
                     assert attribute not in self._config.keys()
                     self._config[attribute] = value
             except (TypeError, AttributeError, KeyError):
                 logging.warning("Could not apply optional attributes!")
             except AssertionError:
                 logging.warning(f"Could not overwrite a required item with the optional dict ({attribute})")
 
+        self._discovery_prefix = f"{mqtt_settings['discovery_prefix']}/" \
+                                 f"{device_settings['device_class']}/" \
+                                 f"{mqtt_settings['bridge_name']}/" \
+                                 f"{self.get_id()}/"
+
+        # store the discovery topic
+        self._config["discovery_topic"] = f"{self._discovery_prefix}config"
+
+        # prepare mqtt channels
+        self._operation_topics = defaultdict(MQTTChannel)
+        self._operating_prefix = f"{mqtt_settings['operating_prefix']}/" \
+                                 f"{mqtt_settings['bridge_name']}/" \
+                                 f"{self.get_id()}/"
+
+        self._logging_channel = None
+        if mqtt_settings["logging"]:
+            self._logging_channel = f"{mqtt_settings['operating_prefix']}/" \
+                                    f"{mqtt_settings['bridge_name']}/" \
+                                    f"{self.get_id()}/" \
+                                    f"log"
+
+        self._add_channel(channel_name="state_topic",
+                          sub_topic="state",
+                          on_message=None)
+
         # connect self._publish to the function publish
         self._publish = mqtt_settings["f_publish"]
 
     def _log_remote(self, *args, **kwargs):
 
         level = getattr(kwargs, "Level", logging.DEBUG)
         print_string = "".join(map(str, args))
@@ -111,20 +126,29 @@
         :param sub_topic: mqtt subtopic after the device topic (read hassio documentation)
         :param on_message: function to call if a message is received on this channel
         :return: None
         """
 
         self._operation_topics[channel_name] = MQTTChannel(self._operating_prefix + sub_topic, on_message)
 
+    def get_id(self) -> str:
+        """Get a human readable ID of the device,
+        unique in this bridge
+
+        :return: ID as string
+        """
+        return f"{self.__class__.__name__}_{self.get_object_id()}"
+
     def get_uid(self) -> str:
-        """Get a ID that is unique in this bridge
+        """Get a real UID of the endpoint,
+        sha1 hash over bridge and device information
 
-        :return: Unique ID as string
+        :return: UID as string
         """
-        return f"{self.__class__.__name__}_{self._config['object_id']}"
+        return self._uid
 
     def get_object_id(self) -> str:
         """Get the object id provided in the config file,
         useful to filter devices of one type
         """
         return self._config['object_id']
 
@@ -136,19 +160,19 @@
         """
         return self._config["name"]
 
     def get_discovery(self) -> tuple:
         """"
         Generate the config dictionary in MQTT Discovery stile
 
-        :return: auto discover tuple with the discovery channel on index 0
+        :return: auto discover tuple with the discovery topic on index 0
         """
 
         auto_config = {**self._config, **{name: channel.topic for (name, channel) in self._operation_topics.items()}}
-        topic = auto_config.pop("topic")
+        topic = auto_config.pop("discovery_topic")
 
         return topic, auto_config
 
     def get_device_topics(self) -> dict:
         """
         Return all mqtt topics this device will listen on or publish to,
         dict with the mqtt topic as key and the callback function (if set) as value
@@ -495,8 +519,7 @@
 
         if target_state == "OFF":
             if self._running_process is None:
                 self._log_remote("Process already stopped")
                 return
 
             self._running_process.kill()
-
```

### Comparing `pydevice2mqtt-0.2.2/test/pydevice2mqtt_test.py` & `pydevice2mqtt-0.2.3/test/pydevice2mqtt_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,18 @@
             subscribed_channels.append(topic)
 
         discover_topic, discover_info = device.get_discovery()
         assert str(discover_topic).startswith(EXAMPLE_MQTT_SETTINGS["discovery_prefix"])
         assert str(discover_topic).endswith("config")
         assert str(discover_info["state_topic"]).startswith(EXAMPLE_MQTT_SETTINGS["operating_prefix"])
         assert str(discover_info["state_topic"]).endswith("state")
+        assert discover_info["device"]["name"] == EXAMPLE_MQTT_SETTINGS["bridge_name"]
+        assert discover_info["device"]["identifiers"][0] == f"{EXAMPLE_MQTT_SETTINGS['operating_prefix']}_" \
+                                                            f"{EXAMPLE_MQTT_SETTINGS['bridge_name']}"
+        assert discover_info["unique_id"] == device.get_uid()
     my_bridge.configure_devices()
 
     assert mqtt_client.called
 
 
 def test_arbitrary_sensor(mocker):
     import pydevice2mqtt
@@ -109,18 +113,18 @@
 
     device_class = {"ArbitrarySensor": pydevice2mqtt.remote_devices.ArbitrarySensor}
 
     my_bridge: pydevice2mqtt.DeviceBridge = create_device_bridge(mocked_module=pydevice2mqtt,
                                                                  device_classes=device_class)
 
     sensor_instance: pydevice2mqtt.remote_devices.ArbitrarySensor
-    expected_uid = f"ArbitrarySensor_{EXAMPLE_DATA[str]}"
+    expected_dev_id = f"ArbitrarySensor_{EXAMPLE_DATA[str]}"
 
-    sensor_instance = my_bridge.get_devices()[expected_uid]
-    assert sensor_instance.get_uid() == expected_uid
+    sensor_instance = my_bridge.get_devices()[expected_dev_id]
+    assert sensor_instance.get_id() == expected_dev_id
     assert sensor_instance.get_object_id() == EXAMPLE_DATA[str]
     assert sensor_instance.get_name() == EXAMPLE_DATA[str]
     assert len(mqtt_client.mock_calls) == 3
     sensor_instance.set_value(1)
     assert len(mqtt_client.mock_calls) == 4
     set_value_call_kwargs = mqtt_client.mock_calls[-1].kwargs
     try:
@@ -164,11 +168,11 @@
     pydevice2mqtt.DeviceBridge.update_config(devices=device_config2, config_file=test_config_file)
     my_bridge: pydevice2mqtt.DeviceBridge = create_device_bridge(mocked_module=pydevice2mqtt,
                                                                  new_config=False)
     devices = my_bridge.get_devices()
     assert len(devices) == 3
 
     assert devices["RpiGpio_GPIO_PIN5"].get_discovery()[1]["gen_attr"] == "unrequired_info"
-
+    print(devices["RpiGpio_GPIO_PIN5"].get_discovery())
 
 if __name__ == "__main__":
     pytest.main(["-s", __file__])
```

### Comparing `pydevice2mqtt-0.2.2/PKG-INFO` & `pydevice2mqtt-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydevice2mqtt
-Version: 0.2.2
+Version: 0.2.3
 Summary:     This project provides a simplified control of devices via MQTT.
             Supports the Hasso auto configuration protocol
             
 Keywords: hassio,mqtt,homeassistent,homeautomation
 Author-email: HighImp <AnyHighZ@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

