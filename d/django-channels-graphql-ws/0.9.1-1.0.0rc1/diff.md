# Comparing `tmp/django-channels-graphql-ws-0.9.1.tar.gz` & `tmp/django_channels_graphql_ws-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-channels-graphql-ws-0.9.1.tar", max compression
+gzip compressed data, was "django_channels_graphql_ws-1.0.0rc1.tar", max compression
```

## Comparing `django-channels-graphql-ws-0.9.1.tar` & `django_channels_graphql_ws-1.0.0rc1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1073 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/LICENSE
--rw-r--r--   0        0        0     1433 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/channels_graphql_ws/__init__.py
--rw-r--r--   0        0        0    10007 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/channels_graphql_ws/client.py
--rw-r--r--   0        0        0    42871 2022-01-27 00:19:05.619035 django-channels-graphql-ws-0.9.1/channels_graphql_ws/graphql_ws_consumer.py
--rw-r--r--   0        0        0     2679 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/channels_graphql_ws/scope_as_context.py
--rw-r--r--   0        0        0     3850 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/channels_graphql_ws/serializer.py
--rw-r--r--   0        0        0    20316 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/channels_graphql_ws/subscription.py
--rw-r--r--   0        0        0     4737 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/channels_graphql_ws/testing.py
--rw-r--r--   0        0        0     6894 2022-01-26 15:15:18.074458 django-channels-graphql-ws-0.9.1/channels_graphql_ws/transport.py
--rw-r--r--   0        0        0     6559 2022-01-27 00:19:05.619035 django-channels-graphql-ws-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1127 2022-01-27 00:20:13.285976 django-channels-graphql-ws-0.9.1/setup.py
--rw-r--r--   0        0        0     1216 2022-01-27 00:20:13.286176 django-channels-graphql-ws-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 20:51:46.646275 django_channels_graphql_ws-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     1433 2023-04-27 20:51:46.646802 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/__init__.py
+-rw-r--r--   0        0        0    10111 2023-04-27 20:51:46.647155 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/client.py
+-rw-r--r--   0        0        0     2637 2023-04-27 20:51:46.647317 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/dict_as_object.py
+-rw-r--r--   0        0        0    58178 2023-04-27 20:51:46.647710 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/graphql_ws_consumer.py
+-rw-r--r--   0        0        0     3850 2023-04-27 20:51:46.647978 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/serializer.py
+-rw-r--r--   0        0        0    16451 2023-04-27 20:51:46.648225 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/subscription.py
+-rw-r--r--   0        0        0     4816 2023-04-27 20:51:46.648455 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/testing.py
+-rw-r--r--   0        0        0     6939 2023-04-27 20:51:46.648726 django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/transport.py
+-rw-r--r--   0        0        0     8477 2023-04-27 20:58:40.241396 django_channels_graphql_ws-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc1/PKG-INFO
```

### Comparing `django-channels-graphql-ws-0.9.1/LICENSE` & `django_channels_graphql_ws-1.0.0rc1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (C) DATADVANCE, 2010-2021
+Copyright (C) DATADVANCE, 2010-2023
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/__init__.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2010-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/client.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2010-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -23,15 +23,16 @@
 
 
 import asyncio
 import textwrap
 import time
 import uuid
 
-from .transport import GraphqlWsTransport
+# Underscored to avoid name clash with GraphqlWsClient init's argument.
+from . import transport as _transport
 
 
 class GraphqlWsClient:
     """A client for the GraphQL WebSocket server.
 
     The client implements a WebSocket-based GraphQL protocol. It is the
     same protocol as the server implemented by the `GraphqlWsConsumer`
@@ -47,27 +48,26 @@
     backend, when used with subscriptions it may either return
     subscription data or some query result. The response type must be
     checked outside the client manually.
 
     Args:
         transport: The `GraphqlWsTransport` instance used to send and
             receive messages over the WebSocket connection.
-
     """
 
-    def __init__(self, transport: GraphqlWsTransport):
+    def __init__(self, transport: _transport.GraphqlWsTransport):
         """Constructor."""
         assert isinstance(
-            transport, GraphqlWsTransport
-        ), "The 'transport' must implement the 'GraphqlWsTransport' interface!"
+            transport, _transport.GraphqlWsTransport
+        ), "Given transport does not implement the 'GraphqlWsTransport' interface!"
         self._transport = transport
         self._is_connected = False
 
     @property
-    def transport(self) -> GraphqlWsTransport:
+    def transport(self) -> _transport.GraphqlWsTransport:
         """Underlying network transport."""
         return self._transport
 
     @property
     def connected(self) -> bool:
         """Indicate whether client is connected."""
         return self._is_connected
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/graphql_ws_consumer.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/graphql_ws_consumer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2011-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -33,36 +33,38 @@
   https://github.com/apollographql/subscriptions-transport-ws/blob/master/src/message-types.ts
 - ASGI specification for WebSockets:
   https://github.com/django/asgiref/blob/master/specs/www.rst#websocket
 - GitHubGist with the root of inspiration:
   https://gist.github.com/tricoder42/af3d0337c1b33d82c1b32d12bd0265ec
 """
 
-
 import asyncio
-import concurrent
 import dataclasses
 import functools
+import inspect
 import logging
+import threading
+import time
 import traceback
-import types
 import weakref
-from typing import Any, Callable, Dict, List, Optional, Sequence
+from collections.abc import Sequence
+from typing import Any, AsyncIterator, Awaitable, Callable, Optional, Type, Union, cast
 
 import asgiref.sync
+import channels.db
 import channels.generic.websocket as ch_websocket
-import django.core.serializers
-import django.db
+import django.db.models.query
+import graphene
 import graphql
 import graphql.error
-import graphql.execution.executors.asyncio
-import promise
-import rx
+import graphql.execution
+import graphql.pyutils
+import graphql.utilities
 
-from .scope_as_context import ScopeAsContext
+from .dict_as_object import DictAsObject
 from .serializer import Serializer
 
 # Module logger.
 LOG = logging.getLogger(__name__)
 
 # WebSocket subprotocol used for the GraphQL.
 GRAPHQL_WS_SUBPROTOCOL = "graphql-ws"
@@ -79,150 +81,214 @@
     https://github.com/apollographql/subscriptions-transport-ws/blob/master/PROTOCOL.md
     """
 
     # ----------------------------------------------------------------- PUBLIC INTERFACE
 
     # Overwrite this in the subclass to specify the GraphQL schema which
     # processes GraphQL queries.
-    schema = None
+    schema: graphene.Schema
 
     # The interval to send keepalive messages to the clients (seconds).
-    send_keepalive_every = None
+    send_keepalive_every: Optional[float] = None
 
     # Set to `True` to process requests (i.e. GraphQL documents) from
     # a client in order of arrival, which is the same as sending order,
     # as guaranteed by the WebSocket protocol. This means that request
     # processing for this particular client becomes serial - in other
     # words, the server will not start processing another request
     # before it finishes the current one. Note that requests from
     # different clients (within different WebSocket connections)
     # are still processed asynchronously. Useful for tests.
-    strict_ordering = False
+    strict_ordering: bool = False
 
     # When set to `True` the server will send an empty data message in
     # response to the subscription. This is needed to let client know
     # when the subscription activates, so he can be sure he doesn't miss
     # any notifications. Disabled by default, cause this is an extension
     # to the original protocol and the client must be tuned accordingly.
-    confirm_subscriptions = False
+    confirm_subscriptions: bool = False
 
     # The message sent to the client when subscription activation
     # confirmation is enabled.
-    subscription_confirmation_message = {"data": None, "errors": None}
+    subscription_confirmation_message: dict[str, Any] = {"data": None, "errors": None}
 
-    # The maximum number of threads designated for GraphQL requests
-    # processing. `None` means that default value is used. Default
-    # value depends on the Python version, check its documentation:
-    # https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor
-    max_worker_threads = None
+    # Issue a warning to the log when operation/resolver takes longer
+    # than specified number in seconds. None disables the warning.
+    warn_operation_timeout: Optional[float] = 1
+    warn_resolver_timeout: Optional[float] = 1
 
     # The size of the subscription notification queue. If there are more
     # notifications (for a single subscription) than the given number,
     # then an oldest notification is dropped and a warning is logged.
-    subscription_notification_queue_limit = 1024
-
-    # A prefix of the Channel group names used for the subscription
-    # notifications. You may change this to avoid name clashes in the
-    # ASGI backend, e.g. in the Redis.
-    group_name_prefix = "GRAPHQL_WS_SUBSCRIPTION"
+    subscription_notification_queue_limit: int = 1024
 
     # GraphQL middleware.
-    # Typically a list of functions (callables) like:
+    # List of functions (callables) like the following:
     # ```python
-    # def my_middleware(next_middleware, root, info, *args, **kwds):
-    #     return next_middleware(root, info, *args, **kwds)
+    # async def my_middleware(next_middleware, root, info, *args, **kwds):
+    #     result = next_middleware(root, info, *args, **kwds)
+    #     if graphql.pyutils.is_awaitable(result):
+    #        result = await result
+    #     return result
     # ```
-    # For more information read:
-    # https://docs.graphene-python.org/en/latest/execution/middleware/#middleware
+    # For more information read docs:
+    # - https://docs.graphene-python.org/en/latest/execution/middleware/#middleware
+    # - https://graphql-core-3.readthedocs.io/en/latest/diffs.html#custom-middleware
+    # Docs about async middlewares are still missing - read the
+    # GraphQL-core sources to know more.
     middleware: Sequence = []
 
+    # A function to execute synchronous resolvers, middlewares, request
+    # parsing functions, etc. from asynchronous context. The default is
+    # a ASGI thread pool in `channels.db.database_sync_to_async` which
+    # cleans up the database connections so resolvers can safely work
+    # with a database.
+    # https://channels.readthedocs.io/en/latest/topics/databases.html#database-sync-to-async
+    # You can redefine this to use designated thread pool or to use
+    # `asgiref.sync.sync_to_async` if you are sure your resolvers does
+    # not work with the database.
+    sync_to_async: asgiref.sync.SyncToAsync = channels.db.database_sync_to_async
+
+    # Subscription implementation shall return this to tell consumer
+    # to suppress subscription notification.
+    SKIP = object()
+
     async def on_connect(self, payload):
         """Client connection handler.
 
         Called after CONNECTION_INIT message from client. Overwrite and
         raise an Exception to tell the server to reject the connection
         when it's necessary.
 
         Args:
             payload: Payload from CONNECTION_INIT message.
+        """
+        del payload
+
+    async def on_operation(self, op_id, payload):
+        """Process business logic before operation processing starts.
+
+        Useful e.g. to check that user session is not yet expired.
 
+        Throw `graphql.error.GraphQLError` to cancel the operation.
+
+        Args:
+            op_id: Operation id.
+            payload: Payload of the operation.
         """
+        del op_id, payload
 
     # ------------------------------------------------------------------- IMPLEMENTATION
 
-    # Subscription implementation may shall return this to tell consumer
-    # to suppress subscription notification.
-    SKIP = object()
-
-    # Threadpool used to process requests.
-    _workers = concurrent.futures.ThreadPoolExecutor(
-        thread_name_prefix="GraphqlWs.", max_workers=max_worker_threads
-    )
-
-    # Disable promise "trampoline" (whatever it means), cause when it
-    # is enabled (which is by default) the promise is not thread-safe.
-    # This leads to hanging threads and unanswered requests.
-    # https://github.com/syrusakbary/promise/issues/57#issuecomment-406778476
-    promise.promise.async_instance.disable_trampoline()
+    # A prefix of Channel groups with subscription notifications.
+    group_name_prefix: str = "GQLWS"
 
     # Structure that holds subscription information.
     @dataclasses.dataclass
     class _SubInf:
         """Subscription information structure."""
 
         # Subscription identifier - protocol operation identifier.
         sid: int
         # Subscription groups the subscription belongs to.
-        groups: List[str]
-        # The subscription notification queue. Required to preserve the
-        # order of notifications within a single subscription.
-        notification_queue: asyncio.Queue
-        # A task which listens to the notification queue and notifies
-        # clients. Task triggers subscription `publish` resolvers.
-        notifier_task: asyncio.Task
+        groups: list[str]
+        # A function which triggets subscription.
+        enqueue_notification: Callable[[Any], None]
         # The callback to invoke when client unsubscribes.
-        unsubscribed_callback: Callable[[], None]
+        unsubscribed_callback: Callable[..., Awaitable[None]]
+
+    class _SubscriptionExecutionContext(graphql.ExecutionContext):
+        """Special execution context for subscriptions.
+
+        Subscription `publish` method is called via `graphql.execute`
+        like normal resolver. But subscription may return
+        `GraphqlWsConsumer.SKIP` object instead of declared result type.
+        When `graphql.execute` can not build resulting type from the
+        resolver return value it sets result to `None` which may lead to
+        GraphQL errors in case of required field or confuse skipped
+        event with missing value. We have to promote
+        `GraphqlWsConsumer.SKIP` value to the GraphQL operation results
+        and remove skipped values from the final response.
+        """
+
+        @staticmethod
+        def build_response(
+            data: Optional[dict[str, Any]], errors: list[graphql.GraphQLError]
+        ) -> graphql.ExecutionResult:
+            """Remove skipped subscription events from results.
+
+            `data` is a dictionary where the key is subscription field
+            name and value is a subscription resolver result. Value will
+            be `GraphqlWsConsumer.SKIP` object for skipped events.
+            """
+            if data:
+                data = {
+                    field_name: value
+                    for field_name, value in data.items()
+                    if value is not GraphqlWsConsumer.SKIP
+                }
+            return graphql.ExecutionContext.build_response(data, errors)
+
+        def complete_value(
+            self,
+            return_type: graphql.GraphQLOutputType,
+            field_nodes: list[graphql.FieldNode],
+            info: graphql.GraphQLResolveInfo,
+            path: graphql.pyutils.Path,
+            result: Any,
+        ):
+            """Do not create return_type value for skipped events.
+
+            We will remove `GraphqlWsConsumer.SKIP` marks from the final
+            result in the `build_response` method.
+            """
+            if result is GraphqlWsConsumer.SKIP:
+                return result
+            return super().complete_value(return_type, field_nodes, info, path, result)
 
     def __init__(self, *args, **kwargs):
         """Consumer constructor."""
+
         assert self.schema is not None, (
             "An attribute 'schema' is not set! Subclasses must specify "
             "the schema which processes GraphQL subscription queries."
         )
 
         # Registry of active (subscribed) subscriptions.
-        self._subscriptions = {}  # {'<sid>': '<SubInf>', ...}
+        self._subscriptions: dict[
+            int, GraphqlWsConsumer._SubInf
+        ] = {}  # {'<sid>': '<SubInf>', ...}
         self._sids_by_group = {}  # {'<grp>': ['<sid0>', '<sid1>', ...], ...}
 
+        # Tasks which send notifications to clients indexed by an
+        # operation/subscription id.
+        self._notifier_tasks: dict[int, asyncio.Task] = {}
+
         # Task that sends keepalive messages periodically.
         self._keepalive_task = None
 
         # Background tasks to clean it up when a client disconnects.
         # We use weak collection so finished task will be autoremoved.
-        self._background_tasks = weakref.WeakSet()
-
-        # Remember current eventloop so we can check it further in
-        # `_assert_thread` method.
-        self._eventloop = asyncio.get_event_loop()
+        self._background_tasks: weakref.WeakSet = weakref.WeakSet()
 
         # Crafty weak collection with per-operation locks. It holds a
         # mapping from the operaion id (protocol message id) to the
         # `asyncio.Lock` used to serialize processing of start & stop
         # requests. Since the collection is weak, it automatically
         # throws away items when locks are garbage collected.
-        self._operation_locks = weakref.WeakValueDictionary()
+        self._operation_locks: weakref.WeakValueDictionary = (
+            weakref.WeakValueDictionary()
+        )
 
         super().__init__(*args, **kwargs)
 
     # ---------------------------------------------------------- CONSUMER EVENT HANDLERS
 
     async def connect(self):
         """Handle new WebSocket connection."""
-        # Assert we run in a proper thread.
-        self._assert_thread()
 
         # Check the subprotocol told by the client.
         #
         # NOTE: In Python 3.6 `scope["subprotocols"]` was a string, but
         # starting with Python 3.7 it is a bytes. This can be a proper
         # change or just a bug in the Channels to be fixed. So let's
         # accept both variants until it becomes clear.
@@ -239,170 +305,162 @@
 
     async def disconnect(self, code):
         """Handle WebSocket disconnect.
 
         Remove itself from the Channels groups, clear triggers and stop
         sending keepalive messages.
         """
-        # Assert we run in a proper thread.
-        self._assert_thread()
 
         # Print debug or warning message depending on the value of the
         # connection close code. We consider all reserved codes (<999),
         # 1000 "Normal Closure", and 1001 "Going Away" as OK.
         # See: https://developer.mozilla.org/en-US/docs/Web/API/CloseEvent
         if not code:
-            LOG.warning("WebSocket connection closed without a code")
+            LOG.warning("WebSocket connection closed without a code!")
         elif code <= 1001:
             LOG.debug("WebSocket connection closed with code: %s.", code)
         else:
             LOG.warning("WebSocket connection closed with code: %s!", code)
 
         # The list of awaitables to simultaneously wait at the end.
-        waitlist = []
+        waitlist: list[asyncio.Task] = []
 
         # Unsubscribe from the Channels groups.
         waitlist += [
-            self._channel_layer.group_discard(group, self.channel_name)
+            asyncio.create_task(
+                self._channel_layer.group_discard(group, self.channel_name)
+            )
             for group in self._sids_by_group
         ]
 
         # Cancel all currently running background tasks.
         for bg_task in self._background_tasks:
             bg_task.cancel()
         waitlist += list(self._background_tasks)
 
         # Stop sending keepalive messages (if enabled).
         if self._keepalive_task is not None:
             self._keepalive_task.cancel()
             waitlist += [self._keepalive_task]
 
+        # Stop tasks which listen to GraphQL lib and send notifications.
+        for notifier_task in self._notifier_tasks.values():
+            notifier_task.cancel()
+            waitlist += [notifier_task]
+
+        # Wait for tasks to stop.
         if waitlist:
             await asyncio.wait(waitlist)
 
-        self._subscriptions.clear()
-        self._sids_by_group.clear()
         self._background_tasks.clear()
+        self._keepalive_task = None
+        self._notifier_tasks.clear()
+        self._operation_locks.clear()
+        self._sids_by_group.clear()
+        self._subscriptions.clear()
 
     async def receive_json(self, content):  # pylint: disable=arguments-differ
         """Process WebSocket message received from the client.
 
         NOTE: We force 'STOP' message processing to wait until 'START'
         with the same operation id finishes (if it is running). This
-        protects us from a raise conditions which may happen when
-        a client stops operation immediately after starting it. An
-        illustrative example is a subscribe-unsubscribe pair. If we
-        spawn processing of both messages concurrently we can deliver
-        subscription confirmation after unsubscription confirmation.
-        """
-        # Disable this check cause the current version of Pylint
-        # improperly complains when we assign a coroutine object to
-        # a local variable `task` below.
-        # pylint: disable=assignment-from-no-return
-
-        # Assert we run in a proper thread.
-        self._assert_thread()
+        protects us from race conditions which may happen when a client
+        stops operation immediately after starting it. An illustrative
+        example is a subscribe-unsubscribe pair. If we spawn processing
+        of both messages concurrently we can deliver subscription
+        confirmation after unsubscription confirmation.
+        """
 
         # Extract message type based on which we select how to proceed.
         msg_type = content["type"].upper()
 
         if msg_type == "CONNECTION_INIT":
             task = self._on_gql_connection_init(payload=content["payload"])
 
         elif msg_type == "CONNECTION_TERMINATE":
             task = self._on_gql_connection_terminate()
 
         elif msg_type == "START":
             op_id = content["id"]
+
             # Create and lock a mutex for this particular operation id,
-            # so STOP processing for the same operation id will wail
+            # so STOP processing for the same operation id will wait
             # until START processing finishes. Locks are stored in a
             # weak collection so we do not have to manually clean it up.
             if op_id in self._operation_locks:
                 raise graphql.error.GraphQLError(
                     f"Operation with msg_id={op_id} is already running!"
                 )
             op_lock = asyncio.Lock()
             self._operation_locks[op_id] = op_lock
             await op_lock.acquire()
 
             async def on_start():
                 try:
-                    await self._on_gql_start(
-                        operation_id=op_id, payload=content["payload"]
-                    )
+                    # User hook which raises to cancel processing.
+                    await self.on_operation(op_id, payload=content["payload"])
+                    # START message processing.
+                    await self._on_gql_start(op_id, payload=content["payload"])
+                except Exception as ex:  # pylint: disable=broad-except
+                    await self._send_gql_error(op_id, ex)
                 finally:
                     op_lock.release()
 
             task = on_start()
 
         elif msg_type == "STOP":
             op_id = content["id"]
 
             async def on_stop():
-                # Will until START message processing finishes, if any.
+                # Wait until START message processing finishes, if any.
                 async with self._operation_locks.setdefault(op_id, asyncio.Lock()):
-                    await self._on_gql_stop(operation_id=op_id)
+                    await self._on_gql_stop(op_id)
 
             task = on_stop()
 
         else:
-            error_msg = f"Message of unknown type '{msg_type}' received!"
             task = self._send_gql_error(
-                content["id"] if "id" in content else -1,
-                error_msg,
+                content["id"] if "id" in content else None,
+                Exception(f"Wrong message type '{msg_type}'!"),
             )
-            LOG.warning("GraphQL WS Client error: %s", error_msg)
 
         # If strict ordering is required then simply wait until the
-        # message processing is finished. Otherwise spawn a task so
+        # message processing finishes. Otherwise spawn a task so
         # Channels may continue calling `receive_json` while requests
         # (i.e. GraphQL documents) are being processed.
         if self.strict_ordering:
             await task
         else:
             self._spawn_background_task(task)
 
     async def broadcast(self, message):
         """The broadcast message handler.
 
-        Method is called when new `broadcast` message received from the
-        Channels group. The message is sent by `Subscription.broadcast`.
-        Here we figure out the group message received from and trigger
-        the observable which makes the subscription process the query
-        and notify the client.
-
-        NOTE: There is an issue in the `channels_redis` implementation
-        which lead to the possibility to receive broadcast messages in
-        wrong order: https://github.com/django/channels_redis/issues/151
-        Currently we recommend to monkey-patch the `channels_redis` to
-        avoid this.
-        """
-        # Assert we run in a proper thread.
-        self._assert_thread()
+        Method is called when new `broadcast` message (sent by
+        `Subscription.broadcast`) received from the Channels group.
 
+        """
         # If strict ordering is required then simply wait until all the
         # broadcast messages are sent. Otherwise spawn a task so this
         # consumer will continue receiving messages.
         if self.strict_ordering:
             await self._process_broadcast(message)
         else:
             self._spawn_background_task(self._process_broadcast(message))
 
     async def _process_broadcast(self, message):
         """Process the broadcast message.
 
+        This triggers subscription notification to all the subscriptions
+        belonging to the group received in the `message`.
+
         NOTE: Depending on the value of the `strict_ordering` setting
         this method is either awaited directly or offloaded to an async
         task by the `broadcast` method (message handler).
         """
-        # Assert we run in a proper thread. In particular, we can access
-        # the `_subscriptions` and `_sids_by_group` without any locks.
-        self._assert_thread()
-
         group = message["group"]
 
         # Do nothing if group does not exist. It is quite possible for
         # a client and a backend to concurrently unsubscribe and send
         # notification. And these events do not need to be synchronized.
         if group not in self._sids_by_group:
             return
@@ -410,468 +468,797 @@
         payload = message["payload"]
 
         # Put the payload to the notification queues of subscriptions
         # belonging to the subscription group. Drop the oldest payloads
         # if the `notification_queue` is full.
         for sid in self._sids_by_group[group]:
             subinf = self._subscriptions[sid]
-            while True:
-                try:
-                    subinf.notification_queue.put_nowait(payload)
-                    break
-                except asyncio.QueueFull:
-                    # The queue is full - issue a warning and throw away
-                    # the oldest item from the queue.
-                    # NOTE: Queue with the size 1 means that it is safe
-                    # to drop intermediate notifications.
-                    if subinf.notification_queue.maxsize != 1:
-                        LOG.warning(
-                            "Subscription notification dropped!"
-                            " Subscription operation id: %s.",
-                            sid,
-                        )
-                    subinf.notification_queue.get_nowait()
+            subinf.enqueue_notification(payload)
 
     async def unsubscribe(self, message):
         """The unsubscribe message handler.
 
         Method is called when new `unsubscribe` message received from
         the Channels group. The message is typically sent by the method
         `Subscription.unsubscribe`. Here we figure out the group message
         received from and stop all the subscriptions in this group.
         """
-        # Assert we run in a proper thread.
-        self._assert_thread()
-
         group = message["group"]
 
         # Do nothing if group does not exist. It is quite possible for
         # a client and a backend to unsubscribe from a subscription
         # concurrently. And these events do not need to be synchronized.
         if group not in self._sids_by_group:
             return
 
         # Send messages which look like user unsubscribes from all
         # subscriptions in the subscription group. This saves us from
         # thinking about raise condition between subscription and
         # unsubscription.
-        await asyncio.wait(
-            [
-                self.receive_json({"type": "stop", "id": sid})
-                for sid in self._sids_by_group[group]
-            ]
-        )
+        if self._sids_by_group[group]:
+            await asyncio.wait(
+                [
+                    asyncio.create_task(self.receive_json({"type": "stop", "id": sid}))
+                    for sid in self._sids_by_group[group]
+                ]
+            )
 
     # ---------------------------------------------------------- GRAPHQL PROTOCOL EVENTS
 
     async def _on_gql_connection_init(self, payload):
         """Process the CONNECTION_INIT message.
 
         Start sending keepalive messages if `send_keepalive_every` set.
         Respond with either CONNECTION_ACK or CONNECTION_ERROR message.
 
         NOTE: Depending on the value of the `strict_ordering` setting
         this method is either awaited directly or offloaded to an async
         task. See the `receive_json` handler.
         """
-        # Assert we run in a proper thread.
-        self._assert_thread()
-
         try:
             # Notify subclass a new client is connected.
             await self.on_connect(payload)
         except Exception as ex:  # pylint: disable=broad-except
-            LOG.error(str(ex))
             await self._send_gql_connection_error(ex)
-            # Close the connection.
-            # NOTE: We use the 4000 code because there are two reasons:
-            # A) We can not use codes greater than 1000 and less than
-            # 3000 because daphne and autobahn do not allow this
-            # (see `sendClose` from `autobahn/websocket/protocol.py`
-            # and `daphne/ws_protocol.py`).
-            # B) https://developer.mozilla.org/en-US/docs/Web/API/CloseEvent
-            # So mozilla offers us the following codes:
-            # 4000–4999 - Available for use by applications.
+            # Close the connection. NOTE: We use the 4000 code because
+            # there are two reasons: A) We can not use codes greater
+            # than 1000 and less than 3000 because Daphne and Autobahn
+            # do not allow this (see `sendClose` from
+            # `autobahn/websocket/protocol.py` and
+            # `daphne/ws_protocol.py`). B)
+            # https://developer.mozilla.org/en-US/docs/Web/API/CloseEvent
+            # Mozilla offers codes 4000–4999 available for all apps.
             await self.close(code=4000)
         else:
             # Send CONNECTION_ACK message.
             await self._send_gql_connection_ack()
             # If keepalive enabled then send one message immediately and
             # schedule periodic messages.
             if self.send_keepalive_every is not None:
+                send_keepalive_every = self.send_keepalive_every
 
                 async def keepalive_sender():
                     """Send keepalive messages periodically."""
                     while True:
-                        await asyncio.sleep(self.send_keepalive_every)
+                        await asyncio.sleep(send_keepalive_every)
                         await self._send_gql_connection_keep_alive()
 
-                self._keepalive_task = asyncio.ensure_future(keepalive_sender())
+                self._keepalive_task = asyncio.create_task(keepalive_sender())
                 # Immediately send keepalive message cause it is
                 # required by the protocol description.
                 await self._send_gql_connection_keep_alive()
 
     async def _on_gql_connection_terminate(self):
         """Process the CONNECTION_TERMINATE message.
 
         NOTE: Depending on the value of the `strict_ordering` setting
         this method is either awaited directly or offloaded to an async
         task. See the `receive_json` handler.
         """
-        # Assert we run in a proper thread.
-        self._assert_thread()
 
         # Close the connection.
         await self.close(code=1000)
 
-    async def _on_gql_start(self, operation_id, payload):
+    async def _on_gql_start(self, op_id, payload):
         """Process the START message.
 
-        Handle the message which holds query, mutation or subscription
-        request.
+        Handle the message with query, mutation or subscription request.
 
         NOTE: Depending on the value of the `strict_ordering` setting
         this method is either awaited directly or offloaded to an async
         task. See the `receive_json` handler.
         """
-        # Assert we run in a proper thread. In particular, we can access
-        # the `_subscriptions` and `_sids_by_group` without any locks.
-        self._assert_thread()
-
         try:
-            if operation_id in self._subscriptions:
-                raise graphql.error.GraphQLError(
-                    f"Subscription with msg_id={operation_id} already exists!"
-                )
+            if op_id in self._subscriptions:
+                message = f"Subscription with msg_id={op_id} already exists!"
+                raise graphql.error.GraphQLError(message)
 
             # Get the message data.
             query = payload["query"]
             op_name = payload.get("operationName")
             variables = payload.get("variables", {})
 
-            # Create object-like context (like in `Query` or `Mutation`)
-            # from the dict-like one provided by the Channels.
-            context = ScopeAsContext(self.scope)
-
-            # Adding channel name to the context because it seems to be
-            # useful for some use cases, take a loot at the issue from
-            # more details:
-            # https://github.com/datadvance/DjangoChannelsGraphqlWs/issues/41#issuecomment-663951595
-            context["channel_name"] = self.channel_name
-
-            # The `register` will be called from the worker thread
-            # (spawned for a GraphQL processing) when a client
-            # subscribes. So we "synchronize" it with `async_to_sync`.
-            # NOTE: It is important to invoke `async_to_sync` in the
-            # thread with the eventloop which serves this consumer. This
-            # assures that IO operations is performed within a single
-            # eventloop.
-            register_subscription = asgiref.sync.async_to_sync(
-                functools.partial(self._register_subscription, operation_id)
-            )
-
-            def register_middleware(next_middleware, root, info, *args, **kwds):
-                """Transfers registration function to the `_subscribe`.
-
-                Check that `next_middleware` is precisely a subscription
-                handler `Subscription._subscribe` and hack it's `root`
-                to deliver the subscription registration function.
+            # Prepare a context object.
+            context = DictAsObject({})
+            context.channels_scope = self.scope
+            context.channel_name = self.channel_name
+
+            # Process the request with Graphene and GraphQL-core.
+            doc_ast, op_ast, errors = await self._on_gql_start__parse_query(
+                op_name, query
+            )
+            if errors:
+                await self._send_gql_data(op_id, None, errors)
+                await self._send_gql_complete(op_id)
+                return
+            # Assert values are not None to suppress MyPy complains.
+            assert doc_ast is not None
+            assert op_ast is not None
+
+            async def unbound_root_middleware(*args, **kwds):
+                """Unbound function for root middleware.
+
+                `graphql.MiddlewareManager` accepts only unbound
+                functions as middleware.
                 """
+                return await self._on_gql_start__root_middleware(
+                    op_id, op_name, *args, **kwds
+                )
 
-                # Avoid circular imports with local import.
-                # pylint: disable=import-outside-toplevel,cyclic-import
-                from .subscription import Subscription
-
-                # We do not expose `Subscription._subscribe` because
-                # `Subscription` is a public interface class. So it OK
-                # to get `Subscription._subscribe` here - we are tightly
-                # coupled anyway.
-                # pylint: disable=protected-access
-                if (
-                    getattr(next_middleware, "__func__", None)
-                    is Subscription._subscribe.__func__
-                ):
-                    root = types.SimpleNamespace(
-                        real_root=root, register_subscription=register_subscription
-                    )
-                return next_middleware(root, info, *args, **kwds)
+            # NOTE: Middlewares order is important, root middleware
+            # should always be the closest to the real resolver (first
+            # in the middleware list).
+            middleware_manager: Optional[
+                graphql.MiddlewareManager
+            ] = graphql.MiddlewareManager(
+                unbound_root_middleware,
+                *self.middleware,
+            )
 
-            # Process the request with Graphene/GraphQL.
+            # If the operation is subscription.
+            if op_ast.operation == graphql.language.ast.OperationType.SUBSCRIPTION:
+                LOG.debug(
+                    "Subscription request. Operation ID: %s, operation name: %s.)",
+                    op_id,
+                    op_name,
+                )
 
-            # Offload the GraphQL processing to the worker thread cause
-            # according to our experiments even GraphQL document parsing
-            # may take a while (and depends approx. linearly on the size
-            # of the selection set). Moreover it is highly probable that
-            # resolvers will invoke blocking DB operations so it is
-            # better to offload the whole thing to a worker thread.
-            # NOTE: The `lambda` is required to force `AsyncioExecutor`
-            # take an eventloop from the worker thread, not the current
-            # one.
-            result = await self._run_in_worker(
-                lambda: graphql.graphql(
-                    self.schema,
-                    request_string=query,
+                # This returns asynchronous generator or ExecutionResult
+                # instance in case of error.
+                subscr_result = await self._on_gql_start__subscribe(
+                    doc_ast,
                     operation_name=op_name,
-                    variables=variables,
-                    context=context,
-                    # NOTE: Wrap with `wrap_in_promise=False`, otherwise
-                    # it raises `GraphQLError` with message:
-                    # "Subscription must return Async Iterable or
-                    # Observable. Received: <Promise...". I do not get
-                    # why it wraps it in promise by default.
-                    middleware=graphql.middlewares(
-                        register_middleware, *self.middleware, wrap_in_promise=False
+                    root_value=None,
+                    variable_values=variables,
+                    context_value=context,
+                    subscribe_field_resolver=functools.partial(
+                        self._on_gql_start__initialize_subscription_stream, op_id
                     ),
-                    allow_subscriptions=True,
-                    executor=graphql.execution.executors.asyncio.AsyncioExecutor(),
+                    middleware=middleware_manager,
+                    execution_context_class=self._SubscriptionExecutionContext,
                 )
-            )
 
-        except Exception:  # pylint: disable=broad-except
-            # Something is wrong - send error message.
-            await self._send_gql_error(operation_id, traceback.format_exc())
+                # When subscr_result is an AsyncGenerator, consume
+                # stream of notifications and send them to clients.
+                if not isinstance(subscr_result, graphql.ExecutionResult):
+                    stream = cast(AsyncIterator[graphql.ExecutionResult], subscr_result)
+                    # Send subscription activation message (if enabled)
+                    # NOTE: We do it before reading the the stream
+                    # stream to guarantee that no notifications are sent
+                    # before the subscription confirmation message.
+                    if self.confirm_subscriptions:
+                        await self._send_gql_data(
+                            op_id,
+                            data=self.subscription_confirmation_message["data"],
+                            errors=self.subscription_confirmation_message["errors"],
+                        )
 
-        else:
-            # Receiving an observer means the subscription has been
-            # processed. Otherwise it is just regular query or mutation.
-            if isinstance(result, rx.Observable):
-                # Client subscribed to a subscription so we subscribe to
-                # the observable returned.
-
-                # Respond with the subscription activation message if
-                # enabled in the consumer configuration.
-                # NOTE: We intentionally do it before subscribing to the
-                # `result` stream. This guarantees that subscription
-                # confirmation message is sent before any subscription
-                # notifications.
-                if self.confirm_subscriptions:
-                    await self._send_gql_data(
-                        operation_id,
-                        data=self.subscription_confirmation_message["data"],
-                        errors=self.subscription_confirmation_message["errors"],
-                    )
+                    consumer_init_done = asyncio.Event()
+
+                    async def consume_stream():
+                        consumer_init_done.set()
+                        try:
+                            async for item in stream:
+                                # Skipped subscription event may have no
+                                # data and no errors. Send message only
+                                # when we have something to send.
+                                if item.data or item.errors:
+                                    try:
+                                        await self._send_gql_data(
+                                            op_id, item.data, item.errors
+                                        )
+                                    except asyncio.CancelledError:
+                                        break
+                        except Exception as ex:  # pylint: disable=broad-except
+                            LOG.debug(
+                                "Exception in the subscription GraphQL resolver!"
+                                "Operation %s(%s).",
+                                op_name,
+                                op_id,
+                                exc_info=ex,
+                            )
+                            await self._send_gql_data(op_id, None, [ex])
+
+                    # We need to end this task when client drops
+                    # connection or unsubscribes, so lets store it.
+                    self._notifier_tasks[op_id] = asyncio.create_task(consume_stream())
+
+                    # We must be sure here that the subscription
+                    # initialization is finished and the stream consumer
+                    # is active before we exit this function. Because in
+                    # the outer scope we have locking mechanism of start
+                    # and stop operations. And we want to say
+                    # "subscription operation is started" only when it
+                    # actually is.
+                    # This allows us to avoid the race condition between
+                    # simultaneous subscribe and unsubscribe calls.
+                    await consumer_init_done.wait()
+                    return
+
+                # Else (when gql_subscribe returns ExecutionResult
+                # containing error) fallback to standard handling below.
+                operation_result = cast(graphql.ExecutionResult, subscr_result)
 
-                # Subscribe to the observable.
-                # NOTE: The function `on_next` is called from a
-                # threadpool which processes all GraphQL requests. So we
-                # wrap `_send_gql_data` into `async_to_sync` here, so
-                # eventually `_send_gql_data` will be invoked from the
-                # current eventloop.
-                send_gql_data = asgiref.sync.async_to_sync(self._send_gql_data)
-                result.subscribe(
-                    lambda r: send_gql_data(operation_id, r.data, r.errors)
+            # If the operation is query or mutation.
+            else:
+                LOG.debug("New query/mutation. Operation %s(%s).", op_name, op_id)
+
+                if self.warn_operation_timeout:
+                    start_time = time.perf_counter()
+
+                # Standard name for "IntrospectionQuery". We might also
+                # check that
+                # `doc_ast.definitions[0].selection_set.selections[0].name.value`
+                # equals to `__schema`. This is a more robust way. But
+                # it will eat up more CPU pre each query. For now lets
+                # check only a query name.
+                if op_name == "IntrospectionQuery":
+                    # No need to call middlewares for the
+                    # IntrospectionQuery. There no real resolvers. Only
+                    # the type information.
+                    middleware_manager = None
+                exec_result = graphql.execution.execute(
+                    self.schema.graphql_schema,
+                    document=doc_ast,
+                    root_value=None,
+                    operation_name=op_name,
+                    variable_values=variables,
+                    context_value=context,
+                    middleware=middleware_manager,
                 )
+                if inspect.isawaitable(exec_result):
+                    exec_result = await exec_result
+                operation_result = cast(graphql.ExecutionResult, exec_result)
+
+                if self.warn_operation_timeout:
+                    duration = time.perf_counter() - start_time
+                    if duration >= self.warn_operation_timeout:
+                        LOG.warning(
+                            "Operation %s(%s) took %.6f seconds. Debug"
+                            " log contains full operation details.",
+                            op_name,
+                            op_id,
+                            duration,
+                        )
+                        LOG.debug(
+                            "Operation %s(%s) took %.6f seconds. Query:"
+                            " %r, variables: %r.",
+                            op_name,
+                            op_id,
+                            duration,
+                            query,
+                            variables,
+                        )
+            # Respond to a query or mutation immediately.
+            await self._send_gql_data(
+                op_id, operation_result.data, operation_result.errors
+            )
+            await self._send_gql_complete(op_id)
 
+        except Exception as ex:  # pylint: disable=broad-except
+            if isinstance(ex, graphql.error.GraphQLError):
+                # Respond with details of GraphQL execution error.
+                LOG.warning(
+                    "GraphQL error! Operation %s(%s).", op_name, op_id, exc_info=True
+                )
+                await self._send_gql_data(op_id, None, [ex])
+                await self._send_gql_complete(op_id)
             else:
-                # Respond to a query or mutation immediately.
+                # Respond with general error responce.
+                await self._send_gql_error(op_id, ex)
+
+    async def _on_gql_start__parse_query(
+        self, op_name: str, query: str
+    ) -> tuple[
+        Optional[graphql.DocumentNode],
+        Optional[graphql.OperationDefinitionNode],
+        Optional[Sequence[graphql.GraphQLError]],
+    ]:
+        """Parse and validate GraphQL query.
+
+        It is highly likely that the same operation will be parsed many
+        times, so this function is wrapped with LRU cache.
+
+        This async function offloads the GraphQL processing to the
+        worker thread cause according to our experiments even GraphQL
+        document parsing and validation take a while and depends approx.
+        linearly on the size of the selection set.
 
-                # If Graphene complains that the request is invalid
-                # (e.g. query contains syntax error), then the `data`
-                # argument is `None` and the 'errors' argument contains
-                # all errors that occurred before or during execution.
-                # The `result` is an instance of the `ExecutionResult`.
-                await self._send_gql_data(operation_id, result.data, result.errors)
-                # Tell the client that the request processing is over.
-                await self._send_gql_complete(operation_id)
+        This is a part of START message processing routine so the name
+        prefixed with `_on_gql_start__` to make this explicit.
 
-    async def _register_subscription(
+        Returns:
+            Tuple with three optional fields:
+                0: AST of parsed GraphQL document.
+                1: GraphQL operation definition.
+                2: Sequence of errors.
+        """
+
+        res = await self.sync_to_async(self._on_gql_start__parse_query_sync_cached)(
+            op_name, query
+        )
+
+        doc_ast: Optional[graphql.DocumentNode] = res[0]
+        op_ast: Optional[graphql.OperationDefinitionNode] = res[1]
+        errors: Optional[Sequence[graphql.GraphQLError]] = res[2]
+
+        return (doc_ast, op_ast, errors)
+
+    @functools.lru_cache(maxsize=128)
+    def _on_gql_start__parse_query_sync_cached(
+        self, op_name: str, query: str
+    ) -> tuple[
+        Optional[graphql.DocumentNode],
+        Optional[graphql.OperationDefinitionNode],
+        Optional[Sequence[graphql.GraphQLError]],
+    ]:
+        """Parse and validate GraphQL query. Cached sync implementation.
+
+        This is a part of START message processing routine so the name
+        prefixed with `_on_gql_start__` to make this explicit.
+        """
+
+        # Parsing.
+        try:
+            doc_ast = graphql.parse(query)
+        except graphql.GraphQLError as ex:
+            return None, None, [ex]
+
+        # Validation.
+        validation_errors: list[graphql.GraphQLError] = graphql.validate(
+            self.schema.graphql_schema, doc_ast
+        )
+        if validation_errors:
+            return None, None, validation_errors
+
+        op_ast = graphql.utilities.get_operation_ast(doc_ast, op_name)
+
+        return doc_ast, op_ast, None
+
+    async def _on_gql_start__subscribe(
         self,
-        operation_id,
-        groups,
-        publish_callback,
-        unsubscribed_callback,
-        notification_queue_limit=None,
+        document: graphql.DocumentNode,
+        root_value: Any = None,
+        context_value: Any = None,
+        variable_values: Optional[dict[str, Any]] = None,
+        operation_name: Optional[str] = None,
+        field_resolver: Optional[graphql.GraphQLFieldResolver] = None,
+        subscribe_field_resolver: Optional[graphql.GraphQLFieldResolver] = None,
+        middleware: graphql.Middleware = None,
+        execution_context_class: Optional[Type[graphql.ExecutionContext]] = None,
+    ) -> Union[AsyncIterator[graphql.ExecutionResult], graphql.ExecutionResult]:
+        """Create a GraphQL subscription.
+
+        This is a copy of `graphql.execution.subscribe.subscribe` from
+        the GraphQL-core library v3.2.3 improved to support middlewares
+        and user defined execution_context_class.
+
+        This is a part of START message processing routine so the name
+        prefixed with `_on_gql_start__` to make this explicit.
+        """
+
+        result_or_stream = await graphql.create_source_event_stream(
+            self.schema.graphql_schema,
+            document,
+            root_value,
+            context_value,
+            variable_values,
+            operation_name,
+            subscribe_field_resolver,
+        )
+        if isinstance(result_or_stream, graphql.ExecutionResult):
+            return result_or_stream
+
+        async def map_source_to_response(payload: Any) -> graphql.ExecutionResult:
+            """Map source to response.
+
+            For each payload yielded from a subscription, map it over
+            the normal GraphQL :func:`~graphql.execute` function, with
+            `payload` as the `root_value`. This implements the
+            "MapSourceToResponseEvent" algorithm described in the
+            GraphQL specification. The :func:`~graphql.execute` function
+            provides the "ExecuteSubscriptionEvent" algorithm, as it is
+            nearly identical to the "ExecuteQuery" algorithm, for which
+            :func:`~graphql.execute` is also used.
+            """
+            result = graphql.execute(
+                self.schema.graphql_schema,
+                document,
+                payload,
+                context_value,
+                variable_values,
+                operation_name,
+                field_resolver,
+                middleware=middleware,
+                execution_context_class=execution_context_class,
+            )  # type: ignore
+            result = await result if inspect.isawaitable(result) else result
+            return cast(graphql.ExecutionResult, result)
+
+        # Map every source value to a ExecutionResult value.
+        return graphql.MapAsyncIterator(result_or_stream, map_source_to_response)
+
+    async def _on_gql_start__root_middleware(
+        self,
+        operation_id: int,
+        operation_name: str,
+        next_middleware,
+        root,
+        info: graphql.GraphQLResolveInfo,
+        *args,
+        **kwds,
     ):
-        """Register a new subscription when client subscribes.
+        """Root middleware injected right before resolver invocation.
+
+        This middleware is here to do two things:
+        1. Offload sync resolvers to the thread out of main event loop.
+        2. Issue a warning if resolver execution time exceeds a limit.
+
+        It is highly probable that resolvers will invoke
+        blocking operations, e.g. database operations. To avoid
+        blocking eventloop this method offloads sync resolvers
+        to the thread pool wrapping it into sync_to_async.
+
+        Since this middleware always comes first in the list of
+        middlewares, it always receives resolver as the first
+        argument instead of another middleware.
 
-        This function is called (by the subscription implementation -
-        "resolver" function `_subscribe`) when a client subscribes to
-        register necessary callbacks.
+        This is a part of START message processing routine so the name
+        prefixed with `_on_gql_start__` to make this explicit.
 
         Args:
-            operation_id: If of the protocol operation.
-            groups: A list of subscription group names to put the
-                subscription into.
-            publish_callback: Called to process the notification (invoke
-                GraphQL resolvers). The callback will be associated with
-                a Channels groups used to deliver messages to the
-                subscription groups current subscription belongs to.
-            unsubscribed_callback: Called to notify when a client
-                unsubscribes.
-            notification_queue_limit: LImit for the subscribtion
-                notification queue. Default is used if not set.
-
-        """
-        # NOTE: It is important to invoke `group_add` from an
-        # eventloop which serves the current consumer. Besides
-        # this is a "proper" way of doing async things, it is
-        # also crucial for at least one Channels layer
-        # implementation - for the `channels_rabbitmq`. See:
-        # https://github.com/CJWorkbench/channels_rabbitmq/issues/3
-        # Moreover this allows us to access the `_subscriptions` and
-        # `_sids_by_group` without any locks.
-        self._assert_thread()
+            resolver: Resolver to "wrap" into this middleware
+            root: Anything. Eventually passed to the resolver.
+            info: Passed to the resolver.
 
-        # The subject we will trigger on the `broadcast` message.
-        trigger = rx.subjects.Subject()
+        Returns:
+            Any value: result returned by the resolver.
+            AsyncGenerator: when subscription starts.
+        """
 
-        # The subscription notification queue.
-        queue_size = notification_queue_limit
+        # Unwrap resolver from functools.partial or other wrappers.
+        real_resolver = self._on_gql_start__unwrap(next_middleware)
+        module = getattr(real_resolver, "__module__", "")
+
+        # Do not offload async resolvers and resolvers from
+        # GraphQL-core/Graphene since they are not blocking.
+        if (
+            not module.startswith("graphql.type.")
+            and not module.startswith("graphene.types.")
+            and not asyncio.iscoroutinefunction(real_resolver)
+        ):
+            # Offload synchronous resolvers.
+            @functools.wraps(next_middleware)
+            def wrapped_next_middleware(root, info, *args, **kwds):
+                result = next_middleware(root, info, *args, **kwds)
+                # Manually evaluate QuerySet, otherwise we will
+                # eventually receive SynchronousOnlyOperation error:
+                # "You cannot call this from an async context - use a
+                # thread or sync_to_async.". This happens when
+                # unevaluated QuerySet moves out of its sync context.
+                if isinstance(result, django.db.models.query.QuerySet):
+                    result = list(result)
+                return result
+
+            next_resolver = self.sync_to_async(wrapped_next_middleware)
+        else:
+            next_resolver = next_middleware
+
+        # Start measuring resolver execution time.
+        if self.warn_resolver_timeout:
+            start_time = time.perf_counter()
+
+        # Execute resolver.
+        result = next_resolver(root, info, *args, **kwds)
+        if inspect.isawaitable(result):
+            result = await result
+
+        # Warn about long resolver execution if the time limit exceeds.
+        if self.warn_resolver_timeout:
+            duration = time.perf_counter() - start_time
+            if duration >= self.warn_resolver_timeout:
+                pretty_name = f"{real_resolver.__qualname__}"
+                if hasattr(real_resolver, "__self__"):
+                    pretty_name = f"{real_resolver.__self__.__qualname__}.{pretty_name}"
+                LOG.warning(
+                    "Resolver %s took %.3f seconds (>%.3f)!"
+                    " Operation %s(%s), path: %s.",
+                    pretty_name,
+                    duration,
+                    self.warn_resolver_timeout,
+                    operation_name,
+                    operation_id,
+                    info.path,
+                )
+
+        return result
+
+    def _on_gql_start__unwrap(self, fn: Callable) -> Callable:
+        """Auxiliary method which unwraps given function.
+
+        This is a part of START message processing routine so the name
+        prefixed with `_on_gql_start__` to make this explicit.
+        """
+        if isinstance(fn, functools.partial):
+            fn = self._on_gql_start__unwrap(fn.func)
+        elif hasattr(fn, "__wrapped__"):
+            fn = self._on_gql_start__unwrap(fn.__wrapped__)
+        return fn
+
+    async def _on_gql_start__initialize_subscription_stream(
+        self, op_id: int, root: Any, info: graphql.GraphQLResolveInfo, *args, **kwds
+    ):
+        """Create asynchronous generator with subscription events.
+
+        Called inside `_on_gql_start__subscribe` function by
+        graphql-core as `subscribe_field_resolver` argument.
+
+        This is a part of START message processing routine so the name
+        prefixed with `_on_gql_start__` to make this explicit.
+        """
+        # Graphene stores original subscription class in `graphene_type`
+        # field of `return_type` object. Since subscriptions are build
+        # on top of `graphene` we always have graphene specific
+        # `return_type` class.
+        subscription_class = info.return_type.graphene_type  # type: ignore[union-attr]
+
+        # It is ok to access private fields of `Subscription`
+        # implementation. `Subscription` class used to create
+        # subscriptions as graphene object but actually it is a part of
+        # consumer implementation.
+        # pylint: disable=protected-access
+
+        # Attach current subscription to the group corresponding to
+        # the concrete class. This allows to trigger all the
+        # subscriptions of the current type, by invoking `publish`
+        # without setting the `group` argument.
+        groups = [subscription_class._group_name()]
+
+        # Invoke the subclass-specified `subscribe` method to get
+        # the groups subscription must be attached to.
+        if subscription_class._meta.subscribe is not None:
+            subclass_groups = subscription_class._meta.subscribe(
+                root, info, *args, **kwds
+            )
+            # Properly handle `async def subscribe`.
+            if asyncio.iscoroutinefunction(subscription_class._meta.subscribe):
+                subclass_groups = await subclass_groups
+            assert subclass_groups is None or isinstance(
+                subclass_groups, (list, tuple)
+            ), (
+                f"Method 'subscribe' returned a value of an incorrect type"
+                f" {type(subclass_groups)}! A list, a tuple, or 'None' expected."
+            )
+            subclass_groups = subclass_groups or []
+        else:
+            subclass_groups = []
+
+        groups += [subscription_class._group_name(group) for group in subclass_groups]
+
+        # The subscription notification queue. Required to preserve the
+        # order of notifications within a single subscription.
+        queue_size = subscription_class.notification_queue_limit
         if not queue_size or queue_size < 0:
+            # Take default limit from the Consumer class.
             queue_size = self.subscription_notification_queue_limit
-        notification_queue = asyncio.Queue(maxsize=queue_size)
+        # The subscription notification queue.
+        # NOTE: The asyncio.Queue class is not thread-safe. So use the
+        # `notification_queue_lock` as a guard while reading or writing
+        # to the queue.
+        notification_queue: asyncio.Queue = asyncio.Queue(maxsize=queue_size)
+        # Lock to ensure that `notification_queue` operations are
+        # thread safe.
+        notification_queue_lock = threading.RLock()
+
+        unsubscribed = subscription_class._meta.unsubscribed
+
+        async def unsubscribed_callback():
+            """Call `unsubscribed` notification.
+
+            The `cls._meta.unsubscribed` might do blocking operations,
+            so offload it to the thread.
+            """
+
+            if unsubscribed is None:
+                return None
+            # Properly handle `async def unsubscribed`.
+            if asyncio.iscoroutinefunction(unsubscribed):
+                await unsubscribed(None, info, *args, **kwds)
+            else:
+                await self.sync_to_async(unsubscribed)(None, info, *args, **kwds)
 
-        # Start an endless task which listens the `notification_queue`
-        # and invokes subscription "resolver" on new notifications.
-        async def notifier():
-            """Watch the notification queue and notify clients."""
+        def enqueue_notification(payload):
+            """Put notification to the queue.
 
-            # Assert we run in a proper thread.
-            self._assert_thread()
+            Called by the WebSocket consumer (instance of the
+            GraphqlWsConsumer subclass) when it receives the broadcast
+            message (from the Channels group) sent by the
+            Subscription.broadcast.
+
+            Args:
+                sid: Operation id of the subscription.
+            """
             while True:
-                payload = await notification_queue.get()
-                # Run a subscription's `publish` method (invoked by the
-                # `trigger.on_next` function) within the threadpool used
-                # for processing other GraphQL resolver functions.
-                # NOTE: `lambda` is important to run the deserialization
-                # in the worker thread as well.
-                await self._run_in_worker(
-                    lambda: trigger.on_next(Serializer.deserialize(payload))
-                )
-                # Message processed. This allows `Queue.join` to work.
-                notification_queue.task_done()
+                with notification_queue_lock:
+                    try:
+                        notification_queue.put_nowait(payload)
+                        break  # The item was enqueued. Exit the loop.
+                    except asyncio.QueueFull:
+                        # The queue is full - issue a warning and throw
+                        # away the oldest item from the queue.
+                        # NOTE: Queue with the size 1 means that it is
+                        # safe to drop intermediate notifications.
+                        if notification_queue.maxsize != 1:
+                            LOG.warning(
+                                "Subscription notification dropped!"
+                                " Operation %s(%s).",
+                                info.context.graphql_operation_name,
+                                info.context.graphql_operation_id,
+                            )
+                        notification_queue.get_nowait()
+                        notification_queue.task_done()
+
+                        # Try to put the incoming item to the queue
+                        # within the same lock. This is an speed
+                        # optimization.
+                        try:
+                            notification_queue.put_nowait(payload)
+                            # The item was enqueued. Exit the loop.
+                            break
+                        except asyncio.QueueFull:
+                            # Kind'a impossible to get here, but if we
+                            # do, then we should retry until the queue
+                            # have capacity to process item.
+                            pass
 
-        # Enqueue the `publish` method execution. But do not notify
-        # clients when `publish` returns `SKIP`.
-        stream = trigger.map(publish_callback).filter(  # pylint: disable=no-member
-            lambda publish_returned: publish_returned is not self.SKIP
-        )
-
-        # Start listening for broadcasts (subscribe to the Channels
-        # groups), spawn the notification processing task and put
-        # subscription information into the registry.
-        # NOTE: Update of `_sids_by_group` & `_subscriptions` must be
-        # atomic i.e. without `awaits` in between.
         waitlist = []
         for group in groups:
-            self._sids_by_group.setdefault(group, []).append(operation_id)
-            waitlist.append(self._channel_layer.group_add(group, self.channel_name))
-        notifier_task = self._spawn_background_task(notifier())
-        self._subscriptions[operation_id] = self._SubInf(
+            self._sids_by_group.setdefault(group, []).append(op_id)
+            waitlist.append(
+                asyncio.create_task(
+                    self._channel_layer.group_add(group, self.channel_name)
+                )
+            )
+        self._subscriptions[op_id] = self._SubInf(
             groups=groups,
-            sid=operation_id,
+            sid=op_id,
             unsubscribed_callback=unsubscribed_callback,
-            notification_queue=notification_queue,
-            notifier_task=notifier_task,
+            enqueue_notification=enqueue_notification,
         )
+        if waitlist:
+            await asyncio.wait(waitlist)
 
-        await asyncio.wait(waitlist)
+        _deserialize = channels.db.database_sync_to_async(Serializer.deserialize)
 
-        return stream
+        # For each notification (event) yielded from this function the
+        # `_on_gql_start__subscribe` function will call subscription
+        # resolver (`publish`) via `graphql.execute` method.
+        while True:
+            with notification_queue_lock:
+                payload = await notification_queue.get()
+            data = await _deserialize(payload)
+            yield data
+            with notification_queue_lock:
+                notification_queue.task_done()
 
-    async def _on_gql_stop(self, operation_id):
+    async def _on_gql_stop(self, op_id):
         """Process the STOP message.
 
         Handle an unsubscribe request.
 
         NOTE: Depending on the value of the `strict_ordering` setting
         this method is either awaited directly or offloaded to an async
         task. See the `receive_json` handler.
         """
-        # Assert we run in a proper thread. In particular, we can access
-        # the `_subscriptions` and `_sids_by_group` without any locks.
-        self._assert_thread()
+        LOG.debug("Stop handling or unsubscribe operation %s.", op_id)
 
         # Currently only subscriptions can be stopped. But we see but
         # some clients (e.g. GraphiQL) send the stop message even for
         # queries and mutations. We also see that the Apollo server
         # ignores such messages, so we ignore them as well.
-        if operation_id not in self._subscriptions:
+        if op_id not in self._subscriptions:
             return
 
-        # Unsubscribe:
-        # - Throw away the subscription from the registry.
-        # - Cancel the task which watches over the notification queue.
-        # - Stop listening corresponding groups.
-        waitlist = []
-        subinf = self._subscriptions.pop(operation_id)
-        subinf.notifier_task.cancel()
-        waitlist.append(subinf.notifier_task)
+        waitlist: list[asyncio.Task] = []
+
+        # Remove the subscription from the registry.
+        subinf = self._subscriptions.pop(op_id)
+
+        # Cancel the task which watches the notification queue.
+        consumer_task = self._notifier_tasks.pop(op_id, None)
+        if consumer_task:
+            consumer_task.cancel()
+            waitlist.append(consumer_task)
+
+        # Stop listening for corresponding groups.
         for group in subinf.groups:
             # Remove the subscription from groups it belongs to. Remove
             # the group itself from the `_sids_by_group` if there are no
             # subscriptions left in it.
-            assert self._sids_by_group[group].count(operation_id) == 1, (
+            assert self._sids_by_group[group].count(op_id) == 1, (
                 f"Registry is inconsistent: group '{group}' has "
-                f"{self._sids_by_group[group].count(operation_id)} "
-                "occurrences of operation_id={operation_id}!"
+                f"{self._sids_by_group[group].count(op_id)} "
+                "occurrences of op_id={op_id}!"
             )
-            self._sids_by_group[group].remove(operation_id)
+            self._sids_by_group[group].remove(op_id)
             if not self._sids_by_group[group]:
                 del self._sids_by_group[group]
                 waitlist.append(
-                    self._channel_layer.group_discard(group, self.channel_name)
+                    asyncio.create_task(
+                        self._channel_layer.group_discard(group, self.channel_name)
+                    )
                 )
-        await asyncio.wait(waitlist)
 
-        # Call the subscription class `unsubscribed` handler in a worker
-        # thread, cause it may invoke long-running synchronous tasks.
-        await self._run_in_worker(subinf.unsubscribed_callback)
+        if waitlist:
+            await asyncio.wait(waitlist)
+
+        await subinf.unsubscribed_callback()
 
         # Send the unsubscription confirmation message.
-        await self._send_gql_complete(operation_id)
+        await self._send_gql_complete(op_id)
 
     # -------------------------------------------------------- GRAPHQL PROTOCOL MESSAGES
 
     async def _send_gql_connection_ack(self):
         """Sent in reply to the `connection_init` request."""
-        self._assert_thread()
         await self.send_json({"type": "connection_ack"})
 
     async def _send_gql_connection_error(self, error: Exception):
         """Connection error sent in reply to the `connection_init`."""
-        self._assert_thread()
+        LOG.warning("GraphQL connection error: %s!", error, exc_info=error)
         await self.send_json(
             {"type": "connection_error", "payload": self._format_error(error)}
         )
 
     async def _send_gql_data(
-        self, operation_id, data: dict, errors: Optional[Sequence[Exception]]
+        self, op_id, data: Optional[dict], errors: Optional[Sequence[Exception]]
     ):
         """Send GraphQL `data` message to the client.
 
         Args:
             data: Dict with GraphQL query response.
             errors: List of exceptions occurred during processing the
                 GraphQL query. (Errors happened in resolvers.)
-
         """
-        self._assert_thread()
         # Log errors with tracebacks so we can understand what happened
         # in a failed resolver.
         for ex in errors or []:
             # Typical exception here is `GraphQLLocatedError` which has
             # reference to the original error raised from a resolver.
             tb = ex.__traceback__
-            if (
-                isinstance(ex, graphql.error.located_error.GraphQLLocatedError)
-                and ex.original_error is not None
-            ):
-                tb = ex.stack
-                ex = ex.original_error
-            LOG.error(
-                "GraphQL resolver failed on operation with id=%s:\n%s",
-                operation_id,
+            LOG.warning(
+                "GraphQL resolver failed! Operation id: %s:\n%s",
+                op_id,
                 "".join(traceback.format_exception(type(ex), ex, tb)).strip(),
             )
 
         await self.send_json(
             {
                 "type": "data",
-                "id": operation_id,
+                "id": op_id,
                 "payload": {
                     "data": data,
                     **(
                         {
                             "errors": [  # type: ignore
                                 self._format_error(e) for e in errors
                             ]
@@ -879,132 +1266,123 @@
                         if errors
                         else {}
                     ),
                 },
             }
         )
 
-    async def _send_gql_error(self, operation_id, error: str):
+    async def _send_gql_error(self, op_id, error: Exception):
         """Tell client there is a query processing error.
 
         Server sends this message upon a failing operation.
         It can be an unexpected or unexplained GraphQL execution error
         or a bug in the code. It is unlikely that this is GraphQL
         validation errors (such errors are part of data message and
         must be sent by the `_send_gql_data` method).
 
         Args:
-            operation_id: Id of the operation that failed on the server.
+            op_id: Id of the operation that failed on the server.
             error: String with the information about the error.
 
         """
-        self._assert_thread()
-        LOG.error("GraphQL query processing error: %s", error)
+        LOG.warning("Operation %s processing error: %s!", op_id, error, exc_info=error)
+        formatted_error = self._format_error(error)
         await self.send_json(
-            {"type": "error", "id": operation_id, "payload": {"errors": [error]}}
+            {
+                "type": "error",
+                "id": op_id,
+                "payload": {"errors": [formatted_error]},
+            }
         )
 
-    async def _send_gql_complete(self, operation_id):
+    async def _send_gql_complete(self, op_id):
         """Send GraphQL `complete` message to the client.
 
         Args:
-            operation_id: If of the corresponding operation.
+            op_id: Id of the corresponding operation.
 
         """
-        self._assert_thread()
-        await self.send_json({"type": "complete", "id": operation_id})
+        await self.send_json({"type": "complete", "id": op_id})
 
     async def _send_gql_connection_keep_alive(self):
         """Send the keepalive (ping) message."""
-        self._assert_thread()
         await self.send_json({"type": "ka"})
 
-    # ------------------------------------------------------------------------ AUXILIARY
+    # ---------------------------------------------------------------------- AUXILIARIES
 
     @staticmethod
-    def _format_error(error: Exception) -> Dict[str, Any]:
-        """Format given exception `error` to send over a network."""
-        if isinstance(error, graphql.error.GraphQLError):
-            return dict(graphql.error.format_error(error))
-
-        return {"message": f"{type(error).__name__}: {str(error)}"}
-
-    async def _run_in_worker(self, func):
-        """Run a function in a thread with an event loop.
+    def _format_error(error: Exception) -> graphql.GraphQLFormattedError:
+        """Format given exception `error` to send over a network.
 
-        Run the `func` in a thread within a thread pool and wait for it
-        to finish. Each such thread has initialized event loop which is
-        NOT running. So the `func` can use it, for example by running
-        `asyncio.get_event_loop().run_until_complete(...)`. We also
-        cleanup Django database connections when `func` finishes.
+        This function will add the "extensions.code" field containing an
+        exception class name. A frontend may use this value to handle
+        errors properly.
 
-        Args:
-            func: The function to run in a thread.
+        If your backend throws an Exception, then an error will be formatted
+        for a client like this:
+            {
+                "id": "NNN",
+                "type": "data",
+                "payload": {
+                    "data": {...},
+                    "errors": [{
+                        "message": "Test error",
+                        "locations": [{"line": NNN, "column": NNN}],
+                        "path": ["somepath"],
+                        "extensions": {"code": "Exception"}
+                    }]
+                }
+            }
 
-        Returns:
-            The result of the `func` invocation.
+        If you define custom exception class (`class
+        CustomErr(Exception)`), then the error code in the "extensions"
+        field will equals to the "CustomErr":
+            "extensions": {"code": "Exception"}
+
+        There is a special case of errors on connection. They behave
+        using same logic: in the "code" field there will be an
+        exception class name:
+            {
+                "payload": {
+                    "message": "message from a exception",
+                    "extensions": {"code": "UserUnauthenticatedError"}
+                },
+                "type": "connection_error"
+            }
 
+        NOTE: If you need to add more fields to the error, then override
+        this function in a subclass. Another way to enrich errors is to
+        use a GraphQLError based classes for your exceptions.
         """
-        # Assert we run in a proper thread.
-        self._assert_thread()
-
-        def thread_func():
-            """Wrap the `func` to init eventloop and to cleanup."""
-            # Create an eventloop if this worker thread does not have
-            # one yet. Eventually each worker will have its own
-            # eventloop so `func` can use it.
-            try:
-                loop = asyncio.get_event_loop()
-            except RuntimeError:
-                loop = asyncio.new_event_loop()
-                # Force the event loop of the worker thread have a
-                # single-threaded default executor, otherwise the total
-                # number of threads may (and will) grow up to the value
-                # of `default_max_workers * default_max_workers` for
-                # each `GraphqlWsConsumer` subclass!
-                loop.set_default_executor(
-                    concurrent.futures.ThreadPoolExecutor(max_workers=1)
-                )
-                asyncio.set_event_loop(loop)
-
-            # Run a given function in a thread.
-            try:
-                return func()
-            finally:
-                # The `func` can open the connections to the database
-                # so let's close them. Django Channels does the same in
-                # the `channels.db.database_sync_to_async`.
-                django.db.close_old_connections()
-
-        return await asyncio.get_event_loop().run_in_executor(
-            self._workers, thread_func
-        )
-
-    def _assert_thread(self):
-        """Assert called from our thread with the eventloop."""
-
-        assert asyncio.get_event_loop() == self._eventloop, (
-            "Function is called from an inappropriate thread! This"
-            " function must be called from the thread where the"
-            " eventloop serving the consumer is running."
-        )
+        if isinstance(error, graphql.error.GraphQLError):
+            if error.extensions and "code" not in error.extensions:
+                if error.original_error:
+                    error.extensions["code"] = type(error.original_error).__name__
+            return error.formatted
+
+        # Usually the GraphQL-core library wraps any exception with
+        # GraphQLError. So this code should be unreachable, unless there
+        # are some bugs in the library.
+        return {
+            "message": f"{type(error).__name__}: {str(error)}",
+            "extensions": {"code": type(error).__name__},
+        }
 
     def _spawn_background_task(self, awaitable):
         """Spawn background task.
 
         Tasks are canceled and awaited when a client disconnects.
         Args:
             awaitable: An awaitable to run in a task.
         Returns:
             A started `asyncio.Task` instance.
 
         """
-        background_task = asyncio.ensure_future(awaitable)
+        background_task = asyncio.create_task(awaitable)
         self._background_tasks.add(background_task)
-
         return background_task
 
     @property
     def _channel_layer(self):
         """Channel layer."""
         # We cannot simply check existence of channel layer in the
         # consumer constructor, so we added this property.
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/scope_as_context.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/dict_as_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2010-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -15,29 +15,29 @@
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-"""Wrapper for the Channels scope."""
+"""Dict wrapper to access keys as attributes."""
 
 
-class ScopeAsContext:
-    """Wrapper to make Channels `scope` appear as an `info.context`."""
+class DictAsObject:
+    """Dict wrapper to access keys as attributes."""
 
     def __init__(self, scope):
         """Remember given `scope`."""
         self._scope = scope
 
     def _asdict(self):
         """Provide inner Channels scope object."""
         return self._scope
 
-    # ---------------------------------------------------------------- WRAPPER FUNCTIONS
+    # ------------------------------------------------ WRAPPER FUNCTIONS
     def __getattr__(self, name):
         """Route attributes to the scope object."""
         if name.startswith("_"):
             raise AttributeError()
         try:
             return self._scope[name]
         except KeyError as ex:
@@ -45,15 +45,15 @@
 
     def __setattr__(self, name, value):
         """Route attributes to the scope object."""
         if name.startswith("_"):
             super().__setattr__(name, value)
         self._scope[name] = value
 
-    # --------------------------------------------------------------------- DICT WRAPPER
+    # ----------------------------------------------------- DICT WRAPPER
     def __getitem__(self, key):
         """Wrap dict method."""
         return self._scope[key]
 
     def __setitem__(self, key, value):
         """Wrap dict method."""
         self._scope[key] = value
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/serializer.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2010-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/subscription.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/subscription.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2010-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -24,16 +24,16 @@
 The `Subscription` class itself is a "creative" copy of `Mutation` class
 from the Graphene (`graphene/types/mutation.py`).
 """
 
 import asyncio
 import collections
 import hashlib
-import inspect
 import logging
+from typing import Optional
 
 import asgiref.sync
 import channels.db
 import channels.layers
 import graphene
 import graphene.types.objecttype
 import graphene.types.utils
@@ -46,58 +46,68 @@
 # Module logger.
 LOG = logging.getLogger(__name__)
 
 
 class Subscription(graphene.ObjectType):
     """Subscription type definition.
 
-    Subclass this class to define a GraphQL subscription. The class
-    works with `GraphqlWsConsumer` which maintains a WebSocket
-    connection with the client.
+    Subclass this the Subscription class to define a GraphQL
+    subscription. The class works with the `GraphqlWsConsumer` which
+    maintains a WebSocket connection with the client.
 
     The subclass specifies the following methods. You can define each of
     them as a `@classmethod`, as a `@staticmethod`, or even as a regular
     method (like Graphene typically does). It shall work fine either
     way. NOTE, if you define the method as a regular method (not a
     classmethod or a staticmethod) you will receive the first argument
     (`payload`/`root`) into the `self` argument.
 
         [async] publish(payload, info, *args, **kwds):
             This method invoked each time subscription "triggers".
             Raising an exception here will lead to sending the
-            notification with the error. To suppress the notification
-            return `Subscription.SKIP`.
-
-            Can be implemented both as a synchronous or as a coroutine
-            function. In both cases a method runs in a worker thread
-            from the GraphQL-processing threadpool.
+            notification with the error. Technically the WebSocket
+            message will contain extra field "extensions.code" holding
+            the classname of the exception raised. To suppress the
+            notification return `Subscription.SKIP`.
+
+            Can be implemented as both asynchronous (`async def`) or
+            synchronous (`def`) function. Asynchronous implementation
+            runs blazingly fast in the main event loop of the main
+            thread. You must be careful with blocking calls though. You
+            can offload blocking operations to a thread in such cases.
+            Synchronous implementation always runs in a worker thread
+            which comes with a price of extra overhead.
 
             Required.
 
             Args:
                 payload: The `payload` from the `broadcast` invocation.
                 info: The value of `info.context` is a Channels
                     websocket context with all the connection
                     information.
                 args, kwds: Values of the GraphQL subscription inputs.
             Returns:
-                The same the any Graphene resolver returns. Returning
-                a special object `Subscription.SKIP` indicates that this
-                notification shall not be sent to the client at all.
+                The same that any Graphene resolver returns. Returning a
+                special object `Subscription.SKIP` indicates that this
+                notification must not be sent to the client at all.
 
         [async] subscribe(root, info, *args, **kwds):
             Called when client subscribes. Define this to do some extra
             work when client subscribes and to group subscriptions into
             different subscription groups. Method signature is the same
-            as in other GraphQL "resolver" methods but it may return
-            the subscription groups names to put the subscription into.
+            as in other GraphQL "resolver" methods but it may return the
+            subscription groups names to put the subscription into.
 
-            Can be implemented both as a synchronous or as a coroutine
-            function. In both cases a method runs in a worker thread
-            from the GraphQL-processing threadpool.
+            Can be implemented as both asynchronous (`async def`) or
+            synchronous (`def`) function. Asynchronous implementation
+            runs blazingly fast in the main event loop of the main
+            thread. You must be careful with blocking calls though. You
+            can offload blocking operations to a thread in such cases.
+            Synchronous implementation always runs in a worker thread
+            which comes with a price of extra overhead.
 
             Optional.
 
             Args:
                 root: Root resolver object. Typically `None`.
                 info: The value of `info.context` is a Channels
                     websocket context with all the connection
@@ -112,17 +122,21 @@
                 subscription is only put to the default group (the one
                 which corresponds to the `Subscription` subclass).
 
         [async] unsubscribed(root, info, *args, **kwds):
             Called when client unsubscribes. Define this to be notified
             when client unsubscribes.
 
-            Can be implemented both as a synchronous or as a coroutine
-            function. In both cases a method runs in a worker thread
-            from the GraphQL-processing threadpool.
+            Can be implemented as both asynchronous (`async def`) or
+            synchronous (`def`) function. Asynchronous implementation
+            runs blazingly fast in the main event loop of the main
+            thread. You must be careful with blocking calls though. You
+            can offload blocking operations to a thread in such cases.
+            Synchronous implementation always runs in a worker thread
+            which comes with a price of extra overhead.
 
             Args:
                 root: Always `None`.
                 info: The value of `info.context` is a Channels
                     websocket context with all the connection
                     information.
                 args, kwds: Values of the GraphQL subscription inputs.
@@ -130,85 +144,75 @@
     The methods enlisted above receives "standard" set of GraphQL
     resolver arguments. The `info` field has `context` which can be used
     to transmit some useful payload between these methods. For example
     if `subscribe` sets `info.context.zen=42` then `publish` will have
     access to this value as `info.context.zen`.
 
     Static methods of subscription subclass:
-        broadcast: Call this method to notify all subscriptions in the
-            group.
-        unsubscribe: Call this method to stop all subscriptions in the
-            group.
+        broadcast(): Call this to notify all subscriptions in the group.
+        unsubscribe(): Call this to stop all subscriptions in the group.
+
     NOTE: If you call any of these methods from the asynchronous context
     then `await` the result of the call.
-
     """
 
     # ----------------------------------------------------------------------- PUBLIC API
 
     # Return this from the `publish` to suppress the notification.
     SKIP = GraphqlWsConsumer.SKIP
 
     # Subscription notifications queue limit. Set this to control the
-    # amount of notifications server keeps in queue when notifications
-    # come faster than server processing them. Set this limit to 1 drops
-    # all notifications in queue except the latest one. Use this only if
-    # you are sure that subscription always returns all required state
-    # to the client and client does not loose information when
-    # intermediate notification is missed.
-    notification_queue_limit = None
+    # amount of notifications server keeps in the queue when
+    # notifications come faster than server processes them. Setting this
+    # to 1 drops all notifications in the queue except the latest one.
+    # Useful to skip intermediate notifications, e.g. progress reports.
+    notification_queue_limit: Optional[int] = None
 
     @classmethod
     def broadcast(cls, *, group=None, payload=None):
         """Call this method to notify all subscriptions in the group.
 
-        This method can be called from both synchronous and asynchronous
-        contexts. If you call it from the asynchronous context then you
-        have to `await`.
+        Can be called from both synchronous and asynchronous contexts.
+
+        It is necessary to `await` if called from the async context.
 
         Args:
             group: Name of the subscription group which members must be
                 notified. `None` means that all the subscriptions of
                 type will be triggered.
             payload: The payload delivered to the `publish` handler.
-                NOTE: The `payload` is serialized before sending
-                to the subscription group.
+                NOTE: The `payload` is serialized before sending to the
+                subscription group.
 
         """
         try:
             event_loop = asyncio.get_event_loop()
         except RuntimeError:
             pass
         else:
             if event_loop.is_running():
-                assert cls._from_coroutine(), (
-                    "The eventloop is running so this call is going to return"
-                    " a coroutine object, but the function is called from"
-                    " a synchronous context, so you cannot simply 'await' the result!"
-                    " This may indicate a wrong usage. To force some particular"
-                    " behavior directly call 'broadcast_sync' or 'broadcast_async'."
+                return event_loop.create_task(
+                    cls.broadcast_async(group=group, payload=payload)
                 )
-                return cls.broadcast_async(group=group, payload=payload)
 
         return cls.broadcast_sync(group=group, payload=payload)
 
     @classmethod
     async def broadcast_async(cls, *, group=None, payload=None):
         """Broadcast, asynchronous version."""
-        # Offload to the thread cause it do DB operations and may work
-        # slowly.
-        db_sync_to_async = channels.db.database_sync_to_async
-
         # Manually serialize the `payload` to allow transfer of Django
-        # models inside the `payload`.
-        serialized_payload = await db_sync_to_async(Serializer.serialize)(payload)
+        # models inside `payload`, auto serialization does not do this.
+        serialized_payload = await channels.db.database_sync_to_async(
+            Serializer.serialize
+        )(payload)
 
         # Send the message to the Channels group.
         group = cls._group_name(group)
         group_send = cls._channel_layer().group_send
+        # Will result in a call of `GraphqlWsConsumer.broadcast`.
         await group_send(
             group=group,
             message={
                 "type": "broadcast",
                 "group": group,
                 "payload": serialized_payload,
             },
@@ -217,18 +221,20 @@
     @classmethod
     def broadcast_sync(cls, *, group=None, payload=None):
         """Broadcast, synchronous version."""
         # Manually serialize the `payload` to allow transfer of Django
         # models inside the `payload`.
         serialized_payload = Serializer.serialize(payload)
 
-        # Send the message to the Channels group.
         group = cls._group_name(group)
-        group_send = asgiref.sync.async_to_sync(cls._channel_layer().group_send)
-        group_send(
+        sync_channel_layer_group_send = asgiref.sync.async_to_sync(
+            cls._channel_layer().group_send
+        )
+        # Will result in a call of `GraphqlWsConsumer.broadcast`.
+        sync_channel_layer_group_send(
             group=group,
             message={
                 "type": "broadcast",
                 "group": group,
                 "payload": serialized_payload,
             },
         )
@@ -241,30 +247,22 @@
         contexts. If you call it from the asynchronous context then you
         have to `await`.
 
         Args:
             group: Name of the subscription group which members must be
                 unsubscribed. `None` means that all the client of the
                 subscription will be unsubscribed.
-
         """
         try:
             event_loop = asyncio.get_event_loop()
         except RuntimeError:
             pass
         else:
             if event_loop.is_running():
-                assert cls._from_coroutine(), (
-                    "The eventloop is running so this call is going to return"
-                    " a coroutine object, but the function is called from"
-                    " a synchronous context, so you cannot simply 'await' the result!"
-                    " This may indicate a wrong usage. To force some particular"
-                    " behavior directly call 'unsubscribe_sync' or 'unsubscribe_async'."
-                )
-                return cls.unsubscribe_async(group=group)
+                return asyncio.create_task(cls.unsubscribe_async(group=group))
 
         return cls.unsubscribe_sync(group=group)
 
     @classmethod
     async def unsubscribe_async(cls, *, group=None):
         """Unsubscribe, asynchronous version."""
         # Send the 'unsubscribe' message to the Channels group.
@@ -274,26 +272,40 @@
         )
 
     @classmethod
     def unsubscribe_sync(cls, *, group=None):
         """Unsubscribe, synchronous version."""
         # Send the message to the Channels group.
         group = cls._group_name(group)
-        group_send = asgiref.sync.async_to_sync(cls._channel_layer().group_send)
-        group_send(group=group, message={"type": "unsubscribe", "group": group})
+        sync_channel_layer_group_send = asgiref.sync.async_to_sync(
+            cls._channel_layer().group_send
+        )
+        sync_channel_layer_group_send(
+            group=group,
+            message={
+                "type": "unsubscribe",
+                "group": group,
+            },
+        )
 
     @classmethod
     def Field(  # pylint: disable=invalid-name
         cls, name=None, description=None, deprecation_reason=None, required=False
     ):
-        """Represent subscription as a field to "deploy" it."""
+        """Represent subscription as a field to mount it to the schema.
+
+        Typical usage:
+            class Subscription(graphene.ObjectType):
+                on_new_chat_message = OnNewChatMessage.Field()
+
+        """
         return graphene.Field(
             cls._meta.output,
             args=cls._meta.arguments,
-            resolver=cls._meta.resolver,
+            resolver=cls._meta.publish,
             name=name,
             description=description,
             deprecation_reason=deprecation_reason,
             required=required,
         )
 
     # ------------------------------------------------------------------- IMPLEMENTATION
@@ -304,192 +316,86 @@
         subscribe=None,
         publish=None,
         unsubscribed=None,
         output=None,
         arguments=None,
         _meta=None,
         **options,
-    ):  # pylint: disable=arguments-differ
-        """Prepare subscription when on subclass creation.
+    ):  # pylint: disable=arguments-renamed
+        """Prepare subscription on subclass creation.
 
         This method is invoked by the superclass `__init__subclass__`.
         It is needed to process class fields, `Meta` and inheritance
-        parameters. This is genuine Graphene approach.
+        parameters. This is genuine Graphene approach inherited/cloned
+        from the original Mutation class implementation.
         """
         if not _meta:
             _meta = SubscriptionOptions(cls)
 
         output = output or getattr(cls, "Output", None)
         # Collect fields if output class is not explicitly defined.
-        fields = {}
+        fields: dict = {}
         if not output:
             fields = collections.OrderedDict()
             for base in reversed(cls.__mro__):
                 fields.update(
                     graphene.types.utils.yank_fields_from_attrs(
                         base.__dict__, _as=graphene.Field
                     )
                 )
             output = cls
 
         if not arguments:
             input_class = getattr(cls, "Arguments", None)
-
             if input_class:
                 arguments = graphene.utils.props.props(input_class)
             else:
                 arguments = {}
 
         # Get `publish`, `subscribe`, and `unsubscribe` handlers.
         subscribe = subscribe or getattr(cls, "subscribe", None)
         publish = publish or getattr(cls, "publish", None)
+        unsubscribed = unsubscribed or getattr(cls, "unsubscribed", None)
         assert publish is not None, (
             f"Subscription '{cls.__qualname__}' does not define a"
             " method 'publish'! All subscriptions must define"
-            " 'publish' which processes a GraphQL query!"
+            " 'publish' which processes GraphQL queries!"
         )
 
-        unsubscribed = unsubscribed or getattr(cls, "unsubscribed", None)
-
         if _meta.fields:
             _meta.fields.update(fields)
         else:
             _meta.fields = fields
 
         # Auxiliary alias.
-        get_function = graphene.utils.get_unbound_function.get_unbound_function
+        graphene_get_function = graphene.utils.get_unbound_function.get_unbound_function
 
         # pylint: disable=attribute-defined-outside-init
         _meta.arguments = arguments
         _meta.output = output
-        _meta.resolver = get_function(cls._subscribe)
-        _meta.subscribe = get_function(subscribe)
-        _meta.publish = get_function(publish)
-        _meta.unsubscribed = get_function(unsubscribed)
+        _meta.publish = graphene_get_function(publish)
+        _meta.subscribe = graphene_get_function(subscribe)
+        _meta.unsubscribed = graphene_get_function(unsubscribed)
 
         super().__init_subclass_with_meta__(_meta=_meta, **options)
 
     @classmethod
-    def _subscribe(cls, root, info, *args, **kwds):
-        """Subscription request received.
-
-        This is called by the Graphene when a client subscribes.
-        """
-        # Extract function which associates the callback with the groups
-        # and bring real root back.
-        register_subscription = root.register_subscription
-        root = root.real_root
-
-        # Attach current subscription to the group corresponding to the
-        # concrete class. This allows to trigger all the subscriptions
-        # of the current type, by invoking `publish` without setting
-        # the `group` argument.
-        groups = [cls._group_name()]
-
-        # Invoke the subclass-specified `subscribe` method to get the
-        # groups subscription must be attached to.
-        if cls._meta.subscribe is not None:
-            subclass_groups = cls._meta.subscribe(root, info, *args, **kwds)
-            # Properly handle `async def subscribe`.
-            if asyncio.iscoroutinefunction(cls._meta.subscribe):
-                subclass_groups = asyncio.get_event_loop().run_until_complete(
-                    subclass_groups
-                )
-            assert subclass_groups is None or isinstance(
-                subclass_groups, (list, tuple)
-            ), (
-                f"Method 'subscribe' returned a value of an incorrect type"
-                f" {type(subclass_groups)}! A list, a tuple, or 'None' expected."
-            )
-            subclass_groups = subclass_groups or []
-        else:
-            subclass_groups = []
-
-        groups += [cls._group_name(group) for group in subclass_groups]
-
-        # Register callbacks to call `publish` and `unsubscribed`.
-        # Function `register` provides an observable which must
-        # be returned from here, cause that is what GraphQL expects from
-        # the subscription "resolver" functions.
-        def publish_callback(payload):
-            """Call `publish` with the payload."""
-            result = cls._meta.publish(payload, info, *args, **kwds)
-            # Properly handle `async def publish`.
-            if asyncio.iscoroutinefunction(cls._meta.publish):
-                result = asyncio.get_event_loop().run_until_complete(result)
-            return result
-
-        def unsubscribed_callback():
-            """Call `unsubscribed` notification."""
-            if cls._meta.unsubscribed is None:
-                return None
-            result = cls._meta.unsubscribed(None, info, *args, **kwds)
-            # Properly handle `async def unsubscribed`.
-            if asyncio.iscoroutinefunction(cls._meta.unsubscribed):
-                result = asyncio.get_event_loop().run_until_complete(result)
-            # There is not particular purpose of returning result of the
-            # callback. We do it just for uniformity with `publish` and
-            # `subscribe`.
-            return result
-
-        return register_subscription(
-            groups,
-            publish_callback,
-            unsubscribed_callback,
-            cls.notification_queue_limit,
-        )
-
-    @classmethod
     def _group_name(cls, group=None):
         """Group name based on the name of the subscription class."""
-        prefix = GraphqlWsConsumer.group_name_prefix
         suffix = f"{cls.__module__}.{cls.__qualname__}"
         if group is not None:
             suffix += "-" + group
 
         # Wrap the suffix into SHA256 to guarantee that the length of
         # the group name is limited. Otherwise Channels will complain
         # about that the group name is wrong (actually is too long).
         suffix_sha256 = hashlib.sha256()
         suffix_sha256.update(suffix.encode("utf-8"))
-        suffix_sha256 = suffix_sha256.hexdigest()
-
-        return f"{prefix}-{suffix_sha256}"
 
-    @staticmethod
-    def _from_coroutine() -> bool:
-        """Check if called from the coroutine function.
-
-        Determine whether the current function is called from a
-        coroutine function (native coroutine, generator-based coroutine,
-        or asynchronous generator function).
-
-        NOTE: That it's only recommended to use for debugging, not as
-        part of your production code's functionality.
-        """
-        try:
-            frame = inspect.currentframe()
-            if frame is None:
-                return False
-            coroutine_function_flags = (
-                inspect.CO_COROUTINE  # pylint: disable=no-member
-                | inspect.CO_ASYNC_GENERATOR  # pylint: disable=no-member
-                | inspect.CO_ITERABLE_COROUTINE  # pylint: disable=no-member
-            )
-            if (
-                frame is not None
-                and frame.f_back is not None
-                and frame.f_back.f_back is not None
-            ):
-                return bool(
-                    frame.f_back.f_back.f_code.co_flags & coroutine_function_flags
-                )
-            return False
-        finally:
-            del frame
+        return f"{GraphqlWsConsumer.group_name_prefix}-{suffix_sha256.hexdigest()}"
 
     @classmethod
     def _channel_layer(cls):
         """Channel layer."""
         # We cannot simply check existence of channel layer in the
         # consumer constructor, so we added this property.
         channel_layer = channels.layers.get_channel_layer()
@@ -500,7 +406,8 @@
 class SubscriptionOptions(graphene.types.objecttype.ObjectTypeOptions):
     """Options stored in the Subscription's `_meta` field."""
 
     arguments = None
     output = None
     subscribe = None
     publish = None
+    unsubscribed = None
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/testing.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2010-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -22,18 +22,19 @@
 """GraphQL client transport for testing purposes."""
 
 import asyncio
 from typing import Optional
 
 import channels.testing
 
-from . import client, transport
+import channels_graphql_ws.client
+import channels_graphql_ws.transport
 
 
-class GraphqlWsClient(client.GraphqlWsClient):
+class GraphqlWsClient(channels_graphql_ws.client.GraphqlWsClient):
     """Add functions useful for testing purposes."""
 
     # Time in seconds to wait to ensure the queue of messages is empty.
     RECEIVE_NOTHING_ATTEMPTS = 10
     # Number of seconds to wait for another check for new events.
     RECEIVE_NOTHING_INTERVAL = 0.1
 
@@ -62,15 +63,15 @@
                 assert False, (
                     f"{error_message}\n{received}"
                     if error_message is not None
                     else f"Message received when nothing expected!\n{received}"
                 )
 
 
-class GraphqlWsTransport(transport.GraphqlWsTransport):
+class GraphqlWsTransport(channels_graphql_ws.transport.GraphqlWsTransport):
     """Testing client transport to work without WebSocket connection.
 
     Client is implemented based on the Channels `WebsocketCommunicator`.
     """
 
     def __init__(self, application, path, communicator_kwds=None):
         """Constructor."""
```

### Comparing `django-channels-graphql-ws-0.9.1/channels_graphql_ws/transport.py` & `django_channels_graphql_ws-1.0.0rc1/channels_graphql_ws/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) DATADVANCE, 2010-2021
+# Copyright (C) DATADVANCE, 2010-2023
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -16,15 +16,15 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-"""GraphQL WebSocket client transports."""
+"""GraphQL WebSocket client transport."""
 
 import asyncio
 import json
 from typing import Optional
 
 import aiohttp
 
@@ -73,30 +73,30 @@
         # Server URL.
         self._url = url
         # HTTP cookies.
         self._cookies = cookies
         # HTTP headers.
         self._headers = headers
         # AIOHTTP connection.
-        self._connection = None
+        self._connection: aiohttp.ClientWebSocketResponse
         # A task which processes incoming messages.
-        self._message_processor = None
+        self._message_processor: asyncio.Task
         # A queue for incoming messages.
-        self._incoming_messages = asyncio.Queue()
+        self._incoming_messages: asyncio.Queue = asyncio.Queue()
 
     async def connect(self, timeout: Optional[float] = None) -> None:
         """Establish a connection with the WebSocket server.
 
         Returns:
             `(True, <chosen-subprotocol>)` if connection accepted.
             `(False, None)` if connection rejected.
 
         """
         connected = asyncio.Event()
-        self._message_processor = asyncio.ensure_future(
+        self._message_processor = asyncio.create_task(
             self._process_messages(connected, timeout or self.TIMEOUT)
         )
         await asyncio.wait(
             [connected.wait(), self._message_processor],
             return_when=asyncio.FIRST_COMPLETED,
         )
         if self._message_processor.done():
```

### Comparing `django-channels-graphql-ws-0.9.1/PKG-INFO` & `django_channels_graphql_ws-1.0.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: django-channels-graphql-ws
-Version: 0.9.1
+Version: 1.0.0rc1
 Summary: Django Channels based WebSocket GraphQL server with Graphene-like subscriptions
 Home-page: https://github.com/datadvance/DjangoChannelsGraphqlWs
 License: MIT
 Author: Alexander A. Prokhorov
 Author-email: alexander.prokhorov@datadvance.net
-Requires-Python: >=3.6.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Django (>=3,<4)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=4,<5)
 Requires-Dist: aiohttp (>=3,<4)
 Requires-Dist: asgiref (>=3,<4)
-Requires-Dist: backports-datetime-fromisoformat (>=1,<2); python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: channels (>=3,<4)
-Requires-Dist: dataclasses (>=0.7,<0.8); python_version >= "3.6" and python_version < "3.7"
-Requires-Dist: graphene (>=2.1,<3.0)
-Requires-Dist: graphql-core (>=2.2)
-Requires-Dist: msgpack (>=0.6.1,<2)
+Requires-Dist: channels (>=4,<5)
+Requires-Dist: graphene (>=3,<4)
+Requires-Dist: graphql-core (==3.2.3)
+Requires-Dist: msgpack (>=1,<2)
 Project-URL: Repository, https://github.com/datadvance/DjangoChannelsGraphqlWs
```

