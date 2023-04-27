# Comparing `tmp/rds-core-0.0.15.tar.gz` & `tmp/rds-core-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-core-0.0.15.tar", last modified: Tue Apr 25 02:54:54 2023, max compression
+gzip compressed data, was "rds-core-0.0.16.tar", last modified: Thu Apr 27 01:01:15 2023, max compression
```

## Comparing `rds-core-0.0.15.tar` & `rds-core-0.0.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:54:54.983751 rds-core-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 02:54:36.000000 rds-core-0.0.15/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-25 02:54:54.983751 rds-core-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 02:54:36.000000 rds-core-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:54:54.979750 rds-core-0.0.15/rds_core/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:54:54.983751 rds-core-0.0.15/rds_core/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/cache/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/cache/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:54:54.983751 rds-core-0.0.15/rds_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:54:54.983751 rds-core-0.0.15/rds_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/helpers/cnes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/helpers/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:54:54.983751 rds-core-0.0.15/rds_core/searchengine/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-25 02:54:36.000000 rds-core-0.0.15/rds_core/searchengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:54:54.979750 rds-core-0.0.15/rds_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-25 02:54:54.000000 rds-core-0.0.15/rds_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 02:54:54.000000 rds-core-0.0.15/rds_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:54:54.000000 rds-core-0.0.15/rds_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-25 02:54:54.000000 rds-core-0.0.15/rds_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 02:54:54.000000 rds-core-0.0.15/rds_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 02:54:54.983751 rds-core-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-25 02:54:36.000000 rds-core-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:15.967361 rds-core-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 01:00:50.000000 rds-core-0.0.16/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-27 01:01:15.967361 rds-core-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-27 01:00:50.000000 rds-core-0.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:15.967361 rds-core-0.0.16/rds_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:15.967361 rds-core-0.0.16/rds_core/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/cache/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/cache/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:15.967361 rds-core-0.0.16/rds_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:15.967361 rds-core-0.0.16/rds_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/helpers/cnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/helpers/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:15.967361 rds-core-0.0.16/rds_core/searchengine/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-27 01:00:50.000000 rds-core-0.0.16/rds_core/searchengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 01:01:15.967361 rds-core-0.0.16/rds_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-27 01:01:15.000000 rds-core-0.0.16/rds_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 01:01:15.000000 rds-core-0.0.16/rds_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 01:01:15.000000 rds-core-0.0.16/rds_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 01:01:15.000000 rds-core-0.0.16/rds_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 01:01:15.000000 rds-core-0.0.16/rds_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 01:01:15.967361 rds-core-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-27 01:00:50.000000 rds-core-0.0.16/setup.py
```

### Comparing `rds-core-0.0.15/PKG-INFO` & `rds-core-0.0.16/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rds-core
-Version: 0.0.15
+Version: 0.0.16
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
-Home-page: UNKNOWN
+Home-page: https://github.com/lais-huol/rds-cep-python
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
+Download-URL: https://github.com/lais-huol/rds-cep-python/tags
 Keywords: rds,cache,config,helper,searchengine
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `rds-core-0.0.15/README.md` & `rds-core-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core/cache/__init__.py` & `rds-core-0.0.16/rds_core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core/cache/base.py` & `rds-core-0.0.16/rds_core/cache/base.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core/cache/nocache.py` & `rds-core-0.0.16/rds_core/cache/nocache.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core/cache/search_engine.py` & `rds-core-0.0.16/rds_core/cache/search_engine.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core/helpers/__init__.py` & `rds-core-0.0.16/rds_core/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core/helpers/http_client.py` & `rds-core-0.0.16/rds_core/helpers/http_client.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core/searchengine/__init__.py` & `rds-core-0.0.16/rds_core/searchengine/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.15/rds_core.egg-info/PKG-INFO` & `rds-core-0.0.16/rds_core.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rds-core
-Version: 0.0.15
+Version: 0.0.16
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
-Home-page: UNKNOWN
+Home-page: https://github.com/lais-huol/rds-cep-python
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
+Download-URL: https://github.com/lais-huol/rds-cep-python/tags
 Keywords: rds,cache,config,helper,searchengine
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `rds-core-0.0.15/setup.py` & `rds-core-0.0.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,15 @@
         subfolders.extend(fast_scandir(dirname))
     return subfolders
 
 
 def package_data_dirs(root, data_dirs):
     data_dirs_path = [x + "/*" for x in data_dirs]
     for data_dir in data_dirs:
-        data_dirs_path += [
-            x.replace(f"{root}/", "") + "/*" for x in fast_scandir(f"{root}/{data_dir}")
-        ]
+        data_dirs_path += [x.replace(f"{root}/", "") + "/*" for x in fast_scandir(f"{root}/{data_dir}")]
 
     return {root: data_dirs_path}
 
 
 requirements = [
     # config
     "dynaconf>=3.1.11",
@@ -35,15 +33,15 @@
 
 with open("requirements.txt", "w") as file1:
     for requirement in requirements:
         file1.write(f"{requirement}\n")
 
 setup(
     name="rds-core",
-    version="0.0.15",
+    version="0.0.16",
     description="Framework para serviços do Rede de Dados em Saúde do LAIS",
     long_description="É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o"
     " desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de"
     " Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias"
     " RDS, a exemplo RDS-RN e RDS-ES.",
     author="Kelson da Costa Medeiros",
     author_email="kelson.medeiros@lais.huol.ufrn.br",
@@ -68,8 +66,10 @@
         "rds_core.cache",
         "rds_core.config",
         "rds_core.helpers",
         "rds_core.searchengine",
     ],
     package_dir={"rds_core": "rds_core"},
     package_data=package_data_dirs("rds_core", []),
+    download_url="https://github.com/lais-huol/rds-cep-python/tags",
+    url="https://github.com/lais-huol/rds-cep-python",
 )
```

