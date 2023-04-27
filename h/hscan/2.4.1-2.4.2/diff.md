# Comparing `tmp/hscan-2.4.1.tar.gz` & `tmp/hscan-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscan-2.4.1.tar", last modified: Tue Apr  4 03:35:11 2023, max compression
+gzip compressed data, was "hscan-2.4.2.tar", last modified: Thu Apr 27 08:37:56 2023, max compression
```

## Comparing `hscan-2.4.1.tar` & `hscan-2.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-04 03:35:11.110541 hscan-2.4.1/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-04-04 03:35:11.110068 hscan-2.4.1/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.4.1/README.md
--rw-r--r--   0 jyanghe    (501) staff       (20)      953 2023-04-04 03:34:16.000000 hscan-2.4.1/Setup.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-04 03:35:11.091065 hscan-2.4.1/hscan.egg-info/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-04-04 03:35:10.000000 hscan-2.4.1/hscan.egg-info/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-04-04 03:35:10.000000 hscan-2.4.1/hscan.egg-info/SOURCES.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-04-04 03:35:10.000000 hscan-2.4.1/hscan.egg-info/dependency_links.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-04 03:35:10.000000 hscan-2.4.1/hscan.egg-info/requires.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-04-04 03:35:10.000000 hscan-2.4.1/hscan.egg-info/top_level.txt
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-04 03:35:11.100100 hscan-2.4.1/scan/
--rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.4.1/scan/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.4.1/scan/common.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.4.1/scan/config.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      845 2022-05-19 02:18:07.000000 hscan-2.4.1/scan/crawl.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-04 03:35:11.107272 hscan-2.4.1/scan/database/
--rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.4.1/scan/database/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.4.1/scan/database/kafka.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.4.1/scan/database/mongodb.py
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.4.1/scan/database/mysql.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.4.1/scan/database/oss.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.4.1/scan/database/pg.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     5515 2022-12-27 12:22:30.000000 hscan-2.4.1/scan/database/rabbitmq.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.4.1/scan/database/redis.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-04 03:35:11.108884 hscan-2.4.1/scan/downloade/
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.4.1/scan/downloade/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     4685 2022-09-09 07:51:51.000000 hscan-2.4.1/scan/downloade/downloader.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.4.1/scan/log.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.4.1/scan/monitor.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.4.1/scan/response.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     9784 2022-12-27 08:14:30.000000 hscan-2.4.1/scan/spider.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1021 2022-03-14 02:23:08.000000 hscan-2.4.1/scan/util.py
--rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-04-04 03:35:11.111009 hscan-2.4.1/setup.cfg
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-27 08:37:56.671912 hscan-2.4.2/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-04-27 08:37:56.671682 hscan-2.4.2/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.4.2/README.md
+-rw-r--r--   0 jyanghe    (501) staff       (20)      953 2023-04-27 08:37:15.000000 hscan-2.4.2/Setup.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-27 08:37:56.659354 hscan-2.4.2/hscan.egg-info/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-04-27 08:37:56.000000 hscan-2.4.2/hscan.egg-info/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-04-27 08:37:56.000000 hscan-2.4.2/hscan.egg-info/SOURCES.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-04-27 08:37:56.000000 hscan-2.4.2/hscan.egg-info/dependency_links.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-27 08:37:56.000000 hscan-2.4.2/hscan.egg-info/requires.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-04-27 08:37:56.000000 hscan-2.4.2/hscan.egg-info/top_level.txt
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-27 08:37:56.665395 hscan-2.4.2/scan/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.4.2/scan/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.4.2/scan/common.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.4.2/scan/config.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      845 2022-05-19 02:18:07.000000 hscan-2.4.2/scan/crawl.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-27 08:37:56.670380 hscan-2.4.2/scan/database/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.4.2/scan/database/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.4.2/scan/database/kafka.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.4.2/scan/database/mongodb.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.4.2/scan/database/mysql.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.4.2/scan/database/oss.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.4.2/scan/database/pg.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6093 2023-04-27 08:36:36.000000 hscan-2.4.2/scan/database/rabbitmq.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.4.2/scan/database/redis.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-04-27 08:37:56.671115 hscan-2.4.2/scan/downloade/
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.4.2/scan/downloade/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     4685 2022-09-09 07:51:51.000000 hscan-2.4.2/scan/downloade/downloader.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.4.2/scan/log.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.4.2/scan/monitor.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.4.2/scan/response.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     9784 2022-12-27 08:14:30.000000 hscan-2.4.2/scan/spider.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1021 2022-03-14 02:23:08.000000 hscan-2.4.2/scan/util.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-04-27 08:37:56.671991 hscan-2.4.2/setup.cfg
```

### Comparing `hscan-2.4.1/Setup.py` & `hscan-2.4.2/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hscan",
-    version="2.4.1",
+    version="2.4.2",
     author="jyanghe",
     author_email="jyanghe1023@gmail.com",
     description="A python framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jyangHe/hscan",
     packages=setuptools.find_packages(),
```

### Comparing `hscan-2.4.1/hscan.egg-info/SOURCES.txt` & `hscan-2.4.2/hscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/config.py` & `hscan-2.4.2/scan/config.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/crawl.py` & `hscan-2.4.2/scan/crawl.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/database/kafka.py` & `hscan-2.4.2/scan/database/kafka.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/database/mongodb.py` & `hscan-2.4.2/scan/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/database/pg.py` & `hscan-2.4.2/scan/database/pg.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/database/rabbitmq.py` & `hscan-2.4.2/scan/database/rabbitmq.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,24 +75,35 @@
                         else:
                             logger.error(f'task fail, resend data:{task_info}')
                             await self.publish(data=task_info, routing_key=queue_name)
                             await message.ack()
         except Exception as e:
             logger.error(f'consume process error: {e}')
 
-    async def publish(self, data, routing_key, priority=None):
+    async def publish(self, data, routing_key, priority=None, channel=None):
         """
         :param priority: 消息优先级
         :param data: 要发送的数据
         :param routing_key: 队列名
+        :param channel: 通道
         :return:
         """
         try:
-            channel = await self.get_channel()
-            async with channel:
+            if not channel:
+                channel = await self.get_channel()
+                async with channel:
+                    data = json.dumps(data)
+                    for _ in range(3):
+                        try:
+                            await channel.default_exchange.publish(aio_pika.Message(body=data.encode(), priority=priority),
+                                                                   routing_key=routing_key)
+                            return True
+                        except Exception as e:
+                            logger.error(f'publish error: {e}')
+            else:
                 data = json.dumps(data)
                 for _ in range(3):
                     try:
                         await channel.default_exchange.publish(aio_pika.Message(body=data.encode(), priority=priority),
                                                                routing_key=routing_key)
                         return True
                     except Exception as e:
```

### Comparing `hscan-2.4.1/scan/database/redis.py` & `hscan-2.4.2/scan/database/redis.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/downloade/downloader.py` & `hscan-2.4.2/scan/downloade/downloader.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/log.py` & `hscan-2.4.2/scan/log.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/monitor.py` & `hscan-2.4.2/scan/monitor.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/response.py` & `hscan-2.4.2/scan/response.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/spider.py` & `hscan-2.4.2/scan/spider.py`

 * *Files identical despite different names*

### Comparing `hscan-2.4.1/scan/util.py` & `hscan-2.4.2/scan/util.py`

 * *Files identical despite different names*

