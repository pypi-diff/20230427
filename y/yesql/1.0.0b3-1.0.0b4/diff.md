# Comparing `tmp/yesql-1.0.0b3.tar.gz` & `tmp/yesql-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yesql-1.0.0b3.tar", max compression
+gzip compressed data, was "yesql-1.0.0b4.tar", max compression
```

## Comparing `yesql-1.0.0b3.tar` & `yesql-1.0.0b4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       47 2023-04-26 21:26:33.956511 yesql-1.0.0b3/LICENSE.md
--rw-r--r--   0        0        0     2624 2023-04-26 21:26:33.956511 yesql-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/__init__.py
--rw-r--r--   0        0        0     5117 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/api.py
--rw-r--r--   0        0        0        0 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/bin/__init__.py
--rw-r--r--   0        0        0      847 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/bin/main.py
--rw-r--r--   0        0        0     5133 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/bin/stubgen.py
--rw-r--r--   0        0        0        0 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/__init__.py
--rw-r--r--   0        0        0     1878 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/__init__.py
--rw-r--r--   0        0        0     4945 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/base.py
--rw-r--r--   0        0        0     2056 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/postgresql/__init__.py
--rw-r--r--   0        0        0    13088 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/postgresql/_asyncpg.py
--rw-r--r--   0        0        0    21761 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/postgresql/_psycopg.py
--rw-r--r--   0        0        0     2432 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/middleware.py
--rw-r--r--   0        0        0    11217 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/parse.py
--rw-r--r--   0        0        0     6988 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/support.py
--rw-r--r--   0        0        0     2857 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/types.py
--rw-r--r--   0        0        0    11577 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/dynamic.py
--rw-r--r--   0        0        0        0 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/py.typed
--rw-r--r--   0        0        0    13182 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/repository.py
--rw-r--r--   0        0        0    16048 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/statement.py
--rw-r--r--   0        0        0     7049 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/stubgen.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 yesql-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-04-27 11:24:57.788229 yesql-1.0.0b4/LICENSE.md
+-rw-r--r--   0        0        0     2646 2023-04-27 11:24:57.788229 yesql-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     6139 2023-04-27 11:24:57.788229 yesql-1.0.0b4/README.md
+-rw-r--r--   0        0        0       47 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/__init__.py
+-rw-r--r--   0        0        0     5117 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/api.py
+-rw-r--r--   0        0        0        0 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/bin/__init__.py
+-rw-r--r--   0        0        0      847 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/bin/main.py
+-rw-r--r--   0        0        0     5133 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/bin/stubgen.py
+-rw-r--r--   0        0        0        0 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/__init__.py
+-rw-r--r--   0        0        0     1878 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/drivers/__init__.py
+-rw-r--r--   0        0        0     4945 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/drivers/base.py
+-rw-r--r--   0        0        0     2056 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/drivers/postgresql/__init__.py
+-rw-r--r--   0        0        0    13088 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/drivers/postgresql/_asyncpg.py
+-rw-r--r--   0        0        0    21761 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/drivers/postgresql/_psycopg.py
+-rw-r--r--   0        0        0     2432 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/middleware.py
+-rw-r--r--   0        0        0    11217 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/parse.py
+-rw-r--r--   0        0        0     6988 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/support.py
+-rw-r--r--   0        0        0     2857 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/core/types.py
+-rw-r--r--   0        0        0    11577 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/dynamic.py
+-rw-r--r--   0        0        0        0 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/py.typed
+-rw-r--r--   0        0        0    13182 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/repository.py
+-rw-r--r--   0        0        0    16048 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/statement.py
+-rw-r--r--   0        0        0     7049 2023-04-27 11:24:57.803805 yesql-1.0.0b4/yesql/stubgen.py
+-rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 yesql-1.0.0b4/PKG-INFO
```

### Comparing `yesql-1.0.0b3/pyproject.toml` & `yesql-1.0.0b4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "yesql"
-version = "1.0.0b3"
+version = "1.0.0b4"
 description = "yesql is a SQL-first data access library that will replace your ORM."
+readme = "README.md"
 authors = ["Sean Stewart <sean_stewart@me.com>"]
 license = "MIT"
 keywords = ["typing", "data", "annotations", "validation", "json-schema"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Natural Language :: English",
@@ -72,15 +73,15 @@
 non_interactive = true
 ignore_missing_imports = true
 no_strict_optional = true
 follow_imports = "silent"
 exclude = ".*tests/.*|.*docs/.*"
 
 [tool.bumpver]
-current_version = "v1.0.0-beta3"
+current_version = "v1.0.0-beta4"
 version_pattern = "vMAJOR.MINOR.PATCH[-TAGNUM]"
 commit_message = "bump version to {new_version} [ci skip]"
 tag = false
 push = false
 commit = true
```

### Comparing `yesql-1.0.0b3/yesql/api.py` & `yesql-1.0.0b4/yesql/api.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/bin/main.py` & `yesql-1.0.0b4/yesql/bin/main.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/bin/stubgen.py` & `yesql-1.0.0b4/yesql/bin/stubgen.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/drivers/__init__.py` & `yesql-1.0.0b4/yesql/core/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/drivers/base.py` & `yesql-1.0.0b4/yesql/core/drivers/base.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/drivers/postgresql/__init__.py` & `yesql-1.0.0b4/yesql/core/drivers/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/drivers/postgresql/_asyncpg.py` & `yesql-1.0.0b4/yesql/core/drivers/postgresql/_asyncpg.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/drivers/postgresql/_psycopg.py` & `yesql-1.0.0b4/yesql/core/drivers/postgresql/_psycopg.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/middleware.py` & `yesql-1.0.0b4/yesql/core/middleware.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/parse.py` & `yesql-1.0.0b4/yesql/core/parse.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/support.py` & `yesql-1.0.0b4/yesql/core/support.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/core/types.py` & `yesql-1.0.0b4/yesql/core/types.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/dynamic.py` & `yesql-1.0.0b4/yesql/dynamic.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/repository.py` & `yesql-1.0.0b4/yesql/repository.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/statement.py` & `yesql-1.0.0b4/yesql/statement.py`

 * *Files identical despite different names*

### Comparing `yesql-1.0.0b3/yesql/stubgen.py` & `yesql-1.0.0b4/yesql/stubgen.py`

 * *Files identical despite different names*

