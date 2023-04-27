# Comparing `tmp/moonstream-entity-0.0.3.tar.gz` & `tmp/moonstream-entity-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstream-entity-0.0.3.tar", last modified: Thu Feb  9 20:27:45 2023, max compression
+gzip compressed data, was "moonstream-entity-0.0.4.tar", last modified: Thu Apr 27 17:42:25 2023, max compression
```

## Comparing `moonstream-entity-0.0.3.tar` & `moonstream-entity-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 20:27:45.701098 moonstream-entity-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-02-09 20:27:45.701098 moonstream-entity-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 20:27:45.701098 moonstream-entity-0.0.3/entity/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9659 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/entity/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     7987 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/entity/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/entity/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/entity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/entity/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/entity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 20:27:45.701098 moonstream-entity-0.0.3/moonstream_entity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-02-09 20:27:45.000000 moonstream-entity-0.0.3/moonstream_entity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-02-09 20:27:45.000000 moonstream-entity-0.0.3/moonstream_entity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-09 20:27:45.000000 moonstream-entity-0.0.3/moonstream_entity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-09 20:27:45.000000 moonstream-entity-0.0.3/moonstream_entity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-09 20:27:45.000000 moonstream-entity-0.0.3/moonstream_entity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-09 20:27:45.000000 moonstream-entity-0.0.3/moonstream_entity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-09 20:27:45.701098 moonstream-entity-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-02-09 20:27:37.000000 moonstream-entity-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/entity/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9659 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/entity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/moonstream_entity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-27 17:42:25.000000 moonstream-entity-0.0.4/moonstream_entity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 17:42:25.052857 moonstream-entity-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-27 17:42:12.000000 moonstream-entity-0.0.4/setup.py
```

### Comparing `moonstream-entity-0.0.3/PKG-INFO` & `moonstream-entity-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstream-entity
-Version: 0.0.3
+Version: 0.0.4
 Summary: Moonstream entity API client library
 Home-page: https://github.com/bugout-dev/entity
 Author: Moonstream
 Author-email: engineering@moonstream.to
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `moonstream-entity-0.0.3/README.md` & `moonstream-entity-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `moonstream-entity-0.0.3/entity/cli.py` & `moonstream-entity-0.0.4/entity/cli.py`

 * *Files identical despite different names*

### Comparing `moonstream-entity-0.0.3/entity/client.py` & `moonstream-entity-0.0.4/entity/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import uuid
-from typing import Any, Dict, List, Union
-
-import requests
+from typing import Any, Dict, List, Union, Optional
+import requests  # type: ignore
 
 from . import data, exceptions
 from .settings import ENTITY_API_URL, ENTITY_REQUEST_TIMEOUT
 
 ENDPOINT_PING = "/ping"
 ENDPOINT_VERSION = "/version"
 ENDPOINT_NOW = "/now"
@@ -154,15 +153,15 @@
             "Authorization": f"{auth_type.value} {token}",
         }
         payload = {
             "address": address,
             "blockchain": blockchain,
             "name": name,
             "required_fields": required_fields,
-            "secondary_fields": secondary_fields,
+            **secondary_fields,
         }
         result = self._call(
             method=data.Method.POST,
             url=f"{self.api.endpoints[ENDPOINT_COLLECTIONS]}/{str(collection_id)}/entities",
             headers=headers,
             json=payload,
             timeout=timeout,
@@ -224,14 +223,47 @@
             method=data.Method.GET,
             url=f"{self.api.endpoints[ENDPOINT_COLLECTIONS]}/{str(collection_id)}/entities",
             headers=headers,
             timeout=timeout,
         )
         return data.EntitiesResponse(**result)
 
+    def update_entity(
+        self,
+        token: Union[str, uuid.UUID],
+        collection_id: Union[str, uuid.UUID],
+        entity_id: Union[str, uuid.UUID],
+        address: str,
+        blockchain: str,
+        name: str,
+        required_fields: List[Dict[str, Union[str, bool, int, list]]] = [],
+        secondary_fields: Dict[str, Any] = {},
+        auth_type: data.AuthType = data.AuthType.bearer,
+        timeout: float = ENTITY_REQUEST_TIMEOUT,
+    ) -> data.EntityResponse:
+        headers = {
+            "Authorization": f"{auth_type.value} {token}",
+        }
+        payload = {
+            "address": address,
+            "blockchain": blockchain,
+            "name": name,
+            "required_fields": required_fields,
+            **secondary_fields,
+        }
+        result = self._call(
+            method=data.Method.PUT,
+            url=f"{self.api.endpoints[ENDPOINT_COLLECTIONS]}/{str(collection_id)}/entities/{str(entity_id)}",
+            headers=headers,
+            json=payload,
+            timeout=timeout,
+        )
+
+        return data.EntityResponse(**result)
+
     def delete_entity(
         self,
         token: Union[str, uuid.UUID],
         collection_id: Union[str, uuid.UUID],
         entity_id: Union[str, uuid.UUID],
         auth_type: data.AuthType = data.AuthType.bearer,
         timeout: float = ENTITY_REQUEST_TIMEOUT,
@@ -243,7 +275,44 @@
             method=data.Method.DELETE,
             url=f"{self.api.endpoints[ENDPOINT_COLLECTIONS]}/{str(collection_id)}/entities/{str(entity_id)}",
             headers=headers,
             timeout=timeout,
         )
 
         return data.EntityResponse(**result)
+
+    def search_entities(
+        self,
+        token: Union[str, uuid.UUID],
+        collection_id: Union[str, uuid.UUID],
+        required_field: List[str] = [],
+        secondary_field: List[str] = [],
+        filters: Optional[List[str]] = None,
+        limit: int = 10,
+        offset: int = 0,
+        content: bool = True,
+        timeout: float = ENTITY_REQUEST_TIMEOUT,
+    ) -> data.EntitySearchResponse:
+
+        headers = {
+            "Authorization": f"{data.AuthType.bearer.value} {token}",
+        }
+
+        params = {
+            "required_field": required_field,
+            "secondary_field": secondary_field,
+            "limit": limit,
+            "offset": offset,
+            "content": content,
+        }
+
+        if filters:
+            params["filters"] = filters
+
+        result = self._call(
+            method=data.Method.GET,
+            url=f"{self.api.endpoints[ENDPOINT_COLLECTIONS]}/{str(collection_id)}{ENDPOINT_SEARCH}",
+            headers=headers,
+            timeout=timeout,
+        )
+
+        return data.EntitySearchResponse(**result)
```

### Comparing `moonstream-entity-0.0.3/entity/data.py` & `moonstream-entity-0.0.4/entity/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,7 +89,15 @@
 
     created_at: Optional[str] = None
     updated_at: Optional[str] = None
 
 
 class EntitiesResponse(BaseModel):
     entities: List[EntityResponse] = Field(default_factory=list)
+
+
+class EntitySearchResponse(BaseModel):
+    total_results: int
+    offset: int
+    next_offset: Optional[int] = None
+    max_score: float
+    entities: List[EntityResponse] = Field(default_factory=list)
```

### Comparing `moonstream-entity-0.0.3/moonstream_entity.egg-info/PKG-INFO` & `moonstream-entity-0.0.4/moonstream_entity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstream-entity
-Version: 0.0.3
+Version: 0.0.4
 Summary: Moonstream entity API client library
 Home-page: https://github.com/bugout-dev/entity
 Author: Moonstream
 Author-email: engineering@moonstream.to
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `moonstream-entity-0.0.3/setup.py` & `moonstream-entity-0.0.4/setup.py`

 * *Files identical despite different names*

