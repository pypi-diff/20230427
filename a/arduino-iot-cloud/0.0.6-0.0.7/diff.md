# Comparing `tmp/arduino_iot_cloud-0.0.6.tar.gz` & `tmp/arduino_iot_cloud-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arduino_iot_cloud-0.0.6.tar", last modified: Wed Apr 12 09:58:21 2023, max compression
+gzip compressed data, was "arduino_iot_cloud-0.0.7.tar", last modified: Thu Apr 27 11:04:59 2023, max compression
```

## Comparing `arduino_iot_cloud-0.0.6.tar` & `arduino_iot_cloud-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/examples/micropython.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ucloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/umqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ussl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 09:58:21.000000 arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:21.907830 arduino_iot_cloud-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:58:07.000000 arduino_iot_cloud-0.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.707756 arduino_iot_cloud-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/examples/micropython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.707756 arduino_iot_cloud-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ucloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/umqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ussl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 11:04:59.000000 arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:59.711757 arduino_iot_cloud-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:04:43.000000 arduino_iot_cloud-0.0.7/tests/__init__.py
```

### Comparing `arduino_iot_cloud-0.0.6/LICENSE` & `arduino_iot_cloud-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.6/PKG-INFO` & `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: arduino_iot_cloud
-Version: 0.0.6
+Name: arduino-iot-cloud
+Version: 0.0.7
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
@@ -15,39 +15,51 @@
 
 # Arduino IoT Cloud Python client ☁️🐍☁️
 This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
 
 ## Minimal Example
 The following basic example shows how to connect to the Arduino IoT cloud using basic username and password authentication, and control an LED from a dashboard's switch widget.
 ```python
+from secrets import DEVICE_ID
+from secrets import SECRET_KEY
+
 # Switch callback, toggles the LED.
 def on_switch_changed(client, value):
     # Note the client object passed to this function can be used to access
     # and modify any registered cloud object. The following line updates
     # the LED value.
     client["led"] = value
 
 # 1. Create a client object, which is used to connect to the IoT cloud and link local
 # objects to cloud objects. Note a username and password can be used for basic authentication
 # on both CPython and MicroPython. For more advanced authentication methods, please see the examples.
-client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
 
 # 2. Register cloud objects.
 # Note: The following objects must be created first in the dashboard and linked to the device.
 # When the switch is toggled from the dashboard, the on_switch_changed function is called with
 # the client object and new value args.
 client.register("sw1", value=None, on_write=on_switch_changed)
 
 # The LED object is updated in the switch's on_write callback.
 client.register("led", value=None)
 
 # 3. Start the Arduino cloud client.
 client.start()
 ```
 
+Your `secrets.py` file should look like this:
+
+```python
+WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
+WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
+DEVICE_ID  = b"" # Provided by Arduino cloud when creating a device.
+SECRET_KEY = b"" # Provided by Arduino cloud when creating a device.
+```
+
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
 
 #### Create softhsm token
 Using the first available slot, in this case 0
```

### Comparing `arduino_iot_cloud-0.0.6/README.md` & `arduino_iot_cloud-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 # Arduino IoT Cloud Python client ☁️🐍☁️
 This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
 
 ## Minimal Example
 The following basic example shows how to connect to the Arduino IoT cloud using basic username and password authentication, and control an LED from a dashboard's switch widget.
 ```python
+from secrets import DEVICE_ID
+from secrets import SECRET_KEY
+
 # Switch callback, toggles the LED.
 def on_switch_changed(client, value):
     # Note the client object passed to this function can be used to access
     # and modify any registered cloud object. The following line updates
     # the LED value.
     client["led"] = value
 
 # 1. Create a client object, which is used to connect to the IoT cloud and link local
 # objects to cloud objects. Note a username and password can be used for basic authentication
 # on both CPython and MicroPython. For more advanced authentication methods, please see the examples.
-client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
 
 # 2. Register cloud objects.
 # Note: The following objects must be created first in the dashboard and linked to the device.
 # When the switch is toggled from the dashboard, the on_switch_changed function is called with
 # the client object and new value args.
 client.register("sw1", value=None, on_write=on_switch_changed)
 
 # The LED object is updated in the switch's on_write callback.
 client.register("led", value=None)
 
 # 3. Start the Arduino cloud client.
 client.start()
 ```
 
+Your `secrets.py` file should look like this:
+
+```python
+WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
+WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
+DEVICE_ID  = b"" # Provided by Arduino cloud when creating a device.
+SECRET_KEY = b"" # Provided by Arduino cloud when creating a device.
+```
+
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
 
 #### Create softhsm token
 Using the first available slot, in this case 0
```

### Comparing `arduino_iot_cloud-0.0.6/examples/example.py` & `arduino_iot_cloud-0.0.7/examples/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 from arduino_iot_cloud import Schedule
 from arduino_iot_cloud import ColoredLight
 from arduino_iot_cloud import Task
 from random import uniform
 import argparse
 import arduino_iot_cloud.ussl as ssl
 
+from secrets import DEVICE_ID
+from secrets import SECRET_KEY  # noqa
+
 KEY_PATH = "pkcs11:token=arduino"
 CERT_PATH = "pkcs11:token=arduino"
 CA_PATH = "ca-root.pem"
-DEVICE_ID = b"fcbb21b8-b5b8-4961-a89f-a3f1abda7957"
 
 
 def on_switch_changed(client, value):
     # This is a write callback for the switch that toggles the LED variable. The LED
     # variable can be accessed via the client object passed in the first argument.
     client["led"] = value
 
@@ -55,15 +57,15 @@
         level=logging.DEBUG if args.debug else logging.INFO,
     )
 
     # Create a client object to connect to the Arduino IoT cloud.
     # To use a secure element, set the token's "pin" and URI in "keyfile" and "certfile", and
     # the CA certificate (if any) in "ssl_params". Alternatively, a username and password can
     # be used to authenticate, for example:
-    #   client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+    #   client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
     client = ArduinoCloudClient(
         device_id=DEVICE_ID,
         ssl_params={
             "pin": "1234",
             "keyfile": KEY_PATH, "certfile": CERT_PATH, "ca_certs": CA_PATH, "cert_reqs": ssl.CERT_REQUIRED
         },
     )
```

### Comparing `arduino_iot_cloud-0.0.6/examples/micropython.py` & `arduino_iot_cloud-0.0.7/examples/micropython.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from arduino_iot_cloud import Schedule
 from arduino_iot_cloud import ColoredLight
 from arduino_iot_cloud import Task
 from arduino_iot_cloud import CADATA
 from random import uniform
 from secrets import WIFI_SSID
 from secrets import WIFI_PASS
+from secrets import DEVICE_ID
+from secrets import SECRET_KEY  # noqa
 
 KEY_PATH = "key.der"
 CERT_PATH = "cert.der"
-DEVICE_ID = b"fcbb21b8-b5b8-4961-a89f-a3f1abda7957"
 
 
 def on_switch_changed(client, value):
     # This is a write callback for the switch that toggles the LED variable. The LED
     # variable can be accessed via the client object passed in the first argument.
     client["led"] = value
 
@@ -64,15 +65,15 @@
 
     # NOTE: Add networking code here or in boot.py
     wifi_connect()
 
     # Create a client object to connect to the Arduino IoT cloud.
     # For MicroPython, the key and cert files must be stored in DER format on the filesystem.
     # Alternatively, a username and password can be used to authenticate:
-    #   client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+    #   client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
     client = ArduinoCloudClient(
         device_id=DEVICE_ID,
         ssl_params={
             "keyfile": KEY_PATH, "certfile": CERT_PATH, "cadata": CADATA, "cert_reqs": ussl.CERT_REQUIRED
         }
     )
```

### Comparing `arduino_iot_cloud-0.0.6/package.json` & `arduino_iot_cloud-0.0.7/package.json`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.6/pyproject.toml` & `arduino_iot_cloud-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/__init__.py` & `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ucloud.py` & `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ucloud.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/umqtt.py` & `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/umqtt.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud/ussl.py` & `arduino_iot_cloud-0.0.7/src/arduino_iot_cloud/ussl.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,23 +28,28 @@
     pkcs11.init()
     _key = pkcs11.load_private_key(keyfile)
     _cert = pkcs11.load_certificate(certfile)
 
 
 def wrap_socket(
     sock_in,
-    pin,
-    certfile,
-    keyfile,
+    pin=None,
+    certfile=None,
+    keyfile=None,
     ca_certs=None,
     cert_reqs=CERT_NONE,
     ciphers=None,
     engine_path=_ENGINE_PATH,
     module_path=_MODULE_PATH,
 ):
+    if certfile is None or keyfile is None:
+        # Fallback to Python's SSL
+        import ssl
+        return ssl.wrap_socket(sock_in)
+
     if _key is None or _cert is None:
         init(pin, certfile, keyfile, engine_path, module_path)
 
     # Create SSL context
     ctx = SSL.Context("tls")
     ctx.set_default_verify_paths()
     ctx.set_allow_unknown_ca(False)
```

### Comparing `arduino_iot_cloud-0.0.6/src/arduino_iot_cloud.egg-info/PKG-INFO` & `arduino_iot_cloud-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: arduino-iot-cloud
-Version: 0.0.6
+Name: arduino_iot_cloud
+Version: 0.0.7
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
@@ -15,39 +15,51 @@
 
 # Arduino IoT Cloud Python client ☁️🐍☁️
 This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
 
 ## Minimal Example
 The following basic example shows how to connect to the Arduino IoT cloud using basic username and password authentication, and control an LED from a dashboard's switch widget.
 ```python
+from secrets import DEVICE_ID
+from secrets import SECRET_KEY
+
 # Switch callback, toggles the LED.
 def on_switch_changed(client, value):
     # Note the client object passed to this function can be used to access
     # and modify any registered cloud object. The following line updates
     # the LED value.
     client["led"] = value
 
 # 1. Create a client object, which is used to connect to the IoT cloud and link local
 # objects to cloud objects. Note a username and password can be used for basic authentication
 # on both CPython and MicroPython. For more advanced authentication methods, please see the examples.
-client = ArduinoCloudClient(device_id=b"DEVICE_ID", username=b"DEVICE_ID", password=b"SECRET_KEY")
+client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
 
 # 2. Register cloud objects.
 # Note: The following objects must be created first in the dashboard and linked to the device.
 # When the switch is toggled from the dashboard, the on_switch_changed function is called with
 # the client object and new value args.
 client.register("sw1", value=None, on_write=on_switch_changed)
 
 # The LED object is updated in the switch's on_write callback.
 client.register("led", value=None)
 
 # 3. Start the Arduino cloud client.
 client.start()
 ```
 
+Your `secrets.py` file should look like this:
+
+```python
+WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
+WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
+DEVICE_ID  = b"" # Provided by Arduino cloud when creating a device.
+SECRET_KEY = b"" # Provided by Arduino cloud when creating a device.
+```
+
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
 
 #### Create softhsm token
 Using the first available slot, in this case 0
```

