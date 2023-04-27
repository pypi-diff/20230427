# Comparing `tmp/watchtower_logging-0.6.3.tar.gz` & `tmp/watchtower_logging-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_logging-0.6.3.tar", last modified: Tue Apr 18 10:48:36 2023, max compression
+gzip compressed data, was "watchtower_logging-0.6.4.tar", last modified: Thu Apr 27 18:07:02 2023, max compression
```

## Comparing `watchtower_logging-0.6.3.tar` & `watchtower_logging-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/
--rw-rw-rw-   0        0        0      265 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     9544 2022-02-05 12:27:35.000000 watchtower_logging-0.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      965 2021-03-24 14:34:42.000000 watchtower_logging-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.017777 watchtower_logging-0.6.3/watchtower_logging/
--rw-rw-rw-   0        0        0      301 2021-03-24 14:31:06.000000 watchtower_logging-0.6.3/watchtower_logging/__init__.py
--rw-rw-rw-   0        0        0      864 2022-08-16 10:20:17.000000 watchtower_logging-0.6.3/watchtower_logging/django.py
--rw-rw-rw-   0        0        0       39 2021-01-11 14:33:51.000000 watchtower_logging-0.6.3/watchtower_logging/exceptions.py
--rw-rw-rw-   0        0        0     1158 2021-06-07 12:10:05.000000 watchtower_logging-0.6.3/watchtower_logging/utils.py
--rw-rw-rw-   0        0        0       21 2023-04-18 10:47:14.000000 watchtower_logging-0.6.3/watchtower_logging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/watchtower_logging/watchtower_handler/
--rw-rw-rw-   0        0        0    14097 2023-04-18 10:45:17.000000 watchtower_logging-0.6.3/watchtower_logging/watchtower_handler/__init__.py
--rw-rw-rw-   0        0        0    10632 2023-01-25 19:36:41.000000 watchtower_logging-0.6.3/watchtower_logging/watchtower_logging.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/watchtower_logging.egg-info/
--rw-rw-rw-   0        0        0      265 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 18:07:02.721814 watchtower_logging-0.6.4/
+-rw-rw-rw-   0        0        0      265 2023-04-27 18:07:02.721814 watchtower_logging-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9544 2022-02-05 12:27:35.000000 watchtower_logging-0.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 18:07:02.721814 watchtower_logging-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      965 2021-03-24 14:34:42.000000 watchtower_logging-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:07:02.703287 watchtower_logging-0.6.4/watchtower_logging/
+-rw-rw-rw-   0        0        0      301 2021-03-24 14:31:06.000000 watchtower_logging-0.6.4/watchtower_logging/__init__.py
+-rw-rw-rw-   0        0        0      864 2022-08-16 10:20:17.000000 watchtower_logging-0.6.4/watchtower_logging/django.py
+-rw-rw-rw-   0        0        0       39 2021-01-11 14:33:51.000000 watchtower_logging-0.6.4/watchtower_logging/exceptions.py
+-rw-rw-rw-   0        0        0     2175 2023-04-27 17:59:11.000000 watchtower_logging-0.6.4/watchtower_logging/utils.py
+-rw-rw-rw-   0        0        0       21 2023-04-27 18:06:30.000000 watchtower_logging-0.6.4/watchtower_logging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:07:02.721814 watchtower_logging-0.6.4/watchtower_logging/watchtower_handler/
+-rw-rw-rw-   0        0        0    14097 2023-04-18 10:45:17.000000 watchtower_logging-0.6.4/watchtower_logging/watchtower_handler/__init__.py
+-rw-rw-rw-   0        0        0    10749 2023-04-27 17:57:35.000000 watchtower_logging-0.6.4/watchtower_logging/watchtower_logging.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:07:02.721814 watchtower_logging-0.6.4/watchtower_logging.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-04-27 18:07:02.000000 watchtower_logging-0.6.4/watchtower_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-27 18:07:02.000000 watchtower_logging-0.6.4/watchtower_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 18:07:02.000000 watchtower_logging-0.6.4/watchtower_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-27 18:07:02.000000 watchtower_logging-0.6.4/watchtower_logging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-27 18:07:02.000000 watchtower_logging-0.6.4/watchtower_logging.egg-info/top_level.txt
```

### Comparing `watchtower_logging-0.6.3/README.md` & `watchtower_logging-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.3/setup.py` & `watchtower_logging-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.3/watchtower_logging/django.py` & `watchtower_logging-0.6.4/watchtower_logging/django.py`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.3/watchtower_logging/watchtower_handler/__init__.py` & `watchtower_logging-0.6.4/watchtower_logging/watchtower_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.3/watchtower_logging/watchtower_logging.py` & `watchtower_logging-0.6.4/watchtower_logging/watchtower_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 import types
 from watchtower_logging.watchtower_handler import WatchTowerHandler
 from watchtower_logging.exceptions import loggingException
 from watchtower_logging.version import __version__
+from watchtower_logging.utils import monitor_func
 from pythonjsonlogger import jsonlogger
 import random
 import string
 import datetime
 import pytz
 import traceback
 import sys
@@ -168,14 +169,15 @@
     logger.start = types.MethodType(start, logger)
     logger.debug = types.MethodType(logdebug, logger)
     logger.info = types.MethodType(info, logger)
     logger.warning = types.MethodType(warning, logger)
     logger.error = types.MethodType(error, logger)
     logger.critical = types.MethodType(critical, logger)
     logger.setExecutionId = types.MethodType(setExecutionId, logger)
+    logger.monitor_func = types.MethodType(monitor_func, logger)
     logger.setLevel(level)
     logger.setDefaultData = types.MethodType(setDefaultData, logger)
     logger.dedup = dedup
     logger.dedup_keys = dedup_keys
     logger.dedup_id_key = dedup_id_key or DEDUP_ID_KEY
     logger.beam_id = beam_id
```

