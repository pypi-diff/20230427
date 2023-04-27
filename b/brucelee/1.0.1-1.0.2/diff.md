# Comparing `tmp/brucelee-1.0.1.tar.gz` & `tmp/brucelee-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brucelee-1.0.1.tar", last modified: Wed Apr 26 10:59:46 2023, max compression
+gzip compressed data, was "brucelee-1.0.2.tar", last modified: Thu Apr 27 07:15:26 2023, max compression
```

## Comparing `brucelee-1.0.1.tar` & `brucelee-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.112176 brucelee-1.0.1/
--rw-rw-rw-   0        0        0       41 2023-04-26 10:26:22.000000 brucelee-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6930 2023-04-26 10:59:46.111178 brucelee-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6145 2023-04-26 10:59:45.000000 brucelee-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.075273 brucelee-1.0.1/brucelee/
--rw-rw-rw-   0        0        0      295 2023-04-24 10:22:01.000000 brucelee-1.0.1/brucelee/__init__.py
--rw-rw-rw-   0        0        0      926 2023-04-26 08:44:44.000000 brucelee-1.0.1/brucelee/_loader.py
--rw-rw-rw-   0        0        0     2098 2023-04-26 07:57:34.000000 brucelee-1.0.1/brucelee/_utils.py
--rw-rw-rw-   0        0        0    10334 2023-04-23 10:09:38.000000 brucelee-1.0.1/brucelee/auth.py
--rw-rw-rw-   0        0        0    10919 2023-04-26 08:29:10.000000 brucelee-1.0.1/brucelee/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 brucelee-1.0.1/brucelee/cbv.py
--rw-rw-rw-   0        0        0     4515 2023-04-26 08:26:10.000000 brucelee-1.0.1/brucelee/config.py
--rw-rw-rw-   0        0        0     4201 2023-04-23 15:52:12.000000 brucelee-1.0.1/brucelee/controller.py
--rw-rw-rw-   0        0        0    12683 2023-04-23 11:33:03.000000 brucelee-1.0.1/brucelee/controller_utils.py
--rw-rw-rw-   0        0        0    12634 2023-04-25 05:16:51.000000 brucelee-1.0.1/brucelee/core.py
--rw-rw-rw-   0        0        0     6280 2023-04-19 08:32:59.000000 brucelee-1.0.1/brucelee/database.py
--rw-rw-rw-   0        0        0     6516 2023-04-26 08:48:08.000000 brucelee-1.0.1/brucelee/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 brucelee-1.0.1/brucelee/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 brucelee-1.0.1/brucelee/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.088240 brucelee-1.0.1/brucelee/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 brucelee-1.0.1/brucelee/scripts/__init__.py
--rw-rw-rw-   0        0        0     4649 2023-04-26 10:26:22.000000 brucelee-1.0.1/brucelee/scripts/_app.py
--rw-rw-rw-   0        0        0     2041 2023-04-26 10:26:22.000000 brucelee-1.0.1/brucelee/scripts/_project.py
--rw-rw-rw-   0        0        0      440 2023-04-26 10:26:22.000000 brucelee-1.0.1/brucelee/scripts/_run.py
--rw-rw-rw-   0        0        0      908 2023-04-26 10:25:22.000000 brucelee-1.0.1/brucelee/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.056186 brucelee-1.0.1/brucelee/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.094223 brucelee-1.0.1/brucelee/scripts/tpls/app/
--rw-rw-rw-   0        0        0     1637 2023-04-26 10:26:22.000000 brucelee-1.0.1/brucelee/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 brucelee-1.0.1/brucelee/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 brucelee-1.0.1/brucelee/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 brucelee-1.0.1/brucelee/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 brucelee-1.0.1/brucelee/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0     1263 2023-04-25 10:41:46.000000 brucelee-1.0.1/brucelee/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.097216 brucelee-1.0.1/brucelee/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.098214 brucelee-1.0.1/brucelee/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.107189 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      831 2023-04-26 09:58:29.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      146 2023-04-26 10:26:22.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.110180 brucelee-1.0.1/brucelee/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1234 2023-04-07 11:12:30.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1056 2023-04-07 11:24:23.000000 brucelee-1.0.1/brucelee/scripts/tpls/project/public/error_500.html
--rw-rw-rw-   0        0        0     1645 2023-04-24 14:18:26.000000 brucelee-1.0.1/brucelee/view.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:46.082256 brucelee-1.0.1/brucelee.egg-info/
--rw-rw-rw-   0        0        0     6930 2023-04-26 10:59:45.000000 brucelee-1.0.1/brucelee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1519 2023-04-26 10:59:46.000000 brucelee-1.0.1/brucelee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:59:45.000000 brucelee-1.0.1/brucelee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-26 10:59:45.000000 brucelee-1.0.1/brucelee.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      767 2023-04-26 10:59:45.000000 brucelee-1.0.1/brucelee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 10:59:45.000000 brucelee-1.0.1/brucelee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 10:59:46.112176 brucelee-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2935 2023-04-26 10:58:38.000000 brucelee-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.851922 brucelee-1.0.2/
+-rw-rw-rw-   0        0        0       41 2023-04-26 10:26:22.000000 brucelee-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6930 2023-04-27 07:15:26.850925 brucelee-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6145 2023-04-27 07:15:26.000000 brucelee-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.806045 brucelee-1.0.2/brucelee/
+-rw-rw-rw-   0        0        0      295 2023-04-24 10:22:01.000000 brucelee-1.0.2/brucelee/__init__.py
+-rw-rw-rw-   0        0        0      926 2023-04-26 08:44:44.000000 brucelee-1.0.2/brucelee/_loader.py
+-rw-rw-rw-   0        0        0     2098 2023-04-26 07:57:34.000000 brucelee-1.0.2/brucelee/_utils.py
+-rw-rw-rw-   0        0        0    10334 2023-04-23 10:09:38.000000 brucelee-1.0.2/brucelee/auth.py
+-rw-rw-rw-   0        0        0    10919 2023-04-26 08:29:10.000000 brucelee-1.0.2/brucelee/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 brucelee-1.0.2/brucelee/cbv.py
+-rw-rw-rw-   0        0        0     5273 2023-04-27 07:09:11.000000 brucelee-1.0.2/brucelee/config.py
+-rw-rw-rw-   0        0        0     4201 2023-04-23 15:52:12.000000 brucelee-1.0.2/brucelee/controller.py
+-rw-rw-rw-   0        0        0    12683 2023-04-23 11:33:03.000000 brucelee-1.0.2/brucelee/controller_utils.py
+-rw-rw-rw-   0        0        0    12634 2023-04-25 05:16:51.000000 brucelee-1.0.2/brucelee/core.py
+-rw-rw-rw-   0        0        0     6280 2023-04-19 08:32:59.000000 brucelee-1.0.2/brucelee/database.py
+-rw-rw-rw-   0        0        0     6516 2023-04-26 08:48:08.000000 brucelee-1.0.2/brucelee/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 brucelee-1.0.2/brucelee/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 brucelee-1.0.2/brucelee/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.821004 brucelee-1.0.2/brucelee/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 brucelee-1.0.2/brucelee/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4785 2023-04-27 07:10:31.000000 brucelee-1.0.2/brucelee/scripts/_app.py
+-rw-rw-rw-   0        0        0     2041 2023-04-26 10:26:22.000000 brucelee-1.0.2/brucelee/scripts/_project.py
+-rw-rw-rw-   0        0        0      601 2023-04-27 07:11:40.000000 brucelee-1.0.2/brucelee/scripts/_run.py
+-rw-rw-rw-   0        0        0     1481 2023-04-27 07:02:02.000000 brucelee-1.0.2/brucelee/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.777122 brucelee-1.0.2/brucelee/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.831974 brucelee-1.0.2/brucelee/scripts/tpls/app/
+-rw-rw-rw-   0        0        0     1637 2023-04-26 10:26:22.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0     1263 2023-04-25 10:41:46.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.833970 brucelee-1.0.2/brucelee/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.834968 brucelee-1.0.2/brucelee/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.844941 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      831 2023-04-26 09:58:29.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      146 2023-04-26 10:26:22.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.849928 brucelee-1.0.2/brucelee/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1234 2023-04-07 11:12:30.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1056 2023-04-07 11:24:23.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_500.html
+-rw-rw-rw-   0        0        0     1645 2023-04-24 14:18:26.000000 brucelee-1.0.2/brucelee/view.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.816021 brucelee-1.0.2/brucelee.egg-info/
+-rw-rw-rw-   0        0        0     6930 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1519 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      767 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:15:26.851922 brucelee-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2935 2023-04-27 07:14:58.000000 brucelee-1.0.2/setup.py
```

### Comparing `brucelee-1.0.1/PKG-INFO` & `brucelee-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brucelee
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/brucelee
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `brucelee-1.0.1/README.md` & `brucelee-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/_loader.py` & `brucelee-1.0.2/brucelee/_loader.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/_utils.py` & `brucelee-1.0.2/brucelee/_utils.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/auth.py` & `brucelee-1.0.2/brucelee/auth.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/base_controller.py` & `brucelee-1.0.2/brucelee/base_controller.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/cbv.py` & `brucelee-1.0.2/brucelee/cbv.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/config.py` & `brucelee-1.0.2/brucelee/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,39 @@
-import os
+import os,sys
 import yaml
 import logging
 from hashlib import md5
 from typing import Dict
-ROOT_PATH = os.path.realpath(os.curdir)
+import os.path
+
 # from fastapi.logger import logger
 
 import re
+ 
+
+def is_in_brucelee(directory):
+    """
+    check exists configs dir, apps dir, main.py and configs/general.yaml 
+    """
+    
+    configs_dir = os.path.join(directory, 'configs')
+    apps_dir = os.path.join(directory, 'apps')
+    main_file = os.path.join(directory, 'main.py')
+
+    if not os.path.exists(configs_dir) or not os.path.exists(apps_dir) or not os.path.exists(main_file):
+        return False  
+    general_file = os.path.join(configs_dir, 'general.yaml')
+
+    if not os.path.exists(general_file):
+        return False
+    
+    return True
+ROOT_PATH = os.path.realpath(os.curdir)
+CLI_MODE = sys.argv[0] == 'brucelee'
+IS_IN_BRUCELEE = is_in_brucelee(ROOT_PATH)
 
 def _extract_name(string):
     match = re.search(r'{([^}]*)}', string)
     if match:
         return match.group(1)
     else:
         return None
@@ -27,15 +50,18 @@
             with open(self.filename, "r") as f:
                 self.config = yaml.safe_load(f)
         elif os.path.isdir(self.filename):
             self.config = self._merge_yaml_files(self.filename)
         elif self.config:
             return True
         else:
-            print(f"{self.filename} is not a file or directory")
+            if CLI_MODE:
+                pass
+            else:
+                raise Exception(f"{self.filename} is not a file or directory")
             return False
     def dump(self):
         return yaml.safe_dump(self.config) if self.config else ""
     def save(self):
         if not self.filename:
             return False
         with open(self.filename, "w") as f:
```

### Comparing `brucelee-1.0.1/brucelee/controller.py` & `brucelee-1.0.2/brucelee/controller.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/controller_utils.py` & `brucelee-1.0.2/brucelee/controller_utils.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/core.py` & `brucelee-1.0.2/brucelee/core.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/database.py` & `brucelee-1.0.2/brucelee/database.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/midware.py` & `brucelee-1.0.2/brucelee/midware.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/midware_casbin.py` & `brucelee-1.0.2/brucelee/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/midware_session.py` & `brucelee-1.0.2/brucelee/midware_session.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/_app.py` & `brucelee-1.0.2/brucelee/scripts/_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import sys,os
 from typing import Any
 from jinja2 import Template
 from brucelee._utils import is_valid_filename
+from  brucelee.config import IS_IN_BRUCELEE
 
 class Generator():
     def __init__(self,args) -> None:
         self.args=args
         pass
     def gen_common(self):
         '''#todo: check configs dir
@@ -102,14 +103,17 @@
         
         self.add_enabled_to_app(app_name)
         
         print("Done!")
     pass
 
 def main():
+    if not IS_IN_BRUCELEE:
+        print(f"Please exec in brucelee dir")
+        exit()
     self_file = __file__.lstrip("_").replace(".py",'')
     parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [--name NAME] [-d DIR]", description='new app')
     parser.add_argument('--name',help="name to create app")
     parser.add_argument('-d','--dir',help="dir to store app files")
     args = parser.parse_args()
     if not any(args.__dict__.values()):
         parser.print_help()
```

### Comparing `brucelee-1.0.1/brucelee/scripts/_project.py` & `brucelee-1.0.2/brucelee/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/app/controller.tpl` & `brucelee-1.0.2/brucelee/scripts/tpls/app/controller.tpl`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/app/css.tpl` & `brucelee-1.0.2/brucelee/scripts/tpls/app/css.tpl`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/app/view.tpl` & `brucelee-1.0.2/brucelee/scripts/tpls/app/view.tpl`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/project/configs/alembic.ini` & `brucelee-1.0.2/brucelee/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/project/configs/database.yaml` & `brucelee-1.0.2/brucelee/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/project/configs/general.yaml` & `brucelee-1.0.2/brucelee/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/project/public/error_404.html` & `brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/scripts/tpls/project/public/error_500.html` & `brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee/view.py` & `brucelee-1.0.2/brucelee/view.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee.egg-info/PKG-INFO` & `brucelee-1.0.2/brucelee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brucelee
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/brucelee
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `brucelee-1.0.1/brucelee.egg-info/SOURCES.txt` & `brucelee-1.0.2/brucelee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/brucelee.egg-info/requires.txt` & `brucelee-1.0.2/brucelee.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.1/setup.py` & `brucelee-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup,find_packages
 import chardet
 
-version = "1.0.1"
+version = "1.0.2"
 def update_readme(source,spec,content=""):
     assert source or content
 
     if not content:
         with open(source, 'r') as file:
             content = file.read()
     with open('README.md', 'r') as file:
```

