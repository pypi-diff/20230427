# Comparing `tmp/TapisCL-ICICLE-0.0.30.tar.gz` & `tmp/TapisCL-ICICLE-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.30.tar", last modified: Thu Apr 20 00:23:50 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.31.tar", last modified: Thu Apr 27 04:36:00 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.30.tar` & `TapisCL-ICICLE-0.0.31.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:50.385810 TapisCL-ICICLE-0.0.30/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/LICENSE
--rw-rw-rw-   0        0        0    44210 2023-04-20 00:23:50.384784 TapisCL-ICICLE-0.0.30/PKG-INFO
--rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.30/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:50.371774 TapisCL-ICICLE-0.0.30/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1474 2023-04-19 03:20:32.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    11005 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     9563 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     5620 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     2059 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10588 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    19567 2023-04-19 04:33:11.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:50.383781 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44210 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-04-20 00:22:41.000000 TapisCL-ICICLE-0.0.30/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 00:23:50.385810 TapisCL-ICICLE-0.0.30/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 04:36:00.572028 TapisCL-ICICLE-0.0.31/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/LICENSE
+-rw-rw-rw-   0        0        0    44210 2023-04-27 04:36:00.570917 TapisCL-ICICLE-0.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.31/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 04:36:00.565819 TapisCL-ICICLE-0.0.31/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1474 2023-04-19 03:20:32.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    11005 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     9563 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     5620 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     2059 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10683 2023-04-27 04:34:09.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    19575 2023-04-27 04:34:09.000000 TapisCL-ICICLE-0.0.31/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:36:00.569881 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44210 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-27 04:36:00.000000 TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-04-27 04:35:02.000000 TapisCL-ICICLE-0.0.31/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 04:36:00.572028 TapisCL-ICICLE-0.0.31/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.30/LICENSE` & `TapisCL-ICICLE-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/PKG-INFO` & `TapisCL-ICICLE-0.0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.30
+Version: 0.0.31
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.30/README.md` & `TapisCL-ICICLE-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/helpers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 from tapipy.tapis import Tapis
 import socket
 import os
 import logging
 from tapisObjectWrappers import Files, Apps, Pods, Systems, Neo4jCLI, PostgresCLI
 import typing
+import traceback
 
 try:
     from . import exceptions
     from . import socketOpts as SO
     from . import helpers
     from . import schemas
     from . import decorators
@@ -20,14 +21,15 @@
     import exceptions
     import socketOpts as SO
     import helpers
     import schemas
     import decorators
     import args
 
+
 class Server(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.DynamicHelpUtility):
     """
     Receives commands from the client and executes Tapis operations
     """
     def __init__(self, IP: str, PORT: int):
         # logger setup
         self.logger = logging.getLogger(__name__)
@@ -257,16 +259,18 @@
             except exceptions.Exit as e:
                 self.logger.info("user exit initiated")
                 error_response = schemas.ResponseData(response_message = str(e), exit_status=1)
                 self.json_send(error_response.dict())
                 self.connection.close()  # close the connection
                 self.accept()  # wait for CLI to reconnect
             except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived, Exception) as e:
-                error_response = schemas.ResponseData(response_message = str(e))
+                error_str = traceback.format_exc()
+                print(error_str)
+                error_response = schemas.ResponseData(response_message = f"{str(e)}")
                 self.json_send(error_response.dict())
-                self.logger.warning(f"{str(e)}\n{e.__traceback__}")
+                self.logger.warning(f"{error_str}")
 
 
 
 if __name__ == '__main__':
     server = Server(socket.gethostbyname(socket.gethostname()), 30000)
     server.main()
```

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.31/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self.__code__ = self.query.__code__
 
     def __call__(self, **kwargs):
         kwargs = self.filter_kwargs(self.query, kwargs)
         result = self.query(**kwargs)
         return result
         
-    def get_credentials(self):
+    def get_credentials(self, id):
         uname, pword = self.t.pods.get_pod_credentials(pod_id=id).user_username, self.t.pods.get_pod_credentials(pod_id=id).user_password
         return uname, pword
 
 
 class Systems(tapisObject):
     """
     @help: Access Tapis systems through the connected service
@@ -174,30 +174,30 @@
 
 class PostgresCLI(TapisQuery):
     """
     @help: integrated CLI to interface with Postgres pods
     """
     @decorators.RequiresExpression
     def query(self, id: str, expression: str) -> str:
-        uname, pword = self.get_credentials()
+        uname, pword = self.get_credentials(id)
         with psycopg2.connect(f"postgresql://{uname}:{pword}@{id}.pods.{self.t.base_url.split('https://')[1]}:443") as conn:
             conn.autocommit = True
             with conn.cursor() as cur:
                 cur.execute(query=expression)
                 return_value = cur.fetchall()
         return str(f'[+][{id}] {return_value}')
 
 
 class Neo4jCLI(TapisQuery):
     """
     @help: integrated CLI to interface with Neo4j pods
     """
     @decorators.RequiresExpression
     def query(self, id: str, expression: str) -> str: # function to submit queries to a Neo4j knowledge graph
-        uname, pword = self.get_credentials()
+        uname, pword = self.get_credentials(id)
         graph = Graph(f"bolt+ssc://{id}.pods.{self.t.base_url.split('https://')[1]}:443", auth=(uname, pword), secure=True, verify=True)
 
         try:
             return_value = graph.run(expression)
             print(type(return_value))
             if str(return_value) == '(No data)' and 'create' in expression.lower(): # if no data is returned (mostly if something is created) then just say 'success'
                 return f'[+][{id}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
```

### Comparing `TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.30
+Version: 0.0.31
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.31/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.30/pyproject.toml` & `TapisCL-ICICLE-0.0.31/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.30"
+version = "0.0.31"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

