# Comparing `tmp/whitson_tool_helper-0.0.8.tar.gz` & `tmp/whitson_tool_helper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitson_tool_helper-0.0.8.tar", last modified: Thu Apr 27 15:22:47 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.1.0.tar", last modified: Thu Apr 27 15:42:05 2023, max compression
```

## Comparing `whitson_tool_helper-0.0.8.tar` & `whitson_tool_helper-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:22:47.259948 whitson_tool_helper-0.0.8/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-27 15:22:47.259948 whitson_tool_helper-0.0.8/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      564 2023-04-27 15:22:41.000000 whitson_tool_helper-0.0.8/pyproject.toml
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-04-27 15:22:47.259948 whitson_tool_helper-0.0.8/setup.cfg
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:22:47.249948 whitson_tool_helper-0.0.8/src/
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:22:47.259948 whitson_tool_helper-0.0.8/src/whitson_tool_helper/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/__init__.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/logger.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:22:47.259948 whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/aux.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2988 2023-04-27 15:14:46.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/main.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4403 2023-04-26 14:33:47.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/pubsub.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3969 2023-04-27 13:40:01.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/timeout.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper/whitson_exceptions.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:22:47.259948 whitson_tool_helper-0.0.8/src/whitson_tool_helper.egg-info/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      138 2023-04-26 12:44:58.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper.egg-info/.SOURCES.txt.~undo-tree~
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-27 15:22:47.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      584 2023-04-27 15:22:47.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-04-27 15:22:47.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-04-27 15:22:47.000000 whitson_tool_helper-0.0.8/src/whitson_tool_helper.egg-info/top_level.txt
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:42:05.959943 whitson_tool_helper-0.1.0/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-27 15:42:05.959943 whitson_tool_helper-0.1.0/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      560 2023-04-27 15:42:00.000000 whitson_tool_helper-0.1.0/pyproject.toml
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-04-27 15:42:05.959943 whitson_tool_helper-0.1.0/setup.cfg
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:42:05.959943 whitson_tool_helper-0.1.0/src/
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:42:05.959943 whitson_tool_helper-0.1.0/src/whitson_tool_helper/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/__init__.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/logger.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:42:05.959943 whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/aux.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2988 2023-04-27 15:14:46.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/main.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4403 2023-04-26 14:33:47.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/pubsub.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3969 2023-04-27 13:40:01.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/timeout.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper/whitson_exceptions.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:42:05.959943 whitson_tool_helper-0.1.0/src/whitson_tool_helper.egg-info/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      138 2023-04-26 12:44:58.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper.egg-info/.SOURCES.txt.~undo-tree~
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-27 15:42:05.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      584 2023-04-27 15:42:05.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-04-27 15:42:05.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-04-27 15:42:05.000000 whitson_tool_helper-0.1.0/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.0.8/pyproject.toml` & `whitson_tool_helper-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-    version =  "0.0.8"
+version =  "0.1.0"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 requires-python = ">=3.11"
```

### Comparing `whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/main.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.0.8/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.1.0/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.0.8/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.1.0/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.0.8/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.1.0/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.0.8/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.1.0/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

