# Comparing `tmp/onestep-0.1.76.tar.gz` & `tmp/onestep-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.1.76.tar", max compression
+gzip compressed data, was "onestep-0.1.77.tar", max compression
```

## Comparing `onestep-0.1.76.tar` & `onestep-0.1.77.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1362 2023-04-21 01:22:59.195390 onestep-0.1.76/README.md
--rw-r--r--   0        0        0      704 2023-04-21 01:22:59.195390 onestep-0.1.76/pyproject.toml
--rw-r--r--   0        0        0     1374 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/__init__.py
--rw-r--r--   0        0        0      221 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4310 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     1997 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/exception.py
--rw-r--r--   0        0        0     4338 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/state.py
--rw-r--r--   0        0        0       36 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/store/__init__.py
--rw-r--r--   0        0        0     4170 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/store/rabbitmq.py
--rw-r--r--   0        0        0     3516 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/worker.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.76/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-04-26 03:26:00.698862 onestep-0.1.77/README.md
+-rw-r--r--   0        0        0      704 2023-04-26 03:26:00.698862 onestep-0.1.77/pyproject.toml
+-rw-r--r--   0        0        0     1374 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4543 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     2423 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2144 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/exception.py
+-rw-r--r--   0        0        0     4530 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6350 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2699 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/state.py
+-rw-r--r--   0        0        0       36 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/store/__init__.py
+-rw-r--r--   0        0        0     4466 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/store/rabbitmq.py
+-rw-r--r--   0        0        0     3516 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/worker.py
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.77/PKG-INFO
```

### Comparing `onestep-0.1.76/README.md` & `onestep-0.1.77/README.md`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/pyproject.toml` & `onestep-0.1.77/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onestep"
-version = "0.1.76"
+version = "0.1.77"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
```

### Comparing `onestep-0.1.76/src/onestep/__init__.py` & `onestep-0.1.77/src/onestep/__init__.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/broker/base.py` & `onestep-0.1.77/src/onestep/broker/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,154 +1,156 @@
 # -*- coding: utf-8 -*-
 import abc
 import json
 from queue import Queue, Empty
+from typing import Any
 
 from ..exception import StopMiddleware
 from ..message import Message
 
 
 class BaseBroker:
-
+    
     def __init__(self, name=None, queue=None, middlewares=None):
         self.queue = queue
         self.name = name or "broker"
         self.middlewares = []
-
+        
         if middlewares:
             for middleware in middlewares:
                 self.add_middleware(middleware)
-
+    
     def add_middleware(self, middleware):
         self.middlewares.append(middleware)
-
+    
     def send(self, message):
         """对消息进行预处理，然后再发送"""
         if not isinstance(message, Message):
             message = Message(body=message)
         # TODO: 对消息发送进行N次重试，确保消息发送成功。
         return self.publish(message.to_json())
-
+    
     @abc.abstractmethod
-    def publish(self, message):
+    def publish(self, message: Any):
         """
         如果当前Broker是Job的to_broker, 则必须实现此方法
         """
         raise NotImplementedError('Please implement in subclasses.')
-
+    
     @abc.abstractmethod
     def consume(self, *args, **kwargs):
         """
         如果当前Broker是Job的from_broker, 则必须实现此方法
         """
         raise NotImplementedError('Please implement in subclasses.')
-
+    
     @abc.abstractmethod
-    def confirm(self, message):
+    def confirm(self, message: Message):
         """确认消息"""
         raise NotImplementedError('Please implement in subclasses.')
-
+    
     @abc.abstractmethod
-    def reject(self, message):
+    def reject(self, message: Message):
         """拒绝消息"""
         raise NotImplementedError('Please implement in subclasses.')
-
+    
     @abc.abstractmethod
-    def requeue(self, message, is_source=False):
+    def requeue(self, message: Message, is_source=False):
         """
         重发消息：先拒绝 再 重入
         is_source = False 重入使用消息的当前状态
         is_source = True 重入使用消息的初始状态
         """
         raise NotImplementedError('Please implement in subclasses.')
-
+    
     def before_emit(self, signal, *args, **kwargs):
         signal = "before_" + signal
         self._emit(signal, *args, **kwargs)
-
+    
     def after_emit(self, signal, *args, **kwargs):
         signal = "after_" + signal
         self._emit(signal, *args, **kwargs)
-
+    
     def _emit(self, signal, *args, **kwargs):
         for middleware in self.middlewares:
             if not hasattr(middleware, signal):
                 continue
             try:
                 getattr(middleware, signal)(self, *args, **kwargs)
             except StopMiddleware:
                 break
-
+    
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.name}>"
-
+    
     def __str__(self):
         return self.name
 
 
 class BaseConsumer:
-
+    
     def __init__(self, queue: Queue, *args, **kwargs):
         self.queue = queue
         self.timeout = kwargs.pop("timeout", 1000)
-
+    
     @abc.abstractmethod
-    def _to_message(self, data):
+    def _to_message(self, data: Any):
         """
         转换消息内容到 Message , 则必须实现此方法
         """
         raise NotImplementedError('Please implement in subclasses.')
-
+    
     def __next__(self):
         try:
-            return self._to_message(self.queue.get(timeout=self.timeout / 1000))
+            data = self.queue.get(timeout=self.timeout / 1000)
+            return self._to_message(data)
         except Empty:
             return None
-
+    
     def __iter__(self):
         return self
 
 
 class BaseLocalBroker(BaseBroker):
-
+    
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.queue = Queue()
-
-    def publish(self, message):
+    
+    def publish(self, message: Any):
         self.queue.put_nowait(message)
-
+    
     def consume(self, *args, **kwargs):
         return BaseLocalConsumer(self.queue, *args, **kwargs)
-
-    def confirm(self, message):
+    
+    def confirm(self, message: Message):
         """确认消息"""
         pass
-
-    def reject(self, message):
+    
+    def reject(self, message: Message):
         """拒绝消息"""
         pass
-
-    def requeue(self, message, is_source=False):
+    
+    def requeue(self, message: Message, is_source=False):
         """重发消息：先拒绝 再 重入"""
         if is_source:
             self.publish(message.msg)
         else:
             self.send(message)
-
+    
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.name}>"
-
+    
     def __str__(self):
         return self.name
 
 
 class BaseLocalConsumer(BaseConsumer):
-
-    def _to_message(self, data):
+    
+    def _to_message(self, data: Any):
         message = Message(msg=data)
         try:
             body = json.loads(data)
             message.replace(**body)
         except (json.JSONDecodeError, TypeError):
             message.body = data
         return message
```

### Comparing `onestep-0.1.76/src/onestep/broker/cron.py` & `onestep-0.1.77/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/broker/rabbitmq.py` & `onestep-0.1.77/src/onestep/broker/rabbitmq.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 import json
 import threading
 from queue import Queue
-from typing import Optional, Dict
+from typing import Optional, Dict, Any
 
 import amqpstorm
 
 from .base import BaseBroker, BaseConsumer
-from ..store.rabbitmq import RabbitmqStore
+from ..store.rabbitmq import RabbitMQStore
 from ..message import Message
 
 
 class RabbitMQBroker(BaseBroker):
 
     def __init__(self, queue_name, params: Optional[Dict] = None, prefetch: Optional[int] = 1, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.queue_name = queue_name
         self.queue = Queue()
         params = params or {}
-        self.client = RabbitmqStore(**params)
+        self.client = RabbitMQStore(**params)
         self.client.declare_queue(self.queue_name)
         self.prefetch = prefetch
 
     def _consume(self, *args, **kwargs):
-        def callback(message):
+        def callback(message: amqpstorm.Message):
             self.queue.put(message)
 
         prefetch = kwargs.pop("prefetch", self.prefetch)
         self.client.start_consuming(queue_name=self.queue_name, callback=callback, prefetch=prefetch, **kwargs)
 
     def consume(self, *args, **kwargs):
         threading.Thread(target=self._consume, *args, **kwargs).start()
         return RabbitMQConsumer(self.queue)
 
-    def publish(self, message):
+    def publish(self, message: Any):
         self.client.send(self.queue_name, message)
 
-    def confirm(self, message):
+    def confirm(self, message: Message):
         """确认消息"""
-        message.msg.ack()
+        self.client.channel.basic.ack(message.msg.delivery_tag)
 
-    def reject(self, message):
+    def reject(self, message: Message):
         """拒绝消息"""
-        message.msg.nack(requeue=False)
+        self.client.channel.basic.nack(message.msg.delivery_tag, requeue=False)
 
-    def requeue(self, message, is_source=False):
-        """重发消息：先拒绝 再 重入"""
+    def requeue(self, message: Message, is_source=False):
+        """
+        重发消息：先拒绝 再 重入
+        
+        :param message: 消息
+        :param is_source: 是否是源消息，True: 使用消息的最新数据重入当前队列，False: 使用消息的最新数据重入当前队列
+        """
         if is_source:
-            message.msg.nack(requeue=True)
+            self.client.channel.basic.nack(message.msg.delivery_tag, requeue=True)
         else:
-            message.msg.nack(requeue=False)
+            self.client.channel.basic.nack(message.msg.delivery_tag, requeue=False)
             self.send(message)
 
 
 class RabbitMQConsumer(BaseConsumer):
     def _to_message(self, data: amqpstorm.Message):
         try:
             message = json.loads(data.body)
```

### Comparing `onestep-0.1.76/src/onestep/broker/webhook.py` & `onestep-0.1.77/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/exception.py` & `onestep-0.1.77/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/message.py` & `onestep-0.1.77/src/onestep/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,22 +111,26 @@
     
     def confirm(self):
         """确认消息"""
         if self.broker:
             self.broker.confirm(self)
     
     def reject(self):
-        """拒绝消息 （原始状态重入）"""
+        """拒绝消息"""
         if self.broker:
             self.broker.reject(self)
     
-    def requeue(self):
-        """重发消息 （最新状态重入）"""
+    def requeue(self, is_source=False):
+        """
+        重发消息：先拒绝 再 重入
+        
+        :param is_source: 是否是源消息，True: 使用消息的最新数据重入当前队列，False: 使用消息的最新数据重入当前队列
+        """
         if self.broker:
-            self.broker.requeue(self)
+            self.broker.requeue(self, is_source=is_source)
     
     def __getattr__(self, item):
         return None
     
     def __delattr__(self, item):
         if hasattr(self, item):
             setattr(self, item, None)
```

### Comparing `onestep-0.1.76/src/onestep/middleware/base.py` & `onestep-0.1.77/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/middleware/config.py` & `onestep-0.1.77/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/onestep.py` & `onestep-0.1.77/src/onestep/onestep.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/retry.py` & `onestep-0.1.77/src/onestep/retry.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/state.py` & `onestep-0.1.77/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/src/onestep/store/rabbitmq.py` & `onestep-0.1.77/src/onestep/store/rabbitmq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
+import time
 from threading import local
 import amqpstorm
 from amqpstorm.exception import AMQPConnectionError
 
 MAX_SEND_ATTEMPTS = 6  # 最大发送重试次数
 MAX_CONNECTION_ATTEMPTS = float('inf')  # 最大连接重试次数
 
 logger = logging.Logger(__name__)
 
 
-class RabbitmqStore:
-
+class RabbitMQStore:
+    
     def __init__(self, *, confirm_delivery=True, host=None, port=None, username=None, password=None,
                  **kwargs):
         """
         :param confirm_delivery: 是否开启消息确认
         :param host: RabbitMQ host
         :param port: RabbitMQ port
         :param username: RabbitMQ username
@@ -27,56 +28,57 @@
             'port': port or 5672,
             'username': username or 'guest',
             'password': password or 'guest',
         }
         if kwargs:
             self.parameters.update(kwargs)
         self.confirm_delivery = confirm_delivery
-
+    
     def _create_connection(self):
         attempts = 1
         while attempts <= MAX_CONNECTION_ATTEMPTS:
             try:
+                # logger.warning("RabbitmqStore connection try: attempts=%s", attempts)
                 return amqpstorm.Connection(**self.parameters)
             except AMQPConnectionError as exc:
                 attempts += 1
                 logger.warning("RabbitmqStore connection error: %s", exc)
         raise AMQPConnectionError("RabbitmqStore connection error, max attempts reached")
-
+    
     @property
-    def connection(self):
+    def connection(self) -> amqpstorm.Connection:
         connection = getattr(self.state, "connection", None)
         if connection is None or not connection.is_open:
             connection = self.state.connection = self._create_connection()
         return connection
-
+    
     @connection.deleter
     def connection(self):
         if _connection := getattr(self.state, "connection", None):
             _connection.close()
             del self.state.connection
             del self.state.channel
-
+    
     @property
-    def channel(self):
+    def channel(self) -> amqpstorm.Channel:
         connection = getattr(self.state, "connection", None)
         channel = getattr(self.state, "channel", None)
         if all([connection, channel]) and all([connection.is_open, channel.is_open]):
             return channel
         channel = self.state.channel = self.connection.channel()
         if self.confirm_delivery:
             channel.confirm_deliveries()
         return channel
-
+    
     def declare_queue(self, queue_name, arguments=None):
         """声明队列"""
         if arguments is None:
             arguments = {}
         return self.channel.queue.declare(queue_name, durable=True, arguments=arguments)
-
+    
     def send(self, queue_name, message, priority=None, **kwargs):
         """发送消息"""
         attempts = 1
         while True:
             try:
                 self.declare_queue(queue_name)
                 self.channel.basic.publish(
@@ -84,30 +86,35 @@
                 )
                 return message
             except Exception as exc:
                 del self.connection
                 attempts += 1
                 if attempts > MAX_SEND_ATTEMPTS:
                     raise exc
-
+    
     def flush_queue(self, queue_name):
         """清空队列"""
         self.channel.queue.purge(queue_name)
-
+    
     def get_message_counts(self, queue_name: str) -> int:
         """获取消息数量"""
         queue_response = self.declare_queue(queue_name)
         return queue_response.get("message_count", 0)
-
+    
     def start_consuming(self, queue_name, callback, prefetch=1, **kwargs):
         """开始消费"""
         while True:
             try:
                 self.channel.basic.qos(prefetch_count=prefetch)
                 self.channel.basic.consume(queue=queue_name, callback=callback, no_ack=False, **kwargs)
                 self.channel.start_consuming(to_tuple=False)
             except AMQPConnectionError:
                 logger.warning("RabbitmqStore consume connection error, reconnecting...")
                 del self.connection
+                time.sleep(1)
             except Exception as e:
                 logger.exception(f"RabbitmqStore consume error<{e}>, reconnecting...")
                 del self.connection
+                time.sleep(1)
+
+
+RabbitmqStore = RabbitMQStore  # 兼容旧版本
```

### Comparing `onestep-0.1.76/src/onestep/worker.py` & `onestep-0.1.77/src/onestep/worker.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.76/PKG-INFO` & `onestep-0.1.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.1.76
+Version: 0.1.77
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

