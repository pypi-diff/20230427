# Comparing `tmp/python_ember_mug-0.7.0b3.tar.gz` & `tmp/python_ember_mug-0.7.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.7.0b3.tar", max compression
+gzip compressed data, was "python_ember_mug-0.7.0b4.tar", max compression
```

## Comparing `python_ember_mug-0.7.0b3.tar` & `python_ember_mug-0.7.0b4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/LICENSE
--rw-r--r--   0        0        0     5282 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/README.md
--rwxr-xr-x   0        0        0      189 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8471 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     4915 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/consts.py
--rw-r--r--   0        0        0     8531 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/formatting.py
--rw-r--r--   0        0        0    17544 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/mug.py
--rw-r--r--   0        0        0     2212 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/scanner.py
--rw-r--r--   0        0        0     1973 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/ember_mug/utils.py
--rw-r--r--   0        0        0     2896 2023-04-25 22:55:31.022734 python_ember_mug-0.7.0b3/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/conftest.py
--rw-r--r--   0        0        0    19254 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_connection.py
--rw-r--r--   0        0        0      776 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_consts.py
--rw-r--r--   0        0        0     2383 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_formatting.py
--rw-r--r--   0        0        0     3366 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-04-25 22:55:31.026734 python_ember_mug-0.7.0b3/tests/test_utils.py
--rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/LICENSE
+-rw-r--r--   0        0        0     5282 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/README.md
+-rwxr-xr-x   0        0        0      189 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8480 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-27 02:53:54.686303 python_ember_mug-0.7.0b4/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     5394 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/consts.py
+-rw-r--r--   0        0        0     8782 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/formatting.py
+-rw-r--r--   0        0        0    18205 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/mug.py
+-rw-r--r--   0        0        0     2212 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/scanner.py
+-rw-r--r--   0        0        0     1973 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/ember_mug/utils.py
+-rw-r--r--   0        0        0     2896 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/conftest.py
+-rw-r--r--   0        0        0    19254 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_connection.py
+-rw-r--r--   0        0        0      776 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_consts.py
+-rw-r--r--   0        0        0     2395 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_formatting.py
+-rw-r--r--   0        0        0     3372 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_scanner.py
+-rw-r--r--   0        0        0      801 2023-04-27 02:53:54.690303 python_ember_mug-0.7.0b4/tests/test_utils.py
+-rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b4/PKG-INFO
```

### Comparing `python_ember_mug-0.7.0b3/LICENSE` & `python_ember_mug-0.7.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/README.md` & `python_ember_mug-0.7.0b4/README.md`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/ember_mug/cli/commands.py` & `python_ember_mug-0.7.0b4/ember_mug/cli/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,20 +187,20 @@
             shared_parser.add_argument(
                 '-a',
                 '--adapter',
                 action='store',
                 help='Use this Bluetooth adapter instead of the default one (for Bluez)',
             )
         subparsers = self.parser.add_subparsers(dest='command', required=True)
-        subparsers.add_parser('find', description='Find the first paired mug', parents=[shared_parser])
-        subparsers.add_parser('discover', description='Discover Mugs in pairing mode', parents=[shared_parser])
+        subparsers.add_parser('find', description='Find the first paired device', parents=[shared_parser])
+        subparsers.add_parser('discover', description='Discover devices in pairing mode', parents=[shared_parser])
         info_parsers = ArgumentParser(add_help=False)
         info_parsers.add_argument('-e', '--extra', help='Show extra info', action='store_true')
         info_parsers.add_argument('--imperial', help='Use Imperial units', action='store_true')
-        subparsers.add_parser('info', description='Fetch all info from mug', parents=[shared_parser, info_parsers])
+        subparsers.add_parser('info', description='Fetch all info from device', parents=[shared_parser, info_parsers])
         subparsers.add_parser('poll', description='Poll mug for information', parents=[shared_parser, info_parsers])
         get_parser = subparsers.add_parser('get', description='Get mug value', parents=[shared_parser, info_parsers])
         get_parser.add_argument(dest='attributes', metavar='ATTRIBUTE', choices=get_attribute_names, nargs='+')
         set_parser = subparsers.add_parser('set', description='Set mug value', parents=[shared_parser, info_parsers])
         set_parser.add_argument('--name', help='Name', required=False)
         set_parser.add_argument('--target-temp', help='Target Temperature', type=float, required=False)
         set_parser.add_argument('--temperature-unit', help='Temperature Unit', choices=['C', 'F'], required=False)
```

### Comparing `python_ember_mug-0.7.0b3/ember_mug/cli/helpers.py` & `python_ember_mug-0.7.0b4/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/ember_mug/consts.py` & `python_ember_mug-0.7.0b4/ember_mug/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,32 @@
         return LIQUID_STATE_LABELS[self.value]
 
     def __str__(self) -> str:
         """String is the label."""
         return self.label
 
 
+class VolumeLevel(str, Enum):
+    """Class to manage volume levels."""
+
+    LOW = "low"
+    MEDIUM = "medium"
+    HIGH = "high"
+
+    @classmethod
+    def from_state(cls, state: int) -> VolumeLevel:
+        """Build Volume level from int value."""
+        return {0: cls.LOW, 1: cls.MEDIUM, 2: cls.HIGH}[state]
+
+    @cached_property
+    def state(self) -> int:
+        """Get int value from value."""
+        return {self.LOW: 0, self.MEDIUM: 1, self.HIGH: 2}[self]
+
+
 # Push event codes
 class PushEvent(IntEnum):
     """IDs for Push Events."""
 
     BATTERY_CHANGED = 1
     CHARGER_CONNECTED = 2
     CHARGER_DISCONNECTED = 3
@@ -158,15 +176,15 @@
     'current_temp': 'Current Temp',
     'target_temp': 'Target Temp',
     'use_metric': 'Use Metric',
     'dsk': 'DSK',
     'udsk': 'UDSK',
     'date_time_zone': 'Date Time + Time Zone',
     'battery_voltage': 'Voltage',
-    'volume': 'Volume',
+    'volume_level': 'Volume Level',
 }
 
 # Attributes
 INITIAL_ATTRS = {
     "meta",
     "udsk",
     "dsk",
```

### Comparing `python_ember_mug-0.7.0b3/ember_mug/data.py` & `python_ember_mug-0.7.0b4/ember_mug/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     EMBER_TRAVEL_MUG,
     EMBER_TRAVEL_MUG_SHORT,
     EXTRA_ATTRS,
     INITIAL_ATTRS,
     UPDATE_ATTRS,
     LiquidState,
     TemperatureUnit,
+    VolumeLevel,
 )
 from .formatting import format_led_colour, format_liquid_level, format_temp
 from .utils import bytes_to_little_int, decode_byte_string
 
 
 class Change(NamedTuple):
     """Helper for storing changes to attributes."""
@@ -161,15 +162,15 @@
         if self.include_extra is False:
             attributes = attributes - EXTRA_ATTRS
         if self.is_cup:
             # The Cup cannot be named
             attributes = attributes - {'name'}
         elif self.is_travel_mug:
             # Tge Travel Mug does not have an LED colour, but has a volume attribute
-            attributes = (attributes - {'led_colour'}) | {'volume'}
+            attributes = (attributes - {'led_colour'}) | {'volume_level'}
         return attributes
 
 
 @dataclass
 class MugMeta:
     """Meta data for mug."""
 
@@ -206,15 +207,15 @@
     liquid_state: LiquidState = LiquidState.UNKNOWN
     liquid_level: int = 0
     temperature_unit: TemperatureUnit = TemperatureUnit.CELSIUS
     current_temp: float = 0.0
     target_temp: float = 0.0
     dsk: str = ""
     udsk: str = ""
-    volume: int | None = None
+    volume_level: VolumeLevel | None = None
     date_time_zone: datetime | None = None
     battery_voltage: int | None = None
 
     @property
     def meta_display(self) -> str:
         """Return Meta infor based on preference."""
         if self.meta and not self.model.include_extra:
@@ -228,14 +229,21 @@
 
     @property
     def liquid_state_display(self) -> str:
         """Human-readable liquid state."""
         return self.liquid_state.label
 
     @property
+    def volume_level_display(self) -> str | None:
+        """Human-readable volume level."""
+        if self.volume_level:
+            return self.volume_level.value.capitalize()
+        return None
+
+    @property
     def liquid_level_display(self) -> str:
         """Human-readable liquid level."""
         return format_liquid_level(self.liquid_level)
 
     @property
     def current_temp_display(self) -> str:
         """Human-readable current temp with unit."""
```

### Comparing `python_ember_mug-0.7.0b3/ember_mug/formatting.py` & `python_ember_mug-0.7.0b4/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/ember_mug/mug.py` & `python_ember_mug-0.7.0b4/ember_mug/mug.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import asyncio
 import contextlib
 import logging
 from collections.abc import AsyncIterator
 from datetime import datetime, timezone
 from enum import Enum
+from functools import cached_property
 from time import time
 from typing import Any, Callable, Literal
 
 from bleak import BleakClient, BleakError
 from bleak.backends.characteristic import BleakGATTCharacteristic
 from bleak.backends.device import BLEDevice
 from bleak_retry_connector import establish_connection
@@ -19,14 +20,15 @@
     IS_LINUX,
     MUG_NAME_REGEX,
     PUSH_EVENT_BATTERY_IDS,
     LiquidState,
     MugCharacteristic,
     PushEvent,
     TemperatureUnit,
+    VolumeLevel,
 )
 from .data import BatteryInfo, Change, Colour, Model, MugData, MugFirmwareInfo, MugMeta
 from .utils import (
     bytes_to_big_int,
     bytes_to_little_int,
     decode_byte_string,
     encode_byte_string,
@@ -71,14 +73,19 @@
         self.set_client_options(**kwargs)
 
     def set_device(self, ble_device: BLEDevice) -> None:
         """Set the ble device."""
         logger.debug("Set new device from %s to %s", self.device, ble_device)
         self.device = ble_device
 
+    @cached_property
+    def model_name(self) -> str:
+        """Shortcut to model name."""
+        return self.data.model.name
+
     async def _ensure_connection(self) -> None:
         """Connect to mug."""
         if self._connect_lock.locked():
             logger.debug("Connection to %s already in progress. Waiting first.", self.device.name)
 
         if self._client is not None and self._client.is_connected:
             return
@@ -213,26 +220,33 @@
         return temp_from_bytes(temp_bytes, self.data.use_metric)
 
     async def get_liquid_level(self) -> int:
         """Get liquid level from mug gatt."""
         liquid_level_bytes = await self._read(MugCharacteristic.LIQUID_LEVEL)
         return bytes_to_little_int(liquid_level_bytes)
 
-    async def get_volume(self) -> int | None:
-        """Get volume from mug gatt."""
+    async def get_volume_level(self) -> VolumeLevel | None:
+        """Get volume level from mug gatt."""
         try:
             volume_bytes = await self._read(MugCharacteristic.VOLUME)
-        except (BleakError, ValueError, TypeError) as e:
-            logger.error('Failed to read volume attribute.  Error was: %s', e)
+        except BleakError as e:
+            if not self.data.model.is_travel_mug:
+                raise NotImplementedError('Ony the travel mug has a volume')
+            logger.error('Failed to fetch volume attribute: %s', e)
             return None
-        try:
-            return bytes_to_little_int(volume_bytes)
-        except (TypeError, ValueError) as e:
-            logger.error('Failed to decode volume value. Values was %s, Error was: %s', volume_bytes, e)
-        return None
+        volume_int = bytes_to_little_int(volume_bytes)
+        return VolumeLevel.from_state(volume_int)
+
+    async def set_volume_level(self, volume: int | VolumeLevel) -> None:
+        """Set volume_level on Travel Mug."""
+        if volume not in (0, 1, 2):
+            raise ValueError('Volume level must be between 0 and 2 inclusively')
+        volume_level = volume if isinstance(volume, VolumeLevel) else VolumeLevel.from_state(volume)
+        await self._write(MugCharacteristic.VOLUME, bytearray(bytearray([volume_level.state])))
+        self.data.volume_level = volume_level
 
     async def get_liquid_state(self) -> LiquidState:
         """Get liquid state from mug gatt."""
         liquid_state_bytes = await self._read(MugCharacteristic.LIQUID_STATE)
         state = bytes_to_little_int(liquid_state_bytes)
         return LiquidState(state)
 
@@ -340,15 +354,15 @@
         """Push events from the mug to indicate changes."""
         event_id = data[0]
         now = time()
         if (last_time := self._latest_events.get(event_id)) and now - last_time < 5:
             return
         self._latest_events[event_id] = now
 
-        logger.debug("Push event received from Mug (%s) - Data: %s.", event_id, data)
+        logger.debug("Push event received from %s (%s) - Data: %s.", self.model_name, event_id, data)
 
         # Check known IDs
         if event_id in PUSH_EVENT_BATTERY_IDS:
             # 1, 2 and 3 : Battery Change
             if event_id in (
                 PushEvent.CHARGER_CONNECTED,
                 PushEvent.CHARGER_DISCONNECTED,
@@ -369,15 +383,15 @@
         elif event_id == PushEvent.LIQUID_LEVEL_CHANGED:
             self._queued_updates.add("liquid_level")
         elif event_id == PushEvent.LIQUID_STATE_CHANGED:
             self._queued_updates.add("liquid_state")
         elif event_id == PushEvent.BATTERY_VOLTAGE_STATE_CHANGED:
             self._queued_updates.add("battery_voltage")
         else:
-            logger.debug('Unknown even received %s', event_id)
+            logger.debug('Unknown event received %s', event_id)
 
     async def unsubscribe(self) -> None:
         """Unsubscribe from Mug notifications."""
         logger.debug("Unsubscribe called")
         if not self._client:
             return
         with contextlib.suppress(BleakError):
```

### Comparing `python_ember_mug-0.7.0b3/ember_mug/scanner.py` & `python_ember_mug-0.7.0b4/ember_mug/scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/ember_mug/utils.py` & `python_ember_mug-0.7.0b4/ember_mug/utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/pyproject.toml` & `python_ember_mug-0.7.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.7.0b3"
+version = "0.7.0b4"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `python_ember_mug-0.7.0b3/tests/cli/test_commands.py` & `python_ember_mug-0.7.0b4/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/tests/cli/test_helpers.py` & `python_ember_mug-0.7.0b4/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/tests/conftest.py` & `python_ember_mug-0.7.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/tests/test_connection.py` & `python_ember_mug-0.7.0b4/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/tests/test_consts.py` & `python_ember_mug-0.7.0b4/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/tests/test_data.py` & `python_ember_mug-0.7.0b4/tests/test_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     assert 'battery_voltage' not in mug.update_attributes
 
     travel_mug = Model(EMBER_TRAVEL_MUG)
     assert travel_mug.is_travel_mug is True
     assert travel_mug.is_cup is False
     assert 'name' in travel_mug.update_attributes
     assert 'name' in travel_mug.attribute_labels
-    assert 'volume' in travel_mug.attribute_labels
+    assert 'volume_level' in travel_mug.attribute_labels
 
     cup = Model(EMBER_CUP)
     assert cup.is_cup is True
     assert cup.is_travel_mug is False
     assert 'name' not in cup.update_attributes
     assert 'name' not in cup.attribute_labels
-    assert 'volume' not in cup.update_attributes
+    assert 'volume_level' not in cup.update_attributes
```

### Comparing `python_ember_mug-0.7.0b3/tests/test_formatting.py` & `python_ember_mug-0.7.0b4/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/tests/test_mug_data.py` & `python_ember_mug-0.7.0b4/tests/test_mug_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,9 +93,9 @@
         'liquid_state_display': 'Unknown',
         'meta': {'mug_id': 'test_id', 'serial_number': 'serial number'},
         'name': '',
         'target_temp': 0.0,
         'target_temp_display': '0.00°C',
         'temperature_unit': TemperatureUnit.CELSIUS,
         'udsk': '',
-        'volume': None,
+        'volume_level': None,
     }
```

### Comparing `python_ember_mug-0.7.0b3/tests/test_scanner.py` & `python_ember_mug-0.7.0b4/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/tests/test_utils.py` & `python_ember_mug-0.7.0b4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b3/PKG-INFO` & `python_ember_mug-0.7.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.7.0b3
+Version: 0.7.0b4
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

