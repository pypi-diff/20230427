# Comparing `tmp/aio_overpass-0.1.1.tar.gz` & `tmp/aio_overpass-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_overpass-0.1.1.tar", max compression
+gzip compressed data, was "aio_overpass-0.1.2.tar", max compression
```

## Comparing `aio_overpass-0.1.1.tar` & `aio_overpass-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-01-07 23:46:48.048295 aio_overpass-0.1.1/LICENSE
--rw-r--r--   0        0        0     7949 2023-04-25 17:48:06.992954 aio_overpass-0.1.1/README.md
--rwxr-xr-x   0        0        0      316 2023-04-25 17:54:12.413446 aio_overpass-0.1.1/aio_overpass/__init__.py
--rw-r--r--   0        0        0      977 2023-04-20 23:16:58.247002 aio_overpass-0.1.1/aio_overpass/_dist.py
--rwxr-xr-x   0        0        0      971 2023-04-20 23:16:58.244337 aio_overpass-0.1.1/aio_overpass/_ql.py
--rwxr-xr-x   0        0        0    10947 2023-04-25 17:41:10.527121 aio_overpass-0.1.1/aio_overpass/client.py
--rwxr-xr-x   0        0        0    28053 2023-04-25 17:43:06.114287 aio_overpass-0.1.1/aio_overpass/element.py
--rwxr-xr-x   0        0        0    13665 2023-04-23 00:09:18.209185 aio_overpass-0.1.1/aio_overpass/error.py
--rwxr-xr-x   0        0        0    24559 2023-04-25 17:41:10.606022 aio_overpass-0.1.1/aio_overpass/pt.py
--rwxr-xr-x   0        0        0    22325 2023-04-25 17:41:10.603938 aio_overpass-0.1.1/aio_overpass/pt_ordered.py
--rwxr-xr-x   0        0        0    14338 2023-04-25 17:41:10.546650 aio_overpass-0.1.1/aio_overpass/query.py
--rwxr-xr-x   0        0        0     2160 2023-04-25 17:54:15.999637 aio_overpass-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9265 1970-01-01 00:00:00.000000 aio_overpass-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8007 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/README.md
+-rwxr-xr-x   0        0        0      316 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/__init__.py
+-rw-r--r--   0        0        0      977 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/_dist.py
+-rwxr-xr-x   0        0        0      971 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/_ql.py
+-rwxr-xr-x   0        0        0    11056 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/client.py
+-rwxr-xr-x   0        0        0    28078 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/element.py
+-rwxr-xr-x   0        0        0    14075 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/error.py
+-rwxr-xr-x   0        0        0    24584 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/pt.py
+-rwxr-xr-x   0        0        0    22350 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/pt_ordered.py
+-rwxr-xr-x   0        0        0    14363 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/query.py
+-rwxr-xr-x   0        0        0     2160 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9323 1970-01-01 00:00:00.000000 aio_overpass-0.1.2/PKG-INFO
```

### Comparing `aio_overpass-0.1.1/LICENSE` & `aio_overpass-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.1/README.md` & `aio_overpass-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 - [Basic Usage](#basic-usage)
   - [Example](#example)
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
-- API reference is forthcoming :construction: 
-- The version history is available in [CHANGELOG.md](CHANGELOG.md).
+- An overview of modules, classes and functions can be found in the [API reference](http://www.timwie.dev/aio-overpass/).
+- The version history is available in [CHANGELOG.md](https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md).
 - Contributor guide is forthcoming :construction:
 
 <br>
 
 ## Features
 - Asynchronous requests using [aiohttp]
 - Concurrent queries
@@ -41,15 +41,15 @@
   - [Shapely] geometries for manipulation and analysis
   - [GeoJSON] exports
   - Simplified querying and processing of public transportation routes
 
 <br>
 
 ## Getting Started
-```
+```sh
 pip install aio-overpass
 pip install aio-overpass[shapely, networkx, joblib]
 
 poetry add aio-overpass
 poetry add aio-overpass[shapely, networkx, joblib]
 ```
 
@@ -95,72 +95,72 @@
     - Either access the raw result dictionaries with `query.result_set`,
     - or use a collector, f.e. `collect_elements(query)` to get a list of typed `Elements`.
     - Collectors are often specific to queries - `collect_routes` requires a `RouteQuery`,
       for instance.
 
 ### Example
 #### Results as Dictionaries
-```
+```python
 from aio_overpass import Client, Query
 
 query = Query("way(24981342); out geom;")
 
 client = Client()
 
 await client.run_query(query)
 
 query.result_set
 ```
 
-```
+```python
 {
-    ...
+    # ...
     "elements": [
         {
             "type": "way",
             "id": 24981342,
-            ...
+            # ...
             "tags": {
                 "addr:city": "Hamburg",
                 "addr:country": "DE",
                 "addr:housename": "Elbphilharmonie",
-                ...
+                # ...
             },
         }
     ],
 }
 ```
 
 #### Results as Objects
-```
+```python
 from aio_overpass.element import collect_elements
 
 elems = collect_elements(query)
 
 elems[0].tags
 ```
 
-```
+```python
 {
     "addr:city": "Hamburg",
     "addr:country": "DE",
     "addr:housename": "Elbphilharmonie",
-    ...
+    # ...
 }
 
 ```
 
 #### Results as GeoJSON
-```
+```python
 import json
 
 json.dumps(elems[0].geojson, indent=4)
 ```
 
-```
+```json
 {
     "type": "Feature",
     "geometry": {
         "type": "Polygon",
         "coordinates": [
             [
                 [
@@ -176,20 +176,15 @@
         "type": "way",
         "tags": {
             "addr:city": "Hamburg",
             "addr:country": "DE",
             "addr:housename": "Elbphilharmonie",
             ...
         },
-        "bounds": [
-            53.540877,
-            9.9832434,
-            53.5416212,
-            9.9849674
-        ]
+        ...
     },
     "bbox": [
         9.9832434,
         53.540877,
         9.9849674
         53.5416212,
     ]
```

### Comparing `aio_overpass-0.1.1/aio_overpass/_dist.py` & `aio_overpass-0.1.2/aio_overpass/_dist.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.1/aio_overpass/_ql.py` & `aio_overpass-0.1.2/aio_overpass/_ql.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.1/aio_overpass/client.py` & `aio_overpass-0.1.2/aio_overpass/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Interface for making API calls."""
 
 import asyncio
 import logging
 import re
+import sys
 from dataclasses import dataclass
 from typing import Optional
 from urllib.parse import urljoin
 
 from aio_overpass import __version__
 from aio_overpass.error import (
     CallError,
@@ -19,14 +20,15 @@
     _to_client_error,
 )
 from aio_overpass.query import DefaultQueryRunner, Query, QueryRunner
 
 import aiohttp
 
 
+__docformat__ = "google"
 __all__ = (
     "Client",
     "Status",
     "DEFAULT_INSTANCE",
     "DEFAULT_USER_AGENT",
 )
 
@@ -93,15 +95,15 @@
         self._url = url
         self._user_agent = user_agent
         self._runner = runner or DefaultQueryRunner()
 
         self._maybe_session = None
         self._maybe_sem = None
 
-    async def _session(self) -> aiohttp.ClientSession:
+    def _session(self) -> aiohttp.ClientSession:
         """The session used for all requests of this client."""
         if not self._maybe_session or self._maybe_session.closed:
             headers = {"User-Agent": self._user_agent}
             self._maybe_session = aiohttp.ClientSession(headers=headers)
 
         return self._maybe_session
 
@@ -111,15 +113,15 @@
 
         This semaphore can be acquired as many times as there are query slots at the API instance.
         If all slots are acquired, further queries need to wait until a slot is released.
         """
         if self._maybe_sem:
             return self._maybe_sem
 
-        session = await self._session()
+        session = self._session()
 
         status = await self._status(session, **kwargs)
 
         self._maybe_sem = asyncio.BoundedSemaphore(status.slots or _DEFAULT_SLOTS)
         return self._maybe_sem
 
     async def close(self) -> None:
@@ -173,30 +175,30 @@
     async def status(self) -> Status:
         """
         Check the current API status.
 
         Raises:
             ClientError: if the status could not be looked up
         """
-        session = await self._session()
+        session = self._session()
         return await self._status(session)
 
     async def cancel_queries(self) -> int:
         """
         Cancel all running queries.
 
         This can be used to terminate runaway queries that prevent you from sending new ones.
 
         Returns:
             the number of terminated queries
 
         Raises:
             ClientError: if the request to cancel queries failed
         """
-        session = await self._session()
+        session = self._session()
         endpoint = urljoin(self._url, "kill_my_queries")
         try:
             async with session.get(endpoint) as response:
                 body = await response.text()
                 killed_pids = re.findall("\\(pid (\\d+)\\)", body)
                 return len(set(killed_pids))
         except aiohttp.ClientError as err:
@@ -219,15 +221,16 @@
             ClientError: when query or status requests fail. If the query was retried, the error
                          of the last try will be raised. The same exception is also captured in
                          `query.error`.
         """
         if query.done:
             return  # nothing to do
 
-        query.reset()  # reset failed queries
+        if query.nb_tries > 0:
+            query.reset()  # reset failed queries
 
         while not query.done:
             await self._run_query_once(query)
 
     async def _run_query_once(self, query: Query) -> None:
         loop = asyncio.get_event_loop()
 
@@ -253,15 +256,15 @@
         check_cooldown = (
             query.error
             and isinstance(query.error, QueryRejectError)
             and query.error.cause == QueryRejectCause.TOO_MANY_QUERIES
         )
 
         try:
-            session = await self._session()
+            session = self._session()
             rate_limiter = await self._rate_limiter(timeout=_next_timeout(query))
 
             if check_cooldown:
                 # If this client is running too many queries, we can check the status for a
                 # cooldown period. This request failing is a bit of an edge case.
                 # 'query.error' will be overwritten, which means we will not check for a
                 # cooldown in the next iteration.
@@ -301,15 +304,16 @@
 
         except ClientError as err:
             query._error = err
 
 
 def _next_timeout_secs(query: Query) -> Optional[float]:
     if query.run_timeout_secs:
-        return max(0.0, query.run_timeout_secs - query.run_duration_secs)
+        # use epsilon since 0 means "no timeout"
+        return max(sys.float_info.epsilon, query.run_timeout_secs - query.run_duration_secs)
 
 
 def _next_timeout(query: Query) -> aiohttp.ClientTimeout:
     return aiohttp.ClientTimeout(total=_next_timeout_secs(query))
 
 
 def _giveup_error(query: Query, loop: asyncio.AbstractEventLoop) -> GiveupError:
```

### Comparing `aio_overpass-0.1.1/aio_overpass/element.py` & `aio_overpass-0.1.2/aio_overpass/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     MultiPolygon,
     Point,
     Polygon,
 )
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
 
+__docformat__ = "google"
 __all__ = (
     "GeoJsonDict",
     "OverpassDict",
     "Bbox",
     "Spatial",
     "Element",
     "Node",
```

### Comparing `aio_overpass-0.1.1/aio_overpass/error.py` & `aio_overpass-0.1.2/aio_overpass/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from json import JSONDecodeError
 from typing import List, Optional, Tuple, Union
 
 import aiohttp
 import aiohttp.typedefs
 
 
+__docformat__ = "google"
 __all__ = (
     "ClientError",
     "CallError",
     "ResponseError",
     "GiveupError",
     "QueryError",
     "QueryLanguageError",
@@ -165,22 +166,32 @@
         kwargs: the query's ``kwargs``
         messages: the error messages provided by the API
     """
 
     kwargs: dict
     messages: List[str]
 
+    def __post_init__(self) -> None:
+        if not self.messages:
+            raise ValueError("expected at least one message")
+
     def __str__(self) -> str:
         if self.kwargs:
             query = f"query {self.kwargs}"
         else:
             query = "query <no kwargs>"
 
-        messages = ", ".join(f"'{msg}'" for msg in self.messages)
-        return f"{query} failed: {messages}"
+        first = f"'{self.messages[0]}'"
+
+        if len(self.messages) > 1:
+            rest = f" (+{len(self.messages) - 1} more)"
+        else:
+            rest = ""
+
+        return f"{query} failed: {first}{rest}"
 
     def __repr__(self) -> str:
         messages = ", ".join(f"'{msg}'" for msg in self.messages)
         return f"{type(self).__name__}(kwargs={self.kwargs}, messages={messages})"
 
 
 @dataclass
@@ -312,29 +323,36 @@
     await _raise_for_html_response(response, query_kwargs)
 
     try:
         json = await response.json()
     except aiohttp.ClientResponseError as err:
         raise _to_client_error(err)
     except JSONDecodeError as err:
-        raise ResponseError(
-            request_info=response.request_info,
-            history=response.history,
-            status=response.status,
-            message=response.reason,
-            headers=response.headers,
-        ) from err
+        raise _response_error(response) from err
+
+    if json is None:
+        raise _response_error(response)
 
     _raise_for_json_remarks(json, query_kwargs)
 
     _raise_for_status(response, query_kwargs)
 
     return json
 
 
+def _response_error(response: aiohttp.ClientResponse) -> ResponseError:
+    return ResponseError(
+        request_info=response.request_info,
+        history=response.history,
+        status=response.status,
+        message=response.reason,
+        headers=response.headers,
+    )
+
+
 def _raise_for_status(response: aiohttp.ClientResponse, query_kwargs: dict) -> None:
     """
     Raise a fitting exception based on the status code.
 
     Raises:
         RejectError: for status "Too Many Requests" and "Gateway Timeout"
         ResponseError: for any status >= 400
```

### Comparing `aio_overpass-0.1.1/aio_overpass/pt.py` & `aio_overpass-0.1.2/aio_overpass/pt.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 )
 from aio_overpass.query import Query
 
 import shapely.ops
 from shapely.geometry import GeometryCollection, Point, Polygon
 
 
+__docformat__ = "google"
 __all__ = (
     "Route",
     "Stop",
     "Connection",
     "Vehicle",
     "RouteScheme",
     "RouteQuery",
```

### Comparing `aio_overpass-0.1.1/aio_overpass/pt_ordered.py` & `aio_overpass-0.1.2/aio_overpass/pt_ordered.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Point,
     Polygon,
 )
 
 from .pt import _MAX_DISTANCE_TO_TRACK, Route, RouteQuery, Stop, collect_routes
 
 
+__docformat__ = "google"
 __all__ = (
     "OrderedRouteView",
     "OrderedRouteViewNode",
     "collect_ordered_routes",
 )
```

### Comparing `aio_overpass-0.1.1/aio_overpass/query.py` & `aio_overpass-0.1.2/aio_overpass/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     QueryLanguageError,
     QueryRejectCause,
     QueryRejectError,
     ResponseError,
 )
 
 
+__docformat__ = "google"
 __all__ = (
     "Query",
     "QueryRunner",
     "DefaultQueryRunner",
     "DEFAULT_MAXSIZE",
     "DEFAULT_TIMEOUT",
 )
```

### Comparing `aio_overpass-0.1.1/pyproject.toml` & `aio_overpass-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-overpass"
-version = "0.1.1"
+version = "0.1.2"
 description = "Async client for the Overpass API"
 authors = ["Tim Wiechers <mail@timwie.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwie/aio-overpass"
 # TODO documentation = "https://..."
 packages = [{ include = "aio_overpass" }]
```

### Comparing `aio_overpass-0.1.1/PKG-INFO` & `aio_overpass-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-overpass
-Version: 0.1.1
+Version: 0.1.2
 Summary: Async client for the Overpass API
 Home-page: https://github.com/timwie/aio-overpass
 License: MIT
 Keywords: geojson,geospatial,gis,open-street-map,osm,overpass-api,public-transport
 Author: Tim Wiechers
 Author-email: mail@timwie.dev
 Requires-Python: >=3.8,<4.0
@@ -54,16 +54,16 @@
 - [Basic Usage](#basic-usage)
   - [Example](#example)
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
-- API reference is forthcoming :construction: 
-- The version history is available in [CHANGELOG.md](CHANGELOG.md).
+- An overview of modules, classes and functions can be found in the [API reference](http://www.timwie.dev/aio-overpass/).
+- The version history is available in [CHANGELOG.md](https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md).
 - Contributor guide is forthcoming :construction:
 
 <br>
 
 ## Features
 - Asynchronous requests using [aiohttp]
 - Concurrent queries
@@ -74,15 +74,15 @@
   - [Shapely] geometries for manipulation and analysis
   - [GeoJSON] exports
   - Simplified querying and processing of public transportation routes
 
 <br>
 
 ## Getting Started
-```
+```sh
 pip install aio-overpass
 pip install aio-overpass[shapely, networkx, joblib]
 
 poetry add aio-overpass
 poetry add aio-overpass[shapely, networkx, joblib]
 ```
 
@@ -128,72 +128,72 @@
     - Either access the raw result dictionaries with `query.result_set`,
     - or use a collector, f.e. `collect_elements(query)` to get a list of typed `Elements`.
     - Collectors are often specific to queries - `collect_routes` requires a `RouteQuery`,
       for instance.
 
 ### Example
 #### Results as Dictionaries
-```
+```python
 from aio_overpass import Client, Query
 
 query = Query("way(24981342); out geom;")
 
 client = Client()
 
 await client.run_query(query)
 
 query.result_set
 ```
 
-```
+```python
 {
-    ...
+    # ...
     "elements": [
         {
             "type": "way",
             "id": 24981342,
-            ...
+            # ...
             "tags": {
                 "addr:city": "Hamburg",
                 "addr:country": "DE",
                 "addr:housename": "Elbphilharmonie",
-                ...
+                # ...
             },
         }
     ],
 }
 ```
 
 #### Results as Objects
-```
+```python
 from aio_overpass.element import collect_elements
 
 elems = collect_elements(query)
 
 elems[0].tags
 ```
 
-```
+```python
 {
     "addr:city": "Hamburg",
     "addr:country": "DE",
     "addr:housename": "Elbphilharmonie",
-    ...
+    # ...
 }
 
 ```
 
 #### Results as GeoJSON
-```
+```python
 import json
 
 json.dumps(elems[0].geojson, indent=4)
 ```
 
-```
+```json
 {
     "type": "Feature",
     "geometry": {
         "type": "Polygon",
         "coordinates": [
             [
                 [
@@ -209,20 +209,15 @@
         "type": "way",
         "tags": {
             "addr:city": "Hamburg",
             "addr:country": "DE",
             "addr:housename": "Elbphilharmonie",
             ...
         },
-        "bounds": [
-            53.540877,
-            9.9832434,
-            53.5416212,
-            9.9849674
-        ]
+        ...
     },
     "bbox": [
         9.9832434,
         53.540877,
         9.9849674
         53.5416212,
     ]
```

