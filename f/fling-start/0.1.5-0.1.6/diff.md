# Comparing `tmp/fling_start-0.1.5.tar.gz` & `tmp/fling_start-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_start-0.1.5.tar", max compression
+gzip compressed data, was "fling_start-0.1.6.tar", max compression
```

## Comparing `fling_start-0.1.5.tar` & `fling_start-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.5/README.md
--rw-r--r--   0        0        0        6 2023-04-27 06:00:42.201559 fling_start-0.1.5/VERSION
--rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.5/fling/__init__.py
--rw-r--r--   0        0        0     1113 2023-04-27 05:22:45.984819 fling_start-0.1.5/fling/middleware.py
--rw-r--r--   0        0        0     4152 2023-04-27 06:05:21.136293 fling_start-0.1.5/fling/start.py
--rw-r--r--   0        0        0      778 2023-04-27 02:17:04.926768 fling_start-0.1.5/fling/static/start/styles.css
--rw-r--r--   0        0        0      415 2023-04-27 04:56:18.423473 fling_start-0.1.5/fling/templates/admin/index.html
--rw-r--r--   0        0        0     1716 2023-04-27 05:13:51.329779 fling_start-0.1.5/fling/templates/start/base.html
--rw-r--r--   0        0        0     8012 2023-04-27 05:17:42.026582 fling_start-0.1.5/fling/templates/start/index.html
--rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.5/fling/templates/start/x3d.html
--rw-r--r--   0        0        0      698 2023-04-27 06:04:36.660890 fling_start-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 fling_start-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.6/README.md
+-rw-r--r--   0        0        0        6 2023-04-27 07:00:19.148293 fling_start-0.1.6/VERSION
+-rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.6/fling/__init__.py
+-rw-r--r--   0        0        0     1113 2023-04-27 05:22:45.984819 fling_start-0.1.6/fling/middleware.py
+-rw-r--r--   0        0        0     4121 2023-04-27 06:37:18.137167 fling_start-0.1.6/fling/start.py
+-rw-r--r--   0        0        0      778 2023-04-27 02:17:04.926768 fling_start-0.1.6/fling/static/start/styles.css
+-rw-r--r--   0        0        0      415 2023-04-27 04:56:18.423473 fling_start-0.1.6/fling/templates/admin/index.html
+-rw-r--r--   0        0        0     1716 2023-04-27 05:13:51.329779 fling_start-0.1.6/fling/templates/start/base.html
+-rw-r--r--   0        0        0     8012 2023-04-27 05:17:42.026582 fling_start-0.1.6/fling/templates/start/index.html
+-rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.6/fling/templates/start/x3d.html
+-rw-r--r--   0        0        0      723 2023-04-27 07:00:15.541505 fling_start-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 fling_start-0.1.6/PKG-INFO
```

### Comparing `fling_start-0.1.5/fling/middleware.py` & `fling_start-0.1.6/fling/middleware.py`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.5/fling/start.py` & `fling_start-0.1.6/fling/start.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from collections import UserDict
-import os
-import signal
 from typing import Any, List
 from flask_bootstrap import Bootstrap5
 from flask import (
     Flask,
     Blueprint,
     render_template,
     render_template_string,
@@ -12,16 +10,18 @@
     request,
 )
 from flask_caching import Cache
 from flask_babel import Babel
 from flask_admin import Admin
 import pip
 import importlib
-from os import environ as osenv
 from dotenv import load_dotenv
+load_dotenv()
+
+from os import environ as osenv
 
 
 app = Flask("starter")
 cache = Cache(config={'CACHE_TYPE': 'SimpleCache'})
 cache.init_app(app)
 
 
@@ -65,15 +65,14 @@
 
 
 class Environ(UserDict):
     MISSING_KEYS: List = []
 
     def __init__(self, *args, **kwargs):
         kwargs.pop("app")
-        load_dotenv()
         keys = {}
         keys.update(**kwargs)
         super().__init__(*args, **keys)
 
     def ensure_keys(self, list_of_keys):
         """Make sure all the environment keys are available.
         If not, dump to the admin interface to capture them."""
```

### Comparing `fling_start-0.1.5/fling/static/start/styles.css` & `fling_start-0.1.6/fling/static/start/styles.css`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.5/fling/templates/start/base.html` & `fling_start-0.1.6/fling/templates/start/base.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.5/fling/templates/start/index.html` & `fling_start-0.1.6/fling/templates/start/index.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.5/fling/templates/start/x3d.html` & `fling_start-0.1.6/fling/templates/start/x3d.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.5/pyproject.toml` & `fling_start-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-start"
-version = "0.1.5"
+version = "0.1.6"
 description = "Side Project Management from the command line"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" }, { path = "README.md" }, 
@@ -24,7 +24,8 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 flask = "*"
 bootstrap-flask = "^2.2.0"
 flask-admin = "^1.6.1"
 flask-babel = "^3.1.0"
 flask-caching = "^2.0.2"
+python-dotenv = "^1.0.0"
```

### Comparing `fling_start-0.1.5/PKG-INFO` & `fling_start-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fling-start
-Version: 0.1.5
+Version: 0.1.6
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
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Fling Start - one-file python web application library
 
 ## Day zero acceleration
 
 This library makes it as easy as possible to build a web app in one file.
```

