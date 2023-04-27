# Comparing `tmp/onestep-0.1.77.tar.gz` & `tmp/onestep-0.1.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.1.77.tar", max compression
+gzip compressed data, was "onestep-0.1.78.tar", max compression
```

## Comparing `onestep-0.1.77.tar` & `onestep-0.1.78.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1362 2023-04-26 03:26:00.698862 onestep-0.1.77/README.md
--rw-r--r--   0        0        0      704 2023-04-26 03:26:00.698862 onestep-0.1.77/pyproject.toml
--rw-r--r--   0        0        0     1374 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/__init__.py
--rw-r--r--   0        0        0      221 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4543 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     2423 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/exception.py
--rw-r--r--   0        0        0     4530 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/state.py
--rw-r--r--   0        0        0       36 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/store/__init__.py
--rw-r--r--   0        0        0     4466 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/store/rabbitmq.py
--rw-r--r--   0        0        0     3516 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/worker.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.77/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-04-27 02:11:06.732273 onestep-0.1.78/README.md
+-rw-r--r--   0        0        0      704 2023-04-27 02:11:06.736273 onestep-0.1.78/pyproject.toml
+-rw-r--r--   0        0        0     1390 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4543 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     2423 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2144 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/exception.py
+-rw-r--r--   0        0        0     4530 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6350 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2699 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/state.py
+-rw-r--r--   0        0        0       86 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/store/__init__.py
+-rw-r--r--   0        0        0     4466 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/store/rabbitmq.py
+-rw-r--r--   0        0        0     3516 2023-04-27 02:11:06.736273 onestep-0.1.78/src/onestep/worker.py
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.78/PKG-INFO
```

### Comparing `onestep-0.1.77/README.md` & `onestep-0.1.78/README.md`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/pyproject.toml` & `onestep-0.1.78/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onestep"
-version = "0.1.77"
+version = "0.1.78"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
```

### Comparing `onestep-0.1.77/src/onestep/__init__.py` & `onestep-0.1.78/src/onestep/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 from .exception import (
     StopMiddleware, DropMessage,
     RetryException, RetryViaQueue, RetryViaLocal
 )
 
 __all__ = [
     'step',
-
+    
     # broker
     'BaseBroker',
     'BaseConsumer',
     'BaseLocalBroker',
     'BaseLocalConsumer',
     'MemoryBroker',
     'RabbitMQBroker',
     'WebHookBroker',
     'CronBroker',
-
+    
     # retry
     'BaseRetry',
     'NeverRetry',
     'AlwaysRetry',
     'TimesRetry',
     'RetryIfException',
     'AdvancedRetry',
     # error callback
     'BaseErrorCallback',
     'NackErrorCallBack',
-
+    
     # middleware
     'BaseMiddleware',
     'BaseConfigMiddleware',
     'NacosPublishConfigMiddleware',
     'NacosConsumeConfigMiddleware',
     'RedisPublishConfigMiddleware',
     'RedisConsumeConfigMiddleware',
-
+    
     # exception
     'StopMiddleware',
     'DropMessage',
     'RetryException',
     'RetryViaQueue',
     'RetryViaLocal'
 ]
```

### Comparing `onestep-0.1.77/src/onestep/broker/base.py` & `onestep-0.1.78/src/onestep/broker/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/broker/cron.py` & `onestep-0.1.78/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/broker/rabbitmq.py` & `onestep-0.1.78/src/onestep/broker/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/broker/webhook.py` & `onestep-0.1.78/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/exception.py` & `onestep-0.1.78/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/message.py` & `onestep-0.1.78/src/onestep/message.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/middleware/base.py` & `onestep-0.1.78/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/middleware/config.py` & `onestep-0.1.78/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/onestep.py` & `onestep-0.1.78/src/onestep/onestep.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/retry.py` & `onestep-0.1.78/src/onestep/retry.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/state.py` & `onestep-0.1.78/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/store/rabbitmq.py` & `onestep-0.1.78/src/onestep/store/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/worker.py` & `onestep-0.1.78/src/onestep/worker.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/PKG-INFO` & `onestep-0.1.78/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.1.77
+Version: 0.1.78
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

