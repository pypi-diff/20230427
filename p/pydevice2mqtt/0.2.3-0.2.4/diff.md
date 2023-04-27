# Comparing `tmp/pydevice2mqtt-0.2.3.tar.gz` & `tmp/pydevice2mqtt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydevice2mqtt-0.2.3.tar", last modified: Thu Apr 27 15:35:49 2023, max compression
+gzip compressed data, was "pydevice2mqtt-0.2.4.tar", last modified: Thu Apr 27 19:18:04 2023, max compression
```

## Comparing `pydevice2mqtt-0.2.3.tar` & `pydevice2mqtt-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1759 2023-04-25 18:12:28.120988 pydevice2mqtt-0.2.3/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.3/.gitignore
--rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.3/LICENSE
--rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.3/README.md
--rw-r--r--   0        0        0     1019 2023-04-27 15:15:54.993960 pydevice2mqtt-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.3/src/pydevice2mqtt/__init__.py
--rw-r--r--   0        0        0     8729 2023-04-27 14:59:29.570632 pydevice2mqtt-0.2.3/src/pydevice2mqtt/pydevice2mqtt.py
--rw-r--r--   0        0        0    19883 2023-04-27 15:32:24.789036 pydevice2mqtt-0.2.3/src/pydevice2mqtt/remote_devices.py
--rw-r--r--   0        0        0     7258 2023-04-27 15:14:55.747429 pydevice2mqtt-0.2.3/test/pydevice2mqtt_test.py
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1759 2023-04-25 18:12:28.120988 pydevice2mqtt-0.2.4/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.4/README.md
+-rw-r--r--   0        0        0     1019 2023-04-27 19:17:58.434145 pydevice2mqtt-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.4/src/pydevice2mqtt/__init__.py
+-rw-r--r--   0        0        0     8729 2023-04-27 14:59:29.570632 pydevice2mqtt-0.2.4/src/pydevice2mqtt/pydevice2mqtt.py
+-rw-r--r--   0        0        0    19853 2023-04-27 19:15:40.305270 pydevice2mqtt-0.2.4/src/pydevice2mqtt/remote_devices.py
+-rw-r--r--   0        0        0     7258 2023-04-27 15:14:55.747429 pydevice2mqtt-0.2.4/test/pydevice2mqtt_test.py
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.4/PKG-INFO
```

### Comparing `pydevice2mqtt-0.2.3/.github/workflows/python-app.yml` & `pydevice2mqtt-0.2.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.3/.gitignore` & `pydevice2mqtt-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.3/LICENSE` & `pydevice2mqtt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.3/README.md` & `pydevice2mqtt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.3/pyproject.toml` & `pydevice2mqtt-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 2e0d 0a20 2020 2053 7570 706f 7274 7320  ...    Supports 
 00000090: 7468 6520 4861 7373 6f20 6175 746f 2063  the Hasso auto c
 000000a0: 6f6e 6669 6775 7261 7469 6f6e 2070 726f  onfiguration pro
 000000b0: 746f 636f 6c0d 0a20 2020 2027 2727 0d0a  tocol..    '''..
 000000c0: 2020 2020 6c69 6365 6e73 6520 3d20 7b66      license = {f
 000000d0: 696c 6520 3d20 224c 4943 454e 5345 227d  ile = "LICENSE"}
 000000e0: 0d0a 2020 2020 7665 7273 696f 6e20 3d20  ..    version = 
-000000f0: 2230 2e32 2e33 220d 0a20 2020 2072 6561  "0.2.3"..    rea
+000000f0: 2230 2e32 2e34 220d 0a20 2020 2072 6561  "0.2.4"..    rea
 00000100: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
 00000110: 220d 0a20 2020 2072 6571 7569 7265 732d  "..    requires-
 00000120: 7079 7468 6f6e 203d 2022 3e3d 332e 3722  python = ">=3.7"
 00000130: 0d0a 2020 2020 6175 7468 6f72 7320 3d20  ..    authors = 
 00000140: 5b7b 6e61 6d65 3d22 4869 6768 496d 7022  [{name="HighImp"
 00000150: 2c20 656d 6169 6c3d 2241 6e79 4869 6768  , email="AnyHigh
 00000160: 5a40 676d 6169 6c2e 636f 6d22 7d5d 0d0a  Z@gmail.com"}]..
```

### Comparing `pydevice2mqtt-0.2.3/src/pydevice2mqtt/pydevice2mqtt.py` & `pydevice2mqtt-0.2.4/src/pydevice2mqtt/pydevice2mqtt.py`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.3/src/pydevice2mqtt/remote_devices.py` & `pydevice2mqtt-0.2.4/src/pydevice2mqtt/remote_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,22 @@
         uid_string = f"{mqtt_settings['operating_prefix']}_" \
                      f"{mqtt_settings['bridge_name']}_" \
                      f"{self.__class__.__name__}_" \
                      f"{device_settings['object_id']}"
 
         uid_hash = hashlib.new("sha1", data=uid_string.encode(), usedforsecurity=False)
         self._uid = uid_hash.hexdigest()[:16]
-
+        self._object_id = device_settings['object_id']
         self._device_class = device_settings['device_class']
 
         # prepare auto config dict
         self._config: dict = {"device": {"identifiers": [f"{mqtt_settings['operating_prefix']}_"
                                                          f"{mqtt_settings['bridge_name']}"],
                                          "name": mqtt_settings['bridge_name']}, "name": device_settings["name"],
-                              "unique_id": self._uid,
-                              "object_id": device_settings["object_id"]}
+                              "unique_id": self._uid}
 
         # some devices may need special attributes to appear in a special manner in hassio,
         # there are too many to handle all of them, so add them via generic dict from config on demand
         if "opt_attr" in device_settings.keys():
             attribute = None
             try:
                 for attribute, value in device_settings["opt_attr"].items():
@@ -146,15 +145,15 @@
         """
         return self._uid
 
     def get_object_id(self) -> str:
         """Get the object id provided in the config file,
         useful to filter devices of one type
         """
-        return self._config['object_id']
+        return self._object_id
 
     def get_name(self) -> str:
         """
         Get the given name of the device, defined in config
 
         :return: name of the device
         """
```

### Comparing `pydevice2mqtt-0.2.3/test/pydevice2mqtt_test.py` & `pydevice2mqtt-0.2.4/test/pydevice2mqtt_test.py`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.3/PKG-INFO` & `pydevice2mqtt-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydevice2mqtt
-Version: 0.2.3
+Version: 0.2.4
 Summary:     This project provides a simplified control of devices via MQTT.
             Supports the Hasso auto configuration protocol
             
 Keywords: hassio,mqtt,homeassistent,homeautomation
 Author-email: HighImp <AnyHighZ@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

