# Comparing `tmp/py_optional-1.0a5.tar.gz` & `tmp/py_optional-1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_optional-1.0a5.tar", max compression
+gzip compressed data, was "py_optional-1.0a6.tar", max compression
```

## Comparing `py_optional-1.0a5.tar` & `py_optional-1.0a6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-04-24 14:08:59.028506 py_optional-1.0a5/LICENSE
--rw-r--r--   0        0        0     3316 2023-04-24 14:08:59.028506 py_optional-1.0a5/README.md
--rw-r--r--   0        0        0      126 2023-04-24 14:08:59.028506 py_optional-1.0a5/optional/__init__.py
--rw-r--r--   0        0        0      109 2023-04-24 14:08:59.028506 py_optional-1.0a5/optional/exceptions.py
--rw-r--r--   0        0        0     7027 2023-04-24 14:08:59.028506 py_optional-1.0a5/optional/optional.py
--rw-r--r--   0        0        0      855 2023-04-24 14:09:26.005612 py_optional-1.0a5/pyproject.toml
--rw-r--r--   0        0        0     3885 1970-01-01 00:00:00.000000 py_optional-1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-24 14:25:51.984970 py_optional-1.0a6/LICENSE
+-rw-r--r--   0        0        0     3316 2023-04-24 14:25:51.988970 py_optional-1.0a6/README.md
+-rw-r--r--   0        0        0      126 2023-04-24 14:25:51.988970 py_optional-1.0a6/optional/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-24 14:25:51.988970 py_optional-1.0a6/optional/exceptions.py
+-rw-r--r--   0        0        0     7027 2023-04-24 14:25:51.988970 py_optional-1.0a6/optional/optional.py
+-rw-r--r--   0        0        0      855 2023-04-24 14:26:08.689181 py_optional-1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     3885 1970-01-01 00:00:00.000000 py_optional-1.0a6/PKG-INFO
```

### Comparing `py_optional-1.0a5/LICENSE` & `py_optional-1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_optional-1.0a5/README.md` & `py_optional-1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `py_optional-1.0a5/optional/optional.py` & `py_optional-1.0a6/optional/optional.py`

 * *Files identical despite different names*

### Comparing `py_optional-1.0a5/pyproject.toml` & `py_optional-1.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-optional"
-version = "1.0a5"
+version = "1.0a6"
 description = "Tools to convert SQLAlchemy models to Pydantic models"
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "optional" }]
 
 [tool.poetry.dependencies]
```

### Comparing `py_optional-1.0a5/PKG-INFO` & `py_optional-1.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-optional
-Version: 1.0a5
+Version: 1.0a6
 Summary: Tools to convert SQLAlchemy models to Pydantic models
 License: MIT
 Author: Francisco Del Roio
 Author-email: francipvb@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-optional Version: 1.0a5 Summary: Tools to
+Metadata-Version: 2.1 Name: py-optional Version: 1.0a6 Summary: Tools to
 convert SQLAlchemy models to Pydantic models License: MIT Author: Francisco Del
 Roio Author-email: francipvb@hotmail.com Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown # py-optional
```

