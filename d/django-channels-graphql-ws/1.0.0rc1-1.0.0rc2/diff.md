# Comparing `tmp/django_channels_graphql_ws-1.0.0rc1.tar.gz` & `tmp/django_channels_graphql_ws-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_channels_graphql_ws-1.0.0rc1.tar", max compression
+gzip compressed data, was "django_channels_graphql_ws-1.0.0rc2.tar", max compression
```

## Comparing `django_channels_graphql_ws-1.0.0rc1.tar` & `django_channels_graphql_ws-1.0.0rc2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-04-27 20:51:46.646275 django_channels_graphql_ws-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     1433 2023-04-27 20:51:46.646802 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/__init__.py
--rw-r--r--   0        0        0    10111 2023-04-27 20:51:46.647155 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/client.py
--rw-r--r--   0        0        0     2637 2023-04-27 20:51:46.647317 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/dict_as_object.py
--rw-r--r--   0        0        0    58178 2023-04-27 20:51:46.647710 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/graphql_ws_consumer.py
--rw-r--r--   0        0        0     3850 2023-04-27 20:51:46.647978 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/serializer.py
--rw-r--r--   0        0        0    16451 2023-04-27 20:51:46.648225 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/subscription.py
--rw-r--r--   0        0        0     4816 2023-04-27 20:51:46.648455 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/testing.py
--rw-r--r--   0        0        0     6939 2023-04-27 20:51:46.648726 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/transport.py
--rw-r--r--   0        0        0     8477 2023-04-27 20:58:40.241396 django_channels_graphql_ws-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 20:51:46.646275 django_channels_graphql_ws-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     1433 2023-04-27 20:51:46.646802 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/__init__.py
+-rw-r--r--   0        0        0    10111 2023-04-27 20:51:46.647155 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/client.py
+-rw-r--r--   0        0        0     2637 2023-04-27 20:51:46.647317 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/dict_as_object.py
+-rw-r--r--   0        0        0    58225 2023-04-27 21:28:38.470594 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/graphql_ws_consumer.py
+-rw-r--r--   0        0        0     3850 2023-04-27 20:51:46.647978 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/serializer.py
+-rw-r--r--   0        0        0    16451 2023-04-27 20:51:46.648225 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/subscription.py
+-rw-r--r--   0        0        0     4816 2023-04-27 20:51:46.648455 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/testing.py
+-rw-r--r--   0        0        0     6939 2023-04-27 20:51:46.648726 django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/transport.py
+-rw-r--r--   0        0        0     8478 2023-04-27 21:29:50.214108 django_channels_graphql_ws-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc2/PKG-INFO
```

### Comparing `django_channels_graphql_ws-1.0.0rc1/LICENSE` & `django_channels_graphql_ws-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/__init__.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/__init__.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/client.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/client.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/dict_as_object.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/dict_as_object.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/graphql_ws_consumer.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/graphql_ws_consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,25 @@
 import inspect
 import logging
 import threading
 import time
 import traceback
 import weakref
 from collections.abc import Sequence
-from typing import Any, AsyncIterator, Awaitable, Callable, Optional, Type, Union, cast
+from typing import (
+    Any,
+    AsyncIterator,
+    Awaitable,
+    Callable,
+    Dict,
+    Optional,
+    Type,
+    Union,
+    cast,
+)
 
 import asgiref.sync
 import channels.db
 import channels.generic.websocket as ch_websocket
 import django.db.models.query
 import graphene
 import graphql
@@ -105,15 +115,15 @@
     # when the subscription activates, so he can be sure he doesn't miss
     # any notifications. Disabled by default, cause this is an extension
     # to the original protocol and the client must be tuned accordingly.
     confirm_subscriptions: bool = False
 
     # The message sent to the client when subscription activation
     # confirmation is enabled.
-    subscription_confirmation_message: dict[str, Any] = {"data": None, "errors": None}
+    subscription_confirmation_message: Dict[str, Any] = {"data": None, "errors": None}
 
     # Issue a warning to the log when operation/resolver takes longer
     # than specified number in seconds. None disables the warning.
     warn_operation_timeout: Optional[float] = 1
     warn_resolver_timeout: Optional[float] = 1
 
     # The size of the subscription notification queue. If there are more
@@ -208,15 +218,15 @@
         event with missing value. We have to promote
         `GraphqlWsConsumer.SKIP` value to the GraphQL operation results
         and remove skipped values from the final response.
         """
 
         @staticmethod
         def build_response(
-            data: Optional[dict[str, Any]], errors: list[graphql.GraphQLError]
+            data: Optional[Dict[str, Any]], errors: list[graphql.GraphQLError]
         ) -> graphql.ExecutionResult:
             """Remove skipped subscription events from results.
 
             `data` is a dictionary where the key is subscription field
             name and value is a subscription resolver result. Value will
             be `GraphqlWsConsumer.SKIP` object for skipped events.
             """
@@ -250,22 +260,22 @@
 
         assert self.schema is not None, (
             "An attribute 'schema' is not set! Subclasses must specify "
             "the schema which processes GraphQL subscription queries."
         )
 
         # Registry of active (subscribed) subscriptions.
-        self._subscriptions: dict[
+        self._subscriptions: Dict[
             int, GraphqlWsConsumer._SubInf
         ] = {}  # {'<sid>': '<SubInf>', ...}
         self._sids_by_group = {}  # {'<grp>': ['<sid0>', '<sid1>', ...], ...}
 
         # Tasks which send notifications to clients indexed by an
         # operation/subscription id.
-        self._notifier_tasks: dict[int, asyncio.Task] = {}
+        self._notifier_tasks: Dict[int, asyncio.Task] = {}
 
         # Task that sends keepalive messages periodically.
         self._keepalive_task = None
 
         # Background tasks to clean it up when a client disconnects.
         # We use weak collection so finished task will be autoremoved.
         self._background_tasks: weakref.WeakSet = weakref.WeakSet()
@@ -835,15 +845,15 @@
         return doc_ast, op_ast, None
 
     async def _on_gql_start__subscribe(
         self,
         document: graphql.DocumentNode,
         root_value: Any = None,
         context_value: Any = None,
-        variable_values: Optional[dict[str, Any]] = None,
+        variable_values: Optional[Dict[str, Any]] = None,
         operation_name: Optional[str] = None,
         field_resolver: Optional[graphql.GraphQLFieldResolver] = None,
         subscribe_field_resolver: Optional[graphql.GraphQLFieldResolver] = None,
         middleware: graphql.Middleware = None,
         execution_context_class: Optional[Type[graphql.ExecutionContext]] = None,
     ) -> Union[AsyncIterator[graphql.ExecutionResult], graphql.ExecutionResult]:
         """Create a GraphQL subscription.
```

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/serializer.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/serializer.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/subscription.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/subscription.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/testing.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/testing.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/transport.py` & `django_channels_graphql_ws-1.0.0rc2/channels_graphql_ws/transport.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc1/pyproject.toml` & `django_channels_graphql_ws-1.0.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # --------------------------------------------------------------- POETRY
 # Python packaging and dependency management.
 # Docs: https://python-poetry.org/docs/
 [tool.poetry]
 name = "django-channels-graphql-ws"
-version = "1.0.0rc1"
+version = "v1.0.0rc2"
 description = """Django Channels based WebSocket GraphQL server with Graphene-like subscriptions"""
 authors = ["Alexander A. Prokhorov <alexander.prokhorov@datadvance.net>"]
 homepage = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 repository = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 license = "MIT"
 packages = [
     { include = "channels_graphql_ws/" },
```

### Comparing `django_channels_graphql_ws-1.0.0rc1/PKG-INFO` & `django_channels_graphql_ws-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-channels-graphql-ws
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Django Channels based WebSocket GraphQL server with Graphene-like subscriptions
 Home-page: https://github.com/datadvance/DjangoChannelsGraphqlWs
 License: MIT
 Author: Alexander A. Prokhorov
 Author-email: alexander.prokhorov@datadvance.net
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

