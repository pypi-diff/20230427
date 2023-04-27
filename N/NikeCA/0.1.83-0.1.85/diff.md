# Comparing `tmp/NikeCA-0.1.83.tar.gz` & `tmp/NikeCA-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.83.tar", last modified: Mon Apr 24 07:25:00 2023, max compression
+gzip compressed data, was "NikeCA-0.1.85.tar", last modified: Thu Apr 27 15:57:54 2023, max compression
```

## Comparing `NikeCA-0.1.83.tar` & `NikeCA-0.1.85.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.369698 NikeCA-0.1.83/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.83/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:25:00.369149 NikeCA-0.1.83/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.83/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 07:25:00.369865 NikeCA-0.1.83/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 07:24:54.000000 NikeCA-0.1.83/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.360946 NikeCA-0.1.83/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.362946 NikeCA-0.1.83/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.364030 NikeCA-0.1.83/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.365292 NikeCA-0.1.83/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5903 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6117 2023-04-24 07:19:42.000000 NikeCA-0.1.83/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:25:00.368386 NikeCA-0.1.83/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 07:25:00.000000 NikeCA-0.1.83/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      332 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23561 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 07:05:21.000000 NikeCA-0.1.83/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.575787 NikeCA-0.1.85/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.85/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-04-27 15:57:54.575460 NikeCA-0.1.85/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.85/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-27 15:57:54.575885 NikeCA-0.1.85/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2468 2023-04-27 15:57:26.000000 NikeCA-0.1.85/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.568361 NikeCA-0.1.85/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.569618 NikeCA-0.1.85/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.570758 NikeCA-0.1.85/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.572585 NikeCA-0.1.85/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5985 2023-04-24 17:37:55.000000 NikeCA-0.1.85/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-24 17:31:51.000000 NikeCA-0.1.85/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-27 15:57:54.575034 NikeCA-0.1.85/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1154 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-27 15:57:54.000000 NikeCA-0.1.85/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      416 2023-04-24 07:31:10.000000 NikeCA-0.1.85/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23731 2023-04-24 08:02:12.000000 NikeCA-0.1.85/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-04-27 15:54:21.000000 NikeCA-0.1.85/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 07:05:21.000000 NikeCA-0.1.85/src/__init__.py
```

### Comparing `NikeCA-0.1.83/LICENSE` & `NikeCA-0.1.85/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/PKG-INFO` & `NikeCA-0.1.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.83
-Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
+Version: 0.1.85
+Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.83/README.md` & `NikeCA-0.1.85/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/setup.py` & `NikeCA-0.1.85/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.83',
-	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
+	version='0.1.85',
+	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
 		"Dashboards/InclusionExclusion/InclusionExclusion",
@@ -71,15 +71,15 @@
 		"jupyterlab-pygments==0.2.2",
 		"jupyterlab_server==2.19.0",
 		"lz4==4.3.2",
 		"numpy==1.23.4",
 		"oauthlib==3.2.2",
 		"oscrypto==1.3.0",
 		"pandas==1.5.3",
-		"polars==0.16.17",
+		"polars==0.17.9",
 		"pyarrow==10.0.1",
 		"pycparser==2.21",
 		"pycryptodomex==3.17",
 		"PyGithub==1.58.0",
 		"PyJWT==2.6.0",
 		"pyOpenSSL==23.0.0",
 		"pyspark==3.3.2",
```

### Comparing `NikeCA-0.1.83/src/Dashboards/Dashboards.py` & `NikeCA-0.1.85/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.85/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.85/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 class ProductUsage:
 
-
     def get_base_query(self
                        , filters: list | None = None
                        , start_date: str = '1900-01-01'
                        , end_date: str = '9999-12-31'
                        ):
 
         import configparser
@@ -145,14 +144,17 @@
                 , start_date: str = '1900-01-01'
                 , end_date: str = '9999-12-31'
                 ):
         import configparser
 
         config = configparser.ConfigParser()
         config.read('pip.ini')
+        import os
+        print(os.system('pwd'))
+        print(config.sections())
         b = config['telemetry_product_usage'].get('col_b')
 
         if order_by is None:
             order_by = config['telemetry_product_usage'].get('order_by')
         else:
             order_by = ', '.join(order_by)
```

### Comparing `NikeCA-0.1.83/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.85/src/NikeCA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.83
-Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
+Version: 0.1.85
+Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.83/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.85/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.85/src/NikeCA.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 jupyterlab-pygments==0.2.2
 jupyterlab_server==2.19.0
 lz4==4.3.2
 numpy==1.23.4
 oauthlib==3.2.2
 oscrypto==1.3.0
 pandas==1.5.3
-polars==0.16.17
+polars==0.17.9
 pyarrow==10.0.1
 pycparser==2.21
 pycryptodomex==3.17
 PyGithub==1.58.0
 PyJWT==2.6.0
 pyOpenSSL==23.0.0
 pyspark==3.3.2
```

### Comparing `NikeCA-0.1.83/src/NikeQA.py` & `NikeCA-0.1.85/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/NikeSF.py` & `NikeCA-0.1.85/src/NikeSF.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
 from Dashboards.Dashboards import Dashboards
 from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
+from Dashboards.Telemetry.Telemetry import Telemetry
+from Dashboards.Telemetry.ProductUsage import ProductUsage
 
 
 class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):#, InclusionExclusion):
 
     Dashboards = Dashboards
+    Telemetry = Telemetry
+    ProductUsage = ProductUsage
 
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
```

### Comparing `NikeCA-0.1.83/src/_BuildSearchQuery.py` & `NikeCA-0.1.85/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/_GitHub.py` & `NikeCA-0.1.85/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/_QA.py` & `NikeCA-0.1.85/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/_SearchFiles.py` & `NikeCA-0.1.85/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/_SnowflakeData.py` & `NikeCA-0.1.85/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.83/src/_SnowflakeDependencies.py` & `NikeCA-0.1.85/src/_SnowflakeDependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,17 @@
             if os.path.isfile(save_path):
                 with open(save_path) as f:
                     d = json.load(f)
             else:
                 d = {}
         else:
             d = {}
+
+        for table in tables:
+            d[table] = {}
         while process_complete == 0:
             item = -1
             process_pass += 1
             if sum(complete) == queries or process_pass == 1000:
                 process_complete = 1
             for result in query_list:
                 item += 1
@@ -160,15 +163,14 @@
                         cs.get_results_from_sfqid(result)
                         data = cs.fetch_pandas_all()
                         for table in tables:
                             try:
                                 if table.upper() + ' ' in data.iloc[0, 0][data.iloc[0, 0].upper().index(
                                         table.upper()):data.iloc[0, 0].upper().index(table.upper()) + len(table) + 1]\
                                         and table.upper() not in data.iloc[0, 0][:data.iloc[0, 0].index('(')]:
-                                    d[table] = {}
                                     d[table][df_return[df_return['sfqid'] == result].index[0]] = data.to_dict('index')
                             except ValueError:
                                 continue
                     else:
                         time.sleep(.1)
                 counter += 1
         cnn.close()
```

### Comparing `NikeCA-0.1.83/src/_SnowflakePull.py` & `NikeCA-0.1.85/src/_SnowflakePull.py`

 * *Files identical despite different names*

