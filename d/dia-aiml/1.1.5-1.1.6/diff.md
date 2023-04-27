# Comparing `tmp/dia-aiml-1.1.5.tar.gz` & `tmp/dia-aiml-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dia-aiml-1.1.5.tar", last modified: Thu Mar 23 14:42:28 2023, max compression
+gzip compressed data, was "dia-aiml-1.1.6.tar", last modified: Thu Apr 27 12:57:47 2023, max compression
```

## Comparing `dia-aiml-1.1.5.tar` & `dia-aiml-1.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 14:42:28.786598 dia-aiml-1.1.5/
--rw-rw-rw-   0        0        0     1089 2021-09-24 08:00:55.000000 dia-aiml-1.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      541 2023-03-23 14:42:28.786598 dia-aiml-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      153 2020-07-03 12:06:50.000000 dia-aiml-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 14:42:28.460212 dia-aiml-1.1.5/aimltools/
--rw-rw-rw-   0        0        0      293 2023-03-23 14:42:05.000000 dia-aiml-1.1.5/aimltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 14:42:28.586264 dia-aiml-1.1.5/aimltools/ts/
--rw-rw-rw-   0        0        0      268 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/__init__.py
--rw-rw-rw-   0        0        0    14824 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/classification.py
--rw-rw-rw-   0        0        0     5166 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/denoising.py
-drwxrwxrwx   0        0        0        0 2023-03-23 14:42:28.633149 dia-aiml-1.1.5/aimltools/ts/dependencies/
--rw-rw-rw-   0        0        0       59 2021-09-24 08:00:55.000000 dia-aiml-1.1.5/aimltools/ts/dependencies/__init__.py
--rw-rw-rw-   0        0        0     2715 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/dependencies/pdc.py
--rw-rw-rw-   0        0        0     1830 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/dependencies/tam.py
--rw-rw-rw-   0        0        0     8084 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/distances.py
--rw-rw-rw-   0        0        0     3840 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/golden.py
--rw-rw-rw-   0        0        0    13250 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/perturbations.py
--rw-rw-rw-   0        0        0    17648 2022-07-22 10:08:14.000000 dia-aiml-1.1.5/aimltools/ts/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-03-23 14:42:28.739720 dia-aiml-1.1.5/aimltools/ts/utils/
--rw-rw-rw-   0        0        0      326 2022-10-19 08:06:00.000000 dia-aiml-1.1.5/aimltools/ts/utils/__init__.py
--rw-rw-rw-   0        0        0     3533 2021-09-24 08:00:56.000000 dia-aiml-1.1.5/aimltools/ts/utils/generic_utils.py
--rw-rw-rw-   0        0        0     9763 2021-09-24 08:00:56.000000 dia-aiml-1.1.5/aimltools/ts/utils/pg_utils.py
--rw-rw-rw-   0        0        0    18407 2023-03-23 14:39:34.000000 dia-aiml-1.1.5/aimltools/ts/utils/pi_utils.py
--rw-rw-rw-   0        0        0     1068 2021-09-14 09:36:31.000000 dia-aiml-1.1.5/aimltools/ts/utils/pi_utils_cfg.py
--rw-rw-rw-   0        0        0      986 2021-09-24 08:00:56.000000 dia-aiml-1.1.5/aimltools/ts/utils/pi_utils_cfg_sample.py
--rw-rw-rw-   0        0        0     8069 2021-09-24 08:00:56.000000 dia-aiml-1.1.5/aimltools/ts/utils/s3_utils.py
--rw-rw-rw-   0        0        0     8107 2022-07-13 09:48:01.000000 dia-aiml-1.1.5/aimltools/ts/validation.py
-drwxrwxrwx   0        0        0        0 2023-03-23 14:42:28.786598 dia-aiml-1.1.5/dia_aiml.egg-info/
--rw-rw-rw-   0        0        0      541 2023-03-23 14:42:27.000000 dia-aiml-1.1.5/dia_aiml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-03-23 14:42:27.000000 dia-aiml-1.1.5/dia_aiml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 14:42:27.000000 dia-aiml-1.1.5/dia_aiml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-03-23 14:42:27.000000 dia-aiml-1.1.5/dia_aiml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-23 14:42:27.000000 dia-aiml-1.1.5/dia_aiml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-03-23 14:42:28.786598 dia-aiml-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1698 2021-09-24 08:00:56.000000 dia-aiml-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.835234 dia-aiml-1.1.6/
+-rw-rw-rw-   0        0        0     1089 2021-09-24 08:00:55.000000 dia-aiml-1.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      541 2023-04-27 12:57:47.836191 dia-aiml-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2020-07-03 12:06:50.000000 dia-aiml-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.540090 dia-aiml-1.1.6/aimltools/
+-rw-rw-rw-   0        0        0      293 2023-04-27 12:56:06.000000 dia-aiml-1.1.6/aimltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.669797 dia-aiml-1.1.6/aimltools/ts/
+-rw-rw-rw-   0        0        0      268 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/__init__.py
+-rw-rw-rw-   0        0        0    14824 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/classification.py
+-rw-rw-rw-   0        0        0     5166 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/denoising.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.716692 dia-aiml-1.1.6/aimltools/ts/dependencies/
+-rw-rw-rw-   0        0        0       59 2021-09-24 08:00:55.000000 dia-aiml-1.1.6/aimltools/ts/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     2715 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/dependencies/pdc.py
+-rw-rw-rw-   0        0        0     1830 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/dependencies/tam.py
+-rw-rw-rw-   0        0        0     8084 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/distances.py
+-rw-rw-rw-   0        0        0     3840 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/golden.py
+-rw-rw-rw-   0        0        0    13250 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/perturbations.py
+-rw-rw-rw-   0        0        0    17648 2022-07-22 10:08:14.000000 dia-aiml-1.1.6/aimltools/ts/preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.747937 dia-aiml-1.1.6/aimltools/ts/utils/
+-rw-rw-rw-   0        0        0      326 2022-10-19 08:06:00.000000 dia-aiml-1.1.6/aimltools/ts/utils/__init__.py
+-rw-rw-rw-   0        0        0     3533 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/aimltools/ts/utils/generic_utils.py
+-rw-rw-rw-   0        0        0    10415 2023-04-27 12:55:44.000000 dia-aiml-1.1.6/aimltools/ts/utils/pg_utils.py
+-rw-rw-rw-   0        0        0    18407 2023-03-23 14:39:34.000000 dia-aiml-1.1.6/aimltools/ts/utils/pi_utils.py
+-rw-rw-rw-   0        0        0     1068 2021-09-14 09:36:31.000000 dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg.py
+-rw-rw-rw-   0        0        0      986 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg_sample.py
+-rw-rw-rw-   0        0        0     8069 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/aimltools/ts/utils/s3_utils.py
+-rw-rw-rw-   0        0        0     8107 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/validation.py
+drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.832197 dia-aiml-1.1.6/dia_aiml.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-27 12:57:47.838188 dia-aiml-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/setup.py
```

### Comparing `dia-aiml-1.1.5/LICENSE.txt` & `dia-aiml-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/PKG-INFO` & `dia-aiml-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-aiml
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python toolkit for the analysis of machine data
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_AIML_Toolkit
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dia-aiml-1.1.5/aimltools/ts/classification.py` & `dia-aiml-1.1.6/aimltools/ts/classification.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/denoising.py` & `dia-aiml-1.1.6/aimltools/ts/denoising.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/dependencies/pdc.py` & `dia-aiml-1.1.6/aimltools/ts/dependencies/pdc.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/dependencies/tam.py` & `dia-aiml-1.1.6/aimltools/ts/dependencies/tam.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/distances.py` & `dia-aiml-1.1.6/aimltools/ts/distances.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/golden.py` & `dia-aiml-1.1.6/aimltools/ts/golden.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/perturbations.py` & `dia-aiml-1.1.6/aimltools/ts/perturbations.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/preprocessing.py` & `dia-aiml-1.1.6/aimltools/ts/preprocessing.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/utils/generic_utils.py` & `dia-aiml-1.1.6/aimltools/ts/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/utils/pg_utils.py` & `dia-aiml-1.1.6/aimltools/ts/utils/pg_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 from psycopg2 import extras
 import logging
 import pandas as pd
 from deprecation import deprecated
 
 logger = logging.getLogger(__name__)
 
+class PGDataAccessException(Exception):
+    pass
+    # """Exception raised for errors in the input to PGDataAccess methods.
+    #
+    # Attributes:
+    #     expression -- input expression in which the error occurred
+    #     message -- explanation of the error
+    # """
+    #
+    # def __init__(self, expression, message):
+    #     self.expression = expression
+    #     self.message = message
+
 class PGDataAccess:
     
     def __init__(self,USER,PASS,HOST,PORT,DB,SSL,SSL_CERT):
         self.__USER = USER
         self.__PASS = PASS
         self.__HOST = HOST
         self.__PORT = PORT
@@ -84,21 +97,24 @@
         stmt = "INSERT INTO {} ({}) VALUES %s".format(table_name, str_col_list)
         record_count = len(df)
         write_list = list(df.itertuples(index=False, name=None))
 
         try:
             cur = self.__connection.cursor()
             extras.execute_values(cur, stmt, write_list)
-        except Exception as error:
-            logger.error("Error while writing data : {}".format(error), exc_info=True)
-            record_count = 0
+            return record_count
+        except (psycopg2.errors.ForeignKeyViolation, psycopg2.errors.UniqueViolation) as e1:
+            logger.error("Foreign key or unique key violation while writing data : {}".format(e1), exc_info=True)
+            raise PGDataAccessException(e1)
+        except Exception as e2:
+            logger.error("Error while writing data : {}".format(e2), exc_info=True)
+            raise e2
         finally:
             self.__connection.commit()
             cur.close()
-            return record_count
 
 
     def vacuum_table(self, table_name, vacuum_type = 'partial'):
 
         if vacuum_type == 'partial':
             vacuum_type = ''
```

### Comparing `dia-aiml-1.1.5/aimltools/ts/utils/pi_utils.py` & `dia-aiml-1.1.6/aimltools/ts/utils/pi_utils.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/utils/pi_utils_cfg.py` & `dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/utils/pi_utils_cfg_sample.py` & `dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg_sample.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/utils/s3_utils.py` & `dia-aiml-1.1.6/aimltools/ts/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/aimltools/ts/validation.py` & `dia-aiml-1.1.6/aimltools/ts/validation.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/dia_aiml.egg-info/PKG-INFO` & `dia-aiml-1.1.6/dia_aiml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-aiml
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python toolkit for the analysis of machine data
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_AIML_Toolkit
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dia-aiml-1.1.5/dia_aiml.egg-info/SOURCES.txt` & `dia-aiml-1.1.6/dia_aiml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.5/setup.py` & `dia-aiml-1.1.6/setup.py`

 * *Files identical despite different names*

