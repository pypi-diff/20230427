# Comparing `tmp/dbxconfig-2.3.0.tar.gz` & `tmp/dbxconfig-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-2.3.0.tar", last modified: Tue Apr 25 23:45:15 2023, max compression
+gzip compressed data, was "dbxconfig-2.4.0.tar", last modified: Thu Apr 27 19:37:09 2023, max compression
```

## Comparing `dbxconfig-2.3.0.tar` & `dbxconfig-2.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/
--rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3158 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      463 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1204 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3115 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3158 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      463 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2808 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1264 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5348 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      963 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3232 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/dbxconfig/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-27 19:37:09.000000 dbxconfig-2.4.0/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-27 19:37:09.584277 dbxconfig-2.4.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-04-27 19:36:19.000000 dbxconfig-2.4.0/setup.py
```

### Comparing `dbxconfig-2.3.0/PKG-INFO` & `dbxconfig-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.3.0
+Version: 2.4.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.3.0/README.md` & `dbxconfig-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.3.0/dbxconfig/_config.py` & `dbxconfig-2.4.0/dbxconfig/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,17 @@
 
     def get_table_mapping(
         self,
         timeslice: Timeslice,
         stage: StageType,
         table: str = _INDEX_WILDCARD,
         database: str = _INDEX_WILDCARD,
-        index: str = None,
     ):
         table_mapping = self.tables.get_table_mapping(
-            stage=stage, table=table, database=database, index=index
+            stage=stage, table=table, database=database
         )
 
         table_mapping.source = dataset_factory.get_data_set(
             self.config, table_mapping.source, timeslice
         )
         table_mapping.destination = dataset_factory.get_data_set(
             self.config, table_mapping.destination, timeslice
```

### Comparing `dbxconfig-2.3.0/dbxconfig/_table.py` & `dbxconfig-2.4.0/dbxconfig/_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 
 class Table(BaseTable):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     depends_on: List[str] = Field(default=[])
-    table_properties: Dict[str, str] = Field(default=None)
+    delta_properties: Dict[str, str] = Field(default=None)
+    custom_properties: Dict[str, Any] = Field(default=None)
     warning_thresholds: ValidationThreshold = Field(default=None)
     exception_thresholds: ValidationThreshold = Field(default=None)
 
 
 class TableMapping(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
```

### Comparing `dbxconfig-2.3.0/dbxconfig/_tables.py` & `dbxconfig-2.4.0/dbxconfig/_tables.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel, Field
-from typing import Union, Any, Dict
+from typing import Union, Any, Dict, List
 from ._stage_type import StageType
 import fnmatch
 from ._table import Table, TableMapping
 
 
 _INDEX_WILDCARD = "*"
 
@@ -11,90 +11,144 @@
 class Tables(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._load_index()
 
     table_data: dict = Field(...)
     tables_index: Dict[str, Table] = Field(default={})
-    table_properties: Dict[str, str] = Field(default=None)
+    delta_properties: Dict[str, str] = Field(default=None)
     config_path: str = Field(...)
 
     @classmethod
     def get_index(
         cls,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
-        table=_INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
+        table=_INDEX_WILDCARD,
+    ):
+        if isinstance(stage, StageType):
+            return f"{stage.name}.{database}.{table}"
+        else:
+            return f"{stage}.{database}.{table}"
+
+    @classmethod
+    def parse_index(
+        cls,
+        index: str,
     ):
-        return f"{stage.name}.{database}.{table}"
+        try:
+            parts = index.split(".")
+            stage = StageType[parts[0]]
+            database = parts[1]
+            table = parts[2]
+        except Exception as e:
+            raise Exception(
+                f"attempted to parse an invalid index {index}. It must be of the form 'stage.database.table'"
+            ) from e
+
+        return stage, database, table
 
     def _load_index(self):
         for stage in StageType:
             stage_data = self.table_data.get(stage.name)
             if stage_data:
-                stage_table_properties = stage_data.get("table_properties", {})
+                stage_delta_properties = stage_data.get("delta_properties", {})
 
                 for database, tables in stage_data.items():
-                    if database == "table_properties":
+                    if database == "delta_properties":
                         continue
 
                     for table, table_details in tables.items():
                         # flatten the config structure for a table
                         if not table_details:
                             table_details = {}
-                        table_properties = table_details.get("table_properties", {})
-                        # table_properties = stage_table_properties | table_properties
-                        table_properties = {
-                            **stage_table_properties,
-                            **table_properties,
+                        delta_properties = table_details.get("delta_properties", {})
+                        # delta_properties = stage_delta_properties | delta_properties
+                        delta_properties = {
+                            **stage_delta_properties,
+                            **delta_properties,
                         }
                         table_details["name"] = table
                         table_details["database"] = database
                         table_details["stage"] = stage
-                        if table_properties:
-                            table_details["table_properties"] = table_properties
+                        if delta_properties:
+                            table_details["delta_properties"] = delta_properties
 
                         # create a table object
                         table = Table(**table_details)
 
                         # index the table object
                         index = f"{stage.name}.{database}.{table.name}"
                         self.tables_index[index] = table
 
-    def lookup_table(self, index: str, first_match: bool = True):
+    def lookup_table(
+        self,
+        stage: Union[StageType, str] = _INDEX_WILDCARD,
+        database=_INDEX_WILDCARD,
+        table=_INDEX_WILDCARD,
+        first_match: bool = True,
+        **kwargs,
+    ):
+        index = Tables.get_index(stage, database, table)
         matches = fnmatch.filter(list(self.tables_index.keys()), index)
 
         if not matches:
             raise Exception(f"index {index} not found in tables_index")
 
+        def match_property(
+            table: Table, properties: Dict[str, Any], matches: List[str]
+        ):
+            for p, v in properties.items():
+                if (
+                    isinstance(table.custom_properties, dict)
+                    and table.custom_properties.get(p) == v
+                ):
+                    return True
+                else:
+                    index = Tables.get_index(table.stage, table.database, table.name)
+                    if index in matches:
+                        matches.remove(
+                            Tables.get_index(table.stage, table.database, table.name)
+                        )
+                    return False
+
+        tables_index = dict(self.tables_index)
+        if kwargs:
+            tables_index = {
+                k: v
+                for k, v in self.tables_index.items()
+                if match_property(v, kwargs, matches)
+            }
+
         if first_match:
             matches = matches[0]
-            table = self.tables_index[matches]
+            table = tables_index[matches]
             return table
         else:
-            tables = [self.tables_index[i] for i in matches]
+            tables = [tables_index[i] for i in matches]
             return tables
 
     def get_table_mapping(
-        self,
-        stage: StageType,
-        table=_INDEX_WILDCARD,
-        database=_INDEX_WILDCARD,
-        index: str = None,
+        self, stage: StageType, table=_INDEX_WILDCARD, database=_INDEX_WILDCARD
     ):
-        if not index:
-            index = Tables.get_index(stage, table, database)
-
-        destination = self.lookup_table(index=index, first_match=True)
+        destination = self.lookup_table(
+            stage=stage, database=database, table=table, first_match=True
+        )
         source = {}
 
         try:
             for index in destination.depends_on:
-                table = self.lookup_table(index=index, first_match=True)
+                do_stage, do_database, do_table = Tables.parse_index(index)
+                table = self.lookup_table(
+                    stage=do_stage,
+                    table=do_table,
+                    database=do_database,
+                    first_match=True,
+                )
                 source[table.name] = table
         except Exception as e:
-            raise Exception("Error looking up dependencies for table {}") from e
+            raise Exception(f"Error looking up dependencies for table {table}") from e
 
         if len(list(source.values())) == 1:
             source = list(source.values())[0]
 
         return TableMapping(source=source, destination=destination)
```

### Comparing `dbxconfig-2.3.0/dbxconfig/_timeslice.py` & `dbxconfig-2.4.0/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.3.0/dbxconfig/_utils.py` & `dbxconfig-2.4.0/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.3.0/dbxconfig/dataset/_dataset.py` & `dbxconfig-2.4.0/dbxconfig/dataset/_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,10 +20,11 @@
     root: str = Field(...)
     path: str = Field(default=None)
     options: dict = Field(...)
     timeslice: Timeslice = Field(...)
     checkpoint: str = Field(default=None)
     stage: StageType = Field(...)
     config_path: str = Field(...)
+    custom_properties: Dict[str, Any] = Field(default=None)
 
     def _render(self):
         pass
```

### Comparing `dbxconfig-2.3.0/dbxconfig/dataset/_deltalake.py` & `dbxconfig-2.4.0/dbxconfig/dataset/_deltalake.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     root: str = Field(...)
     path: str = Field(...)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     checkpoint: str = Field(default=None)
     checkpoint_location: str = Field(default=None)
-    table_properties: Dict[str, str] = Field(default=None)
+    delta_properties: Dict[str, str] = Field(default=None)
     stage: StageType = Field(...)
     warning_thresholds: ValidationThreshold = Field(default=None)
     exception_thresholds: ValidationThreshold = Field(default=None)
 
     def _render(self):
         self._replacements = {
             JinjaVariables.TABLE: self.destination_table,
@@ -64,17 +64,17 @@
     def create_table(self):
         table_ddl = f"""
             CREATE TABLE IF NOT EXISTS `{self.database}`.`{self.table}`
             USING DELTA
             LOCATION '{self.location}'
         """
         # add in the delta properties if there are any
-        if self.table_properties:
+        if self.delta_properties:
             tbl_properties = [
-                f"{k.lower()} = {v.lower()}" for k, v in self.table_properties.items()
+                f"{k.lower()} = {v.lower()}" for k, v in self.delta_properties.items()
             ]
             tbl_properties = ", ".join(tbl_properties)
             table_ddl = f"""{table_ddl}
             TBLPROPERTIES({tbl_properties})
             """
         try:
             spark.sql(f"CREATE DATABASE IF NOT EXISTS `{self.database}`")  # noqa F821
```

### Comparing `dbxconfig-2.3.0/dbxconfig/dataset/_factory.py` & `dbxconfig-2.4.0/dbxconfig/dataset/_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     DELTALAKE = "deltalake"
     WRITE = "write"
 
 
 class _DatasetFactory:
     _TIMESLICE = "timeslice"
     _TABLE = "destination_table"
-    _TABLE_PROPERTIES = "table_properties"
+    _DELTA_PROPERTIES = "delta_properties"
+    _CUSTOM_PROPERTIES = "custom_properties"
     _STAGE = "stage"
     _DATABASE = "database"
     _CONFIG_PATH = "config_path"
     _WARNING_THRESHOLDS = "warning_thresholds"
     _EXCEPTION_THRESHOLDS = "exception_thresholds"
 
     def __init__(self) -> None:
@@ -70,15 +71,16 @@
 
         return dataset
 
     def _get_stage_table_config(self, config: dict, table: Table, timeslice: Timeslice):
         stage_config = config[table.stage.name]
         stage_config[self._TIMESLICE] = timeslice
         stage_config[self._TABLE] = table.name
-        stage_config[self._TABLE_PROPERTIES] = table.table_properties
+        stage_config[self._DELTA_PROPERTIES] = table.delta_properties
+        stage_config[self._CUSTOM_PROPERTIES] = table.custom_properties
         stage_config[self._STAGE] = table.stage
         stage_config[self._DATABASE] = table.database
         stage_config[self._CONFIG_PATH] = config[self._CONFIG_PATH]
         if table.warning_thresholds:
             stage_config[self._WARNING_THRESHOLDS] = table.warning_thresholds
         if table.exception_thresholds:
             stage_config[self._EXCEPTION_THRESHOLDS] = table.exception_thresholds
```

### Comparing `dbxconfig-2.3.0/dbxconfig/dataset/_read.py` & `dbxconfig-2.4.0/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.3.0/dbxconfig/workflow/_multi_threaded.py` & `dbxconfig-2.4.0/dbxconfig/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.3.0/dbxconfig/workflow/_notebook.py` & `dbxconfig-2.4.0/dbxconfig/workflow/_notebook.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.3.0/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-2.4.0/dbxconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.3.0
+Version: 2.4.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.3.0/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-2.4.0/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.3.0/setup.py` & `dbxconfig-2.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="2.3.0",
+    version="2.4.0",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

