# Comparing `tmp/worky-0.1.4.tar.gz` & `tmp/worky-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worky-0.1.4.tar", max compression
+gzip compressed data, was "worky-0.1.5.tar", max compression
```

## Comparing `worky-0.1.4.tar` & `worky-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.4/LICENSE
--rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.4/README.md
--rw-r--r--   0        0        0      822 2023-04-27 12:59:17.437414 worky-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-27 12:30:52.395763 worky-0.1.4/worky/__init__.py
--rw-r--r--   0        0        0     3618 2023-04-27 12:41:51.548388 worky-0.1.4/worky/main.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.4/worky/models/__init__.py
--rw-r--r--   0        0        0     1766 2023-04-27 08:41:36.836037 worky-0.1.4/worky/models/config_model.py
--rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.4/worky/models/log_level.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.4/worky/utils/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-0.1.4/worky/utils/logger.py
--rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.4/worky/utils/util.py
--rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 worky-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.5/LICENSE
+-rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.5/README.md
+-rw-r--r--   0        0        0      821 2023-04-27 13:18:52.724421 worky-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-04-27 13:17:33.681261 worky-0.1.5/worky/__init__.py
+-rw-r--r--   0        0        0      121 2023-04-27 13:11:32.808745 worky-0.1.5/worky/__main__.py
+-rw-r--r--   0        0        0     3618 2023-04-27 13:11:21.488772 worky-0.1.5/worky/main.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.5/worky/models/__init__.py
+-rw-r--r--   0        0        0     1766 2023-04-27 08:41:36.836037 worky-0.1.5/worky/models/config_model.py
+-rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.5/worky/models/log_level.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.5/worky/utils/__init__.py
+-rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-0.1.5/worky/utils/logger.py
+-rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.5/worky/utils/util.py
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 worky-0.1.5/PKG-INFO
```

### Comparing `worky-0.1.4/LICENSE` & `worky-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `worky-0.1.4/README.md` & `worky-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `worky-0.1.4/pyproject.toml` & `worky-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "worky"
-version = "0.1.4"
+version = "0.1.5"
 description = "Worky is a tool that helps to define and load project workspaces."
 authors = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 maintainers = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 readme = "README.md"
 packages = [{ include = "worky" }]
 homepage = "https://github.com/ZappaBoy/worky"
 repository = "https://github.com/ZappaBoy/worky"
@@ -21,8 +21,8 @@
 poetry2setup = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-start = "worky:start"
+worky = "worky:main"
```

### Comparing `worky-0.1.4/worky/main.py` & `worky-0.1.5/worky/main.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.4/worky/models/config_model.py` & `worky-0.1.5/worky/models/config_model.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.4/worky/utils/logger.py` & `worky-0.1.5/worky/utils/logger.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.4/PKG-INFO` & `worky-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worky
-Version: 0.1.4
+Version: 0.1.5
 Summary: Worky is a tool that helps to define and load project workspaces.
 Home-page: https://github.com/ZappaBoy/worky
 Keywords: worky,productivity,workspace,initializer
 Author: ZappaBoy
 Author-email: federico.zappone@justanother.cloud
 Maintainer: ZappaBoy
 Maintainer-email: federico.zappone@justanother.cloud
```

