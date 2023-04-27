# Comparing `tmp/cognite_gql_pygen-0.3.0.tar.gz` & `tmp/cognite_gql_pygen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.3.0.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.4.0.tar", max compression
```

## Comparing `cognite_gql_pygen-0.3.0.tar` & `cognite_gql_pygen-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,32 @@
--rw-r--r--   0        0        0    11349 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/LICENSE
--rw-r--r--   0        0        0     4050 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/README.md
--rw-r--r--   0        0        0     8928 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      238 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/bin/_functions.sh
--rwxr-xr-x   0        0        0      572 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/bin/cdf_signin.sh
--rwxr-xr-x   0        0        0      379 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/bin/schema_publish.sh
--rwxr-xr-x   0        0        0      209 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/bin/schema_render.sh
--rw-r--r--   0        0        0      167 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19055 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3909 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2629 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      346 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6257 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     3046 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    15854 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     3607 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7060 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0      868 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/main.py
--rw-r--r--   0        0        0     1423 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0     1868 2023-04-24 15:22:36.716334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/data_classes.py
--rw-r--r--   0        0        0     1560 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/generator.py
--rw-r--r--   0        0        0     2030 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0      416 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/misc.py
--rw-r--r--   0        0        0     1288 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/parser.py
--rw-r--r--   0        0        0     1333 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/templates/client.txt
--rw-r--r--   0        0        0      803 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1965 2023-04-24 15:22:36.720334 cognite_gql_pygen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5062 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4486 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/README.md
+-rw-r--r--   0        0        0     8657 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    18972 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3909 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2629 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      346 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6324 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     3046 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    16000 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     3607 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7060 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0     1423 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1868 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1560 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     7728 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      596 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1288 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1333 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      803 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-04-27 14:28:28.763462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1995 2023-04-27 14:28:28.763462 cognite_gql_pygen-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.4.0/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.3.0/LICENSE` & `cognite_gql_pygen-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/README.md` & `cognite_gql_pygen-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,26 +41,29 @@
 You can specify the data models either as a `.graphql` schema or a `pydantic` classes in a `.py` file. Then, you can
 use the CLI to automatically generate the other representation as well as the `client.py` file which creates
 the API and the convenience method get_[client_name]_client().
 
 To generate from a `.graphql` schema you use the following command.
 
 ```bash
-dm topython 'PATH_TO_SCHEMA' --name "Cine"
+dm topython 'PATH_TO_SCHEMA'
 ```
 
 This will create a `schema.py` and a `client.py` file in the directory you are running the command.
 
 To generate from `schema.py` use the following command
 
 ```bash
 dm togql 'PATH_TO_FILE'
 ```
 
-This will create the `schema.graphql` and a `client.py` file in the directory you are running the command.
+This will load the python module and create a `schema.graphql` file in the directory you are running the command.
+
+`PATH_TO_FILE` can be either a path to a `.py` file or a Python dot-notation to a package
+(e.g. `my_project.schema_module` make sure that the package in which case the module must be in Python path).
 
 Note the `schema.py` file must follow a specific structure, see [examples/cinematography_domain](https://github.com/cognitedata/cognite-gql-pygen/blob/main/examples/cinematography_domain/schema.py) for an example.
 The overall structure is as follows:
 
 1. Instantiate a new schema with the line, `myschema: Schema[DomainModel] = Schema()`
 2. Register all you Types with `@myschema.register_type`
 3. Close the schema with `myschema.close()`
@@ -70,14 +73,21 @@
 
 * `schema.graphql` The schema defined in GraphQL language.
 * `schema.py` The schema defined in `pydantic` classes.
 * `client.py` Which sets up the client for the data model.
 * `usage.py` Demonstrates the usage of the client.
 
 
+### Settings File
+
+`dm togql` and `dm topython` take their defaults form `settings.toml` if present. See
+[settings.toml](./cognite/dm_clients/settings.toml) for an example, section `[local]` is relevant for `togql` and
+`topython` commands.
+
+
 ### DM Non-GraphQl API
 
 The API developed is based on the non-GraphQL endpoints in Data Model API v3. There is a simplified wrapper which is available
 in `cognite.dm_clients`.
 
 See [dm_clients/README.md](cognite/dm_clients/README.md) for more details.__
```

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,14 @@
    like several clients in a very similar business)
  * Domain Model - a `dm_clients` term - often used interchangeably with "schema type" - a single class of objects with
    all its fields, e.g. "pump" or "generator".
  * Item - a `dm_clients` term - an instance of a Domain Model, e.g. generator "G42".
  * Instance - a DM term - a data entity, either a Node or an Edge (see below).
  * Node - a DM term - a data entity, can contain multiple fields.
  * Edge - a DM term - a data entity that connects two nodes (directionally).
- * DomainAPI - a `dm_clients` term - a top-level Python class for a Domain. It provides easy access to various
-   DomainModelAPIs (see below).
  * DomainModelAPI - a `dm_clients` term - a Python class (or class instance) which provides management over a single
    DomainModel, e.g. create new pumps, delete a pump, list all pumps...
  * DomainClient - a `dm_clients` term - a Python class (or class instance) which serves as a namespace for easy access
    to all DomainModelAPIs in a use case.
 
 
 ## Installation
@@ -111,31 +109,32 @@
   - ```
     if __name__ == "__main__":
         print(my_schema.as_str())
     ```
 
 #### Upload the schema
 
-> Before proceeding, make sure that `config.yaml` is populated with credentials and configuration.
+> Before proceeding, make sure that `settings.toml` and / or `.secrets.toml` is populated with credentials and
+> configuration.
 
 
 ##### Step 1: Render Schema
 
 GraphQL schema file is committed to this repo, so this step is not required, but it is here for completeness.
 
-Execute `dm_clients schema render`. This will update the schema file (defined in `config.yaml`) according to Python code in
+Execute `dm togql`. This will update the schema file (defined in `settings.toml`) according to Python code in
 the schema module.
 
 
 ##### Step 2: Upload Schema
 
-Authenticate against CDF by running `dm_clients signin`. The authentication data is cached on the filesystem
+Authenticate against CDF by running `dm signin`. The authentication data is cached on the filesystem
 locally, so this is needed rarely (every few? days).
 
-Execute `dm_clients schema publish`. This will upload the schema to CDF / DM.
+Execute `dm upload`. This will upload the schema to CDF / DM.
 
 > Note: Depending on the changes made to the schema, you might be required to update the schema version in config.yaml.
 > This happens when the changes are not backwards-compatible, e.g. deleting a field.
 
 
 ### Manipulate Items
 
@@ -184,21 +183,17 @@
  * Unpolished, possibly with some bugs.
    * External IDs are constructed, not safely considering the char limit.
    * ...
 
 
 ### TODO
 
- * Missing support for custom scalar types (`JSON` and `Timestamp`, others in the future)
-    * priority, in progres
- * Better alternative to `config.yaml`.
  * Add support for retrieving items via graphql endpoint.
  * Expand unit test coverage
- * Enable use on Windows (currently Bash scripts make this complicated, see
-   [Issue 9](https://github.com/cognitedata/cognite-gql-pygen/issues/9)).
+ * Test use on Windows, particularly `dm signin` and `dm upload`
  * Lots of TODOs in the code
 
 
 ## Example: Cinematography Domain
 
 Contained in `examples/cinematography_domain`, this is a minimal toy example of the basic features of this package.
 `schema.py` shows implementation of a schema (a.k.a. data model), and `client.py` shows how to manipulate items
@@ -215,9 +210,11 @@
 
 Important modules:
  * `cognite/dm_clients/cdf`
     * general-purpose DM client (nothing specific to PowerOps in here)
     * inspired by https://github.com/cognitedata/tech-demo-powerops/ :]
  * `cognite/dm_clients/domain_modeling`
     * base classes for use cases, "boilerplate"
+ * `cognite/dm_clients/custom_types`
+    * support for Cognite-specific GraphQL scalar types (e.g. JSONObject, Timeseries)
  * `examples/cinematography_domain`
     * a toy example use case with minimal code
```

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,17 +478,14 @@
         self.spaces = SpacesAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.datamodels = DataModelAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.views = ViewsAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.containers = ContainersAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.nodes = NodesAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
         self.edges = EdgesAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
 
-    def post(self, *args, **kwargs):
-        return super().post(*args, **kwargs)
-
     def graph(self, space: str, datamodel: str, version: str, query: str):
         return self.post(
             f"/api/v1/projects/{self.config.project}/userapis"
             f"/spaces/{space}/datamodels/{datamodel}/versions/{version}/graphql",
             json={"query": query},
         ).json()
```

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from threading import Lock
 from typing import TYPE_CHECKING, Dict, Generic, Iterable, List, Optional, Type, TypeVar
 
 from cachelib import BaseCache
 from cognite.client import ClientConfig
 
 from cognite.dm_clients.cdf.client_dm_v3 import CogniteClientDmV3, EdgesAPI, NodesAPI
 from cognite.dm_clients.config import settings
@@ -42,14 +43,15 @@
         schema_version: Optional[int] = None,
         # TODO ^ some of these args are redundant.
     ):
         # TODO make all these attributes "_private" to distinguish from domain model APIs
         self.schema = schema
         self._domain_model_api_class = domain_model_api_class
         self.cache: BaseCache = cache
+        self._cache_lock: Lock = Lock()
         self._client = CogniteClientDmV3(config)
         self._client._config.headers["cdf-version"] = "alpha"
         if space_id is None:
             space_id = settings.dm_clients.space
         self.space_id = space_id
         self._data_model = data_model or settings.dm_clients.get("datamodel")
         self.schema_version = schema_version or settings.dm_clients.get("schema_version")
```

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
           4. Create edges for those one-to-many relationships.
         """
         items = self._prepare_items(items, ext_id_prefix)
 
         if not items:
             return []
 
-        self.domain_client.cache.delete_many(*[item.externalId for item in items if item.externalId])
+        with self.domain_client._cache_lock:
+            self.domain_client.cache.delete_many(*[item.externalId for item in items if item.externalId])
 
         items = self._create_related_o2o_nodes(items)
         items, pending_edges = self._create_related_o2m_items(items)
 
         def _strip_items(item_data: dict) -> dict:
             return {key: val for key, val in item_data.items() if val is not None}
 
@@ -211,16 +212,16 @@
     def _cache_created_items(self, items: Iterable[DomainModelT]) -> None:
         """
         This caching is not just for performance! It also helps with CDF's "eventual consistency" promise.
         Without this cache, what happens is that we create a node (i.e. a DomainModel instance) and if we want to
         retrieve that same instance very soon, it often just isn't present in the response. After some time (seconds,
         sometimes minutes?) the new node appears in CDF.
         """
-
-        self.domain_client.cache.set_many({item.externalId: item for item in items if item.externalId})
+        with self.domain_client._cache_lock:
+            self.domain_client.cache.set_many({item.externalId: item for item in items if item.externalId})
 
     def _get_from_cache(self, external_ids: Iterable[str]) -> Tuple[List[DomainModelT], List[str]]:
         cached_items: List[DomainModelT] = []
         uncached_external_ids: List[str] = []
         for external_id in external_ids:
             cached_instance: DomainModelT = self.domain_client.cache.get(external_id)
             if cached_instance is not None:
@@ -263,15 +264,16 @@
                 subitems: List[DomainModel] = []
                 for item in items:
                     subitems.extend(subitem for subitem in getattr(item, attr, []) if subitem is not None)
                 self.domain_client.delete(subitems, delete_related_items=True)
 
         external_ids = list({item.externalId for item in items if item.externalId})
         self.nodes_api.delete(self.space_id, external_ids)
-        self.domain_client.cache.delete_many(*external_ids)
+        with self.domain_client._cache_lock:
+            self.domain_client.cache.delete_many(*external_ids)
 
     def _retrieve_full(self, nodes: Iterable[Node]) -> List[DomainModelT]:
         """
         For every node, make a fully DomainModel item, including all nested (related) objects.
         """
         full_items: Dict[str, DomainModelT]
         uncached_nodes: List[Node]
```

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.4.0/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/gqlpygen/data_classes.py` & `cognite_gql_pygen-0.4.0/cognite/gqlpygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/gqlpygen/generator.py` & `cognite_gql_pygen-0.4.0/cognite/gqlpygen/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/gqlpygen/parser.py` & `cognite_gql_pygen-0.4.0/cognite/gqlpygen/parser.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/gqlpygen/templates/client.txt` & `cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/cognite/gqlpygen/templates/schema.txt` & `cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.3.0/pyproject.toml` & `cognite_gql_pygen-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.3.0"
+version = "0.4.0"
 description = "Cognite graphQL Python generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
 
@@ -39,14 +39,15 @@
 docopt = "^0.6.2"
 cachelib = "^0.10.2"
 retry = "^0.9.2"
 loguru = "^0.6.0"
 dynaconf = "^3.1.12"
 graphql-core = ">=3.2"
 Jinja2 = ">=3.1"
+packaging = "^23.1"
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pre-commit = "*"
 toml = "*"
 python-dotenv = "*"
 pytest = "*"
@@ -76,9 +77,9 @@
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [build-system]
-requires = ["poetry>=1.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.3"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `cognite_gql_pygen-0.3.0/PKG-INFO` & `cognite_gql_pygen-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Cognite graphQL Python generation SDK
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,15 @@
 Requires-Dist: cognite-sdk[pandas] (>=5.9.0,<6.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: graphql-core (>=3.2)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: msal (>=1.16.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
+Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pydantic (>=1.10)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: strawberry-graphql (>=0.156.4,<0.157.0)
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 Cognite GraphQL Python Generator
@@ -69,26 +70,29 @@
 You can specify the data models either as a `.graphql` schema or a `pydantic` classes in a `.py` file. Then, you can
 use the CLI to automatically generate the other representation as well as the `client.py` file which creates
 the API and the convenience method get_[client_name]_client().
 
 To generate from a `.graphql` schema you use the following command.
 
 ```bash
-dm topython 'PATH_TO_SCHEMA' --name "Cine"
+dm topython 'PATH_TO_SCHEMA'
 ```
 
 This will create a `schema.py` and a `client.py` file in the directory you are running the command.
 
 To generate from `schema.py` use the following command
 
 ```bash
 dm togql 'PATH_TO_FILE'
 ```
 
-This will create the `schema.graphql` and a `client.py` file in the directory you are running the command.
+This will load the python module and create a `schema.graphql` file in the directory you are running the command.
+
+`PATH_TO_FILE` can be either a path to a `.py` file or a Python dot-notation to a package
+(e.g. `my_project.schema_module` make sure that the package in which case the module must be in Python path).
 
 Note the `schema.py` file must follow a specific structure, see [examples/cinematography_domain](https://github.com/cognitedata/cognite-gql-pygen/blob/main/examples/cinematography_domain/schema.py) for an example.
 The overall structure is as follows:
 
 1. Instantiate a new schema with the line, `myschema: Schema[DomainModel] = Schema()`
 2. Register all you Types with `@myschema.register_type`
 3. Close the schema with `myschema.close()`
@@ -98,14 +102,21 @@
 
 * `schema.graphql` The schema defined in GraphQL language.
 * `schema.py` The schema defined in `pydantic` classes.
 * `client.py` Which sets up the client for the data model.
 * `usage.py` Demonstrates the usage of the client.
 
 
+### Settings File
+
+`dm togql` and `dm topython` take their defaults form `settings.toml` if present. See
+[settings.toml](./cognite/dm_clients/settings.toml) for an example, section `[local]` is relevant for `togql` and
+`topython` commands.
+
+
 ### DM Non-GraphQl API
 
 The API developed is based on the non-GraphQL endpoints in Data Model API v3. There is a simplified wrapper which is available
 in `cognite.dm_clients`.
 
 See [dm_clients/README.md](cognite/dm_clients/README.md) for more details.__
```

