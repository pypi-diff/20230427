# Comparing `tmp/olstecnologia-1.1.3.tar.gz` & `tmp/olstecnologia-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olstecnologia-1.1.3.tar", max compression
+gzip compressed data, was "olstecnologia-1.1.4.tar", max compression
```

## Comparing `olstecnologia-1.1.3.tar` & `olstecnologia-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.3/olstecnologia/__init__.py
--rw-r--r--   0        0        0    10752 2023-04-25 15:07:24.525635 olstecnologia-1.1.3/olstecnologia/app.py
--rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.3/olstecnologia/config/__init__.py
--rw-r--r--   0        0        0     1836 2023-04-17 11:29:49.555822 olstecnologia-1.1.3/olstecnologia/config/database.py
--rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.3/olstecnologia/config/fbclient.dll
--rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.3/olstecnologia/features/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-26 13:17:41.244954 olstecnologia-1.1.3/olstecnologia/features/read_fb_for_postgres_feature.py
--rw-r--r--   0        0        0     8810 2023-04-25 15:26:55.236961 olstecnologia-1.1.3/olstecnologia/features/update_addres_feature.py
--rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.3/olstecnologia/services/__init__.py
--rw-r--r--   0        0        0     6532 2023-04-25 14:38:00.752471 olstecnologia-1.1.3/olstecnologia/services/check_db_service.py
--rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.3/olstecnologia/services/connection_service.py
--rw-r--r--   0        0        0     7069 2023-04-25 18:35:48.039984 olstecnologia-1.1.3/olstecnologia/services/services_service.py
--rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.3/olstecnologia/services/utils_service.py
--rw-r--r--   0        0        0      732 2023-04-27 18:14:38.943339 olstecnologia-1.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.3/README.md
--rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 olstecnologia-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.4/olstecnologia/__init__.py
+-rw-r--r--   0        0        0    10752 2023-04-25 15:07:24.525635 olstecnologia-1.1.4/olstecnologia/app.py
+-rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.4/olstecnologia/config/__init__.py
+-rw-r--r--   0        0        0     1836 2023-04-17 11:29:49.555822 olstecnologia-1.1.4/olstecnologia/config/database.py
+-rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.4/olstecnologia/config/fbclient.dll
+-rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.4/olstecnologia/features/__init__.py
+-rw-r--r--   0        0        0     4913 2023-04-27 18:16:49.954217 olstecnologia-1.1.4/olstecnologia/features/read_fb_for_postgres_feature.py
+-rw-r--r--   0        0        0     8810 2023-04-25 15:26:55.236961 olstecnologia-1.1.4/olstecnologia/features/update_addres_feature.py
+-rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.4/olstecnologia/services/__init__.py
+-rw-r--r--   0        0        0     6532 2023-04-25 14:38:00.752471 olstecnologia-1.1.4/olstecnologia/services/check_db_service.py
+-rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.4/olstecnologia/services/connection_service.py
+-rw-r--r--   0        0        0     7069 2023-04-25 18:35:48.039984 olstecnologia-1.1.4/olstecnologia/services/services_service.py
+-rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.4/olstecnologia/services/utils_service.py
+-rw-r--r--   0        0        0      692 2023-04-27 18:18:46.551653 olstecnologia-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.4/README.md
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 olstecnologia-1.1.4/PKG-INFO
```

### Comparing `olstecnologia-1.1.3/olstecnologia/app.py` & `olstecnologia-1.1.4/olstecnologia/app.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/olstecnologia/config/database.py` & `olstecnologia-1.1.4/olstecnologia/config/database.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/olstecnologia/config/fbclient.dll` & `olstecnologia-1.1.4/olstecnologia/config/fbclient.dll`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/olstecnologia/features/read_fb_for_postgres_feature.py` & `olstecnologia-1.1.4/olstecnologia/features/read_fb_for_postgres_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from sqlalchemy import Table, select, update, bindparam, MetaData, inspect
 from sqlalchemy.dialects.postgresql import insert
 from olstecnologia.services.utils_service import colors, abort_system, get_ibges
 from olstecnologia.services.connection_service import Conn
 import os, time, random as rd
-import ipdb
 
 
 def loading_dot(connect_string):
     x = rd.randint(0,10)
 
     for i in range(10):
         print(".", end="", flush=True)
@@ -98,15 +97,15 @@
                         id_contrato=x[7],\
                         valor_contrato=x[8])
         
         # do_nothing_stmt = stmt.on_conflict_do_nothing()
 
         try:
             # session.add(stmt)
-            # session.commit()
+            # session.commit()         
             with engine.connect() as s:
                 result = s.execute(stmt)
             ipdb.set_trace()
         except Exception as e:
             print(e)
             ipdb.set_trace()
```

### Comparing `olstecnologia-1.1.3/olstecnologia/features/update_addres_feature.py` & `olstecnologia-1.1.4/olstecnologia/features/update_addres_feature.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/olstecnologia/services/check_db_service.py` & `olstecnologia-1.1.4/olstecnologia/services/check_db_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/olstecnologia/services/connection_service.py` & `olstecnologia-1.1.4/olstecnologia/services/connection_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/olstecnologia/services/services_service.py` & `olstecnologia-1.1.4/olstecnologia/services/services_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/olstecnologia/services/utils_service.py` & `olstecnologia-1.1.4/olstecnologia/services/utils_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.3/pyproject.toml` & `olstecnologia-1.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [tool.poetry]
 name = "olstecnologia"
-version = "1.1.3"
+version = "1.1.4"
 description = ""
 authors = ["Julio Pereira <juliopereira.dev@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlalchemy-firebird = "^0.7.6"
 fdb = "^2.0.2"
 firebird = "^0.0.2"
 tqdm = "^4.65.0"
 sqlalchemy = "1.4.39"
 geopandas = "^0.12.2"
 psycopg2 = "^2.9.6"
+ipdb = "^0.13.13"
 
 [tool.poetry.scripts]
 ols = "olstecnologia:start"
 vb = "olstecnologia.services:check_db"
 vt = "olstecnologia.services:check_tables"
 vc = "olstecnologia.services:check_columns"
 vl = "olstecnologia.services:check_lines"
 
-[tool.poetry.group.dev.dependencies]
-ipdb = "^0.13.13"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `olstecnologia-1.1.3/PKG-INFO` & `olstecnologia-1.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: olstecnologia
-Version: 1.1.3
+Version: 1.1.4
 Summary: 
 Author: Julio Pereira
 Author-email: juliopereira.dev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fdb (>=2.0.2,<3.0.0)
 Requires-Dist: firebird (>=0.0.2,<0.0.3)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
+Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: sqlalchemy (==1.4.39)
 Requires-Dist: sqlalchemy-firebird (>=0.7.6,<0.8.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
```

