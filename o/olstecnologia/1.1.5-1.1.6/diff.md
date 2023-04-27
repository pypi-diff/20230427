# Comparing `tmp/olstecnologia-1.1.5.tar.gz` & `tmp/olstecnologia-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olstecnologia-1.1.5.tar", max compression
+gzip compressed data, was "olstecnologia-1.1.6.tar", max compression
```

## Comparing `olstecnologia-1.1.5.tar` & `olstecnologia-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.5/olstecnologia/__init__.py
--rw-r--r--   0        0        0    10774 2023-04-27 20:39:34.794001 olstecnologia-1.1.5/olstecnologia/app.py
--rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.5/olstecnologia/config/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-27 20:39:50.927606 olstecnologia-1.1.5/olstecnologia/config/database.py
--rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.5/olstecnologia/config/fbclient.dll
--rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.5/olstecnologia/features/__init__.py
--rw-r--r--   0        0        0     4897 2023-04-27 20:12:06.885547 olstecnologia-1.1.5/olstecnologia/features/read_fb_for_postgres_feature.py
--rw-r--r--   0        0        0     8810 2023-04-25 15:26:55.236961 olstecnologia-1.1.5/olstecnologia/features/update_addres_feature.py
--rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.5/olstecnologia/services/__init__.py
--rw-r--r--   0        0        0     6532 2023-04-25 14:38:00.752471 olstecnologia-1.1.5/olstecnologia/services/check_db_service.py
--rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.5/olstecnologia/services/connection_service.py
--rw-r--r--   0        0        0     7070 2023-04-27 20:25:55.929678 olstecnologia-1.1.5/olstecnologia/services/services_service.py
--rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.5/olstecnologia/services/utils_service.py
--rw-r--r--   0        0        0      692 2023-04-27 20:40:21.561202 olstecnologia-1.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.5/README.md
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 olstecnologia-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.6/olstecnologia/__init__.py
+-rw-r--r--   0        0        0    10795 2023-04-27 20:42:51.556739 olstecnologia-1.1.6/olstecnologia/app.py
+-rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.6/olstecnologia/config/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-27 20:39:50.927606 olstecnologia-1.1.6/olstecnologia/config/database.py
+-rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.6/olstecnologia/config/fbclient.dll
+-rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.6/olstecnologia/features/__init__.py
+-rw-r--r--   0        0        0     4897 2023-04-27 20:12:06.885547 olstecnologia-1.1.6/olstecnologia/features/read_fb_for_postgres_feature.py
+-rw-r--r--   0        0        0     8810 2023-04-25 15:26:55.236961 olstecnologia-1.1.6/olstecnologia/features/update_addres_feature.py
+-rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.6/olstecnologia/services/__init__.py
+-rw-r--r--   0        0        0     6532 2023-04-25 14:38:00.752471 olstecnologia-1.1.6/olstecnologia/services/check_db_service.py
+-rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.6/olstecnologia/services/connection_service.py
+-rw-r--r--   0        0        0     7070 2023-04-27 20:25:55.929678 olstecnologia-1.1.6/olstecnologia/services/services_service.py
+-rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.6/olstecnologia/services/utils_service.py
+-rw-r--r--   0        0        0      692 2023-04-27 20:43:42.871353 olstecnologia-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.6/README.md
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 olstecnologia-1.1.6/PKG-INFO
```

### Comparing `olstecnologia-1.1.5/olstecnologia/app.py` & `olstecnologia-1.1.6/olstecnologia/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from olstecnologia.services.utils_service import colors, abort_system
 from olstecnologia.services.services_service import Services
 from olstecnologia.services.check_db_service import check_db, check_tables, check_columns, check_lines
 from olstecnologia.features.update_addres_feature import update_address_admini7, update_address_clini7
 import json, os, time, random as rd
 from sqlalchemy import MetaData, Table
 from tqdm import tqdm
+import urllib.parse
 import ipdb
 
 def menu_app():
     os.system('cls' if os.name == 'nt' else 'clear')
     print(colors("gold", "====== MENU PRINCIPAL ======\n\n"))
     print(f"{colors('gold', '1')} => Análises no banco\n{colors('gold', '2')} => Atualizar endereços Clin7\n{colors('gold', '3')} => Atualizar endereços Admini7\n{colors('gold', '4')} => Sair do sistema\n\n")
```

### Comparing `olstecnologia-1.1.5/olstecnologia/config/database.py` & `olstecnologia-1.1.6/olstecnologia/config/database.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/olstecnologia/config/fbclient.dll` & `olstecnologia-1.1.6/olstecnologia/config/fbclient.dll`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/olstecnologia/features/read_fb_for_postgres_feature.py` & `olstecnologia-1.1.6/olstecnologia/features/read_fb_for_postgres_feature.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/olstecnologia/features/update_addres_feature.py` & `olstecnologia-1.1.6/olstecnologia/features/update_addres_feature.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/olstecnologia/services/check_db_service.py` & `olstecnologia-1.1.6/olstecnologia/services/check_db_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/olstecnologia/services/connection_service.py` & `olstecnologia-1.1.6/olstecnologia/services/connection_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/olstecnologia/services/services_service.py` & `olstecnologia-1.1.6/olstecnologia/services/services_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/olstecnologia/services/utils_service.py` & `olstecnologia-1.1.6/olstecnologia/services/utils_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.5/pyproject.toml` & `olstecnologia-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olstecnologia"
-version = "1.1.5"
+version = "1.1.6"
 description = ""
 authors = ["Julio Pereira <juliopereira.dev@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlalchemy-firebird = "^0.7.6"
```

### Comparing `olstecnologia-1.1.5/PKG-INFO` & `olstecnologia-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olstecnologia
-Version: 1.1.5
+Version: 1.1.6
 Summary: 
 Author: Julio Pereira
 Author-email: juliopereira.dev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fdb (>=2.0.2,<3.0.0)
```

