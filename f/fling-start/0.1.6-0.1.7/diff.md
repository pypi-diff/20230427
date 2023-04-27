# Comparing `tmp/fling_start-0.1.6.tar.gz` & `tmp/fling_start-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_start-0.1.6.tar", max compression
+gzip compressed data, was "fling_start-0.1.7.tar", max compression
```

## Comparing `fling_start-0.1.6.tar` & `fling_start-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.6/README.md
--rw-r--r--   0        0        0        6 2023-04-27 07:00:19.148293 fling_start-0.1.6/VERSION
--rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.6/fling/__init__.py
--rw-r--r--   0        0        0     1113 2023-04-27 05:22:45.984819 fling_start-0.1.6/fling/middleware.py
--rw-r--r--   0        0        0     4121 2023-04-27 06:37:18.137167 fling_start-0.1.6/fling/start.py
--rw-r--r--   0        0        0      778 2023-04-27 02:17:04.926768 fling_start-0.1.6/fling/static/start/styles.css
--rw-r--r--   0        0        0      415 2023-04-27 04:56:18.423473 fling_start-0.1.6/fling/templates/admin/index.html
--rw-r--r--   0        0        0     1716 2023-04-27 05:13:51.329779 fling_start-0.1.6/fling/templates/start/base.html
--rw-r--r--   0        0        0     8012 2023-04-27 05:17:42.026582 fling_start-0.1.6/fling/templates/start/index.html
--rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.6/fling/templates/start/x3d.html
--rw-r--r--   0        0        0      723 2023-04-27 07:00:15.541505 fling_start-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 fling_start-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.7/README.md
+-rw-r--r--   0        0        0        6 2023-04-27 16:50:02.805291 fling_start-0.1.7/VERSION
+-rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.7/fling/__init__.py
+-rw-r--r--   0        0        0     1113 2023-04-27 05:22:45.984819 fling_start-0.1.7/fling/middleware.py
+-rw-r--r--   0        0        0     4127 2023-04-27 16:49:54.982507 fling_start-0.1.7/fling/start.py
+-rw-r--r--   0        0        0      778 2023-04-27 02:17:04.926768 fling_start-0.1.7/fling/static/start/styles.css
+-rw-r--r--   0        0        0      487 2023-04-27 16:49:12.318822 fling_start-0.1.7/fling/templates/admin/index.html
+-rw-r--r--   0        0        0     1716 2023-04-27 05:13:51.329779 fling_start-0.1.7/fling/templates/start/base.html
+-rw-r--r--   0        0        0     8012 2023-04-27 05:17:42.026582 fling_start-0.1.7/fling/templates/start/index.html
+-rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.7/fling/templates/start/x3d.html
+-rw-r--r--   0        0        0      754 2023-04-27 16:50:10.502122 fling_start-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 fling_start-0.1.7/PKG-INFO
```

### Comparing `fling_start-0.1.6/fling/middleware.py` & `fling_start-0.1.7/fling/middleware.py`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.6/fling/start.py` & `fling_start-0.1.7/fling/start.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     request,
 )
 from flask_caching import Cache
 from flask_babel import Babel
 from flask_admin import Admin
 import pip
 import importlib
-from dotenv import load_dotenv
+from dotenv_vault import load_dotenv
 load_dotenv()
 
 from os import environ as osenv
 
 
 app = Flask("starter")
 cache = Cache(config={'CACHE_TYPE': 'SimpleCache'})
```

### Comparing `fling_start-0.1.6/fling/static/start/styles.css` & `fling_start-0.1.7/fling/static/start/styles.css`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.6/fling/templates/start/base.html` & `fling_start-0.1.7/fling/templates/start/base.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.6/fling/templates/start/index.html` & `fling_start-0.1.7/fling/templates/start/index.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.6/fling/templates/start/x3d.html` & `fling_start-0.1.7/fling/templates/start/x3d.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.6/pyproject.toml` & `fling_start-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-start"
-version = "0.1.6"
+version = "0.1.7"
 description = "Side Project Management from the command line"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" }, { path = "README.md" }, 
@@ -24,8 +24,9 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 flask = "*"
 bootstrap-flask = "^2.2.0"
 flask-admin = "^1.6.1"
 flask-babel = "^3.1.0"
 flask-caching = "^2.0.2"
-python-dotenv = "^1.0.0"
+python-dotenv = "0.21.1"
+python-dotenv-vault = "^0.4.1"
```

### Comparing `fling_start-0.1.6/PKG-INFO` & `fling_start-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fling-start
-Version: 0.1.6
+Version: 0.1.7
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bootstrap-flask (>=2.2.0,<3.0.0)
 Requires-Dist: flask
 Requires-Dist: flask-admin (>=1.6.1,<2.0.0)
 Requires-Dist: flask-babel (>=3.1.0,<4.0.0)
 Requires-Dist: flask-caching (>=2.0.2,<3.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: python-dotenv (==0.21.1)
+Requires-Dist: python-dotenv-vault (>=0.4.1,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Fling Start - one-file python web application library
 
 ## Day zero acceleration
 
 This library makes it as easy as possible to build a web app in one file.
```

