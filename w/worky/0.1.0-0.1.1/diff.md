# Comparing `tmp/worky-0.1.0.tar.gz` & `tmp/worky-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worky-0.1.0.tar", max compression
+gzip compressed data, was "worky-0.1.1.tar", max compression
```

## Comparing `worky-0.1.0.tar` & `worky-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.0/LICENSE
--rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.0/README.md
--rw-r--r--   0        0        0      416 2023-04-25 21:54:39.904902 worky-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-26 20:23:42.987307 worky-0.1.0/src/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.0/src/models/__init__.py
--rw-r--r--   0        0        0     1766 2023-04-27 08:41:36.836037 worky-0.1.0/src/models/config_model.py
--rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.0/src/models/log_level.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.0/src/utils/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-27 09:57:43.625672 worky-0.1.0/src/utils/logger.py
--rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.0/src/utils/util.py
--rw-r--r--   0        0        0     3677 2023-04-27 10:37:19.313507 worky-0.1.0/src/worky.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 worky-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.1/LICENSE
+-rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.1/README.md
+-rw-r--r--   0        0        0      438 2023-04-27 11:35:33.942315 worky-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-04-27 11:33:02.976107 worky-0.1.1/src/worky/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.1/src/worky/models/__init__.py
+-rw-r--r--   0        0        0     1766 2023-04-27 08:41:36.836037 worky-0.1.1/src/worky/models/config_model.py
+-rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.1/src/worky/models/log_level.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.1/src/worky/utils/__init__.py
+-rw-r--r--   0        0        0     1246 2023-04-27 11:33:02.976107 worky-0.1.1/src/worky/utils/logger.py
+-rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.1/src/worky/utils/util.py
+-rw-r--r--   0        0        0     3695 2023-04-27 11:33:02.972773 worky-0.1.1/src/worky/worky.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 worky-0.1.1/PKG-INFO
```

### Comparing `worky-0.1.0/LICENSE` & `worky-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `worky-0.1.0/README.md` & `worky-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `worky-0.1.0/src/models/config_model.py` & `worky-0.1.1/src/worky/models/config_model.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.0/src/utils/logger.py` & `worky-0.1.1/src/worky/utils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from src.models.log_level import LogLevel
+from src.worky.models.log_level import LogLevel
 
 
 class Logger:
     def __init__(self, log_level: LogLevel | int = LogLevel.INFO):
         self.log_level = log_level
         self.logger = logging.getLogger()
         self.set_log_level(log_level)
```

### Comparing `worky-0.1.0/src/worky.py` & `worky-0.1.1/src/worky/worky.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 import os.path
 import subprocess
 import sys
 from typing import List
 
-from src.models.config_model import Config
-from src.utils.logger import Logger
-from src.utils.util import file_type
+from src.worky.models.config_model import Config
+from src.worky.utils.logger import Logger
+from src.worky.utils.util import file_type
 
 DEFAULT_CONFIG_DIR = os.path.expanduser('~/.config/worky')
 DEFAULT_CONFIG_FILE_NAME = 'config.toml'
 
 
 class Worky:
     config: Config = None
```

### Comparing `worky-0.1.0/PKG-INFO` & `worky-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worky
-Version: 0.1.0
+Version: 0.1.1
 Summary: Worky is a tool that helps to define and load project workspaces.
 Author: ZappaBoy
 Author-email: federico.zappone@justanother.cloud
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

