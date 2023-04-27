# Comparing `tmp/pyIndego-3.0.0.tar.gz` & `tmp/pyIndego-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyIndego-3.0.0.tar", last modified: Wed Apr 26 19:31:14 2023, max compression
+gzip compressed data, was "pyIndego-3.0.1.tar", last modified: Thu Apr 27 05:39:16 2023, max compression
```

## Comparing `pyIndego-3.0.0.tar` & `pyIndego-3.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.851857 pyIndego-3.0.0/
--rw-rw-rw-   0        0        0     1091 2023-04-26 19:17:02.000000 pyIndego-3.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0    21551 2023-04-26 19:31:14.851857 pyIndego-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    21113 2023-04-26 19:17:02.000000 pyIndego-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.819347 pyIndego-3.0.0/pyIndego/
--rw-rw-rw-   0        0        0      397 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/__init__.py
--rw-rw-rw-   0        0        0     6589 2023-04-26 19:22:15.000000 pyIndego-3.0.0/pyIndego/const.py
--rw-rw-rw-   0        0        0     2301 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/helpers.py
--rw-rw-rw-   0        0        0    22250 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/indego_async_client.py
--rw-rw-rw-   0        0        0    14888 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/indego_base_client.py
--rw-rw-rw-   0        0        0    17567 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/indego_client.py
--rw-rw-rw-   0        0        0     9103 2023-04-26 19:17:02.000000 pyIndego-3.0.0/pyIndego/states.py
-drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.846847 pyIndego-3.0.0/pyIndego.egg-info/
--rw-rw-rw-   0        0        0    21551 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-26 19:31:14.000000 pyIndego-3.0.0/pyIndego.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 19:31:14.851857 pyIndego-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      809 2023-04-26 19:30:25.000000 pyIndego-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 19:31:14.846847 pyIndego-3.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 19:17:02.000000 pyIndego-3.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0    39869 2023-04-26 19:17:02.000000 pyIndego-3.0.0/tests/test_indego.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.851784 pyIndego-3.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-26 19:17:02.000000 pyIndego-3.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    21543 2023-04-27 05:39:16.850801 pyIndego-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    21093 2023-04-27 05:28:43.000000 pyIndego-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.783809 pyIndego-3.0.1/pyIndego/
+-rw-rw-rw-   0        0        0      397 2023-04-26 19:17:02.000000 pyIndego-3.0.1/pyIndego/__init__.py
+-rw-rw-rw-   0        0        0     6612 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/const.py
+-rw-rw-rw-   0        0        0     2301 2023-04-26 19:17:02.000000 pyIndego-3.0.1/pyIndego/helpers.py
+-rw-rw-rw-   0        0        0    20193 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/indego_async_client.py
+-rw-rw-rw-   0        0        0    15805 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/indego_base_client.py
+-rw-rw-rw-   0        0        0    15500 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/indego_client.py
+-rw-rw-rw-   0        0        0     9103 2023-04-26 19:17:02.000000 pyIndego-3.0.1/pyIndego/states.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.830516 pyIndego-3.0.1/pyIndego.egg-info/
+-rw-rw-rw-   0        0        0    21543 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 05:39:16.851784 pyIndego-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-04-27 05:33:58.000000 pyIndego-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.846774 pyIndego-3.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 19:17:02.000000 pyIndego-3.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    39869 2023-04-26 19:17:02.000000 pyIndego-3.0.1/tests/test_indego.py
```

### Comparing `pyIndego-3.0.0/LICENSE.txt` & `pyIndego-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.0/PKG-INFO` & `pyIndego-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyIndego
-Version: 3.0.0
+Version: 3.0.1
 Summary: API for Bosch Indego mower
 Home-page: https://github.com/jm-73/pyIndego
-Author: jm-73
+Author: jm-73, sander1988
 Author-email: jens@myretyr.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.txt
@@ -390,21 +390,18 @@
 Get the user adjustment of the mowing frequency
 
     update_automatic_update()
 Get the automatic update settings
 
 
 # API CALLS
-https://api.indego.iot.bosch-si.com:443/api/v1
+https://api.indego-cloud.iot.bosch-si.com/api/v1/
 
 
 ```python
-post
-/authenticate
-
 get
 /alerts
 /alms
 /alms/<serial>
 /alms/<serial>/automaticUpdate
 /alms/<serial>/calendar
 /alms/<serial>/config
```

### Comparing `pyIndego-3.0.0/README.md` & `pyIndego-3.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -376,21 +376,18 @@
 Get the user adjustment of the mowing frequency
 
     update_automatic_update()
 Get the automatic update settings
 
 
 # API CALLS
-https://api.indego.iot.bosch-si.com:443/api/v1
+https://api.indego-cloud.iot.bosch-si.com/api/v1/
 
 
 ```python
-post
-/authenticate
-
 get
 /alerts
 /alms
 /alms/<serial>
 /alms/<serial>/automaticUpdate
 /alms/<serial>/calendar
 /alms/<serial>/config
```

### Comparing `pyIndego-3.0.0/pyIndego/const.py` & `pyIndego-3.0.1/pyIndego/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,25 @@
     PUT = "PUT"
     DELETE = "DELETE"
     PATCH = "PATCH"
     OPTIONS = "OPTIONS"
     HEAD = "HEAD"
 
 
-DEFAULT_URL = "https://api.indego.iot.bosch-si.com/api/v1/"
+DEFAULT_URL = "https://api.indego-cloud.iot.bosch-si.com/api/v1/"
 CONTENT_TYPE_JSON = "application/json"
 CONTENT_TYPE = "Content-Type"
-DEFAULT_BODY = {
-    "accept_tc_id": "202012",
-    "device": "",
-    "os_type": "Android",
-    "os_version": "4.0",
-    "dvc_manuf": "unknown",
-    "dvc_type": "unknown",
-}
 COMMANDS = ("mow", "pause", "returnToDock")
 
-DEFAULT_HEADER = {CONTENT_TYPE: CONTENT_TYPE_JSON}
+DEFAULT_HEADER = {
+    CONTENT_TYPE: CONTENT_TYPE_JSON,
+    # We need to change the user-agent!
+    # The Microsoft Azure proxy seems to block all requests (HTTP 403) for the default 'python-requests' user-agent.
+    "User-Agent": "pyIndego"
+}
 DEFAULT_LOOKUP_VALUE = "Not in database."
 
 DEFAULT_CALENDAR = {
     "sel_cal": 1,
     "cals": [
         {
             "cal": 1,
```

### Comparing `pyIndego-3.0.0/pyIndego/helpers.py` & `pyIndego-3.0.1/pyIndego/helpers.py`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.0/pyIndego/indego_async_client.py` & `pyIndego-3.0.1/pyIndego/indego_async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """API for Bosch API server for Indego lawn mower."""
 import asyncio
 import logging
 from socket import error as SocketError
-from typing import Any
+from typing import Any, Optional, Callable, Awaitable
 
 import aiohttp
 from aiohttp import (
     ClientOSError,
     ClientResponseError,
     ServerTimeoutError,
     TooManyRedirects,
 )
-from aiohttp.helpers import BasicAuth
 from aiohttp.web_exceptions import HTTPGatewayTimeout
 
 from . import __version__
 from .const import (
     COMMANDS,
     CONTENT_TYPE_JSON,
-    DEFAULT_BODY,
     DEFAULT_CALENDAR,
     DEFAULT_HEADER,
     DEFAULT_URL,
     Methods,
 )
 from .indego_base_client import IndegoBaseClient
 from .states import Calendar
@@ -31,54 +29,57 @@
 
 
 class IndegoAsyncClient(IndegoBaseClient):
     """Class for Indego Async Client."""
 
     def __init__(
         self,
-        username: str,
-        password: str,
+        token: str,
+        token_refresh_method: Optional[Callable[[], Awaitable[str]]] = None,
         serial: str = None,
         map_filename: str = None,
         api_url: str = DEFAULT_URL,
         session: aiohttp.ClientSession = None,
+        raise_request_exceptions: bool = False,
     ):
         """Initialize the Async Client.
 
         Args:
-            username (str): username for Indego Account
-            password (str): password for Indego Account
+            token (str): Bosch SingleKey ID OAuth token
+            token_refresh_method (callback): Callback method to request an OAuth token refresh
             serial (str): serial number of the mower
             map_filename (str, optional): Filename to store maps in. Defaults to None.
             api_url (str, optional): url for the api, defaults to DEFAULT_URL.
-
+            raise_request_exceptions (bool): Should unexpected API request exception be raised or not. Default False to keep things backwards compatible.
         """
-        super().__init__(username, password, serial, map_filename, api_url)
+        super().__init__(token, token_refresh_method, serial, map_filename, api_url, raise_request_exceptions)
         if session:
             self._session = session
+            # We should only close session we own.
+            # In this case don't own it, probably a reference from HA.
+            self._should_close_session = False
         else:
             self._session = aiohttp.ClientSession(raise_for_status=False)
-
-    async def __aenter__(self):
-        """Enter for async with."""
-        await self.start()
-        return self
+            self._should_close_session = True
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         """Exit for async with."""
         await self.close()
 
-    async def start(self):
-        """Login if not done."""
-        if not self._logged_in:
-            await self.login()
-
     async def close(self):
         """Close the aiohttp session."""
-        await self._session.close()
+        if self._should_close_session:
+            await self._session.close()
+
+    async def get_mowers(self):
+        """Get a list of the available mowers (serials) in the account."""
+        result = await self.get("alms")
+        if result is None:
+            return []
+        return [mower['alm_sn'] for mower in result]
 
     async def delete_alert(self, alert_index: int):
         """Delete the alert with the specified index.
 
         Args:
             alert_index (int): index of alert to be deleted, should be in range or length of alerts.
 
@@ -439,151 +440,102 @@
         self._update_user(await self.get(f"users/{self._userid}"))
 
     async def get_user(self):
         """Update user and return it."""
         await self.update_user()
         return self.user
 
-    async def login(self, attempts: int = 0):
-        """Login to the api and store the context."""
-        response = await self._request(
-            method=Methods.GET,
-            path="authenticate/check",
-            data=DEFAULT_BODY,
-            headers=DEFAULT_HEADER,
-            auth=BasicAuth(self._username, self._password),
-            timeout=30,
-            attempts=attempts,
-        )
-        self._login(response)
-        if response is not None:
-            _LOGGER.debug("Logged in")
-            if not self._serial:
-                list_of_mowers = await self.get("alms")
-                self._serial = list_of_mowers[0].get("alm_sn")
-                _LOGGER.debug("Serial added")
-            return True
-        return False
-
     async def _request(  # noqa: C901
         self,
         method: Methods,
         path: str,
         data: dict = None,
         headers: dict = None,
-        auth: BasicAuth = None,
         timeout: int = 30,
         attempts: int = 0,
     ):
         """Request implemented by the subclasses either synchronously or asynchronously.
 
         Args:
             method (Methods): HTTP method to be executed.
             path (str): url to call on top of base_url.
             data (dict, optional): if applicable, data to be sent, defaults to None.
             headers (dict, optional): headers to be included, defaults to None, which should be filled by the method.
-            auth (BasicAuth or HTTPBasicAuth, optional): login specific attribute, defaults to None.
             timeout (int, optional): Timeout for the api call. Defaults to 30.
             attempts (int, optional): Number to keep track of retries, after three starts delaying, after five quites.
 
         """
         if 3 <= attempts < 5:
             _LOGGER.info("Three or four attempts done, waiting 30 seconds")
             await asyncio.sleep(30)
+
         if attempts == 5:
             _LOGGER.warning("Five attempts done, please try again later")
             return None
+
+        if self._token_refresh_method is not None:
+            _LOGGER.debug("Refreshing token")
+            self._token = await self._token_refresh_method()
+        else:
+            _LOGGER.debug("Token refresh is NOT available")
+
         url = f"{self._api_url}{path}"
+
         if not headers:
             headers = DEFAULT_HEADER.copy()
-            headers["x-im-context-id"] = self._contextid
-        _LOGGER.debug("Sending %s to %s", method.value, url)
+            headers["Authorization"] = "Bearer %s" % self._token
+
         try:
+            _LOGGER.debug("%s call to API endpoint %s", method.value, url)
             async with self._session.request(
                 method=method.value,
                 url=url,
-                json=data if data else DEFAULT_BODY,
+                json=data,
                 headers=headers,
-                auth=auth,
                 timeout=timeout,
             ) as response:
                 status = response.status
-                _LOGGER.debug("status: %s", status)
+                _LOGGER.debug("HTTP status code: %i", status)
                 if status == 200:
                     if response.content_type == CONTENT_TYPE_JSON:
                         resp = await response.json()
                         _LOGGER.debug("Response: %s", resp)
-                        return resp  # await response.json()
+                        return resp
                     return await response.content.read()
-                if status == 204:
-                    _LOGGER.debug("204: No content in response from server")
-                    return None
-                if status == 400:
-                    _LOGGER.warning(
-                        "400: Bad Request: won't retry. Message: %s",
-                        (await response.content.read()).decode("UTF-8"),
-                    )
-                    return None
-                if status == 401:
-                    if path == "authenticate/check":
-                        _LOGGER.info(
-                            "401: Unauthorized, credentials are wrong, won't retry"
-                        )
-                        return None
-                    _LOGGER.info("401: Unauthorized: logging in again")
-                    login_result = await self.login()
-                    if login_result:
-                        return await self._request(
-                            method=method,
-                            path=path,
-                            data=data,
-                            timeout=timeout,
-                            attempts=attempts + 1,
-                        )
-                    return None
-                if status == 403:
-                    _LOGGER.error("403: Forbidden: won't retry")
-                    return None
-                if status == 405:
-                    _LOGGER.error(
-                        "405: Method not allowed: %s is used but not allowed, try a different method for path %s, won't retry",
-                        method,
-                        path,
-                    )
-                    return None
-                if status == 500:
-                    _LOGGER.debug("500: Internal Server Error")
-                    return None
-                if status == 501:
-                    _LOGGER.debug("501: Not implemented yet")
+
+                if self._log_request_result(status, url):
                     return None
-                if status == 504:
-                    if url.find("longpoll=true") > 0:
-                        _LOGGER.debug("504: longpoll stopped, no updates")
-                        return None
+
                 response.raise_for_status()
+
         except (asyncio.TimeoutError, ServerTimeoutError, HTTPGatewayTimeout) as exc:
-            _LOGGER.info("%s: Timeout on Bosch servers, retrying", exc)
+            _LOGGER.info("%s: Timeout on Bosch servers (mower offline?), retrying...", exc)
             return await self._request(
                 method=method,
                 path=path,
                 data=data,
                 timeout=timeout,
                 attempts=attempts + 1,
             )
+
         except ClientOSError as exc:
             _LOGGER.debug("%s: Failed to update Indego status, longpoll timeout", exc)
             return None
+
         except (TooManyRedirects, ClientResponseError, SocketError) as exc:
             _LOGGER.error("%s: Failed %s to Indego, won't retry", exc, method.value)
             return None
+
         except asyncio.CancelledError:
             _LOGGER.debug("Task cancelled by task runner")
             return None
+
         except Exception as exc:
+            if self._raise_request_exceptions:
+                raise
             _LOGGER.error("Request to %s gave a unhandled error: %s", url, exc)
             return None
 
     async def get(self, path: str, timeout: int = 30):
         """Get implemented by the subclasses either synchronously or asynchronously.
 
         Args:
```

### Comparing `pyIndego-3.0.0/pyIndego/indego_base_client.py` & `pyIndego-3.0.1/pyIndego/indego_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,474 +1,461 @@
-"""Base class for indego."""
+"""API for Bosch API server for Indego lawn mower."""
 import logging
-from abc import ABC, abstractmethod
-from typing import Any
+import time
+import typing
 
-import pytz
+import requests
+from requests.exceptions import RequestException, Timeout, TooManyRedirects
 
+from . import __version__
 from .const import (
+    COMMANDS,
+    CONTENT_TYPE,
+    CONTENT_TYPE_JSON,
     DEFAULT_CALENDAR,
-    DEFAULT_LOOKUP_VALUE,
-    DEFAULT_URL,
-    MOWER_STATE_DESCRIPTION,
-    MOWER_STATE_DESCRIPTION_DETAIL,
+    DEFAULT_HEADER,
     Methods,
 )
-from .helpers import convert_bosch_datetime, generate_update
-from .states import (
-    Alert,
-    Calendar,
-    Config,
-    GenericData,
-    Location,
-    Network,
-    OperatingData,
-    PredictiveSchedule,
-    Security,
-    Setup,
-    State,
-    User,
-)
+from .indego_base_client import IndegoBaseClient
+from .states import Calendar
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class IndegoBaseClient(ABC):
-    """Indego base client class."""
+class IndegoClient(IndegoBaseClient):
+    """Class for Indego Non-Async Client."""
 
-    def __init__(
-        self,
-        username: str,
-        password: str,
-        serial: str = None,
-        map_filename: str = None,
-        api_url: str = DEFAULT_URL,
-    ):
-        """Abstract class for the Indego Clent, only use the Indego Client or Indego Async Client.
+    def __enter__(self):
+        """Enter for with."""
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """Exit for with."""
+        pass
+
+    def get_mowers(self):
+        """Get a list of the available mowers (serials) in the account."""
+        result = self.get("alms")
+        if result is None:
+            return []
+        return [mower['alm_sn'] for mower in result]
+
+    def delete_alert(self, alert_index: int):
+        """Delete the alert with the specified index.
 
         Args:
-            username (str): username for Indego Account
-            password (str): password for Indego Account
-            serial (str): serial number of the mower
-            map_filename (str, optional): Filename to store maps in. Defaults to None.
-            api_url (str, optional): url for the api, defaults to DEFAULT_URL.
+            alert_index (int): index of alert to be deleted, should be in range or length of alerts.
 
         """
-        self._username = username
-        self._password = password
-        self._serial = serial
-        self.map_filename = map_filename
-        self._api_url = api_url
-        self._logged_in = False
-        self._online = False
-        self._contextid = ""
-        self._userid = None
-
-        self.alerts = []
-        self._alerts_loaded = False
-        self.calendar = None
-        self.config = None
-        self.generic_data = None
-        self.last_completed_mow = None
-        self.location = None
-        self.network = None
-        self.next_mow = None
-        self.operating_data = None
-        self.predictive_calendar = None
-        self.predictive_schedule = None
-        self.security = None
-        self.state = None
-        self.setup = None
-        self.runtime = None
-        self.update_available = False
-        self.user = None
-
-    # Properties
-    @property
-    def serial(self):
-        """Return the serial number of the mower."""
-        if self._serial:
-            return self._serial
-        _LOGGER.warning("Serial not yet set, please login first")
-        return None
+        if not self._alerts_loaded:
+            raise ValueError("Alerts not loaded, please run update_alerts first.")
+        alert_id = self._get_alert_by_index(alert_index)
+        if not alert_id:
+            return None
+        return self._request(Methods.DELETE, f"alerts/{alert_id}/")
 
-    @property
-    def alerts_count(self):
-        """Return the count of alerts."""
-        if self.alerts:
-            return len(self.alerts)
-        return 0
-
-    @property
-    def state_description(self):
-        """Return the description of the state."""
-        if self.state:
-            return MOWER_STATE_DESCRIPTION.get(self.state.state, DEFAULT_LOOKUP_VALUE)
-        _LOGGER.warning("Please call update_state before calling this property")
+    def delete_all_alerts(self):
+        """Delete all the alerts."""
+        if not self._alerts_loaded:
+            raise ValueError("Alerts not loaded, please run update_alerts first.")
+        if self.alerts_count > 0:
+            return [
+                self._request(Methods.DELETE, f"alerts/{alert.alert_id}")
+                for alert in self.alerts
+            ]
+        _LOGGER.info("No alerts to delete")
         return None
 
-    @property
-    def state_description_detail(self):
-        """Return the description detail of the state."""
-        if self.state:
-            return MOWER_STATE_DESCRIPTION_DETAIL.get(
-                self.state.state, DEFAULT_LOOKUP_VALUE
+    def download_map(self, filename: str = None):
+        """Download the map.
+
+        Args:
+            filename (str, optional): Filename for the map. Defaults to None, can also be filled by the filename set in init.
+
+        """
+        if not self.serial:
+            return
+        if filename:
+            self.map_filename = filename
+        if not self.map_filename:
+            raise ValueError("No map filename defined.")
+        lawn_map = self.get(f"alms/{self.serial}/map")
+        if lawn_map:
+            with open(self.map_filename, "wb") as afp:
+                afp.write(lawn_map)
+
+    def put_alert_read(self, alert_index: int):
+        """Set the alert to read.
+
+        Args:
+            alert_index (int): index of alert to be deleted, should be in range or length of alerts.
+
+        """
+        if not self._alerts_loaded:
+            raise ValueError("Alerts not loaded, please run update_alerts first.")
+        alert_id = self._get_alert_by_index(alert_index)
+        if alert_id:
+            return self._request(
+                Methods.PUT, f"alerts/{alert_id}", data={"read_status": "read"}
             )
-        _LOGGER.warning("Please call update_state before calling this property")
-        return None
 
-    @property
-    def next_mows(self):
-        """Return the next mows from the calendar without a timezone."""
-        if self.calendar:
+    def put_all_alerts_read(self):
+        """Set to read the read_status of all alerts."""
+        if not self._alerts_loaded:
+            raise ValueError("Alerts not loaded, please run update_alerts first.")
+        if self.alerts_count > 0:
             return [
-                slot.dt for day in self.calendar.days for slot in day.slots if slot.dt
+                self._request(
+                    Methods.PUT,
+                    f"alerts/{alert.alert_id}",
+                    data={"read_status": "read"},
+                )
+                for alert in self.alerts
             ]
-        _LOGGER.warning("Please call update_calendar before calling this property")
+        _LOGGER.info("No alerts to set to read")
         return None
 
-    @property
-    def next_mows_with_tz(self):
-        """Return the next mows from the calendar with timezone from location."""
-        if self.location and self.calendar:
-            return [
-                slot.dt.astimezone(pytz.timezone(self.location.timezone))
-                for day in self.calendar.days
-                for slot in day.slots
-                if slot.dt
-            ]
-        if not self.location:
-            _LOGGER.warning("Please call update_location before calling this property")
-        if not self.calendar:
-            _LOGGER.warning("Please call update_calendar before calling this property")
-        return None
+    def put_command(self, command: str):
+        """Send a command to the mower.
 
-    # Methods
-    @abstractmethod
-    def delete_alert(self, alert_index: int):
-        """Delete the alert with the specified index."""
+        Args:
+            command (str): command should be one of "mow", "pause", "returnToDock"
 
-    @abstractmethod
-    def delete_all_alerts(self):
-        """Delete all the alerts."""
+        Returns:
+            str: either result of the call or 'Wrong Command'
 
-    @abstractmethod
-    def download_map(self, filename=None):
-        """Download the map."""
+        """
+        if command in COMMANDS:
+            if not self.serial:
+                return None
+            return self.put(f"alms/{self.serial}/state", {"state": command})
+        raise ValueError("Wrong Command, use one of 'mow', 'pause', 'returnToDock'")
 
-    @abstractmethod
-    def put_alert_read(self, alert_index: int):
-        """Set to read the read_status of the alert with the specified index."""
+    def put_mow_mode(self, command: typing.Any):
+        """Set the mower to mode manual (false-ish) or predictive (true-ish).
 
-    @abstractmethod
-    def put_all_alerts_read(self):
-        """Set to read the read_status of all alerts."""
+        Args:
+            command (str/bool): should be str that is bool-ish (true, True, false, False) or a bool.
 
-    @abstractmethod
-    def put_command(self, command: str):
-        """Send a command to the mower."""
+        Returns:
+            str: either result of the call or 'Wrong Command'
 
-    @abstractmethod
-    def put_mow_mode(self, command: Any):
-        """Set the mower to mode manual (false-ish) or predictive (true-ish)."""
+        """
+        if command in ("true", "false", "True", "False") or isinstance(command, bool):
+            if not self.serial:
+                return None
+            return self.put(f"alms/{self.serial}/predictive", {"enabled": command})
+        raise ValueError("Wrong Command, use True or False")
 
-    @abstractmethod
     def put_predictive_cal(self, calendar: dict = DEFAULT_CALENDAR):
         """Set the predictive calendar."""
+        try:
+            Calendar(**calendar["cals"][0])
+        except TypeError as exc:
+            raise ValueError("Value for calendar is not valid") from exc
+        if not self.serial:
+            return
+        return self.put(f"alms/{self.serial}/predictive/calendar", calendar)
 
-    @abstractmethod
     def update_alerts(self):
         """Update alerts."""
+        self._update_alerts(self.get("alerts"))
 
-    @abstractmethod
     def get_alerts(self):
         """Update alerts and return them."""
+        self.update_alerts()
+        return self.alerts
 
-    def _update_alerts(self, new):
-        """Update alerts."""
-        self._alerts_loaded = True
-        if new:
-            self.alerts = [Alert(**a) for a in new]
-        else:
-            self.alerts = []
-
-    @abstractmethod
     def update_all(self):
         """Update all states."""
+        self.update_alerts()
+        self.update_calendar()
+        self.update_config()
+        self.update_generic_data()
+        self.update_last_completed_mow()
+        self.update_location()
+        self.update_network()
+        self.update_next_mow()
+        self.update_operating_data()
+        self.update_predictive_calendar()
+        self.update_predictive_schedule()
+        self.update_security()
+        self.update_setup()
+        self.update_state()
+        self.update_updates_available()
+        self.update_user()
 
-    @abstractmethod
     def update_calendar(self):
         """Update calendar."""
+        if not self.serial:
+            return
+        self._update_calendar(self.get(f"alms/{self.serial}/calendar"))
 
-    @abstractmethod
     def get_calendar(self):
         """Update calendar and return it."""
+        self.update_calendar()
+        return self.calendar
 
-    def _update_calendar(self, new):
-        """Update calendar."""
-        if new:
-            self.calendar = generate_update(self.calendar, new["cals"][0], Calendar)
-
-    @abstractmethod
     def update_config(self):
         """Update config."""
+        if not self.serial:
+            return
+        self._update_config(self.get(f"alms/{self.serial}/config"))
 
-    @abstractmethod
     def get_config(self):
         """Update config and return it."""
+        self.update_config()
+        return self.config
 
-    def _update_config(self, new):
-        """Update config."""
-        if new:
-            self.config = generate_update(self.config, new, Config)
-
-    @abstractmethod
     def update_generic_data(self):
         """Update generic data."""
+        if not self.serial:
+            return
+        self._update_generic_data(self.get(f"alms/{self.serial}"))
 
-    @abstractmethod
     def get_generic_data(self):
         """Update generic_data and return it."""
+        self.update_generic_data()
+        return self.generic_data
 
-    def _update_generic_data(self, new):
-        """Update generic data."""
-        if new:
-            self.generic_data = generate_update(self.generic_data, new, GenericData)
-            self._update_battery_percentage_adjusted()
-
-    @abstractmethod
     def update_last_completed_mow(self):
         """Update last completed mow."""
+        if not self.serial:
+            return
+        self._update_last_completed_mow(
+            self.get(f"alms/{self.serial}/predictive/lastcutting")
+        )
 
-    @abstractmethod
     def get_last_completed_mow(self):
         """Update last_completed_mow and return it."""
+        self.update_last_completed_mow()
+        return self.last_completed_mow
 
-    def _update_last_completed_mow(self, new):
-        """Update last completed mow."""
-        if new:
-            self.last_completed_mow = convert_bosch_datetime(new["last_mowed"])
-
-    @abstractmethod
     def update_location(self):
         """Update location."""
+        if not self.serial:
+            return
+        self._update_location(self.get(f"alms/{self.serial}/predictive/location"))
 
-    @abstractmethod
     def get_location(self):
         """Update location and return it."""
+        self.update_location()
+        return self.location
 
-    def _update_location(self, new):
-        """Update location."""
-        if new:
-            self.location = generate_update(self.location, new, Location)
-
-    @abstractmethod
     def update_network(self):
         """Update network."""
+        if not self.serial:
+            return
+        self._update_network(self.get(f"alms/{self.serial}/network"))
 
-    @abstractmethod
     def get_network(self):
         """Update network and return it."""
+        self.update_network()
+        return self.network
 
-    def _update_network(self, new):
-        """Update network."""
-        if new:
-            self.network = generate_update(self.network, new, Network)
-
-    @abstractmethod
     def update_next_mow(self):
         """Update next mow datetime."""
+        if not self.serial:
+            return
+        self._update_next_mow(self.get(f"alms/{self.serial}/predictive/nextcutting"))
 
-    @abstractmethod
     def get_next_mow(self):
         """Update next_mow and return it."""
+        self.update_next_mow()
+        return self.next_mow
 
-    def _update_next_mow(self, new):
-        """Update next mow datetime."""
-        if new:
-            self.next_mow = convert_bosch_datetime(new["mow_next"])
-
-    @abstractmethod
     def update_operating_data(self):
         """Update operating data."""
+        if not self.serial:
+            return
+        self._update_operating_data(self.get(f"alms/{self.serial}/operatingData"))
 
-    @abstractmethod
     def get_operating_data(self):
         """Update operating_data and return it."""
+        self.update_operating_data()
+        return self.operating_data
 
-    def _update_operating_data(self, new):
-        """Update operating data."""
-        if new:
-            self.operating_data = generate_update(
-                self.operating_data, new, OperatingData
-            )
-            self._update_battery_percentage_adjusted()
-            self._online = True
-        else:
-            self._online = False
-
-    @abstractmethod
     def update_predictive_calendar(self):
         """Update predictive_calendar."""
+        if not self.serial:
+            return
+        self._update_predictive_calendar(
+            self.get(f"alms/{self.serial}/predictive/calendar")
+        )
 
-    @abstractmethod
     def get_predictive_calendar(self):
         """Update predictive_calendar and return it."""
+        self.update_predictive_calendar()
+        return self.predictive_calendar
 
-    def _update_predictive_calendar(self, new):
-        """Update predictive_calendar."""
-        if new:
-            self.predictive_calendar = generate_update(
-                self.predictive_calendar, new["cals"][0], Calendar
-            )
-
-    @abstractmethod
     def update_predictive_schedule(self):
-        """Update predictive schedule."""
+        """Update predictive_schedule."""
+        if not self.serial:
+            return
+        self._update_predictive_schedule(
+            self.get(f"alms/{self.serial}/predictive/schedule")
+        )
 
-    @abstractmethod
     def get_predictive_schedule(self):
         """Update predictive_schedule and return it."""
+        self.update_predictive_schedule()
+        return self.predictive_schedule
 
-    def _update_predictive_schedule(self, new):
-        """Update predictive schedule."""
-        if new:
-            self.predictive_schedule = generate_update(
-                self.predictive_schedule, new, PredictiveSchedule
-            )
-
-    @abstractmethod
     def update_security(self):
         """Update security."""
+        if not self.serial:
+            return
+        self._update_security(self.get(f"alms/{self.serial}/security"))
 
-    @abstractmethod
     def get_security(self):
         """Update security and return it."""
+        self.update_security()
+        return self.security
 
-    def _update_security(self, new):
-        """Update security."""
-        if new:
-            self.security = generate_update(self.security, new, Security)
-
-    @abstractmethod
     def update_setup(self):
         """Update setup."""
+        if not self.serial:
+            return
+        self._update_setup(self.get(f"alms/{self.serial}/setup"))
 
-    @abstractmethod
     def get_setup(self):
         """Update setup and return it."""
+        self.update_setup()
+        return self.setup
 
-    def _update_setup(self, new):
-        """Update setup."""
-        if new:
-            self.setup = generate_update(self.setup, new, Setup)
-
-    @abstractmethod
     def update_state(self, force=False, longpoll=False, longpoll_timeout=120):
-        """Update state. Can be both forced and with longpoll."""
+        """Update state. Can be both forced and with longpoll.
+
+        Args:
+            force (bool, optional): Force the state refresh, wakes up the mower. Defaults to False.
+            longpoll (bool, optional): Do a longpoll. Defaults to False.
+            longpoll_timeout (int, optional): Timeout of the longpoll. Defaults to 120.
+
+        """
+        if not self.serial:
+            return
+        path = f"alms/{self.serial}/state"
+        if longpoll:
+            last_state = 0
+            if self.state:
+                if self.state.state:
+                    last_state = self.state.state
+            path = f"{path}?longpoll=true&timeout={longpoll_timeout}&last={last_state}"
+        if force:
+            if longpoll:
+                path = f"{path}&forceRefresh=true"
+            else:
+                path = f"{path}?forceRefresh=true"
+
+        self._update_state(self.get(path, timeout=longpoll_timeout + 30))
 
-    @abstractmethod
     def get_state(self, force=False, longpoll=False, longpoll_timeout=120):
-        """Update state and return it."""
+        """Update state. Can be both forced and with longpoll.
 
-    def _update_state(self, new):
-        """Update state."""
-        if new:
-            self.state = generate_update(self.state, new, State)
+        Args:
+            force (bool, optional): Force the state refresh, wakes up the mower. Defaults to False.
+            longpoll (bool, optional): Do a longpoll. Defaults to False.
+            longpoll_timeout (int, optional): Timeout of the longpoll. Defaults to 120.
+
+        """
+        self.update_state(force, longpoll, longpoll_timeout)
+        return self.state
 
-    @abstractmethod
     def update_updates_available(self):
         """Update updates available."""
+        if not self.serial:
+            return
+        if self._online:
+            self._update_updates_available(self.get(f"alms/{self.serial}/updates"))
 
-    @abstractmethod
     def get_updates_available(self):
         """Update updates_available and return it."""
+        self.update_updates_available()
+        return self.update_available
 
-    def _update_updates_available(self, new):
-        """Update updates available."""
-        if new:
-            self.update_available = bool(new["available"])
-
-    @abstractmethod
     def update_user(self):
         """Update users."""
+        self._update_user(self.get(f"users/{self._userid}"))
 
-    @abstractmethod
     def get_user(self):
-        """Update user and return it."""
-
-    def _update_user(self, new):
-        """Update users."""
-        if new:
-            self.user = generate_update(self.user, new, User)
-
-    @abstractmethod
-    def login(self, attempts: int = 0):
-        """Login to the Indego API."""
-
-    def _login(self, login):
-        """Login to the Indego API."""
-        if login:
-            self._contextid = login["contextId"]
-            self._userid = login["userId"]
-            self._logged_in = True
-        else:
-            self._logged_in = False
+        """Update network and return it."""
+        self.update_user()
+        return self.user
 
-    @abstractmethod
-    def _request(
+    def _request(  # noqa: C901
         self,
         method: Methods,
         path: str,
         data: dict = None,
         headers: dict = None,
-        auth: Any = None,
         timeout: int = 30,
         attempts: int = 0,
     ):
-        """Request implemented by the subclasses either synchronously or asynchronously."""
+        """Send a request and return the response."""
+        if attempts >= 3:
+            _LOGGER.warning("Three attempts done, waiting 30 seconds.")
+            time.sleep(30)
 
-    @abstractmethod
-    def get(self, path: str, timeout: int):
-        """Get implemented by the subclasses either synchronously or asynchronously."""
-
-    @abstractmethod
-    def put(self, path: str, data: dict, timeout: int):
-        """Put implemented by the subclasses either synchronously or asynchronously."""
-
-    # internal methods
-    def _get_alert_by_index(self, alert_index: int) -> int:
-        """Return the alert_id based on index."""
-        if not self._alerts_loaded:
-            raise ValueError("Alerts not loaded, please run update_alerts first.")
-        if self.alerts_count == 0:
-            _LOGGER.info("No alerts to get")
+        if attempts >= 5:
+            _LOGGER.warning("Five attempts done, please try again manually.")
             return None
+
+        if self._token_refresh_method is not None:
+            self.token = self._token_refresh_method()
+
+        url = f"{self._api_url}{path}"
+
+        if not headers:
+            headers = DEFAULT_HEADER.copy()
+            headers["Authorization"] = "Bearer %s" % self._token
+
         try:
-            return self.alerts[alert_index].alert_id
-        except IndexError as exc:
-            raise IndexError(
-                f"Wrong index for the alert, there are {self.alerts_count} alerts, so the highest index is: {self.alerts_count - 1}, supplied was {alert_index}"
-            ) from exc
-
-    def _update_battery_percentage_adjusted(self):
-        """Update the battery percentage adjusted field, relies on generic and operating data populated."""
-        if self.generic_data and self.operating_data:
-            self.operating_data.battery.update_percent_adjusted(
-                self.generic_data.model_voltage
+            _LOGGER.debug("%s call to API endpoint %s", method.value, url)
+            response = requests.request(
+                method=method.value,
+                url=url,
+                json=data,
+                headers=headers,
+                timeout=timeout,
             )
+            status = response.status_code
+            _LOGGER.debug("HTTP status code: %i", status)
 
-    def __repr__(self):
-        """Create a string representing the mower."""
-        str1 = (
-            f"{self.generic_data.model_description} ({self.generic_data.alm_sn})"
-            if self.generic_data
-            else f"Indego mower"
-        )
-        str2 = f" owned by {self.user.display_name}." if self.user else f"."
-        str3 = f" {self.generic_data}, " if self.generic_data else ""
-        str4 = f" {self.state}, " if self.state else ""
-        str5 = f" {self.operating_data}, " if self.operating_data else ""
-        str6 = f", last mowed: {self.last_completed_mow}, next mow: {self.next_mow}, {self.location}, {self.network}, {self.alerts}, map filename: {self.map_filename}, {self.runtime}"
-        str7 = f"{self.operating_data.battery} " if self.operating_data else ""
-        str8 = f"update available: {self.update_available}, State Descr: {self.state_description}."
-        return f"{str1}{str2}{str3}{str4}{str5}{str6}{str7}{str8}"
+            if status == 200:
+                if method in (Methods.DELETE, Methods.PATCH, Methods.PUT):
+                    return True
+                if CONTENT_TYPE_JSON in response.headers[CONTENT_TYPE].split(";"):
+                    return response.json()
+                return response.content
+
+            if self._log_request_result(status, url):
+                return None
+
+            response.raise_for_status()
+
+        except Timeout as exc:
+            _LOGGER.error("%s: Timeout on Bosch servers, retrying.", exc)
+            return self._request(
+                method=method,
+                path=path,
+                data=data,
+                timeout=timeout,
+                attempts=attempts + 1,
+            )
+
+        except (TooManyRedirects, RequestException) as exc:
+            _LOGGER.error("%s: Failed to update Indego status.", exc)
+
+        except Exception as exc:
+            if self._raise_request_exceptions:
+                raise
+            _LOGGER.error("Request to %s gave a unhandled error: %s", url, exc)
+
+        return None
+
+    def get(self, path: str, timeout: int = 30):
+        """Send a GET request and return the response as a dict."""
+        return self._request(method=Methods.GET, path=path, timeout=timeout)
+
+    def put(self, path: str, data: dict, timeout: int = 30):
+        """Send a PUT request and return the response as a dict."""
+        return self._request(method=Methods.PUT, path=path, data=data, timeout=timeout)
```

### Comparing `pyIndego-3.0.0/pyIndego/states.py` & `pyIndego-3.0.1/pyIndego/states.py`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.0/pyIndego.egg-info/PKG-INFO` & `pyIndego-3.0.1/pyIndego.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyIndego
-Version: 3.0.0
+Version: 3.0.1
 Summary: API for Bosch Indego mower
 Home-page: https://github.com/jm-73/pyIndego
-Author: jm-73
+Author: jm-73, sander1988
 Author-email: jens@myretyr.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.txt
@@ -390,21 +390,18 @@
 Get the user adjustment of the mowing frequency
 
     update_automatic_update()
 Get the automatic update settings
 
 
 # API CALLS
-https://api.indego.iot.bosch-si.com:443/api/v1
+https://api.indego-cloud.iot.bosch-si.com/api/v1/
 
 
 ```python
-post
-/authenticate
-
 get
 /alerts
 /alms
 /alms/<serial>
 /alms/<serial>/automaticUpdate
 /alms/<serial>/calendar
 /alms/<serial>/config
```

### Comparing `pyIndego-3.0.0/setup.py` & `pyIndego-3.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pyIndego",
-    version="3.0.0",
-    author="jm-73",
+    version="3.0.1",
+    author="jm-73, sander1988",
     author_email="jens@myretyr.se",
     description="API for Bosch Indego mower",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jm-73/pyIndego",
     packages=find_packages("."),
     install_requires=["requests", "aiohttp", "pytz"],
```

### Comparing `pyIndego-3.0.0/tests/test_indego.py` & `pyIndego-3.0.1/tests/test_indego.py`

 * *Files identical despite different names*

