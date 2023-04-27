# Comparing `tmp/anilibria.py-1.0.1.tar.gz` & `tmp/anilibria.py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anilibria.py-1.0.1.tar", last modified: Thu Feb  9 15:03:49 2023, max compression
+gzip compressed data, was "anilibria.py-1.0.2.tar", last modified: Thu Apr 27 14:18:56 2023, max compression
```

## Comparing `anilibria.py-1.0.1.tar` & `anilibria.py-1.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.009761 anilibria.py-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-02-09 15:03:49.009761 anilibria.py-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.005761 anilibria.py-1.0.1/anilibria/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.005761 anilibria.py-1.0.1/anilibria/api/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.005761 anilibria.py-1.0.1/anilibria/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/gateway/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.005761 anilibria.py-1.0.1/anilibria/api/gateway/events/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/gateway/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/gateway/events/anilibria.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/gateway/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/gateway/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.009761 anilibria.py-1.0.1/anilibria/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/http/public.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.009761 anilibria.py-1.0.1/anilibria/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/models/attrs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/models/cattrs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/models/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/api/models/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.009761 anilibria.py-1.0.1/anilibria/client/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40128 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.009761 anilibria.py-1.0.1/anilibria/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/anilibria/utils/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:03:49.005761 anilibria.py-1.0.1/anilibria.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-02-09 15:03:48.000000 anilibria.py-1.0.1/anilibria.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-09 15:03:49.000000 anilibria.py-1.0.1/anilibria.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 15:03:48.000000 anilibria.py-1.0.1/anilibria.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-09 15:03:48.000000 anilibria.py-1.0.1/anilibria.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-09 15:03:48.000000 anilibria.py-1.0.1/anilibria.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 15:03:49.009761 anilibria.py-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-02-09 15:03:35.000000 anilibria.py-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.783875 anilibria.py-1.0.2/anilibria/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.783875 anilibria.py-1.0.2/anilibria/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.783875 anilibria.py-1.0.2/anilibria/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/gateway/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/anilibria/api/gateway/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/gateway/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/gateway/events/anilibria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/gateway/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/gateway/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/anilibria/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/http/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/anilibria/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/models/attrs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/models/cattrs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/models/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/api/models/title.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/anilibria/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42379 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/anilibria/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/anilibria/utils/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:18:56.783875 anilibria.py-1.0.2/anilibria.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-27 14:18:56.000000 anilibria.py-1.0.2/anilibria.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-27 14:18:56.000000 anilibria.py-1.0.2/anilibria.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:18:56.000000 anilibria.py-1.0.2/anilibria.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-27 14:18:56.000000 anilibria.py-1.0.2/anilibria.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 14:18:56.000000 anilibria.py-1.0.2/anilibria.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:18:56.787875 anilibria.py-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-27 14:18:45.000000 anilibria.py-1.0.2/setup.py
```

### Comparing `anilibria.py-1.0.1/LICENSE` & `anilibria.py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/PKG-INFO` & `anilibria.py-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anilibria.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: An async API wrapper for the anilibria.tv
 Home-page: https://github.com/Damego/anilibria.py
 Author: Damego
 Author-email: danyabatueff@gmail.com
 License: GPL-3.0 License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -99,8 +99,9 @@
 и с другими.
 
 Примеры использования представлены `здесь <https://github.com/Damego/anilibria.py/tree/main/examples>`__
 
 Документация
 ^^^^^^^^^^^^
 `Официальная документация API <https://github.com/anilibria/docs/blob/master/api_v3.md>`__
+
 `Документация библиотеки <https://anilibriapy.readthedocs.io/ru/latest/>`__
```

### Comparing `anilibria.py-1.0.1/README.rst` & `anilibria.py-1.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -74,8 +74,9 @@
 и с другими.
 
 Примеры использования представлены `здесь <https://github.com/Damego/anilibria.py/tree/main/examples>`__
 
 Документация
 ^^^^^^^^^^^^
 `Официальная документация API <https://github.com/anilibria/docs/blob/master/api_v3.md>`__
-`Документация библиотеки <https://anilibriapy.readthedocs.io/ru/latest/>`__
+
+`Документация библиотеки <https://anilibriapy.readthedocs.io/ru/latest/>`__
```

### Comparing `anilibria.py-1.0.1/anilibria/api/dispatch.py` & `anilibria.py-1.0.2/anilibria/api/dispatch.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria/api/gateway/client.py` & `anilibria.py-1.0.2/anilibria/api/gateway/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,27 @@
         if response.type is WSMsgType.CLOSING:
             self._closed = True
             return response
 
         return response.json(loads=loads)
 
     def _track_data(self, data: dict):
+        log.debug(
+            f"Received an event with data {data}",
+        )
+
         type: str
         if not (type := data.get("type")):
             return self._track_unknown_event(data)
 
         event_model = EventType[type.upper()].value
 
         if event_model is None:
             return log.warning(f"Received a not excepted event `{type}`!")
 
-        log.debug(f"Received {type} event {data}")
-
         obj = converter.structure(data["data"], event_model)
         self.dispatch.call(f"on_{type}", obj)
 
     def _track_unknown_event(self, data: dict):
         if "subscribe" in data:
             self.dispatch.call("on_subscription", converter.structure(data, Subscription))
```

### Comparing `anilibria.py-1.0.1/anilibria/api/gateway/events/anilibria.py` & `anilibria.py-1.0.2/anilibria/api/gateway/events/anilibria.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 
     .. code-block:: python
 
       @client.on(Subscription)
       async def event_subscription(event: Subscription):
           ...
     """
+
     subscribe: str
     "Статус подписки"
     subscription_id: int
     "ID подписки"
 
 
 class EventType(Enum):
```

### Comparing `anilibria.py-1.0.1/anilibria/api/gateway/events/internal.py` & `anilibria.py-1.0.2/anilibria/api/gateway/events/internal.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria/api/http/public.py` & `anilibria.py-1.0.2/anilibria/api/http/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,7 +369,35 @@
     async def add_user_favorite(self, session: str, title_id: int) -> dict:
         payload: dict = dict_filter_none(session=session, title_id=title_id)
         return await self.request(Route("PUT", "/user/favourites/add"), payload)
 
     async def remove_user_favorite(self, session: str, title_id: int) -> dict:
         payload: dict = dict_filter_none(session=session, title_id=title_id)
         return await self.request(Route("DELETE", "/user/favourites/remove"), payload)
+
+    async def get_title_franchises(
+        self,
+        id: int,
+        filter: list[str] | None = None,
+        remove: list[str] | None = None,
+    ) -> dict:
+        payload: dict = dict_filter_none(id=id, filter=filter, remove=remove)
+        return await self.request(Route("GET", "/title/franchises"), payload)
+
+    async def get_franchises(
+        self,
+        filter: list[str] | None = None,
+        remove: list[str] | None = None,
+        limit: int | None = None,
+        after: int | None = None,
+        page: int | None = None,
+        items_per_page: int | None = None,
+    ) -> list[dict]:
+        payload: dict = dict_filter_none(
+            filter=filter,
+            remove=remove,
+            limit=limit,
+            after=after,
+            page=page,
+            items_per_page=items_per_page,
+        )
+        return await self.request(Route("GET", "/franchise/list"), payload)
```

### Comparing `anilibria.py-1.0.1/anilibria/api/http/request.py` & `anilibria.py-1.0.2/anilibria/api/http/request.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria/api/models/cattrs_utils.py` & `anilibria.py-1.0.2/anilibria/api/models/cattrs_utils.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria/api/models/enums.py` & `anilibria.py-1.0.2/anilibria/api/models/enums.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria/api/models/misc.py` & `anilibria.py-1.0.2/anilibria/api/models/misc.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria/api/models/title.py` & `anilibria.py-1.0.2/anilibria/api/models/title.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     "Player",
     "Quality",
     "TorrentFile",
     "TorrentMetaData",
     "Torrent",
     "Torrents",
     "Title",
+    "Franchise",
+    "FranchiseRelease",
+    "TitleFranchise",
 )
 
 
 @define()
 class TitleNames:
     """
     Объект, содержащий названия тайтла на различных языках.
@@ -206,14 +209,16 @@
     "Время создания/изменения в формате UNIX timestamp"
     hls: HLS | None = None
     "Ссылки на серию"
     preview: str | None = None
     "Ссылка на превью серии"
     skips: SerieSkips | None = None
     "Таймкоды на пропуски"
+    uuid: str
+    "UUID эпизода"
 
     # TODO: Добавить свойство 'created_at' с datetime
 
 
 @define()
 class RutubeEpisode:
     """
@@ -353,14 +358,42 @@
     no_view_order: str | None = None
     "Описание тайтла в виде текста без дополнительного форматирования и порядка просмотра"
     plain: str | None = None
     "Описание тайтла без дополнительного форматирования"
 
 
 @define()
+class Franchise:
+    id: str
+    "UUID франшизы"
+    name: str
+    "Название франшизы"
+
+
+@define()
+class FranchiseRelease:
+    id: int
+    "ID тайтла"
+    code: str
+    "Код тайтла"
+    names: TitleNames
+    "Названия тайтла"
+    ordinal: int
+    "Порядковый номер в списке"
+
+
+@define()
+class TitleFranchise:
+    franchise: Franchise
+    "Объект с информацией о франшизе"
+    releases: list[FranchiseRelease]
+    "Список релизов франшизы"
+
+
+@define()
 class Title:
     """
     Объект тайтла
     """
 
     id: int | None = None
     "ID тайтла"
@@ -392,14 +425,16 @@
     "Сколько раз тайтл добавили в избранное"
     blocked: Blocked | None = None
     "Информация о блокировке тайтла"
     player: Player | None = None
     "Информация о плеере"
     torrents: Torrents | None = None
     "Информация о торрентах"
+    franchises: list[TitleFranchise] | None = None
+    "Список франшиз"
 
     @property
     def url(self) -> str:
         """
         Возвращает полную ссылку на тайтл
         """
         return f"https://anilibria.tv/release/{self.code}.html"
```

### Comparing `anilibria.py-1.0.1/anilibria/client/client.py` & `anilibria.py-1.0.2/anilibria/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Include,
     ListPagination,
     PlaylistType,
     RSSType,
     Schedule,
     SeedStats,
     Title,
+    TitleFranchise,
     TitleTeam,
     User,
     YouTubeVideo,
 )
 from ..api.models.cattrs_utils import converter
 from ..utils.serializer import dict_filter_missing
 from ..utils.typings import MISSING, Absent
@@ -793,14 +794,65 @@
         Удаляет тайтл из списка избранных
 
         :param str session_id: ID сессии.
         :param int title_id: ID тайтла.
         """
         await self._http.remove_user_favorite(session=session_id, title_id=title_id)
 
+    async def get_title_franchises(
+        self,
+        id: int,
+        filter: Absent[list[str]] = MISSING,
+        remove: Absent[list[str]] = MISSING,
+    ) -> TitleFranchise | None:
+        """
+        Получение франшизы тайтла
+
+        :param id: ID тайтла
+        :param Absent[list[str]] filter: Список значений, которые будут в ответе.
+        :param Absent[list[str]] remove: Список значений, которые будут удалены из ответа.
+        """
+        payload = dict_filter_missing(
+            id=id,
+            filter=filter,
+            remove=remove,
+        )
+        data = await self._http.get_title_franchises(**payload)
+        return converter.structure(data, TitleFranchise) if data else None
+
+    async def get_franchises(
+        self,
+        filter: Absent[list[str]] = MISSING,
+        remove: Absent[list[str]] = MISSING,
+        after: Absent[int] = MISSING,
+        limit: Absent[int] = MISSING,
+        page: Absent[int] = MISSING,
+        items_per_page: Absent[int] = MISSING,
+    ) -> ListPagination[TitleFranchise]:
+        """
+        Возвращает список всех франшиз
+
+        :param Absent[list[str]] filter: Список значений, которые будут в ответе.
+        :param Absent[list[str]] remove: Список значений, которые будут удалены из ответа.
+        :param Absent[int] after: Удаляет первые n записей из выдачи.
+        :param Absent[int] limit: Количество объектов в ответе.
+        :param Absent[int] page: Номер страницы. По умолчанию 1
+        :param Absent[int] items_per_page: Количество элементов на одной странице.
+        """
+        payload = dict_filter_missing(
+            filter=filter,
+            remove=remove,
+            after=after,
+            limit=limit,
+            page=page,
+            items_per_page=items_per_page,
+        )
+        data = await self._http.get_franchises(**payload)
+        return converter.structure(data, ListPagination[TitleFranchise])
+
     async def astart(self, *, auto_reconnect: bool = True):
         """
         Запускает клиент асинхронно
         """
 
         while True:
             try:
```

### Comparing `anilibria.py-1.0.1/anilibria/utils/serializer.py` & `anilibria.py-1.0.2/anilibria/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria/utils/typings.py` & `anilibria.py-1.0.2/anilibria/utils/typings.py`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/anilibria.py.egg-info/PKG-INFO` & `anilibria.py-1.0.2/anilibria.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anilibria.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: An async API wrapper for the anilibria.tv
 Home-page: https://github.com/Damego/anilibria.py
 Author: Damego
 Author-email: danyabatueff@gmail.com
 License: GPL-3.0 License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -99,8 +99,9 @@
 и с другими.
 
 Примеры использования представлены `здесь <https://github.com/Damego/anilibria.py/tree/main/examples>`__
 
 Документация
 ^^^^^^^^^^^^
 `Официальная документация API <https://github.com/anilibria/docs/blob/master/api_v3.md>`__
+
 `Документация библиотеки <https://anilibriapy.readthedocs.io/ru/latest/>`__
```

### Comparing `anilibria.py-1.0.1/anilibria.py.egg-info/SOURCES.txt` & `anilibria.py-1.0.2/anilibria.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anilibria.py-1.0.1/pyproject.toml` & `anilibria.py-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 100
 
 [tool.poetry]
 name = "anilibria.py"
-version = "1.0.1"
+version = "1.0.2"
 description = "An async API wrapper for the anilibria.tv"
 authors = ["Damego <damego.dev@gmail.com>"]
 license = "GPL-3.0"
 packages=[
     {include = "anilibria"}
 ]
```

### Comparing `anilibria.py-1.0.1/setup.py` & `anilibria.py-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     version=pyproject["tool"]["poetry"]["version"],
     author="Damego",
     author_email="danyabatueff@gmail.com",
     description=pyproject["tool"]["poetry"]["description"],
     extras_require=extra_requirements,
     include_package_data=True,
     install_requires=[
-        "aiohttp==3.8.3",
+        "aiohttp>=3.8.3",
         "attrs==22.2.0",
         "cattrs==22.2.0",
         "orjson==3.8.5",
         "tomli==2.0.1",
     ],
     license="GPL-3.0 License",
     long_description_content_type="text/markdown",
```

