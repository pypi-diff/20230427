# Comparing `tmp/karcher-home-0.1.1.tar.gz` & `tmp/karcher-home-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karcher-home-0.1.1.tar", last modified: Wed Apr 26 13:54:53 2023, max compression
+gzip compressed data, was "karcher-home-0.2.tar", last modified: Thu Apr 27 20:54:23 2023, max compression
```

## Comparing `karcher-home-0.1.1.tar` & `karcher-home-0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 13:54:53.722537 karcher-home-0.1.1/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.1.1/LICENSE
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1319 2023-04-26 13:54:53.722537 karcher-home-0.1.1/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      930 2023-04-26 10:52:32.000000 karcher-home-0.1.1/README.md
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 13:54:53.718537 karcher-home-0.1.1/karcher/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.1.1/karcher/__init__.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2445 2023-04-25 13:06:17.000000 karcher-home-0.1.1/karcher/auth.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3614 2023-04-26 12:07:59.000000 karcher-home-0.1.1/karcher/cli.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1786 2023-04-26 12:09:12.000000 karcher-home-0.1.1/karcher/consts.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2401 2023-04-26 12:09:19.000000 karcher-home-0.1.1/karcher/countries.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2157 2023-04-26 12:09:23.000000 karcher-home-0.1.1/karcher/device.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1344 2023-04-26 12:09:27.000000 karcher-home-0.1.1/karcher/exception.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.1.1/karcher/identifiers.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7589 2023-04-26 12:13:54.000000 karcher-home-0.1.1/karcher/karcher.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-26 12:09:49.000000 karcher-home-0.1.1/karcher/map.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.1.1/karcher/mapdata_pb2.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2893 2023-04-26 12:10:34.000000 karcher-home-0.1.1/karcher/utils.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 13:54:53.722537 karcher-home-0.1.1/karcher_home.egg-info/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1319 2023-04-26 13:54:53.000000 karcher-home-0.1.1/karcher_home.egg-info/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      498 2023-04-26 13:54:53.000000 karcher-home-0.1.1/karcher_home.egg-info/SOURCES.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-04-26 13:54:53.000000 karcher-home-0.1.1/karcher_home.egg-info/dependency_links.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-04-26 13:54:53.000000 karcher-home-0.1.1/karcher_home.egg-info/entry_points.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       45 2023-04-26 13:54:53.000000 karcher-home-0.1.1/karcher_home.egg-info/requires.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-04-26 13:54:53.000000 karcher-home-0.1.1/karcher_home.egg-info/top_level.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-04-26 13:54:53.722537 karcher-home-0.1.1/setup.cfg
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      844 2023-04-26 13:54:40.000000 karcher-home-0.1.1/setup.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 13:54:53.722537 karcher-home-0.1.1/tests/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.1.1/tests/test_enc.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 20:54:23.409224 karcher-home-0.2/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.2/LICENSE
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1317 2023-04-27 20:54:23.409224 karcher-home-0.2/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      930 2023-04-26 10:52:32.000000 karcher-home-0.2/README.md
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 20:54:23.405224 karcher-home-0.2/karcher/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.2/karcher/__init__.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2445 2023-04-25 13:06:17.000000 karcher-home-0.2/karcher/auth.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4943 2023-04-27 20:53:34.000000 karcher-home-0.2/karcher/cli.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-27 15:04:06.000000 karcher-home-0.2/karcher/consts.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2401 2023-04-27 15:02:53.000000 karcher-home-0.2/karcher/countries.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4882 2023-04-27 15:00:35.000000 karcher-home-0.2/karcher/device.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1344 2023-04-26 12:09:27.000000 karcher-home-0.2/karcher/exception.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.2/karcher/identifiers.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    13355 2023-04-27 20:49:16.000000 karcher-home-0.2/karcher/karcher.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-26 12:09:49.000000 karcher-home-0.2/karcher/map.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.2/karcher/mapdata_pb2.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3308 2023-04-27 20:27:17.000000 karcher-home-0.2/karcher/mqtt.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3030 2023-04-27 15:03:24.000000 karcher-home-0.2/karcher/utils.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 20:54:23.405224 karcher-home-0.2/karcher_home.egg-info/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1317 2023-04-27 20:54:23.000000 karcher-home-0.2/karcher_home.egg-info/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-04-27 20:54:23.000000 karcher-home-0.2/karcher_home.egg-info/SOURCES.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-04-27 20:54:23.000000 karcher-home-0.2/karcher_home.egg-info/dependency_links.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-04-27 20:54:23.000000 karcher-home-0.2/karcher_home.egg-info/entry_points.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       45 2023-04-27 20:54:23.000000 karcher-home-0.2/karcher_home.egg-info/requires.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-04-27 20:54:23.000000 karcher-home-0.2/karcher_home.egg-info/top_level.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-04-27 20:54:23.409224 karcher-home-0.2/setup.cfg
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      842 2023-04-27 20:41:30.000000 karcher-home-0.2/setup.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-27 20:54:23.409224 karcher-home-0.2/tests/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.2/tests/test_enc.py
```

### Comparing `karcher-home-0.1.1/LICENSE` & `karcher-home-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `karcher-home-0.1.1/PKG-INFO` & `karcher-home-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.1.1
+Version: 0.2
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
 Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.1.1/karcher-home-0.1.1.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
```

### Comparing `karcher-home-0.1.1/README.md` & `karcher-home-0.2/README.md`

 * *Files identical despite different names*

### Comparing `karcher-home-0.1.1/karcher/auth.py` & `karcher-home-0.2/karcher/auth.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.1.1/karcher/cli.py` & `karcher-home-0.2/karcher/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,121 +4,170 @@
 # -----------------------------------------------------------
 
 import click
 import dataclasses
 import json
 import logging
 
-from karcher.auth import Session
 from karcher.exception import KarcherHomeException
 from karcher.karcher import KarcherHome
 from karcher.consts import Region
 
 try:
     from rich import print as echo
 except ImportError:
     echo = click.echo
 
+
 class EnhancedJSONEncoder(json.JSONEncoder):
     def default(self, o):
         if dataclasses.is_dataclass(o):
             return dataclasses.asdict(o)
         return super().default(o)
 
+
 class GlobalContextObject:
     def __init__(self,
-        debug: int = 0,
-        output: str = "json",
-        region: Region = Region.EU
-    ):
+                 debug: int = 0,
+                 output: str = 'json',
+                 region: Region = Region.EU
+                 ):
         self.debug = debug
         self.output = output
         self.region = region
 
     def print(self, result):
-        data_variable = getattr(result, "data", None)
+        data_variable = getattr(result, 'data', None)
         if data_variable is not None:
             result = data_variable
-        if self.output == "json_pretty":
+        if self.output == 'json_pretty':
             echo(json.dumps(result, cls=EnhancedJSONEncoder, indent=4))
         else:
             echo(json.dumps(result, cls=EnhancedJSONEncoder))
 
+
 @click.group()
-@click.option("-d", "--debug", is_flag=True)
+@click.option('-d', '--debug', is_flag=True, help='Enable debug mode.')
 @click.option(
-    "-o",
-    "--output",
-    type=click.Choice(["json", "json_pretty"]),
-    default="json",
-    help="Output format. Default: 'json'")
+    '-o',
+    '--output',
+    type=click.Choice(['json', 'json_pretty']),
+    default='json',
+    help='Output format. Default: "json"')
 @click.option(
-    "-r",
-    "--region", 
+    '-r',
+    '--region',
     type=click.Choice([Region.EU, Region.US, Region.CN]),
     default=Region.EU,
-    help="Region of the server to query. Default: 'eu'")
+    help='Region of the server to query. Default: "eu"')
 @click.pass_context
 def cli(ctx: click.Context, debug: int, output: str, region: Region):
     """Tool for connectiong and getting information from Kärcher Home Robots."""
     level = logging.INFO
     if debug > 0:
         level = logging.DEBUG
 
     logging.basicConfig(level=level)
 
     ctx.obj = GlobalContextObject(debug=debug, output=output, region=region)
 
+
 def safe_cli():
     try:
         cli()
     except KarcherHomeException as ex:
         echo(json.dumps({
             'code': ex.code,
             'message': ex.message
         }))
         return
 
+
 @cli.command()
 @click.pass_context
-def get_urls(ctx: click.Context):
+def urls(ctx: click.Context):
     """Get region information."""
 
     kh = KarcherHome(region=ctx.obj.region)
     d = kh.get_urls()
 
     ctx.obj.print(d)
 
+
 @cli.command()
 @click.option('--username', '-u', help='Username to login with.')
 @click.option('--password', '-p', help='Password to login with.')
 @click.pass_context
 def login(ctx: click.Context, username: str, password: str):
     """Get user session tokens."""
 
     kh = KarcherHome(region=ctx.obj.region)
     ctx.obj.print(kh.login(username, password))
 
+
 @cli.command()
 @click.option('--username', '-u', default=None, help='Username to login with.')
 @click.option('--password', '-p', default=None, help='Password to login with.')
-@click.option('--token', '-t', default=None, help='Authorization token.')
+@click.option('--auth-token', '-t', default=None, help='Authorization token.')
 @click.pass_context
 def devices(ctx: click.Context, username: str, password: str, token: str):
     """List all devices."""
 
     kh = KarcherHome(region=ctx.obj.region)
-    sess = None
     if token is not None:
-        sess = Session.from_token(token, '')
+        kh.login_token(token, '')
     elif username is not None and password is not None:
-        sess = kh.login(username, password)
+        kh.login(username, password)
     else:
-        raise click.BadParameter('Must provide either token or username and password.')
+        raise click.BadParameter(
+            'Must provide either token or username and password.')
 
-    devices = kh.get_devices(sess)
+    devices = kh.get_devices()
 
     # Logout if we used a username and password
     if token is None:
-        kh.logout(sess)
+        kh.logout()
 
     ctx.obj.print(devices)
+
+
+@cli.command()
+@click.option('--username', '-u', default=None, help='Username to login with.')
+@click.option('--password', '-p', default=None, help='Password to login with.')
+@click.option('--auth-token', '-t', default=None, help='Authorization token.')
+@click.option('--mqtt-token', '-m', default=None, help='MQTT authorization token.')
+@click.option('--device-id', '-d', required=True, help='Device ID.')
+@click.pass_context
+def device_properties(
+    ctx: click.Context,
+    username: str,
+    password: str,
+    auth_token: str,
+    mqtt_token: str,
+    device_id: str):
+    """Get device properties."""
+
+    kh = KarcherHome(region=ctx.obj.region)
+    if auth_token is not None:
+        kh.login_token(auth_token, mqtt_token)
+    elif username is not None and password is not None:
+        kh.login(username, password)
+    else:
+        raise click.BadParameter(
+            'Must provide either token or username and password.')
+
+    dev = None
+    for device in kh.get_devices():
+        if device.device_id == device_id:
+            dev = device
+            break
+
+    if dev is None:
+        raise click.BadParameter('Device ID not found.')
+
+    props = kh.get_device_properties(dev)
+
+    # Logout if we used a username and password
+    if auth_token is None:
+        kh.logout()
+
+    ctx.obj.print(props)
```

### Comparing `karcher-home-0.1.1/karcher/consts.py` & `karcher-home-0.2/karcher/consts.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,23 +65,54 @@
 
     RCV3 = '1528986273083777024'
     RCV5 = '1540149850806333440'
     RCF5 = '1599715149861306368'
 
 
 REGION_URLS = {
-    Region.EU: "https://eu-appaiot.3irobotix.net",
-    Region.US: "https://us-appaiot.3irobotix.net",
-    Region.CN: "https://cn-appaiot.3irobotix.net",
+    Region.EU: 'https://eu-appaiot.3irobotix.net',
+    Region.US: 'https://us-appaiot.3irobotix.net',
+    Region.CN: 'https://cn-appaiot.3irobotix.net',
 }
 
 REGION_INDEX = {
     Region.EU: 1,
     Region.US: 2,
     Region.CN: 0,
 }
 
-TENANT_ID = "1528983614213726208"
-PROJECT_TYPE = "android_iot.karcher"
-PROTOCOL_VERSION = "v1"
+ROBOT_PROPERTIES = [
+    'status',
+    'firmware_code',
+    'firmware',
+    'fault',
+    'mode',
+    'wind',
+    'water',
+    'repeat_state',
+    'charge_state',
+    'quantity',
+    'work_mode',
+    'sweep_type',
+    'build_map',
+    'cleaning_area',
+    'cleaning_time',
+    'current_map_id',
+    'custom_type',
+    'privacy',
+    'alarm',
+    'volume',
+    'tank_state',
+    'cloth_state',
+    'mop_route',
+    'map_num',
+    'language',
+    'voice_type',
+    'quiet_status',
+    'quiet_is_open'
+]
+
+TENANT_ID = '1528983614213726208'
+PROJECT_TYPE = 'android_iot.karcher'
+PROTOCOL_VERSION = 'v1'
 APP_VERSION_CODE = 10004
 APP_VERSION_NAME = '1.0.4'
```

### Comparing `karcher-home-0.1.1/karcher/device.py` & `karcher-home-0.2/karcher/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,114 @@
 # -----------------------------------------------------------
 # Copyright (c) 2023 Lauris BH
 # SPDX-License-Identifier: MIT
 # -----------------------------------------------------------
 
-from dataclasses import dataclass, fields
-from enum import Enum
-import json
-from typing import List
-
-from .consts import Product
-from .utils import snake_case
-
-
-class DeviceStatus(int, Enum):
-    """Device status enum."""
-    Offline = 0
-    Online = 1
-
-
-@dataclass(init=False)
-class DeviceVersion:
-    """Device version class.
-
-    This class represents a Karcher Home device version.
-    """
-    package_type: str
-    version: int
-    version_name: str
-    ctrl_version: str
-
-    def __init__(self, **kwargs):
-        names = set([f.name for f in fields(self)])
-        for k, v in kwargs.items():
-            k = snake_case(k)
-            if k in names:
-                setattr(self, k, v)
-
-
-@dataclass(init=False)
-class Device:
-    """Device class.
-
-    This class represents a Karcher Home device.
-    """
-
-    device_id: str
-    sn: str
-    mac: str
-    nickname: str
-    versions: List[DeviceVersion]
-    status: DeviceStatus
-    is_default: bool
-    is_selected: bool
-    is_shared: bool
-    online_time: int
-    photo_url: str
-    product_id: Product
-    product_mode_code: str
-    bind_time: int
-    room_id: str
-
-    def __init__(self, **kwargs):
-        # Set default values
-        for k, v in [('isSelected', False), ('isShare', False), ('isDefault', False)]:
-            if k not in kwargs:
-                kwargs[k] = v
-
-        names = set([f.name for f in fields(self)])
-        for k, v in kwargs.items():
-            k = snake_case(k)
-            if k == 'is_share':
-                k = 'is_shared'
-            if k in names:
-                if k == 'status':
-                    v = DeviceStatus(v)
-                if k == 'product_id':
-                    v = Product(v)
-                elif k == 'versions':
-                    v = json.loads(v)
-                    v = [DeviceVersion(**x) for x in v]
-                setattr(self, k, v)
-
-    def is_online(self):
-        """Get device status."""
-        return self.status == DeviceStatus.Online
+import base64
+import hashlib
+import random
+import re
+import string
+import time
+import zlib
+from Crypto.Cipher import AES
+
+from .consts import TENANT_ID, Product
+
+
+EMAIL_REGEX = "^\\w+([-+.]\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$"
+
+
+def get_random_string(length):
+    letters = string.digits + string.ascii_lowercase + string.ascii_uppercase
+    return ''.join(random.choice(letters) for i in range(length))
+
+
+def get_random_device_id():
+    return ''.join(random.choice('0123456789abcdef') for i in range(16))
+
+
+def get_nonce():
+    return get_random_string(32)
+
+
+def get_timestamp():
+    return int(time.time())
+
+
+def get_timestamp_ms():
+    return int(time.time() * 1000)
+
+
+def get_enc_key():
+    m = hashlib.md5()
+    m.update(bytes(TENANT_ID, 'utf-8'))
+    h = m.hexdigest()
+    return bytes(h[8:24], 'utf-8')
+
+
+def decrypt(data):
+    cipher = AES.new(get_enc_key(), AES.MODE_ECB)
+    buf = cipher.decrypt(base64.b64decode(data))
+    return str(buf[:-ord(buf[-1:])], 'utf-8')
+
+
+def encrypt(data):
+    cipher = AES.new(get_enc_key(), AES.MODE_ECB)
+    buf = bytes(data, 'utf-8')
+    pad_len = cipher.block_size - (len(buf) % cipher.block_size)
+    buf = buf + bytes([pad_len]) * pad_len
+    return base64.b64encode(cipher.encrypt(buf)).decode()
+
+
+def get_map_enc_key(sn: str, mac: str, product_id: Product):
+    sub_key = mac.replace(':', '').lower() + str(product_id.value)
+    cipher = AES.new(bytes(sub_key[0:16], 'utf-8'), AES.MODE_ECB)
+    buf = bytes(sn + '+' + str(product_id.value) + '+' + sn, 'utf-8')
+    pad_len = cipher.block_size - (len(buf) % cipher.block_size)
+    buf = buf + bytes([pad_len]) * pad_len
+
+    key = base64.b64encode(cipher.encrypt(buf)).decode()
+
+    m = hashlib.md5()
+    m.update(bytes(key, 'utf-8'))
+    h = m.hexdigest()
+    return bytes(h[8:24], 'utf-8')
+
+
+def decrypt_map(sn: str, mac: str, product_id: Product, data: bytes):
+    cipher = AES.new(get_map_enc_key(sn, mac, product_id), AES.MODE_ECB)
+    buf = cipher.decrypt(base64.b64decode(data))
+    try:
+        return zlib.decompress(bytes.fromhex(str(buf[:-ord(buf[-1:])], 'utf-8')))
+    except Exception:
+        return bytes.fromhex(str(buf[:-ord(buf[-1:])], 'utf-8'))
+
+
+def md5(data):
+    m = hashlib.md5()
+    m.update(bytes(data, 'utf-8'))
+    return m.hexdigest()
+
+
+def is_email(email):
+    return re.search(EMAIL_REGEX, email) is not None
+
+
+def snake_case(value):
+    first_underscore = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', value)
+    return re.sub('([a-z0-9])([A-Z])', r'\1_\2', first_underscore).lower()
+
+
+def snake_case_fields(data):
+    if type(data) is dict:
+        n = {}
+        for k, v in data.items():
+            n[snake_case(k)] = snake_case_fields(v)
+        return n
+    elif type(data) is list:
+        n = []
+        for v in data:
+            n.append(snake_case_fields(v))
+        return n
+    else:
+        return data
```

### Comparing `karcher-home-0.1.1/karcher/exception.py` & `karcher-home-0.2/karcher/exception.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.1.1/karcher/identifiers.py` & `karcher-home-0.2/karcher/identifiers.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.1.1/karcher/map.py` & `karcher-home-0.2/karcher/map.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.1.1/karcher/mapdata_pb2.py` & `karcher-home-0.2/karcher/mapdata_pb2.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.1.1/karcher_home.egg-info/PKG-INFO` & `karcher-home-0.2/karcher_home.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.1.1
+Version: 0.2
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
 Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.1.1/karcher-home-0.1.1.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
```

### Comparing `karcher-home-0.1.1/setup.py` & `karcher-home-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='karcher-home',
     packages=['karcher'],
     include_package_data=True,
-    version='0.1.1',
+    version='0.2',
     license='MIT',
     description='Kärcher Home Robots client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Lauris BH',
     author_email='lauris@nix.lv',
     url='https://github.com/lafriks/python-karcher',
```

### Comparing `karcher-home-0.1.1/tests/test_enc.py` & `karcher-home-0.2/tests/test_enc.py`

 * *Files identical despite different names*

