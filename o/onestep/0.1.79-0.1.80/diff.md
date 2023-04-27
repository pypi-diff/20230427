# Comparing `tmp/onestep-0.1.79.tar.gz` & `tmp/onestep-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.1.79.tar", max compression
+gzip compressed data, was "onestep-0.1.80.tar", max compression
```

## Comparing `onestep-0.1.79.tar` & `onestep-0.1.80.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1362 2023-04-27 06:52:41.840061 onestep-0.1.79/README.md
--rw-r--r--   0        0        0      704 2023-04-27 06:52:41.840061 onestep-0.1.79/pyproject.toml
--rw-r--r--   0        0        0     1390 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/__init__.py
--rw-r--r--   0        0        0      414 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/_utils.py
--rw-r--r--   0        0        0      221 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4543 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     2271 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/exception.py
--rw-r--r--   0        0        0     4537 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/state.py
--rw-r--r--   0        0        0       86 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/store/__init__.py
--rw-r--r--   0        0        0     4466 2023-04-27 06:52:41.840061 onestep-0.1.79/src/onestep/store/rabbitmq.py
--rw-r--r--   0        0        0     3516 2023-04-27 06:52:41.844061 onestep-0.1.79/src/onestep/worker.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.79/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-04-27 07:06:13.500527 onestep-0.1.80/README.md
+-rw-r--r--   0        0        0      704 2023-04-27 07:06:13.500527 onestep-0.1.80/pyproject.toml
+-rw-r--r--   0        0        0     1390 2023-04-27 07:06:13.500527 onestep-0.1.80/src/onestep/__init__.py
+-rw-r--r--   0        0        0      414 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/_utils.py
+-rw-r--r--   0        0        0      221 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4543 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     2271 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2144 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/exception.py
+-rw-r--r--   0        0        0     4543 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6350 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2699 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/state.py
+-rw-r--r--   0        0        0       86 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/store/__init__.py
+-rw-r--r--   0        0        0     4466 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/store/rabbitmq.py
+-rw-r--r--   0        0        0     3516 2023-04-27 07:06:13.504526 onestep-0.1.80/src/onestep/worker.py
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.80/PKG-INFO
```

### Comparing `onestep-0.1.79/README.md` & `onestep-0.1.80/README.md`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/pyproject.toml` & `onestep-0.1.80/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onestep"
-version = "0.1.79"
+version = "0.1.80"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
```

### Comparing `onestep-0.1.79/src/onestep/__init__.py` & `onestep-0.1.80/src/onestep/__init__.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/broker/base.py` & `onestep-0.1.80/src/onestep/broker/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/broker/cron.py` & `onestep-0.1.80/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/broker/rabbitmq.py` & `onestep-0.1.80/src/onestep/broker/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/broker/webhook.py` & `onestep-0.1.80/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/exception.py` & `onestep-0.1.80/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/message.py` & `onestep-0.1.80/src/onestep/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,25 +107,25 @@
                     data['exception'] = str(self.exception)
         
         return data
     
     def to_json(self, include_exception=False) -> str:
         return json.dumps(self.to_dict(include_exception))
     
-    @catch_error
+    @catch_error()
     def confirm(self):
         """确认消息"""
         self.broker.confirm(self)
     
-    @catch_error
+    @catch_error()
     def reject(self):
         """拒绝消息"""
         self.broker.reject(self)
     
-    @catch_error
+    @catch_error()
     def requeue(self, is_source=False):
         """
         重发消息：先拒绝 再 重入
         
         :param is_source: 是否是源消息，True: 使用消息的最新数据重入当前队列，False: 使用消息的最新数据重入当前队列
         """
         self.broker.requeue(self, is_source=is_source)
```

### Comparing `onestep-0.1.79/src/onestep/middleware/base.py` & `onestep-0.1.80/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/middleware/config.py` & `onestep-0.1.80/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/onestep.py` & `onestep-0.1.80/src/onestep/onestep.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/retry.py` & `onestep-0.1.80/src/onestep/retry.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/state.py` & `onestep-0.1.80/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/store/rabbitmq.py` & `onestep-0.1.80/src/onestep/store/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/src/onestep/worker.py` & `onestep-0.1.80/src/onestep/worker.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.79/PKG-INFO` & `onestep-0.1.80/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.1.79
+Version: 0.1.80
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

