# Comparing `tmp/ovos-bus-client-0.0.4a3.tar.gz` & `tmp/ovos-bus-client-0.0.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.4a3.tar", last modified: Sat Apr 22 20:59:55 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.4a4.tar", last modified: Thu Apr 27 21:10:52 2023, max compression
```

## Comparing `ovos-bus-client-0.0.4a3.tar` & `ovos-bus-client-0.0.4a4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:59:55.446701 ovos-bus-client-0.0.4a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 20:59:55.446701 ovos-bus-client-0.0.4a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:59:55.442701 ovos-bus-client-0.0.4a3/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:59:55.442701 ovos-bus-client-0.0.4a3/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:59:55.442701 ovos-bus-client-0.0.4a3/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:59:55.442701 ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-22 20:59:55.000000 ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-22 20:59:55.000000 ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:59:55.000000 ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 20:59:55.000000 ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-22 20:59:55.000000 ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 20:59:55.000000 ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 20:59:55.446701 ovos-bus-client-0.0.4a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-22 20:59:54.000000 ovos-bus-client-0.0.4a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 21:10:52.000000 ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:10:52.645172 ovos-bus-client-0.0.4a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-27 21:10:51.000000 ovos-bus-client-0.0.4a4/setup.py
```

### Comparing `ovos-bus-client-0.0.4a3/LICENSE.md` & `ovos-bus-client-0.0.4a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/PKG-INFO` & `ovos-bus-client-0.0.4a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a3
+Version: 0.0.4a4
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from ovos_bus_client.client.client import MessageBusClient
-from ovos_bus_client.message import Message
+from ovos_bus_client.client.client import MessageBusClient, GUIWebsocketClient
+from ovos_bus_client.message import Message, GUIMessage
 from ovos_bus_client.send_func import send
 from ovos_bus_client.session import Session, SessionManager, UtteranceState
 from ovos_bus_client.conf import client_from_config
 
 """
 Mycroft Messagebus Client.
 
@@ -25,11 +25,13 @@
 The messagebus client allows the developer to register handlers for
 specific message types and emitting messages to other services and
 clients connected to the bus.
 """
 
 __all__ = [
     MessageBusClient,
+    GUIWebsocketClient,
+    GUIMessage,
     Message,
     send,
     client_from_config
 ]
```

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from pyee import ExecutorEventEmitter
 from websocket import (WebSocketApp,
                        WebSocketConnectionClosedException,
                        WebSocketException)
 
 from ovos_bus_client.client.collector import MessageCollector
 from ovos_bus_client.client.waiter import MessageWaiter
-from ovos_bus_client.message import Message, CollectionMessage
+from ovos_bus_client.message import Message, CollectionMessage, GUIMessage
 from ovos_bus_client.session import SessionManager, Session
 from ovos_bus_client.util import create_echo_function
-from ovos_bus_client.conf import load_message_bus_config, MessageBusClientConf
+from ovos_bus_client.conf import load_message_bus_config, MessageBusClientConf, load_gui_message_bus_config
 
 
 try:
     from mycroft_bus_client import MessageBusClient as _MessageBusClientBase
 except ImportError:
     # TODO - code in the wild does isinstance checks
     # this conditional subclassing should be removed ASAP, it is only here for the migration period
@@ -336,14 +336,65 @@
         """Launches the run_forever in a separate daemon thread."""
         t = Thread(target=self.run_forever)
         t.daemon = True
         t.start()
         return t
 
 
+class GUIWebsocketClient(MessageBusClient):
+
+    def __init__(self, host=None, port=None, route=None, ssl=None,
+                 emitter=None, cache=False):
+        config_overrides = dict(host=host, port=port, route=route, ssl=ssl)
+        config = load_gui_message_bus_config(**config_overrides)
+        super().__init__(host=config.host, port=config.port, route=config.route,
+                         ssl=config.ssl, emitter=emitter, cache=cache)
+
+    def emit(self, message):
+        """Send a message onto the message bus.
+
+        This will both send the message to the local process using the
+        event emitter and onto the Mycroft websocket for other processes.
+
+        Args:
+            message (GUIMessage): Message to send
+        """
+
+        if not self.connected_event.wait(10):
+            if not self.started_running:
+                raise ValueError('You must execute run_forever() '
+                                 'before emitting messages')
+            self.connected_event.wait()
+
+        try:
+            if hasattr(message, 'serialize'):
+                self.client.send(message.serialize())
+            else:
+                self.client.send(json.dumps(message.__dict__))
+        except WebSocketConnectionClosedException:
+            LOG.warning('Could not send %s message because connection '
+                        'has been closed', message.msg_type)
+
+    def on_message(self, *args):
+        """Handle incoming websocket message.
+
+        Args:
+            message (str): GUI protocol bus message
+        """
+        if len(args) == 1:
+            message = args[0]
+        else:
+            message = args[1]
+
+        self.emitter.emit('message', message)
+
+        parsed_message = GUIMessage.deserialize(message)
+        self.emitter.emit(parsed_message.msg_type, parsed_message)
+
+
 def echo():
     """Echo function repeating all input from a user."""
     message_bus_client = MessageBusClient()
 
     def repeat_utterance(message):
         message.msg_type = 'speak'
         message_bus_client.emit(message)
```

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,25 +21,54 @@
 
     try:
         websocket_configs = config['websocket']
     except KeyError as ke:
         LOG.error('No websocket configs found ({})'.format(repr(ke)))
         raise
     else:
+        overrides = overrides or {}
+        websocket_configs = websocket_configs or {}
         mb_config = MessageBusConfig(
             host=overrides.get('host') or websocket_configs.get('host') or "127.0.0.1",
             port=overrides.get('port') or websocket_configs.get('port') or 8181,
             route=overrides.get('route') or websocket_configs.get('route') or "/core",
             ssl=overrides.get('ssl') or config.get('ssl') or False
         )
         if not all([mb_config.host, mb_config.port, mb_config.route]):
             error_msg = 'Missing one or more websocket configs'
             LOG.error(error_msg)
             raise ValueError(error_msg)
 
+    return mb_config
+
+
+def load_gui_message_bus_config(**overrides):
+    """Load the bits of device configuration needed to run the message bus."""
+    LOG.info('Loading message bus configs')
+    config = Configuration()
+
+    try:
+        websocket_configs = config['gui']
+    except KeyError as ke:
+        LOG.error('No gui configs found ({})'.format(repr(ke)))
+        raise
+    else:
+        overrides = overrides or {}
+        websocket_configs = websocket_configs or {}
+        mb_config = MessageBusConfig(
+            host=overrides.get('host') or websocket_configs.get('host') or "127.0.0.1",
+            port=overrides.get('port') or websocket_configs.get('port') or 18181,
+            route=overrides.get('route') or websocket_configs.get('route') or "/",
+            ssl=overrides.get('ssl') or config.get('ssl') or False
+        )
+        if not all([mb_config.host, mb_config.port, mb_config.route]):
+            error_msg = 'Missing one or more websocket configs'
+            LOG.error(error_msg)
+            raise ValueError(error_msg)
+
     return mb_config
 
 
 def client_from_config(subconf='core', file_path='/etc/mycroft/bus.conf'):
     """Load messagebus configuration from file.
 
     The config is a basic json file with a number of "sub configurations"
```

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/message.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,17 +87,21 @@
 
     def __init__(self, msg_type, data=None, context=None):
         """Used to construct a message object
 
         Message objects will be used to send information back and forth
         between processes of mycroft service, voice, skill and cli
         """
+        data = data or {}
+        context = context or {}
+        assert isinstance(data, dict)
+        assert isinstance(context, dict)
         self.msg_type = msg_type
-        self.data = data or {}
-        self.context = context or {}
+        self.data = data
+        self.context = context
 
     def __eq__(self, other):
         if not isinstance(other, Message):
             return False
         return other.msg_type == self.msg_type and \
             other.data == self.data and \
             other.context == self.context
@@ -107,38 +111,56 @@
 
         This makes it easy to send over a websocket. This uses
         json dumps to generate the string with type, data and context
 
         Returns:
             str: a json string representation of the message.
         """
+        # handle Session and Message objects
+        data = self._json_dump(self.data)
+        ctxt = self._json_dump(self.context)
+
+        msg = json.dumps({'type': self.msg_type, 'data': data, 'context': ctxt})
+        if self._secret_key:
+            payload = encrypt_as_dict(msg)
+            return json.dumps(payload)
+        return msg
 
+    @staticmethod
+    def _json_dump(value):
         def serialize_item(x):
             try:
                 if hasattr(x, "serialize"):
                     return x.serialize()
             except:
                 pass
             if isinstance(x, list):
                 for idx, it in enumerate(x):
                     x[idx] = serialize_item(it)
             if isinstance(x, dict) and not isinstance(x, _GUIDict):
                 for k, v in x.items():
                     x[k] = serialize_item(v)
             return x
+        assert isinstance(value, dict)
+        data = {k: serialize_item(v) for k, v in value.items()}
+        return data
 
-        # handle Session and Message objects
-        data = {k: serialize_item(v) for k, v in self.data.items()}
-        ctxt = {k: serialize_item(v) for k, v in self.context.items()}
-
-        msg = json.dumps({'type': self.msg_type, 'data': data, 'context': ctxt})
-        if self._secret_key:
-            payload = encrypt_as_dict(msg)
-            return json.dumps(payload)
-        return msg
+    @staticmethod
+    def _json_load(value):
+        if isinstance(value, str):
+            obj = json.loads(value)
+        else:
+            obj = value
+        assert isinstance(obj, dict)
+        if Message._secret_key:
+            if 'ciphertext' in obj:
+                obj = decrypt_from_dict(obj)
+            elif not Message._allow_unencrypted:
+                raise RuntimeError("got an unencrypted message, configured to refuse")
+        return obj
 
     @staticmethod
     def deserialize(value):
         """This takes a string and constructs a message object.
 
         This makes it easy to take strings from the websocket and create
         a message object.  This uses json loads to get the info and generate
@@ -148,20 +170,15 @@
             value(str): This is the json string received from the websocket
 
         Returns:
             Message: message object constructed from the json string passed
             int the function.
             value(str): This is the string received from the websocket
         """
-        obj = json.loads(value)
-        if Message._secret_key:
-            if 'ciphertext' in obj:
-                obj = decrypt_from_dict(obj)
-            elif not Message._allow_unencrypted:
-                raise RuntimeError("got an unencrypted message, configured to refuse")
+        obj = Message._json_load(value)
         return Message(obj.get('type') or '',
                        obj.get('data') or {},
                        obj.get('context') or {})
 
     def forward(self, msg_type, data=None):
         """ Keep context and forward message
 
@@ -399,14 +416,41 @@
         data['timeout'] = timeout
         response_message = self.reply(self.msg_type + '.handling',
                                       data,
                                       self.context)
         return response_message
 
 
+class GUIMessage(Message):
+    def __init__(self, msg_type, **kwargs):
+        super().__init__(msg_type, data=kwargs)
+
+    def serialize(self):
+        """This returns a string of the message info.
+
+        This makes it easy to send over a websocket. This uses
+        json dumps to generate the string with type, data and context
+
+        Returns:
+            str: a json string representation of the message.
+        """
+        data = self._json_dump(self.data)
+        msg = json.dumps({'type': self.msg_type, **data})
+        if self._secret_key:
+            payload = encrypt_as_dict(msg)
+            return json.dumps(payload)
+        return msg
+
+    @staticmethod
+    def deserialize(value):
+        value = Message._json_load(value)
+        msg_type = value.pop("type")
+        return GUIMessage(msg_type, **value)
+
+
 if __name__ == "__main__":
     from mycroft_bus_client.message import Message as _MycroftMessage
 
     m1 = _MycroftMessage("")
     m2 = Message("")
     print(m1 == m2)
     print(m2 == m1)
```

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/session.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/session.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.4a4/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a3
+Version: 0.0.4a4
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a3/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.4a4/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a3/setup.py` & `ovos-bus-client-0.0.4a4/setup.py`

 * *Files identical despite different names*

