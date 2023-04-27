# Comparing `tmp/dbt-glue-1.4.1.tar.gz` & `tmp/dbt-glue-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.4.1.tar", last modified: Fri Apr  7 09:06:35 2023, max compression
+gzip compressed data, was "dbt-glue-1.4.2.tar", last modified: Thu Apr 27 13:54:44 2023, max compression
```

## Comparing `dbt-glue-1.4.1.tar` & `dbt-glue-1.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.185955 dbt-glue-1.4.1/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.4.1/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.4.1/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    43804 2023-04-07 09:06:35.183330 dbt-glue-1.4.1/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    42903 2023-04-06 14:05:38.000000 dbt-glue-1.4.1/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.132606 dbt-glue-1.4.1/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.131892 dbt-glue-1.4.1/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.147822 dbt-glue-1.4.1/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.4.1/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-04-07 09:05:13.000000 dbt-glue-1.4.1/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3431 2023-04-06 15:50:22.000000 dbt-glue-1.4.1/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2590 2023-04-06 15:50:17.000000 dbt-glue-1.4.1/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.154261 dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2022-07-11 06:48:28.000000 dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8767 2023-04-06 14:25:36.000000 dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    35933 2023-04-07 08:10:50.000000 dbt-glue-1.4.1/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.4.1/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.132813 dbt-glue-1.4.1/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.158657 dbt-glue-1.4.1/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.4.1/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.4.1/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.160416 dbt-glue-1.4.1/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.4.1/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.162635 dbt-glue-1.4.1/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.4.1/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.4.1/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.166221 dbt-glue-1.4.1/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.169022 dbt-glue-1.4.1/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4348 2023-01-18 17:12:34.000000 dbt-glue-1.4.1/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.4.1/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.4.1/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10358 2023-01-18 17:12:34.000000 dbt-glue-1.4.1/dbt/include/glue/macros/materializations/snapshot.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.4.1/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      592 2022-10-21 07:23:23.000000 dbt-glue-1.4.1/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.136295 dbt-glue-1.4.1/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.171087 dbt-glue-1.4.1/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.4.1/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-07 09:06:35.180634 dbt-glue-1.4.1/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    43804 2023-04-07 09:06:35.000000 dbt-glue-1.4.1/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1157 2023-04-07 09:06:35.000000 dbt-glue-1.4.1/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-04-07 09:06:35.000000 dbt-glue-1.4.1/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.4.1/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-04-07 09:06:35.000000 dbt-glue-1.4.1/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-04-07 09:06:35.000000 dbt-glue-1.4.1/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-04-07 09:06:35.186519 dbt-glue-1.4.1/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2872 2023-04-07 09:04:41.000000 dbt-glue-1.4.1/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.537853 dbt-glue-1.4.2/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.4.2/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.4.2/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    43804 2023-04-27 13:54:44.537172 dbt-glue-1.4.2/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    42903 2023-04-06 14:05:38.000000 dbt-glue-1.4.2/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:16.899735 dbt-glue-1.4.2/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:16.899295 dbt-glue-1.4.2/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.509833 dbt-glue-1.4.2/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.4.2/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-04-27 13:54:09.000000 dbt-glue-1.4.2/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3431 2023-04-06 15:50:22.000000 dbt-glue-1.4.2/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2590 2023-04-06 15:50:17.000000 dbt-glue-1.4.2/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.515351 dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2022-07-11 06:48:28.000000 dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8767 2023-04-06 14:25:36.000000 dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    36485 2023-04-27 13:24:38.000000 dbt-glue-1.4.2/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.4.2/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:16.899861 dbt-glue-1.4.2/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.518481 dbt-glue-1.4.2/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.4.2/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.4.2/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.519662 dbt-glue-1.4.2/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.4.2/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.521547 dbt-glue-1.4.2/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.4.2/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.4.2/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.524960 dbt-glue-1.4.2/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.527339 dbt-glue-1.4.2/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4348 2023-01-18 17:12:34.000000 dbt-glue-1.4.2/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.4.2/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.4.2/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10358 2023-01-18 17:12:34.000000 dbt-glue-1.4.2/dbt/include/glue/macros/materializations/snapshot.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.4.2/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      592 2022-10-21 07:23:23.000000 dbt-glue-1.4.2/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.496414 dbt-glue-1.4.2/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.528470 dbt-glue-1.4.2/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.4.2/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 13:54:44.535680 dbt-glue-1.4.2/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    43804 2023-04-27 13:54:16.000000 dbt-glue-1.4.2/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1157 2023-04-27 13:54:16.000000 dbt-glue-1.4.2/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-04-27 13:54:16.000000 dbt-glue-1.4.2/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.4.2/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-04-27 13:54:16.000000 dbt-glue-1.4.2/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-04-27 13:54:16.000000 dbt-glue-1.4.2/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-04-27 13:54:44.538086 dbt-glue-1.4.2/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2872 2023-04-27 13:24:38.000000 dbt-glue-1.4.2/setup.py
```

### Comparing `dbt-glue-1.4.1/LICENSE` & `dbt-glue-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/PKG-INFO` & `dbt-glue-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.1
+Version: 1.4.2
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.4.1/README.md` & `dbt-glue-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/adapters/glue/connections.py` & `dbt-glue-1.4.2/dbt/adapters/glue/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/adapters/glue/credentials.py` & `dbt-glue-1.4.2/dbt/adapters/glue/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.4.2/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/adapters/glue/impl.py` & `dbt-glue-1.4.2/dbt/adapters/glue/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,14 +621,15 @@
             'hoodie.datasource.write.precombine.field': 'update_hudi_ts',
             'hoodie.consistency.check.enabled': 'true',
             'hoodie.datasource.write.recordkey.field': primary_key,
             'hoodie.table.name': target_relation.name,
             'hoodie.datasource.hive_sync.database': target_relation.schema,
             'hoodie.datasource.hive_sync.table': target_relation.name,
             'hoodie.datasource.hive_sync.enable': 'true',
+            'hoodie.datasource.write.hive_style_partitioning': 'true',
         }
 
         if partition_key:
             partition_list = ','.join(partition_key)
             partition_config = {
                 'hoodie.datasource.write.partitionpath.field': f'{partition_list}',
                 'hoodie.datasource.hive_sync.partition_extractor_class': 'org.apache.hudi.hive.MultiPartKeysValueExtractor',
@@ -842,7 +843,27 @@
             """)
         try:
             cursor.execute(code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueIcebergExpireSnapshotsFailed") from e
         except Exception as e:
             logger.error(e)
+
+    @available
+    def execute_pyspark(self, codeblock):
+        session, client, cursor = self.get_connection()
+
+        code = f"""
+custom_glue_code_for_dbt_adapter
+{codeblock}
+        """
+
+        logger.debug(f"""pyspark code :
+        {code}
+        """)
+
+        try:
+            cursor.execute(code)
+        except DatabaseException as e:
+            raise DatabaseException(msg="GlueExecutePySparkFailed") from e
+        except Exception as e:
+            logger.error(e)
```

### Comparing `dbt-glue-1.4.1/dbt/adapters/glue/relation.py` & `dbt-glue-1.4.2/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.4.2/dbt/include/glue/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.4.2/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.4.2/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.4.2/dbt/include/glue/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.4.2/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.4.2/dbt/include/glue/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.4.2/dbt_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.1
+Version: 1.4.2
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.4.1/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.4.2/dbt_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.1/setup.py` & `dbt-glue-1.4.2/setup.py`

 * *Files identical despite different names*

