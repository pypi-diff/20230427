# Comparing `tmp/worky-0.1.5.tar.gz` & `tmp/worky-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worky-0.1.5.tar", max compression
+gzip compressed data, was "worky-0.1.6.tar", max compression
```

## Comparing `worky-0.1.5.tar` & `worky-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.5/LICENSE
--rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.5/README.md
--rw-r--r--   0        0        0      821 2023-04-27 13:18:52.724421 worky-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       29 2023-04-27 13:17:33.681261 worky-0.1.5/worky/__init__.py
--rw-r--r--   0        0        0      121 2023-04-27 13:11:32.808745 worky-0.1.5/worky/__main__.py
--rw-r--r--   0        0        0     3618 2023-04-27 13:11:21.488772 worky-0.1.5/worky/main.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.5/worky/models/__init__.py
--rw-r--r--   0        0        0     1766 2023-04-27 08:41:36.836037 worky-0.1.5/worky/models/config_model.py
--rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.5/worky/models/log_level.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.5/worky/utils/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-0.1.5/worky/utils/logger.py
--rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.5/worky/utils/util.py
--rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 worky-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.6/LICENSE
+-rw-r--r--   0        0        0      795 2023-04-27 10:46:52.364225 worky-0.1.6/README.md
+-rw-r--r--   0        0        0      821 2023-04-27 13:58:26.636824 worky-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-04-27 13:17:33.681261 worky-0.1.6/worky/__init__.py
+-rw-r--r--   0        0        0      121 2023-04-27 13:11:32.808745 worky-0.1.6/worky/__main__.py
+-rw-r--r--   0        0        0     3618 2023-04-27 13:11:21.488772 worky-0.1.6/worky/main.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.6/worky/models/__init__.py
+-rw-r--r--   0        0        0     1766 2023-04-27 08:41:36.836037 worky-0.1.6/worky/models/config_model.py
+-rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.6/worky/models/log_level.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.6/worky/utils/__init__.py
+-rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-0.1.6/worky/utils/logger.py
+-rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.6/worky/utils/util.py
+-rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 worky-0.1.6/PKG-INFO
```

### Comparing `worky-0.1.5/LICENSE` & `worky-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `worky-0.1.5/README.md` & `worky-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `worky-0.1.5/pyproject.toml` & `worky-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "worky"
-version = "0.1.5"
+version = "0.1.6"
 description = "Worky is a tool that helps to define and load project workspaces."
 authors = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 maintainers = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 readme = "README.md"
 packages = [{ include = "worky" }]
 homepage = "https://github.com/ZappaBoy/worky"
 repository = "https://github.com/ZappaBoy/worky"
 documentation = "https://github.com/ZappaBoy/worky/blob/main/README.md"
 keywords = ["worky", "productivity", "workspace", "initializer"]
 classifiers = [
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 poetry2setup = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `worky-0.1.5/worky/main.py` & `worky-0.1.6/worky/main.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.5/worky/models/config_model.py` & `worky-0.1.6/worky/models/config_model.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.5/worky/utils/logger.py` & `worky-0.1.6/worky/utils/logger.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.5/PKG-INFO` & `worky-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: worky
-Version: 0.1.5
+Version: 0.1.6
 Summary: Worky is a tool that helps to define and load project workspaces.
 Home-page: https://github.com/ZappaBoy/worky
 Keywords: worky,productivity,workspace,initializer
 Author: ZappaBoy
 Author-email: federico.zappone@justanother.cloud
 Maintainer: ZappaBoy
 Maintainer-email: federico.zappone@justanother.cloud
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Project-URL: Documentation, https://github.com/ZappaBoy/worky/blob/main/README.md
 Project-URL: Repository, https://github.com/ZappaBoy/worky
 Description-Content-Type: text/markdown
 
 # Worky
```

