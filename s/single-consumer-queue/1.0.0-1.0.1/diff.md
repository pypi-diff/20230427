# Comparing `tmp/single_consumer_queue-1.0.0.tar.gz` & `tmp/single_consumer_queue-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "single_consumer_queue-1.0.0.tar", max compression
+gzip compressed data, was "single_consumer_queue-1.0.1.tar", max compression
```

## Comparing `single_consumer_queue-1.0.0.tar` & `single_consumer_queue-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-27 03:38:00.811325 single_consumer_queue-1.0.0/LICENSE
--rw-r--r--   0        0        0     1770 2023-04-27 04:22:12.457869 single_consumer_queue-1.0.0/README.md
--rw-r--r--   0        0        0      553 2023-04-27 04:22:39.778804 single_consumer_queue-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 03:49:17.245132 single_consumer_queue-1.0.0/single_consumer_queue/__init__.py
--rw-r--r--   0        0        0     3454 2023-04-27 04:22:13.090857 single_consumer_queue-1.0.0/single_consumer_queue/queue.py
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 single_consumer_queue-1.0.0/setup.py
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 single_consumer_queue-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-27 03:38:00.811325 single_consumer_queue-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1770 2023-04-27 04:22:12.457869 single_consumer_queue-1.0.1/README.md
+-rw-r--r--   0        0        0      576 2023-04-27 04:38:56.621640 single_consumer_queue-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 03:49:17.245132 single_consumer_queue-1.0.1/single_consumer_queue/__init__.py
+-rw-r--r--   0        0        0     3454 2023-04-27 04:22:13.090857 single_consumer_queue-1.0.1/single_consumer_queue/queue.py
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 single_consumer_queue-1.0.1/setup.py
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 single_consumer_queue-1.0.1/PKG-INFO
```

### Comparing `single_consumer_queue-1.0.0/LICENSE` & `single_consumer_queue-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `single_consumer_queue-1.0.0/README.md` & `single_consumer_queue-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `single_consumer_queue-1.0.0/pyproject.toml` & `single_consumer_queue-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "single-consumer-queue"
-version = "1.0.0"
+version = "1.0.1"
 description = "Asyncio high-performance single consumer queue"
 authors = ["Lukas Krocek <krocek.lukas@email.cz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "single_consumer_queue"}]
+include = ["py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-asyncio = "*"
```

### Comparing `single_consumer_queue-1.0.0/single_consumer_queue/queue.py` & `single_consumer_queue-1.0.1/single_consumer_queue/queue.py`

 * *Files identical despite different names*

### Comparing `single_consumer_queue-1.0.0/setup.py` & `single_consumer_queue-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['single_consumer_queue']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'single-consumer-queue',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Asyncio high-performance single consumer queue',
     'long_description': "# Single Consumer Queue\nSingle Consumer Queue is a Python library that provides an alternative to the standard asyncio.Queue for single consumer scenarios. It consists of two classes: SingleConsumerQueue and SingleConsumerPriorityQueue. Both classes implement the AbstractSingleConsumerQueue abstract base class, which provides the basic functionality of a single consumer queue.\n\n## Why Single Consumer Queue?\nIn some scenarios, the standard asyncio.Queue can be slower than necessary. This is because asyncio.Queue is designed to be used with multiple consumers, which means that it has additional overhead to handle multiple concurrent accesses. If you only have one consumer, you can use SingleConsumerQueue or SingleConsumerPriorityQueue to reduce this overhead and improve performance.\n\n## How to use Single Consumer Queue\nInstallation\nYou can install Single Consumer Queue using pip:\n\n```pip install single-consumer-queue```\n\n## Usage\nHere's an example of how to use SingleConsumerQueue:\n\n```\nasync def consumer(queue: SingleConsumerQueue | SingleConsumerPriorityQueue):\n    async for item in queue.start_consuming():\n        print(item)\n```\n\nSingleConsumerQueue raises exception if you try to add multiple consumers:\n\n```\nasync def consumer(queue: SingleConsumerQueue | SingleConsumerPriorityQueue):\n    async for item in queue.start_consuming():\n        print(item)\n\nqueue = SingleConsumerQueue()\nasyncio.create_task(consumer(queue))\nawait asyncio sleep(0.1)\nawait queue.get()  # raises runtime error\n```\n\nLock is checked and acquired when consumer starts and every time that get is awaited.\n\nGet has considerate overhead because it has to use lock every time, so it is recommended to use `start_consuming` generator when you want to consume items in the loop.\n",
     'author': 'Lukas Krocek',
     'author_email': 'krocek.lukas@email.cz',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `single_consumer_queue-1.0.0/PKG-INFO` & `single_consumer_queue-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: single-consumer-queue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asyncio high-performance single consumer queue
 License: MIT
 Author: Lukas Krocek
 Author-email: krocek.lukas@email.cz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

