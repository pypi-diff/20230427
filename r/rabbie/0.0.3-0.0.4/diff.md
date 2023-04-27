# Comparing `tmp/rabbie-0.0.3.tar.gz` & `tmp/rabbie-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbie-0.0.3.tar", last modified: Mon Apr 24 20:40:08 2023, max compression
+gzip compressed data, was "rabbie-0.0.4.tar", last modified: Thu Apr 27 19:31:56 2023, max compression
```

## Comparing `rabbie-0.0.3.tar` & `rabbie-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.556895 rabbie-0.0.3/
--rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5960 2023-04-24 20:40:08.556895 rabbie-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5484 2023-04-24 20:01:12.000000 rabbie-0.0.3/README.md
--rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.522893 rabbie-0.0.3/rabbie/
--rw-rw-rw-   0        0        0      171 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.535892 rabbie-0.0.3/rabbie/broker_types/
--rw-rw-rw-   0        0        0       22 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/broker_types/__init__.py
--rw-rw-rw-   0        0        0      182 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/broker_types/types.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.540892 rabbie-0.0.3/rabbie/consumer/
--rw-rw-rw-   0        0        0      178 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/consumer/__init__.py
--rw-rw-rw-   0        0        0     4660 2023-04-24 20:32:32.000000 rabbie-0.0.3/rabbie/consumer/consumer.py
--rw-rw-rw-   0        0        0      657 2023-03-29 10:06:37.000000 rabbie-0.0.3/rabbie/consumer/consumer_config.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.544892 rabbie-0.0.3/rabbie/consumer/listener/
--rw-rw-rw-   0        0        0       79 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/consumer/listener/__init__.py
--rw-rw-rw-   0        0        0     4936 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/consumer/listener/listener.py
--rw-rw-rw-   0        0        0      361 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/consumer/listener/listener_details.py
--rw-rw-rw-   0        0        0     2191 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/consumer/microconsumer.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.546891 rabbie-0.0.3/rabbie/decoder/
--rw-rw-rw-   0        0        0       65 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/decoder/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/decoder/decoder.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.549891 rabbie-0.0.3/rabbie/decoder/decoders/
--rw-rw-rw-   0        0        0       39 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/decoder/decoders/__init__.py
--rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/decoder/decoders/json_decoder.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.551891 rabbie-0.0.3/rabbie/decoder/exceptions/
--rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.3/rabbie/decoder/exceptions/__init__.py
--rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.3/rabbie/decoder/exceptions/decode_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.552894 rabbie-0.0.3/rabbie/logger/
--rw-rw-rw-   0        0        0      312 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.554895 rabbie-0.0.3/rabbie/supervisor/
--rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/supervisor/__init__.py
--rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.3/rabbie/supervisor/supervisor.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:40:08.533894 rabbie-0.0.3/rabbie.egg-info/
--rw-rw-rw-   0        0        0     5960 2023-04-24 20:40:08.000000 rabbie-0.0.3/rabbie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2023-04-24 20:40:08.000000 rabbie-0.0.3/rabbie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 20:40:08.000000 rabbie-0.0.3/rabbie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-24 20:40:08.000000 rabbie-0.0.3/rabbie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 20:40:08.000000 rabbie-0.0.3/rabbie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 20:40:08.557895 rabbie-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-04-24 20:38:59.000000 rabbie-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.749215 rabbie-0.0.4/
+-rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     7998 2023-04-27 19:31:56.748216 rabbie-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7522 2023-04-27 19:19:55.000000 rabbie-0.0.4/README.md
+-rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.696215 rabbie-0.0.4/rabbie/
+-rw-rw-rw-   0        0        0      230 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.715215 rabbie-0.0.4/rabbie/broker_types/
+-rw-rw-rw-   0        0        0       60 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/broker_types/__init__.py
+-rw-rw-rw-   0        0        0     4632 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/broker_types/channel.py
+-rw-rw-rw-   0        0        0      182 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/broker_types/relayed_types.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.717215 rabbie-0.0.4/rabbie/connection/
+-rw-rw-rw-   0        0        0       44 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/connection/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/connection/details.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.720218 rabbie-0.0.4/rabbie/consumer/
+-rw-rw-rw-   0        0        0      175 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/__init__.py
+-rw-rw-rw-   0        0        0     6274 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/consumer.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.724215 rabbie-0.0.4/rabbie/consumer/listener/
+-rw-rw-rw-   0        0        0       79 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/consumer/listener/__init__.py
+-rw-rw-rw-   0        0        0     5214 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/listener/listener.py
+-rw-rw-rw-   0        0        0      400 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/listener/listener_details.py
+-rw-rw-rw-   0        0        0     3057 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/consumer/microconsumer.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.726218 rabbie-0.0.4/rabbie/decoder/
+-rw-rw-rw-   0        0        0       65 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/decoder.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.728219 rabbie-0.0.4/rabbie/decoder/decoders/
+-rw-rw-rw-   0        0        0       39 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/decoders/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/decoder/decoders/json_decoder.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.730215 rabbie-0.0.4/rabbie/decoder/exceptions/
+-rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.4/rabbie/decoder/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.4/rabbie/decoder/exceptions/decode_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.732216 rabbie-0.0.4/rabbie/encoder/
+-rw-rw-rw-   0        0        0       65 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.734214 rabbie-0.0.4/rabbie/encoder/encoders/
+-rw-rw-rw-   0        0        0       39 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/encoders/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/encoder/encoders/json_encoder.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.735215 rabbie-0.0.4/rabbie/logger/
+-rw-rw-rw-   0        0        0      312 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.738215 rabbie-0.0.4/rabbie/producer/
+-rw-rw-rw-   0        0        0       46 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/__init__.py
+-rw-rw-rw-   0        0        0     2923 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/producer.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.740245 rabbie-0.0.4/rabbie/producer/publisher/
+-rw-rw-rw-   0        0        0       34 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/publisher/__init__.py
+-rw-rw-rw-   0        0        0     3176 2023-04-27 19:19:55.000000 rabbie-0.0.4/rabbie/producer/publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.742215 rabbie-0.0.4/rabbie/supervisor/
+-rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/supervisor/__init__.py
+-rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.4/rabbie/supervisor/supervisor.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.711215 rabbie-0.0.4/rabbie.egg-info/
+-rw-rw-rw-   0        0        0     7998 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1258 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-27 19:31:56.000000 rabbie-0.0.4/rabbie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 19:31:56.749215 rabbie-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      854 2023-04-27 19:19:55.000000 rabbie-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 19:31:56.747218 rabbie-0.0.4/tests/
+-rw-rw-rw-   0        0        0     4748 2023-04-27 19:19:55.000000 rabbie-0.0.4/tests/test_consumer.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.4/tests/test_decoder.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.4/tests/test_listener.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.4/tests/test_microconsumer.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 19:19:55.000000 rabbie-0.0.4/tests/test_producer.py
```

### Comparing `rabbie-0.0.3/LICENSE` & `rabbie-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.3/PKG-INFO` & `rabbie-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # <p align="center">🥕 Rabbie 🥕</p>
 
 
-![Image](https://img.shields.io/github/last-commit/scuffi/rabbie)![Image](https://img.shields.io/github/license/scuffi/rabbie)![Image](https://img.shields.io/pypi/pyversions/rabbie)
+<p align="center">
+<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/scuffi/rabbie"> <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rabbie"> <img alt="GitHub" src="https://img.shields.io/github/license/scuffi/rabbie"> <a href="https://pypi.org/project/rabbie/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rabbie"></a>
+</p>
 
 
 Rabbie is a Python package designed to provide a simple and helpful interface for interacting with AMQP message brokers, with a particular focus on RabbitMQ. This package is perfect for developers who want to build robust, scalable, and fault-tolerant messaging systems in Python without the need for extensive knowledge of AMQP protocol.
 
 Rabbie provides a high-level API for sending and receiving messages using RabbitMQ, allowing developers to focus on their application logic rather than low-level details of AMQP. It includes features such as easy setup of exchanges, queues, and bindings, support for message publishing and consuming, automatic message acknowledgments, and easy handling of message routing.
 
 Rabbie also provides support for various RabbitMQ features such as message persistence, TTL, priority queues, and exclusive queues. It allows developers to configure and fine-tune these features with ease using its simple and intuitive API.
@@ -124,15 +126,15 @@
     ...
 )
 
 if __name__ == "__main__":
     consumer.add_consumer(my_module.nested_consumer)
     consumer.start()
 ```
-### 💾 Decoders
+### 💾 Encoders & Decoders
 When receiving messages through Rabbie, you have the option to pass a Decoder. This acts as a preliminary step before the data passes into your function. If you received a message like: `{"hello": "world"}`, you can use the inbuilt `JSONDecoder` to automatically parse this text into a dictionary:
 ```python
 from rabbie import Consumer, JSONDecoder
 
 consumer = Consumer(
     host="localhost",
     port=5672,
@@ -161,15 +163,62 @@
         return # Your custom logic here
 
 consumer = Consumer(
     ...
     default_decoder=CustomDecoder()
 )
 ```
+
+Encoders work in the exact same way (just to encode outgoing messages rather than decode incoming), however you have a new function `content_type()` to override when encoding the message in a particular fashion, this will be the content type sent in the request, and should reflect the bodies applicatio type. *For example the inbuilt JSONEncoder returns a 'application/json' content type*
+```python
+from rabbie import Encoder
+
+class CustomEncoder(Encoder):
+    def encoder(self, body: bytes):
+        return # Your custom logic here
+
+    def content_type(self):
+        return "application/my_type"
+```
     
+### 🖨️ Producers
+Producers allow for a simple way to publish messages to exchanges. A simple example would be like so:
+```python
+from rabbie import Producer, JSONEncoder
+
+producer = Producer(
+    host="localhost",
+    port=5672,
+    username="user",
+    password="password",
+)
+
+if __name__ == "__main__":
+    with producer.connect() as channel:
+        channel.publish("hello world!", "my_queue")
+```
+
+Producers also support encoders (same interfaces as decoders, just the opposing side) like so:
+```python
+from rabbie import Producer, JSONEncoder
+
+from my_encoders import CustomEncoder
+
+producer = Producer(
+    host="localhost",
+    port=5672,
+    username="user",
+    password="password",
+)
+
+if __name__ == "__main__":
+    with producer.connect(encoder=JSONEncoder()) as channel:
+        channel.publish({"hello": "world"}, "my_queue", encoder=CustomEncoder())
+```
+> ℹ️ Notice above two encoders are specified. Any parameters passed in to the `channel.publish()` method will take priority, so `CustomEncoder` will be used. It is sometimes easier to define a default value in `producer.connect()` if you will be publishing a lot of similar messages though.
 # TODO
 - Hot Reloading (Refresh listeners on file changes) 🔄
 
 
 ## ➤ License
 Distributed under the MIT License. See [LICENSE](LICENSE) for more information.
```

### Comparing `rabbie-0.0.3/rabbie/consumer/listener/listener.py` & `rabbie-0.0.4/rabbie/consumer/listener/listener.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from .listener_details import ListenerDetails
 from ...broker_types import Channel, Method, Properties
 from ...logger import logger as log
 
 import pika
 from pika.exceptions import AMQPError
+from pika.adapters.blocking_connection import BlockingChannel
 
 
 class Listener:
     def __init__(
         self,
         details: ListenerDetails,
         connection_parameters: pika.ConnectionParameters,
@@ -28,15 +29,19 @@
         self.connection_parameters = connection_parameters
         self.workers: List[Process] = []
 
     def is_listening(self) -> bool:
         return all([worker.is_alive() for worker in self.workers])
 
     def _callback(
-        self, channel: Channel, method: Method, properties: Properties, body: Any
+        self,
+        channel: BlockingChannel,
+        method: Method,
+        properties: Properties,
+        body: Any,
     ):
         """
         This function is called when a message is received on the queue.
         """
 
         log.info(
             f"[{os.getpid()}] Received new message on queue '{self.details.queue_name}'"
@@ -46,15 +51,16 @@
         if self.details.decoder:
             body = self.details.decoder.decode(body)
 
         # Get the signature of the function
         sig = signature(self.details.callback)
 
         all_arguments = {
-            Channel: channel,
+            # TODO: Wrap this channel in a custom channel, that provides utility functionality over acks, nacks, publishing, etc
+            Channel: Channel(channel),
             Method: method,
             Properties: properties,
         }
 
         # Match variables to their types, and pass them in. Default to body
         arguments = {
             arg: all_arguments[sig.parameters[arg].annotation]
@@ -72,28 +78,29 @@
         """
         try:
             callback(*args, **kwargs)
         except Exception:
             traceback.print_exc()
 
     def _start_worker(self, index: int):
+        # TODO: Change this function, it's ugly
         try:
             # Create a BlockingConnection into the queue
             connection = pika.BlockingConnection(self.connection_parameters)
 
             # Open a channel to receive messages through
             channel = connection.channel()
 
             channel.queue_declare(queue=self.details.queue_name, durable=True)
             channel.basic_qos(prefetch_count=1)
 
             channel.basic_consume(
                 queue=self.details.queue_name,
                 on_message_callback=self._callback,
-                auto_ack=True,
+                auto_ack=self.details.auto_ack,
             )
 
             # TODO: Use this instead for more control of what variables to pass?
             # for method, properties, body in channel.consume(self.queue_name):
             #         self._callback(channel, method, properties, body)
 
             # Create a signal handler to close the connection when we receive a SIGINT
@@ -104,19 +111,19 @@
                 sys.exit(0)
 
             # Register the signal handler for SIGTERM
             signal.signal(signal.SIGTERM, handle_sigterm)
 
             channel.start_consuming()
 
-            # TODO: Change how this entire thing works, it's not very elegant.
-        except AMQPError as e:
-            log.error("Connection failed, retrying in 2s...")
-            time.sleep(2)
-            self._start_worker(index)
+        except AMQPError:
+            if self.details.restart:
+                log.error("Connection failed, retrying in 2s...")
+                time.sleep(2)
+                self._start_worker(index)
 
     def stop(self):
         """
         This function stops all workers by killing them.
         """
         for worker in self.workers:
             # Kill the thread
```

### Comparing `rabbie-0.0.3/rabbie/supervisor/supervisor.py` & `rabbie-0.0.4/rabbie/supervisor/supervisor.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.3/rabbie.egg-info/PKG-INFO` & `rabbie-0.0.4/rabbie.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # <p align="center">🥕 Rabbie 🥕</p>
 
 
-![Image](https://img.shields.io/github/last-commit/scuffi/rabbie)![Image](https://img.shields.io/github/license/scuffi/rabbie)![Image](https://img.shields.io/pypi/pyversions/rabbie)
+<p align="center">
+<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/scuffi/rabbie"> <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rabbie"> <img alt="GitHub" src="https://img.shields.io/github/license/scuffi/rabbie"> <a href="https://pypi.org/project/rabbie/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rabbie"></a>
+</p>
 
 
 Rabbie is a Python package designed to provide a simple and helpful interface for interacting with AMQP message brokers, with a particular focus on RabbitMQ. This package is perfect for developers who want to build robust, scalable, and fault-tolerant messaging systems in Python without the need for extensive knowledge of AMQP protocol.
 
 Rabbie provides a high-level API for sending and receiving messages using RabbitMQ, allowing developers to focus on their application logic rather than low-level details of AMQP. It includes features such as easy setup of exchanges, queues, and bindings, support for message publishing and consuming, automatic message acknowledgments, and easy handling of message routing.
 
 Rabbie also provides support for various RabbitMQ features such as message persistence, TTL, priority queues, and exclusive queues. It allows developers to configure and fine-tune these features with ease using its simple and intuitive API.
@@ -124,15 +126,15 @@
     ...
 )
 
 if __name__ == "__main__":
     consumer.add_consumer(my_module.nested_consumer)
     consumer.start()
 ```
-### 💾 Decoders
+### 💾 Encoders & Decoders
 When receiving messages through Rabbie, you have the option to pass a Decoder. This acts as a preliminary step before the data passes into your function. If you received a message like: `{"hello": "world"}`, you can use the inbuilt `JSONDecoder` to automatically parse this text into a dictionary:
 ```python
 from rabbie import Consumer, JSONDecoder
 
 consumer = Consumer(
     host="localhost",
     port=5672,
@@ -161,15 +163,62 @@
         return # Your custom logic here
 
 consumer = Consumer(
     ...
     default_decoder=CustomDecoder()
 )
 ```
+
+Encoders work in the exact same way (just to encode outgoing messages rather than decode incoming), however you have a new function `content_type()` to override when encoding the message in a particular fashion, this will be the content type sent in the request, and should reflect the bodies applicatio type. *For example the inbuilt JSONEncoder returns a 'application/json' content type*
+```python
+from rabbie import Encoder
+
+class CustomEncoder(Encoder):
+    def encoder(self, body: bytes):
+        return # Your custom logic here
+
+    def content_type(self):
+        return "application/my_type"
+```
     
+### 🖨️ Producers
+Producers allow for a simple way to publish messages to exchanges. A simple example would be like so:
+```python
+from rabbie import Producer, JSONEncoder
+
+producer = Producer(
+    host="localhost",
+    port=5672,
+    username="user",
+    password="password",
+)
+
+if __name__ == "__main__":
+    with producer.connect() as channel:
+        channel.publish("hello world!", "my_queue")
+```
+
+Producers also support encoders (same interfaces as decoders, just the opposing side) like so:
+```python
+from rabbie import Producer, JSONEncoder
+
+from my_encoders import CustomEncoder
+
+producer = Producer(
+    host="localhost",
+    port=5672,
+    username="user",
+    password="password",
+)
+
+if __name__ == "__main__":
+    with producer.connect(encoder=JSONEncoder()) as channel:
+        channel.publish({"hello": "world"}, "my_queue", encoder=CustomEncoder())
+```
+> ℹ️ Notice above two encoders are specified. Any parameters passed in to the `channel.publish()` method will take priority, so `CustomEncoder` will be used. It is sometimes easier to define a default value in `producer.connect()` if you will be publishing a lot of similar messages though.
 # TODO
 - Hot Reloading (Refresh listeners on file changes) 🔄
 
 
 ## ➤ License
 Distributed under the MIT License. See [LICENSE](LICENSE) for more information.
```

### Comparing `rabbie-0.0.3/setup.py` & `rabbie-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.0.3"
+version = "0.0.4"
 requirements = ["pika", "multiprocess", "rich", "watchdog"]
 
 setup(
     name="rabbie",
     version=version,
     author="Archie Ferguson",
     author_email="iamarchieferguson@gmail.com",
```

