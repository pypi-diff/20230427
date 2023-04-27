# Comparing `tmp/taskiq_aiohttp-0.1.0.tar.gz` & `tmp/taskiq_aiohttp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aiohttp-0.1.0.tar", max compression
+gzip compressed data, was "taskiq_aiohttp-0.1.1.tar", max compression
```

## Comparing `taskiq_aiohttp-0.1.0.tar` & `taskiq_aiohttp-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-04-23 02:45:03.015822 taskiq_aiohttp-0.1.0/LICENSE
--rw-r--r--   0        0        0     1067 2023-04-23 02:45:03.015822 taskiq_aiohttp-0.1.0/README.md
--rw-r--r--   0        0        0     1716 2023-04-23 02:45:03.015822 taskiq_aiohttp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      106 2023-04-23 02:45:03.015822 taskiq_aiohttp-0.1.0/taskiq_aiohttp/__init__.py
--rw-r--r--   0        0        0     3637 2023-04-23 02:45:03.015822 taskiq_aiohttp-0.1.0/taskiq_aiohttp/initializer.py
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1067 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/README.md
+-rw-r--r--   0        0        0     1716 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/taskiq_aiohttp/__init__.py
+-rw-r--r--   0        0        0     3789 2023-04-27 14:34:06.091547 taskiq_aiohttp-0.1.1/taskiq_aiohttp/initializer.py
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.1.1/PKG-INFO
```

### Comparing `taskiq_aiohttp-0.1.0/LICENSE` & `taskiq_aiohttp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.0/README.md` & `taskiq_aiohttp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.0/pyproject.toml` & `taskiq_aiohttp-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-aiohttp"
 description = "Taskiq integration with AioHTTP framework"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_aiohttp-0.1.0/PKG-INFO` & `taskiq_aiohttp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-aiohttp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Taskiq integration with AioHTTP framework
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
```

