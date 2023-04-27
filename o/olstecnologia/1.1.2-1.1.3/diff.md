# Comparing `tmp/olstecnologia-1.1.2.tar.gz` & `tmp/olstecnologia-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olstecnologia-1.1.2.tar", max compression
+gzip compressed data, was "olstecnologia-1.1.3.tar", max compression
```

## Comparing `olstecnologia-1.1.2.tar` & `olstecnologia-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.2/olstecnologia/__init__.py
--rw-r--r--   0        0        0    10752 2023-04-25 15:07:24.525635 olstecnologia-1.1.2/olstecnologia/app.py
--rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.2/olstecnologia/config/__init__.py
--rw-r--r--   0        0        0     1836 2023-04-17 11:29:49.555822 olstecnologia-1.1.2/olstecnologia/config/database.py
--rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.2/olstecnologia/config/fbclient.dll
--rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.2/olstecnologia/features/__init__.py
--rw-r--r--   0        0        0      607 2023-04-24 20:47:38.576706 olstecnologia-1.1.2/olstecnologia/features/read_fb_for_postgres_feature.py
--rw-r--r--   0        0        0     8810 2023-04-25 15:26:55.236961 olstecnologia-1.1.2/olstecnologia/features/update_addres_feature.py
--rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.2/olstecnologia/services/__init__.py
--rw-r--r--   0        0        0     6532 2023-04-25 14:38:00.752471 olstecnologia-1.1.2/olstecnologia/services/check_db_service.py
--rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.2/olstecnologia/services/connection_service.py
--rw-r--r--   0        0        0     7034 2023-04-25 15:25:30.524083 olstecnologia-1.1.2/olstecnologia/services/services_service.py
--rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.2/olstecnologia/services/utils_service.py
--rw-r--r--   0        0        0      711 2023-04-25 15:34:17.488672 olstecnologia-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.2/README.md
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 olstecnologia-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.3/olstecnologia/__init__.py
+-rw-r--r--   0        0        0    10752 2023-04-25 15:07:24.525635 olstecnologia-1.1.3/olstecnologia/app.py
+-rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.3/olstecnologia/config/__init__.py
+-rw-r--r--   0        0        0     1836 2023-04-17 11:29:49.555822 olstecnologia-1.1.3/olstecnologia/config/database.py
+-rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.3/olstecnologia/config/fbclient.dll
+-rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.3/olstecnologia/features/__init__.py
+-rw-r--r--   0        0        0     4917 2023-04-26 13:17:41.244954 olstecnologia-1.1.3/olstecnologia/features/read_fb_for_postgres_feature.py
+-rw-r--r--   0        0        0     8810 2023-04-25 15:26:55.236961 olstecnologia-1.1.3/olstecnologia/features/update_addres_feature.py
+-rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.3/olstecnologia/services/__init__.py
+-rw-r--r--   0        0        0     6532 2023-04-25 14:38:00.752471 olstecnologia-1.1.3/olstecnologia/services/check_db_service.py
+-rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.3/olstecnologia/services/connection_service.py
+-rw-r--r--   0        0        0     7069 2023-04-25 18:35:48.039984 olstecnologia-1.1.3/olstecnologia/services/services_service.py
+-rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.3/olstecnologia/services/utils_service.py
+-rw-r--r--   0        0        0      732 2023-04-27 18:14:38.943339 olstecnologia-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.3/README.md
+-rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 olstecnologia-1.1.3/PKG-INFO
```

### Comparing `olstecnologia-1.1.2/olstecnologia/app.py` & `olstecnologia-1.1.3/olstecnologia/app.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.2/olstecnologia/config/database.py` & `olstecnologia-1.1.3/olstecnologia/config/database.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.2/olstecnologia/config/fbclient.dll` & `olstecnologia-1.1.3/olstecnologia/config/fbclient.dll`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.2/olstecnologia/features/update_addres_feature.py` & `olstecnologia-1.1.3/olstecnologia/features/update_addres_feature.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.2/olstecnologia/services/check_db_service.py` & `olstecnologia-1.1.3/olstecnologia/services/check_db_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.2/olstecnologia/services/connection_service.py` & `olstecnologia-1.1.3/olstecnologia/services/connection_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.2/olstecnologia/services/services_service.py` & `olstecnologia-1.1.3/olstecnologia/services/services_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import os, time, random as rd
 from olstecnologia.features.update_addres_feature import update_address_clini7, update_address_admini7
 from olstecnologia.features.read_fb_for_postgres_feature import population_postgres
 from sqlalchemy import MetaData, Table
 from tqdm import tqdm
 
 class Services:
-    def __init__(self, string_connection) -> None:
+    def __init__(self, string_connection, dialect="firebird") -> None:
         self.string_connection = string_connection
 
         try:
-            connection = Conn(f"firebird://{string_connection}")
+            connection = Conn(f"{dialect}://{string_connection}")
+            
 
             engine = connection.engine()
             metadata = connection.metadata()
             inspect = connection.inspect()
             session = connection.session()
             session_maker = connection.session_maker()
```

### Comparing `olstecnologia-1.1.2/olstecnologia/services/utils_service.py` & `olstecnologia-1.1.3/olstecnologia/services/utils_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.2/pyproject.toml` & `olstecnologia-1.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "olstecnologia"
-version = "1.1.2"
+version = "1.1.3"
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
+psycopg2 = "^2.9.6"
 
 [tool.poetry.scripts]
 ols = "olstecnologia:start"
 vb = "olstecnologia.services:check_db"
 vt = "olstecnologia.services:check_tables"
 vc = "olstecnologia.services:check_columns"
 vl = "olstecnologia.services:check_lines"
```

### Comparing `olstecnologia-1.1.2/PKG-INFO` & `olstecnologia-1.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: olstecnologia
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Author: Julio Pereira
 Author-email: juliopereira.dev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fdb (>=2.0.2,<3.0.0)
 Requires-Dist: firebird (>=0.0.2,<0.0.3)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: sqlalchemy (==1.4.39)
 Requires-Dist: sqlalchemy-firebird (>=0.7.6,<0.8.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
```

