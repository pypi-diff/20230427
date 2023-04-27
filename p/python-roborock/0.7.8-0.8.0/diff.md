# Comparing `tmp/python_roborock-0.7.8.tar.gz` & `tmp/python_roborock-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.7.8.tar", max compression
+gzip compressed data, was "python_roborock-0.8.0.tar", max compression
```

## Comparing `python_roborock-0.7.8.tar` & `python_roborock-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-26 23:11:15.987564 python_roborock-0.7.8/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-26 23:11:15.987564 python_roborock-0.7.8/README.md
--rw-r--r--   0        0        0     1370 2023-04-26 23:11:16.863564 python_roborock-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/__init__.py
--rw-r--r--   0        0        0    19297 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/cli.py
--rw-r--r--   0        0        0     8241 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/cloud_api.py
--rw-r--r--   0        0        0     4329 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/code_mappings.py
--rw-r--r--   0        0        0     9872 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/exceptions.py
--rw-r--r--   0        0        0     6416 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/roborock_future.py
--rw-r--r--   0        0        0     6232 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/roborock_message.py
--rw-r--r--   0        0        0    12046 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/typing.py
--rw-r--r--   0        0        0      783 2023-04-26 23:11:15.987564 python_roborock-0.7.8/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 14:49:37.960720 python_roborock-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-27 14:49:37.960720 python_roborock-0.8.0/README.md
+-rw-r--r--   0        0        0     1370 2023-04-27 14:49:38.732733 python_roborock-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/__init__.py
+-rw-r--r--   0        0        0    20172 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/cli.py
+-rw-r--r--   0        0        0     8241 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4329 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/code_mappings.py
+-rw-r--r--   0        0        0      209 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/const.py
+-rw-r--r--   0        0        0    10730 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/containers.py
+-rw-r--r--   0        0        0     1487 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/exceptions.py
+-rw-r--r--   0        0        0     6416 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6232 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12651 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/typing.py
+-rw-r--r--   0        0        0      783 2023-04-27 14:49:37.960720 python_roborock-0.8.0/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.8.0/PKG-INFO
```

### Comparing `python_roborock-0.7.8/LICENSE` & `python_roborock-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/README.md` & `python_roborock-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/pyproject.toml` & `python_roborock-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.7.8"
+version = "0.8.0"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.7.8/roborock/api.py` & `python_roborock-0.8.0/roborock/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,23 @@
     RoborockDeviceInfo,
     RoomMapping,
     SmartWashParams,
     Status,
     UserData,
     WashTowelMode,
 )
-from .exceptions import RoborockException, RoborockTimeout, VacuumError
+from .exceptions import (
+    RoborockAccountDoesNotExist,
+    RoborockException,
+    RoborockInvalidCode,
+    RoborockInvalidEmail,
+    RoborockTimeout,
+    RoborockUrlException,
+    VacuumError,
+)
 from .roborock_future import RoborockFuture
 from .roborock_message import RoborockMessage
 from .typing import DeviceProp, DockSummary, RoborockCommand
 from .util import unpack_list
 
 _LOGGER = logging.getLogger(__name__)
 QUEUE_TIMEOUT = 4
@@ -341,20 +349,23 @@
             url_request = PreparedRequest(self._default_url)
             response = await url_request.request(
                 "post",
                 "/api/v1/getUrlByEmail",
                 params={"email": self._username, "needtwostepauth": "false"},
             )
             if response is None:
-                raise RoborockException("get url by email returned None")
-            if response.get("code") != 200:
-                raise RoborockException(response.get("error"))
+                raise RoborockUrlException("get url by email returned None")
+            response_code = response.get("code")
+            if response_code != 200:
+                if response_code == 2003:
+                    raise RoborockInvalidEmail("Your email was incorrectly formatted.")
+                raise RoborockUrlException(response.get("error"))
             response_data = response.get("data")
             if response_data is None:
-                raise RoborockException("response does not have 'data'")
+                raise RoborockUrlException("response does not have 'data'")
             self.base_url = response_data.get("url")
         return self.base_url
 
     def _get_header_client_id(self):
         md5 = hashlib.md5()
         md5.update(self._username.encode())
         md5.update(self._device_identifier.encode())
@@ -371,16 +382,20 @@
             params={
                 "username": self._username,
                 "type": "auth",
             },
         )
         if code_response is None:
             raise RoborockException("Failed to get a response from send email code")
-        if code_response.get("code") != 200:
-            raise RoborockException(code_response.get("msg"))
+        response_code = code_response.get("code")
+        if response_code != 200:
+            if response_code == 2008:
+                raise RoborockAccountDoesNotExist("Account does not exist - check your login and try again.")
+            else:
+                raise RoborockException(f"{code_response.get('msg')} - response code: {code_response.get('code')}")
 
     async def pass_login(self, password: str) -> UserData:
         base_url = await self._get_base_url()
         header_clientid = self._get_header_client_id()
 
         login_request = PreparedRequest(base_url, {"header_clientid": header_clientid})
         login_response = await login_request.request(
@@ -391,15 +406,15 @@
                 "password": password,
                 "needtwostepauth": "false",
             },
         )
         if login_response is None:
             raise RoborockException("Login response is none")
         if login_response.get("code") != 200:
-            raise RoborockException(login_response.get("msg"))
+            raise RoborockException(f"{login_response.get('msg')} - response code: {login_response.get('code')}")
         user_data = login_response.get("data")
         if not isinstance(user_data, dict):
             raise RoborockException("Got unexpected data type for user_data")
         return UserData.from_dict(user_data)
 
     async def code_login(self, code) -> UserData:
         base_url = await self._get_base_url()
@@ -413,16 +428,19 @@
                 "username": self._username,
                 "verifycode": code,
                 "verifycodetype": "AUTH_EMAIL_CODE",
             },
         )
         if login_response is None:
             raise RoborockException("Login request response is None")
-        if login_response.get("code") != 200:
-            raise RoborockException(login_response.get("msg"))
+        response_code = login_response.get("code")
+        if response_code != 200:
+            if response_code == 2018:
+                raise RoborockInvalidCode("Invalid code - check your code and try again.")
+            raise RoborockException(f"{login_response.get('msg')} - response code: {response_code}")
         user_data = login_response.get("data")
         if not isinstance(user_data, dict):
             raise RoborockException("Got unexpected data type for user_data")
         return UserData.from_dict(user_data)
 
     async def get_home_data(self, user_data: UserData) -> HomeData:
         base_url = await self._get_base_url()
@@ -435,15 +453,15 @@
             "get",
             "/api/v1/getHomeDetail",
             headers={"Authorization": user_data.token},
         )
         if home_id_response is None:
             raise RoborockException("home_id_response is None")
         if home_id_response.get("code") != 200:
-            raise RoborockException(home_id_response.get("msg"))
+            raise RoborockException(f"{home_id_response.get('msg')} - response code: {home_id_response.get('code')}")
 
         home_id = home_id_response["data"].get("rrHomeId")
         timestamp = math.floor(time.time())
         nonce = secrets.token_urlsafe(6)
         prestr = ":".join(
             [
                 rriot.u,
```

### Comparing `python_roborock-0.7.8/roborock/cli.py` & `python_roborock-0.8.0/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/roborock/cloud_api.py` & `python_roborock-0.8.0/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/roborock/code_mappings.py` & `python_roborock-0.8.0/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/roborock/containers.py` & `python_roborock-0.8.0/roborock/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .code_mappings import (
     RoborockDockDustCollectionModeCode,
     RoborockDockErrorCode,
     RoborockErrorCode,
     RoborockFanPowerCode,
     RoborockMopModeCode,
 )
+from .const import FILTER_REPLACE_TIME, MAIN_BRUSH_REPLACE_TIME, SENSOR_DIRTY_REPLACE_TIME, SIDE_BRUSH_REPLACE_TIME
 
 
 def camelize(s: str):
     first, *others = s.split("_")
     if len(others) == 0:
         return s
     return "".join([first.lower(), *map(str.title, others)])
@@ -275,14 +276,28 @@
     side_brush_work_time: Optional[int] = None
     filter_work_time: Optional[int] = None
     filter_element_work_time: Optional[int] = None
     sensor_dirty_time: Optional[int] = None
     strainer_work_times: Optional[int] = None
     dust_collection_work_times: Optional[int] = None
     cleaning_brush_work_times: Optional[int] = None
+    main_brush_time_left: Optional[int] = None
+    side_brush_time_left: Optional[int] = None
+    filter_time_left: Optional[int] = None
+    sensor_time_left: Optional[int] = None
+
+    def __post_init__(self):
+        self.main_brush_time_left = (
+            MAIN_BRUSH_REPLACE_TIME - self.main_brush_work_time if self.main_brush_work_time else None
+        )
+        self.side_brush_time_left = (
+            SIDE_BRUSH_REPLACE_TIME - self.side_brush_work_time if self.side_brush_work_time else None
+        )
+        self.filter_time_left = FILTER_REPLACE_TIME - self.filter_work_time if self.filter_work_time else None
+        self.sensor_time_left = SENSOR_DIRTY_REPLACE_TIME - self.sensor_dirty_time if self.sensor_dirty_time else None
 
 
 @dataclass
 class MultiMapsListMapInfoBakMaps(RoborockBase):
     mapflag: Optional[Any] = None
     add_time: Optional[Any] = None
```

### Comparing `python_roborock-0.7.8/roborock/exceptions.py` & `python_roborock-0.8.0/roborock/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,7 +32,23 @@
 
 class CommandVacuumError(RoborockException):
     """Class for command vacuum errors."""
 
     def __init__(self, command: str, vacuum_error: VacuumError):
         self.message = f"{command}: {str(vacuum_error)}"
         super().__init__(self.message)
+
+
+class RoborockAccountDoesNotExist(RoborockException):
+    """Class for Roborock account does not exist exceptions."""
+
+
+class RoborockUrlException(RoborockException):
+    """Class for being unable to get the URL for the Roborock account."""
+
+
+class RoborockInvalidCode(RoborockException):
+    """Class for Roborock invalid code exceptions."""
+
+
+class RoborockInvalidEmail(RoborockException):
+    """Class for Roborock invalid formatted email exceptions."""
```

### Comparing `python_roborock-0.7.8/roborock/local_api.py` & `python_roborock-0.8.0/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/roborock/roborock_future.py` & `python_roborock-0.8.0/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/roborock/roborock_message.py` & `python_roborock-0.8.0/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/roborock/typing.py` & `python_roborock-0.8.0/roborock/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,7 +217,21 @@
 class DeviceProp:
     status: Optional[Status] = None
     dnd_timer: Optional[DNDTimer] = None
     clean_summary: Optional[CleanSummary] = None
     consumable: Optional[Consumable] = None
     last_clean_record: Optional[CleanRecord] = None
     dock_summary: Optional[DockSummary] = None
+
+    def update(self, device_prop: DeviceProp) -> None:
+        if device_prop.status:
+            self.status = device_prop.status
+        if device_prop.dnd_timer:
+            self.dnd_timer = device_prop.dnd_timer
+        if device_prop.clean_summary:
+            self.clean_summary = device_prop.clean_summary
+        if device_prop.consumable:
+            self.consumable = device_prop.consumable
+        if device_prop.last_clean_record:
+            self.last_clean_record = device_prop.last_clean_record
+        if device_prop.dock_summary:
+            self.dock_summary = device_prop.dock_summary
```

### Comparing `python_roborock-0.7.8/roborock/util.py` & `python_roborock-0.8.0/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.8/PKG-INFO` & `python_roborock-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.7.8
+Version: 0.8.0
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
-Metadata-Version: 2.1 Name: python-roborock Version: 0.7.8 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.8.0 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

