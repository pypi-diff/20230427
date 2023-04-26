# Comparing `tmp/python-can-bluetooth-0.1.1.tar.gz` & `tmp/python-can-bluetooth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-can-bluetooth-0.1.1.tar", last modified: Wed Jan 25 19:45:34 2023, max compression
+gzip compressed data, was "python-can-bluetooth-0.1.2.tar", last modified: Wed Apr 26 22:11:54 2023, max compression
```

## Comparing `python-can-bluetooth-0.1.1.tar` & `python-can-bluetooth-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 19:45:34.836507 python-can-bluetooth-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-01-25 19:45:34.836507 python-can-bluetooth-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 19:45:34.836507 python-can-bluetooth-0.1.1/can_bluetooth/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/can_bluetooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16574 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/can_bluetooth/_bluetooth_can.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/can_bluetooth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 19:45:34.836507 python-can-bluetooth-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/examples/bluetooth_tx_example.py
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 19:45:34.836507 python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-01-25 19:45:34.000000 python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-01-25 19:45:34.000000 python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-25 19:45:34.000000 python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-01-25 19:45:34.000000 python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-01-25 19:45:34.000000 python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-01-25 19:45:34.000000 python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-01-25 19:45:34.836507 python-can-bluetooth-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-25 19:45:34.836507 python-can-bluetooth-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7097 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/test/test_interface_bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-01-25 19:45:23.000000 python-can-bluetooth-0.1.1/test/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.641863 python-can-bluetooth-0.1.2/can_bluetooth/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth/_bluetooth_can.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.641863 python-can-bluetooth-0.1.2/can_bluetooth_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_examples/bluetooth_tx_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/can_bluetooth_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_test/test_interface_bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-26 22:11:54.649863 python-can-bluetooth-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/setup.py
```

### Comparing `python-can-bluetooth-0.1.1/PKG-INFO` & `python-can-bluetooth-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can-bluetooth
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python-can interface driver for CAN transmitted over a Bluetooth SPP connection
 Author-email: Matt Woodhead <woody.w62@gmail.com>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: homepage, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: documentation, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: repository, https://github.com/MattWoodhead/python-can-bluetooth
 Keywords: CANbus,Bluetooth,python-can,ESP32
```

### Comparing `python-can-bluetooth-0.1.1/README.rst` & `python-can-bluetooth-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-can-bluetooth-0.1.1/can_bluetooth/_bluetooth_can.py` & `python-can-bluetooth-0.1.2/can_bluetooth/_bluetooth_can.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 import io
 import logging
 import string
 import struct
 import time
 from typing import Any, List, Tuple, Optional
 
-from can import BusABC, BusState, Message
 from can import (
+    BusABC,
+    BusState,
     CanError,
     CanInterfaceNotImplementedError,
     CanInitializationError,
     CanOperationError,
     CanTimeoutError,
+    Message,
 )
 from can.typechecking import AutoDetectedConfig
 
 logger = logging.getLogger("can.bluetoothspp")
 
 try:
     import serial
@@ -76,15 +78,15 @@
 
     def __init__(
         self,
         channel: str,
         bitrate: int = 250000,
         bt_baudrate: int = 921600,
         timeout: float = 0.1,
-        state: int = BusState.PASSIVE,
+        state: BusState = BusState.PASSIVE,
         rtscts: bool = False,
         timestamps_use_computer_time: bool = True,
         *args,
         **kwargs,
     ) -> None:
         """
         :param channel:
@@ -132,19 +134,29 @@
             self._bus_pc_start_time_s = round(time.time(), 4)
         else:
             self._bus_pc_start_time_s = 0
 
         # interface configuration attributes
         # if these are changed after initialisation, self._send_interface_can_config() must be called
         self.bitrate = bitrate  # CAN Bit rate
-        self.state = state  # 0 = Active, 1 = passive, 2 = error
+        self._state = state  # 0 = Active, 1 = passive, 2 = error
         self.interface_enable_can = True  # Enable/disable can interface
 
         super().__init__(channel, *args, **kwargs)
 
+    @property
+    def state(self):
+        return self._state
+
+    @state.setter
+    def state(self, new_state):
+        # declare here, which is called by __init__()
+        self._state = new_state  # pylint: disable=attribute-defined-outside-init
+        self._send_interface_can_config()
+
     def shutdown(self) -> None:
         """
         Close the serial interface.
         """
         super().shutdown()
         self._ser.close()
 
@@ -343,37 +355,38 @@
 
     def _process_interface_msg(self, message_obj: Message = None) -> Tuple[Optional[Message], bool]:
         """
         This private function processes any messages from the interface board. Generally these are responses to
         confiuration requests or IO statuses for some implementations of the bluetooth interface.
         """
         print("Received interface message:", message_obj)
-        pass  # TODO
+        # TODO
 
     def set_device_bt_name(self, name: str = "") -> bool:
+        """
+        This method sends a message containing a string to the bluetooth CAN adapter. The adapter then changes
+        its name to match the sent string.
+        """
 
         if not isinstance(name, str):
             return False
         name.strip()
         if not name:
             return False
 
         allowed_chars = set(string.ascii_letters + string.digits + "_-")
         if set(name) - allowed_chars:  # if the name contains characters that arent allowed
-            # TODO raise exception
-            return False
+            raise ValueError(f"The bluetooth name can only contain {allowed_chars}" f"Provided name: '{name}'")
 
         string_chunk_len = 7  # 7 bytes - the eighth is used as a message counter (i.e. message)
         string_chunks = [name[i : i + string_chunk_len] for i in range(0, len(name), string_chunk_len)]
         number_of_chunks = len(string_chunks)
 
         if len(string_chunks) > 0xF:
-            print("The bluetooth name cannot be more than 35 characters")
-            # TODO: raise exception
-            return False
+            raise ValueError("The bluetooth name cannot be more than 35 characters")
 
         for i, chunk in enumerate(string_chunks):
             config_msg = Message(arbitration_id=0x002, is_extended_id=False)
             # bits 0-3 are the message number, 4-7 is the total number of messages
             config_msg.data += i + (number_of_chunks << 4)
             config_msg.data += chunk.encode("ASCII")
             self.send(config_msg, interface_control=True)
@@ -383,15 +396,15 @@
     def _send_interface_can_config(self) -> bool:
         """
         This private function sends the values of the class configuration attributes to the BT interface
         """
 
         config_msg = Message(arbitration_id=0x001, is_extended_id=False)
         if self.interface_enable_can:  # if the bus is enabled when the update function is called
-            if self.state == BusState.ACTIVE:
+            if self._state == BusState.ACTIVE:
                 config_bits = (1 << 1) + int(self.interface_enable_can)
             else:
                 config_bits = (0 << 1) + int(self.interface_enable_can)
             config_msg.data += struct.pack(">B", config_bits)
             config_msg.data += struct.pack(">I", int(self.bitrate))
         else:
             config_msg.data += bytearray((0, 0, 0, 0, 0))  # otherwise disable CAN on the interface
```

### Comparing `python-can-bluetooth-0.1.1/examples/bluetooth_tx_example.py` & `python-can-bluetooth-0.1.2/can_bluetooth_examples/bluetooth_tx_example.py`

 * *Files identical despite different names*

### Comparing `python-can-bluetooth-0.1.1/pyproject.toml` & `python-can-bluetooth-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-can-bluetooth"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python-can interface driver for CAN transmitted over a Bluetooth SPP connection"
 readme = "README.rst"
 license = { text = "GNU Lesser General Public License v3 (LGPLv3)" }
 requires-python = ">=3.7"
 authors = [
     { name = "Matt Woodhead", email = "woody.w62@gmail.com" }
 ]
@@ -33,15 +33,15 @@
 ]
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.entry-points."can.interface"]
-bluetooth = "can_bluetooth._bluetooth_can:BluetoothSPPBus"
+bluetooth = "can_bluetooth:BluetoothSPPBus"
 
 [project.urls]
 homepage = "https://github.com/MattWoodhead/python-can-bluetooth"
 documentation = "https://github.com/MattWoodhead/python-can-bluetooth"
 repository = "https://github.com/MattWoodhead/python-can-bluetooth"
 
 [tool.black]
```

### Comparing `python-can-bluetooth-0.1.1/python_can_bluetooth.egg-info/PKG-INFO` & `python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can-bluetooth
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python-can interface driver for CAN transmitted over a Bluetooth SPP connection
 Author-email: Matt Woodhead <woody.w62@gmail.com>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: homepage, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: documentation, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: repository, https://github.com/MattWoodhead/python-can-bluetooth
 Keywords: CANbus,Bluetooth,python-can,ESP32
```

### Comparing `python-can-bluetooth-0.1.1/test/test_interface_bluetooth.py` & `python-can-bluetooth-0.1.2/can_bluetooth_test/test_interface_bluetooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 # from can.interfaces.serial.serial_can import SerialBus
 from can_bluetooth import BluetoothSPPBus, BusCRCError
 from .test_setup import SerialDummy, ComparingMessagesTestCase, TIMEOUT
 
 
 class SimpleSerialTestBase(ComparingMessagesTestCase):
-
     MAX_TIMESTAMP = 0xFFFFFFFF / 1000
 
     def __init__(self):
         ComparingMessagesTestCase.__init__(self, allowed_timestamp_delta=None, preserves_channel=True)
 
     # def test_serial_module_missing(self):  # TODO - get check for missing serial module working
     #     """
```

### Comparing `python-can-bluetooth-0.1.1/test/test_setup.py` & `python-can-bluetooth-0.1.2/can_bluetooth_test/test_setup.py`

 * *Files identical despite different names*

