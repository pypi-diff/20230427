# Comparing `tmp/simplerabbit-0.0.6.tar.gz` & `tmp/simplerabbit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplerabbit-0.0.6.tar", last modified: Mon Apr 17 09:33:53 2023, max compression
+gzip compressed data, was "simplerabbit-0.0.7.tar", last modified: Thu Apr 27 11:34:51 2023, max compression
```

## Comparing `simplerabbit-0.0.6.tar` & `simplerabbit-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.6/README.md
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-17 09:33:09.000000 simplerabbit-0.0.6/pyproject.toml
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/setup.cfg
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.217900 simplerabbit-0.0.6/src/
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/src/simplerabbit/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.6/src/simplerabbit/__init__.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     3111 2023-04-17 09:32:39.000000 simplerabbit-0.0.6/src/simplerabbit/receiver.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2553 2023-04-11 12:40:10.000000 simplerabbit-0.0.6/src/simplerabbit/sender.py
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/src/simplerabbit.egg-info/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      283 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/SOURCES.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/dependency_links.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       13 2023-04-17 09:33:53.000000 simplerabbit-0.0.6/src/simplerabbit.egg-info/top_level.txt
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-17 09:33:53.221900 simplerabbit-0.0.6/tests/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:29:32.000000 simplerabbit-0.0.6/tests/test.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:34:51.064615 simplerabbit-0.0.7/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-27 11:34:51.064615 simplerabbit-0.0.7/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.7/README.md
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-27 11:34:39.000000 simplerabbit-0.0.7/pyproject.toml
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-27 11:34:51.064615 simplerabbit-0.0.7/setup.cfg
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:34:51.060615 simplerabbit-0.0.7/src/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-25 11:00:31.000000 simplerabbit-0.0.7/src/__init__.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:34:51.064615 simplerabbit-0.0.7/src/simplerabbit/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.7/src/simplerabbit/__init__.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1993 2023-04-27 04:09:00.000000 simplerabbit-0.0.7/src/simplerabbit/rabbit_base.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2609 2023-04-25 12:22:11.000000 simplerabbit-0.0.7/src/simplerabbit/receiver.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2020 2023-04-25 12:21:35.000000 simplerabbit-0.0.7/src/simplerabbit/sender.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      325 2023-04-25 11:38:19.000000 simplerabbit-0.0.7/src/simplerabbit/test_receiver.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      473 2023-04-27 11:22:11.000000 simplerabbit-0.0.7/src/simplerabbit/test_receiver_ssl.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      243 2023-04-25 11:32:42.000000 simplerabbit-0.0.7/src/simplerabbit/test_sender.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      392 2023-04-27 03:27:41.000000 simplerabbit-0.0.7/src/simplerabbit/test_sender_ssl.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:34:51.064615 simplerabbit-0.0.7/src/simplerabbit.egg-info/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-27 11:34:51.000000 simplerabbit-0.0.7/src/simplerabbit.egg-info/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      471 2023-04-27 11:34:51.000000 simplerabbit-0.0.7/src/simplerabbit.egg-info/SOURCES.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-27 11:34:51.000000 simplerabbit-0.0.7/src/simplerabbit.egg-info/dependency_links.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       22 2023-04-27 11:34:51.000000 simplerabbit-0.0.7/src/simplerabbit.egg-info/top_level.txt
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:34:51.064615 simplerabbit-0.0.7/tests/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:29:32.000000 simplerabbit-0.0.7/tests/test.py
```

### Comparing `simplerabbit-0.0.6/PKG-INFO` & `simplerabbit-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplerabbit-0.0.6/README.md` & `simplerabbit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.6/pyproject.toml` & `simplerabbit-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplerabbit"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Phuong Do", email="phdo@energidanmark.dk" },
 ]
 description = "Simple RabbitMQ library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplerabbit-0.0.6/src/simplerabbit/receiver.py` & `simplerabbit-0.0.7/src/simplerabbit/receiver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 import pika
 import threading
 import time
 
-class RabbitReceiver:
-    def __init__(self, host='localhost', port='5672', username=None, password=None, virtual_host='/'):
-        self.host = host
-        self.queues = []
-        self.username = username
-        self.password = password
-        self.virtual_host = virtual_host
-        self.port = port
-        self.connection = None
-        self.channel = None
+from rabbit_base import RabBase
+
+
+class RabbitReceiver(RabBase):
+    def __init__(self, host='localhost', port='5672', username=None, password=None, virtual_host='/', ca_cert='', client_cert='', client_key=''):
+        super().__init__(host, port, username, password, virtual_host, ca_cert, client_cert, client_key)
         self.on_message = None
         self.on_connection_closed = None
         self.is_consuming = False
         self.consumer_tag = None
         self.stop_event = threading.Event()
         self.consumer_thread = None
-
-    def connect(self):
-        # Set connection parameters
-        credentials = pika.PlainCredentials(self.username, self.password) if self.username and self.password else None
-        parameters = pika.ConnectionParameters(host=self.host, port=self.port, virtual_host=self.virtual_host, credentials=credentials)
-
-        # Establish connection to RabbitMQ server
-        self.connection = pika.BlockingConnection(parameters)
-        self.channel = self.connection.channel()
+        self.queues = []
 
     def subscribe(self, queue_name, exchange, routing_key):
         print(f'Subcribe to exchange : {exchange} with routing key : {routing_key}')
         self.queues.append(queue_name)
         self.channel.queue_declare(queue=queue_name, durable=True)
         self.channel.queue_bind(exchange=exchange, queue=queue_name, routing_key=routing_key)
```

### Comparing `simplerabbit-0.0.6/src/simplerabbit/sender.py` & `simplerabbit-0.0.7/src/simplerabbit/sender.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 import threading
 import pika
 import time
 
-class RabbitSender:
-    def __init__(self, host='localhost', port='5672', username=None, password=None, virtual_host='/'):
-        self.host = host
-        self.port = port
-        self.username = username
-        self.password = password
-        self.virtual_host = virtual_host
-        self.connection = None
-        self.channel = None
+from rabbit_base import RabBase
+
+
+class RabbitSender(RabBase):
+    def __init__(self, host='localhost', port='5672', username=None, password=None, virtual_host='/', ca_cert='', client_cert='', client_key=''):
+        super().__init__(host, port, username, password, virtual_host, ca_cert, client_cert, client_key)
         self.heartbeat_channel = None
         self.heartbeat_thread = None
         self.is_heartbeat_running = False
         self.lock = threading.Lock()
 
     def connect(self):
-        # Set connection parameters
-        credentials = pika.PlainCredentials(self.username, self.password) if self.username and self.password else None
-        parameters = pika.ConnectionParameters(host=self.host, port=self.port, virtual_host=self.virtual_host,
-                                               credentials=credentials)
-
-        # Establish connection to RabbitMQ server
-        self.connection = pika.BlockingConnection(parameters)
-        self.channel = self.connection.channel()
-
-        # Start heartbeat thread
+        super().connect()
         self.heartbeat_channel = self.connection.channel()
         self.is_heartbeat_running = True
         self.heartbeat_thread = threading.Thread(target=self.send_heartbeat)
         self.heartbeat_thread.start()
 
     def send_heartbeat(self):
         while self.is_heartbeat_running:
```

### Comparing `simplerabbit-0.0.6/src/simplerabbit.egg-info/PKG-INFO` & `simplerabbit-0.0.7/src/simplerabbit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

