# Comparing `tmp/pikajson-0.1.5.tar.gz` & `tmp/pikajson-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikajson-0.1.5.tar", last modified: Wed Apr  5 08:35:59 2023, max compression
+gzip compressed data, was "pikajson-0.1.6.tar", last modified: Thu Apr 27 08:12:41 2023, max compression
```

## Comparing `pikajson-0.1.5.tar` & `pikajson-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-05 08:35:59.964364 pikajson-0.1.5/
--rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)      329 2023-04-05 08:35:59.962419 pikajson-0.1.5/PKG-INFO
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      114 2022-12-05 04:08:07.000000 pikajson-0.1.5/README.rst
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-05 08:35:59.865055 pikajson-0.1.5/pikajson/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)       23 2023-04-05 08:35:42.000000 pikajson-0.1.5/pikajson/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     6162 2022-12-05 04:08:07.000000 pikajson-0.1.5/pikajson/client.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-05 08:35:59.919205 pikajson-0.1.5/pikajson/exceptions/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2023-04-03 09:52:49.000000 pikajson-0.1.5/pikajson/exceptions/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      203 2023-04-03 09:52:49.000000 pikajson-0.1.5/pikajson/exceptions/need_retry_exception.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     9462 2023-04-05 08:35:42.000000 pikajson-0.1.5/pikajson/server.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-05 08:35:59.954039 pikajson-0.1.5/pikajson/tests/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2022-12-05 04:08:07.000000 pikajson-0.1.5/pikajson/tests/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     3492 2022-12-05 04:08:07.000000 pikajson-0.1.5/pikajson/tests/performance_test.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     7153 2023-04-03 09:07:19.000000 pikajson-0.1.5/pikajson/tests/test_client.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)    12488 2023-04-05 08:35:42.000000 pikajson-0.1.5/pikajson/tests/test_server.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-05 08:35:59.905411 pikajson-0.1.5/pikajson.egg-info/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      329 2023-04-05 08:35:59.000000 pikajson-0.1.5/pikajson.egg-info/PKG-INFO
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      435 2023-04-05 08:35:59.000000 pikajson-0.1.5/pikajson.egg-info/SOURCES.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        1 2023-04-05 08:35:59.000000 pikajson-0.1.5/pikajson.egg-info/dependency_links.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        5 2023-04-05 08:35:59.000000 pikajson-0.1.5/pikajson.egg-info/requires.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        9 2023-04-05 08:35:59.000000 pikajson-0.1.5/pikajson.egg-info/top_level.txt
--rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)       38 2023-04-05 08:35:59.964364 pikajson-0.1.5/setup.cfg
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      372 2022-12-05 04:52:49.000000 pikajson-0.1.5/setup.py
+drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.572249 pikajson-0.1.6/
+-rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)      329 2023-04-27 08:12:45.570299 pikajson-0.1.6/PKG-INFO
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      114 2022-12-05 04:08:07.000000 pikajson-0.1.6/README.rst
+drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.467127 pikajson-0.1.6/pikajson/
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)       23 2023-04-27 08:11:54.000000 pikajson-0.1.6/pikajson/__init__.py
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     6162 2022-12-05 04:08:07.000000 pikajson-0.1.6/pikajson/client.py
+drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.526123 pikajson-0.1.6/pikajson/exceptions/
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2023-04-03 09:52:49.000000 pikajson-0.1.6/pikajson/exceptions/__init__.py
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      203 2023-04-03 09:52:49.000000 pikajson-0.1.6/pikajson/exceptions/need_retry_exception.py
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     9760 2023-04-27 08:11:54.000000 pikajson-0.1.6/pikajson/server.py
+drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.560966 pikajson-0.1.6/pikajson/tests/
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2022-12-05 04:08:07.000000 pikajson-0.1.6/pikajson/tests/__init__.py
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     3492 2022-12-05 04:08:07.000000 pikajson-0.1.6/pikajson/tests/performance_test.py
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     7153 2023-04-03 09:07:19.000000 pikajson-0.1.6/pikajson/tests/test_client.py
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)    12488 2023-04-05 08:35:42.000000 pikajson-0.1.6/pikajson/tests/test_server.py
+drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.510368 pikajson-0.1.6/pikajson.egg-info/
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      329 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/PKG-INFO
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      435 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        1 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        5 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/requires.txt
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        9 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/top_level.txt
+-rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)       38 2023-04-27 08:12:45.573229 pikajson-0.1.6/setup.cfg
+-rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      372 2022-12-05 04:52:49.000000 pikajson-0.1.6/setup.py
```

### Comparing `pikajson-0.1.5/pikajson/client.py` & `pikajson-0.1.6/pikajson/client.py`

 * *Files identical despite different names*

### Comparing `pikajson-0.1.5/pikajson/server.py` & `pikajson-0.1.6/pikajson/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,15 +175,18 @@
                             if self._handlers[action](message):
                                 try:
                                     ch.basic_ack(delivery_tag=method.delivery_tag)
                                 except Exception as ex:
                                     logging.error("cannot send acknowledge: %s" % str(ex))
                                     self._repeatable_messages.append(unique)
                         except NeedRetryException as ex:
+                            logging.info("Resubmit required in line %s: %s" % (str(sys.exc_info()[-1].tb_lineno), str(ex)),
+                                extra={"queue": self._queue, "body": body, "host": self._host})
                             self._retry(ex.message, ex.timeout)
+                            ch.basic_ack(delivery_tag=method.delivery_tag)
                     else:
                         ch.basic_ack(delivery_tag=method.delivery_tag)
                 else:
                     logging.error("no such handler: %s" % action)
             else:
                 logging.error("wrong message format: no column action")
         except JSONDecodeError as ex:
```

### Comparing `pikajson-0.1.5/pikajson/tests/performance_test.py` & `pikajson-0.1.6/pikajson/tests/performance_test.py`

 * *Files identical despite different names*

### Comparing `pikajson-0.1.5/pikajson/tests/test_client.py` & `pikajson-0.1.6/pikajson/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pikajson-0.1.5/pikajson/tests/test_server.py` & `pikajson-0.1.6/pikajson/tests/test_server.py`

 * *Files identical despite different names*

