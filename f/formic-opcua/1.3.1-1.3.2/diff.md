# Comparing `tmp/formic_opcua-1.3.1.tar.gz` & `tmp/formic_opcua-1.3.2.tar.gz`

## Comparing `formic_opcua-1.3.1.tar` & `formic_opcua-1.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/core/parse.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.2/PKG-INFO
```

### Comparing `formic_opcua-1.3.1/.pre-commit-config.yaml` & `formic_opcua-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/examples/opcua_client.py` & `formic_opcua-1.3.2/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.3.2/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.3.2/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.3.2/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.3.2/formic_opcua/client/opcua_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # Copyright Formic Technologies 2023
-import asyncio
 import logging
 import warnings
+from asyncio.exceptions import TimeoutError
 from datetime import datetime
 from typing import Any, Dict, List, Tuple
 
-from asyncua import Client, Node
+from asyncua import Node
+from asyncua.sync import Client, ThreadLoopNotRunning
 from asyncua.ua import NodeClass
 from asyncua.ua.uatypes import DataValue, DateTime, Variant
 
 from formic_opcua.core import InvalidClientArgsError, convert_type, parse_settings
 
 logger = logging.getLogger(__name__)
 warnings.simplefilter('error')
 
 
-class AsyncOpcuaClient:
+class OpcuaClient:
     def __init__(
-        self,
-        server_config_file: str = None,
-        connect_timeout: float = 0.25,
-        url: str = None,
-        uri: str = None,
+        self, server_config_file: str = None, url: str = None, uri: str = None, connect_timeout: float = 0.25
     ) -> None:
         if server_config_file is None and (url is None and uri is None):
             error_message = 'No configuration arguments passed to client.'
             logger.critical(error_message)
             raise InvalidClientArgsError(error_message)
 
         if server_config_file is not None and (url is not None or uri is not None):
@@ -49,220 +46,184 @@
 
         self._idx = -1
         self._node_path_list: List[str] = []
         self._client = Client(url=self._url)
         self.connect_timeout = connect_timeout
         self._has_connected = False
         self._node_map: Dict[str, Tuple] = {}
+        self._identifier_map: Dict[str, List[str]] = {}
 
         logger.info(f'Client created with url: {self._url}, and uri: {self._uri}')
 
-    async def __aenter__(self):
-        await self._connect()
-        await self._establish_server_structure()
+    def __enter__(self):
+        self._connect()
+        self._establish_server_structure()
         return self
 
-    async def __aexit__(self, *args) -> None:
-        await self._disconnect()
+    def __exit__(self, *args) -> None:
+        self._disconnect()
 
-    async def _connect(self):
+    def _connect(self):
         try:
-            if await self._test_server_connection():
+            if self._test_server_connection():
                 logger.info('_connect called but there is a connection to the server.')
                 self._has_connected = True
                 return
-            if await self._disconnect():
+            if self._disconnect():
                 self._client = Client(url=self._url, timeout=self.connect_timeout)
             logger.info('Connecting...')
-            await self._client.connect()
+            self._client.connect()
             logger.info('Connected...')
             self._has_connected = True
         except (ConnectionRefusedError, ConnectionError, RuntimeError, RuntimeWarning, TimeoutError):
             logger.error(
                 f'Unable to connect to server. Client expects server to have url: {self._url} and uri: {self._uri}. '
                 f'Server is not running or the configs are not matched with client.'
             )
             self._has_connected = False
-        except Exception as e:
-            logger.error(
-                'Unhandled exception while to connecting to server. '
-                f'Client expects server to have url: {self._url} and uri: {self._uri}. '
-                f'{e}'
-            )
-            self._has_connected = False
 
-    async def _disconnect(self) -> bool:
+    def _disconnect(self) -> bool:
         logger.info('Cleaning up client.')
         try:
-            await self._client.disconnect()
+            self._client.disconnect()
             return True
-        except (RuntimeError, ConnectionError):
+        except (RuntimeError, ConnectionError, ThreadLoopNotRunning):
             logger.warning('Tried to disconnect but there is no connection.')
             return False
-        except Exception as e:
-            logger.error(f'Unhandled exception while to disconnecting from server. {e} ')
-            return False
-
-    async def _dfs_mapper(self, node: Node, path: str) -> None:
-        browse_path = await node.read_browse_name()
 
-        if browse_path.NamespaceIndex != self._idx and browse_path.NamespaceIndex != 0:
-            return
-
-        node_class = await node.read_node_class()
+    def _dfs_mapper(self, node: Node, path: str):
+        # if node.read_node_class() == NodeClass.Variable and node.NamespaceIndex == self._idx:
+        browse_path = node.read_browse_name()
+        node_class = node.read_node_class()
         path_to_node = path + '/' + browse_path.Name
-
-        # if node_class == NodeClass.Variable and browse_path.NamespaceIndex == self._idx:
-        if node_class == NodeClass.Variable:
+        if node_class == NodeClass.Variable and browse_path.NamespaceIndex == self._idx:
             # Remove "/Objects/" since this client is intended for reading only custom nodes
-            if path_to_node.startswith('/Objects/'):
-                path_to_node = path_to_node[9:]
-            var_type = await node.read_data_type_as_variant_type()
+            path_to_node = path_to_node[9:]
+            var_type = node.read_data_type_as_variant_type()
             logger.info(f'Found OPCUA variable {path_to_node}, of variant type {var_type}')
-            if not path_to_node.startswith('/'):
-                self._node_map['/' + path_to_node] = (node, var_type)
-            else:
-                self._node_map[path_to_node] = (node, var_type)
-            return
-
-        child_node_list = []
-        node_children = await node.get_children()
+            self._node_map[path_to_node] = (node, var_type)
 
-        for child_node in node_children:
-            child_node_list.append(self._dfs_mapper(child_node, path_to_node))
+        for child_node in node.get_children():
+            self._dfs_mapper(child_node, path_to_node)
 
-        await asyncio.gather(*child_node_list)
-        return
-
-    async def _establish_server_structure(self) -> None:
+    def _establish_server_structure(self) -> None:
         try:
             logger.info(f'Mapping namespace using {self._url} and {self._uri}')
-            self._idx = await self._client.get_namespace_index(self._uri)
+            self._idx = self._client.get_namespace_index(self._uri)
             logger.info(f'Namespace index = {self._idx}')
-            root_object_node = await self._client.nodes.root.get_child(['0:Objects'])
-            await self._dfs_mapper(node=root_object_node, path='')
-
+            root_object_node = self._client.nodes.root.get_child(['0:Objects'])
+            self._dfs_mapper(node=root_object_node, path='')
             self._node_path_list = list(self._node_map.keys())
             logger.info(f'All nodes successfully mapped: {self._node_path_list}')
-        except (AttributeError, ConnectionError, RuntimeWarning, ValueError):
+        except (AttributeError, ConnectionError, RuntimeWarning, ValueError, ThreadLoopNotRunning):
             logger.error(f'Unable to map opcua nodes from {self._url} and {self._uri}')
-        except Exception as e:
-            logger.error(f'Unhandled exception while to mapping server structure. {e}')
 
-    async def _test_server_connection(self) -> bool:
+    def _test_server_connection(self) -> bool:
         try:
-            await self._client.get_namespace_index(self._uri)
+            self._client.get_namespace_index(self._uri)
             return True
         except Exception as e:
             logger.warning(e)
             logger.warning('Failed server connectivity test.')
             return False
 
-    async def _write_helper(self, path: str, value: Any) -> bool:
-        try:
-            var, var_type = self._node_map[path]
-        except KeyError:
-            logger.warning(f'Unable to find {path} in client map {self._node_map}')
-            return False
-        try:
-            value = convert_type(value=value, var_type=var_type)
-        except (KeyError, TypeError, Exception):
-            logger.warning(f'Unable to convert value {value} to variant type {var_type}')
-            return False
-        try:
-            current_time: DateTime = datetime.utcnow()
-            await var.write_value(
-                DataValue(
-                    Value=Variant(value, var_type),
-                    SourceTimestamp=current_time,
-                    ServerTimestamp=current_time,
+    def _write_helper(self, path: str, value: Any) -> bool:
+        if self._has_connected:
+            try:
+                var, var_type = self._node_map[path]
+            except KeyError:
+                logger.warning(f'Unable to find {path} in client map {self._node_map}')
+                return False
+            try:
+                value = convert_type(value=value, var_type=var_type)
+            except (KeyError, TypeError):
+                logger.warning(f'Unable to convert value {value} to variant type {var_type}')
+                return False
+            try:
+                current_time: DateTime = datetime.utcnow()  # type: ignore
+                var.write_value(
+                    DataValue(
+                        Value=Variant(value, var_type),
+                        SourceTimestamp=current_time,
+                        ServerTimestamp=current_time,
+                    )
                 )
-            )
-            logger.info(f'Wrote value {value} of type {var_type} to {path}')
-            return True
-        except ConnectionError as e:
-            logger.warning(f'{e}')
-            logger.warning(f'Unable to write value {value} of type {var_type} to {path}')
+                logger.info(f'Wrote value {value} of type {var_type} to {path}')
+                return True
+            except (ConnectionError, ThreadLoopNotRunning) as e:
+                logger.warning(f'{e}')
+                logger.warning(f'Unable to write value {value} of type {var_type} to {path}')
+        else:
+            logger.warning(f'No connection has been made to server. Cannot write value {value} to path {path}')
         return False
 
-    async def write(self, path: str, value: Any) -> bool:
+    def write(self, path: str, value: Any) -> bool:
         logger.info(f'Attempting to write value {value} to path {path}.')
         if not self._has_connected:  # Write attempt has failed or client never connected.
             logger.info('Client has not connected to server. Attempting to connect.')
-            await self.__aenter__()
-        if await self._write_helper(path=path, value=value):
+            self.__enter__()
+        if self._write_helper(path=path, value=value):
             logger.info('Write attempt succeeded')
             return True
         else:
             logger.warning('Write attempt failed')
             self._has_connected = False
 
         return False
 
-    async def _read_helper(self, path: str) -> Any:
-        try:
-            node = self._node_map[path][0]
-        except (KeyError, IndexError):
-            logger.warning(f'Unable to get node {path} from client map {self._node_map}')
-            return None
-        try:
-            value = await node.read_value()
-            logger.info(f'Read value {value} from path {path}')
-            return value
-        except Exception as e:
-            logger.warning(f'{e}')
-            logger.warning(f'Unable to read node at {path}')
+    def _read_helper(self, path: str) -> Any:
+        if self._has_connected:
+            try:
+                node = self._node_map[path][0]
+            except (KeyError, IndexError):
+                logger.warning(f'Unable to get node {path} from client map {self._node_map}')
+                return None
+            try:
+                value = node.read_value()
+                logger.info(f'Read value {value} from path {path}')
+                return value
+            except (ConnectionError, ThreadLoopNotRunning) as e:
+                logger.warning(f'{e}')
+                logger.warning(f'Unable to read node at {path}')
+        else:
+            logger.warning(f'No connection has been made to server. Cannot read node at path {path}')
         return None
 
-    async def read(self, path: str) -> Any:
+    def read(self, path: str) -> Any:
         logger.info(f'Attempting to read path {path}.')
         if not self._has_connected:  # Read attempt has failed or client never connected.
             logger.info('Client has not connected to server. Attempting to connect.')
-            await self.__aenter__()
-        value = await self._read_helper(path=path)
+            self.__enter__()
+        value = self._read_helper(path=path)
         if value is not None:
             logger.info('Read attempt succeeded')
             logger.info(f'Value: {value}')
             return value
         else:
             logger.warning('Read attempt failed')
             self._has_connected = False
         return None
 
-    async def read_all(self) -> Dict[str, Any]:
+    def read_all(self) -> Dict[str, Any]:
         logger.info(f'Attempting to read all variables on server at uri: {self._uri} and url: {self._url}.')
         results = {}
-        future_results = {}
-
         if not self._has_connected:  # Client has never successfully connected to the server
             logger.info('Client may not be connected to server. Attempting to connect.')
-            await self.__aenter__()  # Creates a new client object and adjusts self._has_connected() appropriately
-
+            self.__enter__()  # Creates a new client object and adjusts self._has_connected() appropriately
         if self._has_connected:  # In case self.__enter__() changed value to true by establishing a connection
             for path in self._node_path_list:
-                task_value = asyncio.create_task(self._read_helper(path))
-                # print(f'{path}: {value}')
-                future_results[path] = task_value
-
-        if len(self._node_path_list) == 0:
-            # There may never have been a connection
+                value = self._read_helper(path)
+                if value is not None:
+                    logger.info(f'Successfully read value: {value} for path: {path}')
+                    results[path] = value
+                else:
+                    # This could happens if there is a disconnect during reading
+                    logger.warning(f'Unsuccessful read attempt for path {path}')
+                    self._has_connected = False
+                    break
+
+        if len(self._node_path_list) == 0 or len(results) != len(self._node_path_list):
+            # Either there was never a connection or there was a disconnect
+            # while reading and only some results were read
             self._has_connected = False
-
-        await asyncio.gather(*future_results.values())
-
-        for path, task in future_results.items():
-            task_value = task.result()
-
-            if task_value is not None:
-                logger.info(f'Successfully read value: {task_value} for path: {path}')
-            else:
-                # This could happens if there is a disconnect during reading
-                logger.warning(f'Unsuccessful read attempt for path {path}')
-                self._has_connected = False
-            results[path] = task_value
-
         logger.info(f'{results}')
         return results
-
-    def identifier_from_string(self, path: str) -> List[str]:
-        identifier = [f'{self._idx}:{path_part}' for path_part in path.split('/')]
-        return ['0:Objects'] + identifier
```

### Comparing `formic_opcua-1.3.1/formic_opcua/client/opcua_client.py` & `formic_opcua-1.3.2/formic_opcua/client/async_opcua_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 # Copyright Formic Technologies 2023
+import asyncio
+from enum import Enum
 import logging
 import warnings
-from asyncio.exceptions import TimeoutError
 from datetime import datetime
 from typing import Any, Dict, List, Tuple
 
-from asyncua import Node
-from asyncua.sync import Client, ThreadLoopNotRunning
+from asyncua import Client, Node
 from asyncua.ua import NodeClass
 from asyncua.ua.uatypes import DataValue, DateTime, Variant
 
 from formic_opcua.core import InvalidClientArgsError, convert_type, parse_settings
 
 logger = logging.getLogger(__name__)
 warnings.simplefilter('error')
 
+class ConnectionStatus(Enum):
+    CONNECTED = 0
+    CONNECTING = 1
+    DISCONNECTED = 2
 
-class OpcuaClient:
+
+class AsyncOpcuaClient:
     def __init__(
-        self, server_config_file: str = None, url: str = None, uri: str = None, connect_timeout: float = 0.25
+        self,
+        server_config_file: str = None,
+        connect_timeout: float = 0.5,
+        url: str = None,
+        uri: str = None,
     ) -> None:
         if server_config_file is None and (url is None and uri is None):
             error_message = 'No configuration arguments passed to client.'
             logger.critical(error_message)
             raise InvalidClientArgsError(error_message)
 
         if server_config_file is not None and (url is not None or uri is not None):
@@ -44,186 +53,227 @@
             self._url = url
             self._uri = uri
 
         self._idx = -1
         self._node_path_list: List[str] = []
         self._client = Client(url=self._url)
         self.connect_timeout = connect_timeout
-        self._has_connected = False
+        self._connection_status = ConnectionStatus.DISCONNECTED
         self._node_map: Dict[str, Tuple] = {}
-        self._identifier_map: Dict[str, List[str]] = {}
 
         logger.info(f'Client created with url: {self._url}, and uri: {self._uri}')
 
-    def __enter__(self):
-        self._connect()
-        self._establish_server_structure()
-        return self
-
-    def __exit__(self, *args) -> None:
-        self._disconnect()
-
-    def _connect(self):
-        try:
-            if self._test_server_connection():
-                logger.info('_connect called but there is a connection to the server.')
-                self._has_connected = True
-                return
-            if self._disconnect():
+    async def __aenter__(self):
+        if self._connection_status != ConnectionStatus.CONNECTING:
+            self._connection_status = ConnectionStatus.CONNECTING
+            await self._connect()
+            await self._establish_server_structure()
+            self._connection_status = ConnectionStatus.CONNECTED
+            return self
+
+    async def __aexit__(self, *args) -> None:
+        await self._disconnect()
+
+    async def _connect(self):
+        try:
+            # if await self._test_server_connection():
+            #     logger.info('_connect called but there is a connection to the server.')
+            #     self._connection_status =
+            #     return
+            if await self._disconnect():
                 self._client = Client(url=self._url, timeout=self.connect_timeout)
             logger.info('Connecting...')
-            self._client.connect()
+            await self._client.connect()
             logger.info('Connected...')
-            self._has_connected = True
         except (ConnectionRefusedError, ConnectionError, RuntimeError, RuntimeWarning, TimeoutError):
             logger.error(
                 f'Unable to connect to server. Client expects server to have url: {self._url} and uri: {self._uri}. '
                 f'Server is not running or the configs are not matched with client.'
             )
-            self._has_connected = False
+            self._connection_status = ConnectionStatus.DISCONNECTED
+        except Exception as e:
+            logger.error(
+                'Unhandled exception while to connecting to server. '
+                f'Client expects server to have url: {self._url} and uri: {self._uri}. '
+                f'{e}'
+            )
+            self._connection_status = ConnectionStatus.DISCONNECTED
 
-    def _disconnect(self) -> bool:
+    async def _disconnect(self) -> bool:
         logger.info('Cleaning up client.')
         try:
-            self._client.disconnect()
+            await self._client.disconnect()
             return True
-        except (RuntimeError, ConnectionError, ThreadLoopNotRunning):
+        except (RuntimeError, ConnectionError):
             logger.warning('Tried to disconnect but there is no connection.')
             return False
+        except Exception as e:
+            logger.error(f'Unhandled exception while to disconnecting from server. {e} ')
+            return False
+
+    async def _dfs_mapper(self, node: Node, path: str) -> None:
+        browse_path = await node.read_browse_name()
+
+        if browse_path.NamespaceIndex != self._idx and browse_path.NamespaceIndex != 0:
+            return
 
-    def _dfs_mapper(self, node: Node, path: str):
-        # if node.read_node_class() == NodeClass.Variable and node.NamespaceIndex == self._idx:
-        browse_path = node.read_browse_name()
-        node_class = node.read_node_class()
+        node_class = await node.read_node_class()
         path_to_node = path + '/' + browse_path.Name
-        if node_class == NodeClass.Variable and browse_path.NamespaceIndex == self._idx:
+
+        # if node_class == NodeClass.Variable and browse_path.NamespaceIndex == self._idx:
+        if node_class == NodeClass.Variable:
             # Remove "/Objects/" since this client is intended for reading only custom nodes
-            path_to_node = path_to_node[9:]
-            var_type = node.read_data_type_as_variant_type()
+            if path_to_node.startswith('/Objects/'):
+                path_to_node = path_to_node[9:]
+            var_type = await node.read_data_type_as_variant_type()
             logger.info(f'Found OPCUA variable {path_to_node}, of variant type {var_type}')
-            self._node_map[path_to_node] = (node, var_type)
+            if not path_to_node.startswith('/'):
+                self._node_map['/' + path_to_node] = (node, var_type)
+            else:
+                self._node_map[path_to_node] = (node, var_type)
+            return
+
+        child_node_list = []
+        node_children = await node.get_children()
+
+        for child_node in node_children:
+            child_node_list.append(self._dfs_mapper(child_node, path_to_node))
 
-        for child_node in node.get_children():
-            self._dfs_mapper(child_node, path_to_node)
+        await asyncio.gather(*child_node_list)
+        return
 
-    def _establish_server_structure(self) -> None:
+    async def _establish_server_structure(self) -> None:
         try:
             logger.info(f'Mapping namespace using {self._url} and {self._uri}')
-            self._idx = self._client.get_namespace_index(self._uri)
+            self._idx = await self._client.get_namespace_index(self._uri)
             logger.info(f'Namespace index = {self._idx}')
-            root_object_node = self._client.nodes.root.get_child(['0:Objects'])
-            self._dfs_mapper(node=root_object_node, path='')
+            root_object_node = await self._client.nodes.root.get_child(['0:Objects'])
+            await self._dfs_mapper(node=root_object_node, path='')
+
             self._node_path_list = list(self._node_map.keys())
             logger.info(f'All nodes successfully mapped: {self._node_path_list}')
-        except (AttributeError, ConnectionError, RuntimeWarning, ValueError, ThreadLoopNotRunning):
+        except (AttributeError, ConnectionError, RuntimeWarning, ValueError):
             logger.error(f'Unable to map opcua nodes from {self._url} and {self._uri}')
+        except Exception as e:
+            logger.error(f'Unhandled exception while to mapping server structure. {e}')
 
-    def _test_server_connection(self) -> bool:
+    async def _test_server_connection(self) -> bool:
         try:
-            self._client.get_namespace_index(self._uri)
+            await self._client.get_namespace_index(self._uri)
             return True
         except Exception as e:
             logger.warning(e)
             logger.warning('Failed server connectivity test.')
             return False
 
-    def _write_helper(self, path: str, value: Any) -> bool:
-        if self._has_connected:
-            try:
-                var, var_type = self._node_map[path]
-            except KeyError:
-                logger.warning(f'Unable to find {path} in client map {self._node_map}')
-                return False
-            try:
-                value = convert_type(value=value, var_type=var_type)
-            except (KeyError, TypeError):
-                logger.warning(f'Unable to convert value {value} to variant type {var_type}')
-                return False
-            try:
-                current_time: DateTime = datetime.utcnow()  # type: ignore
-                var.write_value(
-                    DataValue(
-                        Value=Variant(value, var_type),
-                        SourceTimestamp=current_time,
-                        ServerTimestamp=current_time,
-                    )
+    async def _write_helper(self, path: str, value: Any) -> bool:
+        try:
+            var, var_type = self._node_map[path]
+        except KeyError:
+            logger.warning(f'Unable to find {path} in client map {self._node_map}')
+            return False
+        try:
+            value = convert_type(value=value, var_type=var_type)
+        except (KeyError, TypeError, Exception):
+            logger.warning(f'Unable to convert value {value} to variant type {var_type}')
+            return False
+        try:
+            current_time: DateTime = datetime.utcnow()
+            await var.write_value(
+                DataValue(
+                    Value=Variant(value, var_type),
+                    SourceTimestamp=current_time,
+                    ServerTimestamp=current_time,
                 )
-                logger.info(f'Wrote value {value} of type {var_type} to {path}')
-                return True
-            except (ConnectionError, ThreadLoopNotRunning) as e:
-                logger.warning(f'{e}')
-                logger.warning(f'Unable to write value {value} of type {var_type} to {path}')
-        else:
-            logger.warning(f'No connection has been made to server. Cannot write value {value} to path {path}')
+            )
+            logger.info(f'Wrote value {value} of type {var_type} to {path}')
+            return True
+        except ConnectionError as e:
+            logger.warning(f'{e}')
+            logger.warning(f'Unable to write value {value} of type {var_type} to {path}')
         return False
 
-    def write(self, path: str, value: Any) -> bool:
+    async def write(self, path: str, value: Any) -> bool:
         logger.info(f'Attempting to write value {value} to path {path}.')
-        if not self._has_connected:  # Write attempt has failed or client never connected.
+        if self._connection_status == ConnectionStatus.DISCONNECTED:
+            # Write attempt has failed or client never connected.
             logger.info('Client has not connected to server. Attempting to connect.')
-            self.__enter__()
-        if self._write_helper(path=path, value=value):
-            logger.info('Write attempt succeeded')
-            return True
-        else:
-            logger.warning('Write attempt failed')
-            self._has_connected = False
-
+            await self.__aenter__()
+        if self._connection_status == ConnectionStatus.CONNECTED:
+            if await self._write_helper(path=path, value=value):
+                logger.info('Write attempt succeeded')
+                return True
+            else:
+                logger.warning('Write attempt failed')
+                self._connection_status = ConnectionStatus.DISCONNECTED
         return False
 
-    def _read_helper(self, path: str) -> Any:
-        if self._has_connected:
-            try:
-                node = self._node_map[path][0]
-            except (KeyError, IndexError):
-                logger.warning(f'Unable to get node {path} from client map {self._node_map}')
-                return None
-            try:
-                value = node.read_value()
-                logger.info(f'Read value {value} from path {path}')
-                return value
-            except (ConnectionError, ThreadLoopNotRunning) as e:
-                logger.warning(f'{e}')
-                logger.warning(f'Unable to read node at {path}')
-        else:
-            logger.warning(f'No connection has been made to server. Cannot read node at path {path}')
+    async def _read_helper(self, path: str) -> Any:
+        try:
+            node = self._node_map[path][0]
+        except (KeyError, IndexError):
+            logger.warning(f'Unable to get node {path} from client map {self._node_map}')
+            return None
+        try:
+            value = await node.read_value()
+            logger.info(f'Read value {value} from path {path}')
+            return value
+        except Exception as e:
+            logger.warning(f'{e}')
+            logger.warning(f'Unable to read node at {path}')
         return None
 
-    def read(self, path: str) -> Any:
+    async def read(self, path: str) -> Any:
         logger.info(f'Attempting to read path {path}.')
-        if not self._has_connected:  # Read attempt has failed or client never connected.
+        if self._connection_status == ConnectionStatus.DISCONNECTED:
+            # Read attempt has failed or client never connected.
             logger.info('Client has not connected to server. Attempting to connect.')
-            self.__enter__()
-        value = self._read_helper(path=path)
-        if value is not None:
-            logger.info('Read attempt succeeded')
-            logger.info(f'Value: {value}')
-            return value
-        else:
-            logger.warning('Read attempt failed')
-            self._has_connected = False
+            await self.__aenter__()
+        if self._connection_status == ConnectionStatus.CONNECTED:
+            value = await self._read_helper(path=path)
+            if value is not None:
+                logger.info('Read attempt succeeded')
+                logger.info(f'Value: {value}')
+                return value
+            else:
+                logger.warning('Read attempt failed')
+                self._connection_status = ConnectionStatus.DISCONNECTED
         return None
 
-    def read_all(self) -> Dict[str, Any]:
+    async def read_all(self) -> Dict[str, Any]:
         logger.info(f'Attempting to read all variables on server at uri: {self._uri} and url: {self._url}.')
         results = {}
-        if not self._has_connected:  # Client has never successfully connected to the server
+        future_results = {}
+
+        if self._connection_status == ConnectionStatus.DISCONNECTED:
             logger.info('Client may not be connected to server. Attempting to connect.')
-            self.__enter__()  # Creates a new client object and adjusts self._has_connected() appropriately
-        if self._has_connected:  # In case self.__enter__() changed value to true by establishing a connection
+            await self.__aenter__()  # Creates a new client object and adjusts self._has_connected() appropriately
+
+        if self._connection_status == ConnectionStatus.CONNECTED:
             for path in self._node_path_list:
-                value = self._read_helper(path)
-                if value is not None:
-                    logger.info(f'Successfully read value: {value} for path: {path}')
-                    results[path] = value
-                else:
-                    # This could happens if there is a disconnect during reading
-                    logger.warning(f'Unsuccessful read attempt for path {path}')
-                    self._has_connected = False
-                    break
-
-        if len(self._node_path_list) == 0 or len(results) != len(self._node_path_list):
-            # Either there was never a connection or there was a disconnect
-            # while reading and only some results were read
-            self._has_connected = False
+                task_value = asyncio.create_task(self._read_helper(path))
+                # print(f'{path}: {value}')
+                future_results[path] = task_value
+
+        if len(self._node_path_list) == 0:
+            # There may never have been a connection
+            self._connection_status = ConnectionStatus.DISCONNECTED
+
+        await asyncio.gather(*future_results.values())
+
+        for path, task in future_results.items():
+            task_value = task.result()
+
+            if task_value is not None:
+                logger.info(f'Successfully read value: {task_value} for path: {path}')
+            else:
+                # This could happens if there is a disconnect during reading
+                logger.warning(f'Unsuccessful read attempt for path {path}')
+                self._connection_status = ConnectionStatus.DISCONNECTED
+            results[path] = task_value
+
         logger.info(f'{results}')
         return results
+
+    def identifier_from_string(self, path: str) -> List[str]:
+        identifier = [f'{self._idx}:{path_part}' for path_part in path.split('/')]
+        return ['0:Objects'] + identifier
```

### Comparing `formic_opcua-1.3.1/formic_opcua/core/parse.py` & `formic_opcua-1.3.2/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/formic_opcua/core/type_conversions.py` & `formic_opcua-1.3.2/formic_opcua/core/type_conversions.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.3.2/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.3.2/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/formic_opcua/server/opcua_server.py` & `formic_opcua-1.3.2/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/hooks/add_issue_prefix.py` & `formic_opcua-1.3.2/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/tests/test_server_config.py` & `formic_opcua-1.3.2/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/.gitignore` & `formic_opcua-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.1/pyproject.toml` & `formic_opcua-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

