# Comparing `tmp/dbt-duckdb-1.4.2.tar.gz` & `tmp/dbt-duckdb-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-duckdb-1.4.2.tar", last modified: Wed Apr 26 16:31:10 2023, max compression
+gzip compressed data, was "dbt-duckdb-1.5.0rc1.tar", last modified: Wed Apr 19 20:36:09 2023, max compression
```

## Comparing `dbt-duckdb-1.4.2.tar` & `dbt-duckdb-1.5.0rc1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.606938 dbt-duckdb-1.4.2/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)    13048 2023-04-26 16:31:10.606687 dbt-duckdb-1.4.2/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)    12744 2023-03-21 22:22:36.000000 dbt-duckdb-1.4.2/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.596988 dbt-duckdb-1.4.2/dbt/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.597293 dbt-duckdb-1.4.2/dbt/adapters/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/adapters/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.600040 dbt-duckdb-1.4.2/dbt/adapters/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       18 2023-04-26 16:30:54.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-04-26 16:08:10.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/buenavista.py
--rw-r--r--   0 jwills     (501) staff       (20)     3163 2023-04-24 22:15:34.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 jwills     (501) staff       (20)     6057 2023-04-17 03:57:27.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/credentials.py
--rw-r--r--   0 jwills     (501) staff       (20)     7866 2023-04-26 16:08:10.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/environments.py
--rw-r--r--   0 jwills     (501) staff       (20)     7965 2023-03-26 18:59:50.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/glue.py
--rw-r--r--   0 jwills     (501) staff       (20)     6984 2023-04-26 16:08:10.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.601280 dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 jwills     (501) staff       (20)     1291 2023-04-17 03:57:27.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)      589 2023-04-17 03:57:27.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 jwills     (501) staff       (20)     1669 2023-04-17 03:57:27.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-04-18 19:29:01.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 jwills     (501) staff       (20)     1034 2023-04-17 03:57:27.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 jwills     (501) staff       (20)     2050 2023-04-17 03:57:27.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 jwills     (501) staff       (20)     1141 2023-04-24 23:16:33.000000 dbt-duckdb-1.4.2/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.601460 dbt-duckdb-1.4.2/dbt/include/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.601804 dbt-duckdb-1.4.2/dbt/include/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.602918 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/
--rw-r--r--   0 jwills     (501) staff       (20)     7122 2023-04-26 16:08:10.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 jwills     (501) staff       (20)      950 2023-03-21 22:16:25.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/catalog.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.603922 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 jwills     (501) staff       (20)     3916 2023-03-30 16:27:45.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 jwills     (501) staff       (20)     4633 2023-02-15 20:16:22.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1417 2023-04-03 22:00:10.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 jwills     (501) staff       (20)      862 2023-04-26 16:08:10.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/snapshot_merge.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.605525 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/upstream.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-26 16:31:10.606451 dbt-duckdb-1.4.2/dbt_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)    13048 2023-04-26 16:31:10.000000 dbt-duckdb-1.4.2/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1551 2023-04-26 16:31:10.000000 dbt-duckdb-1.4.2/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-04-26 16:31:10.000000 dbt-duckdb-1.4.2/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       60 2023-04-26 16:31:10.000000 dbt-duckdb-1.4.2/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        4 2023-04-26 16:31:10.000000 dbt-duckdb-1.4.2/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-04-26 16:31:10.607030 dbt-duckdb-1.4.2/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1366 2023-04-26 16:08:10.000000 dbt-duckdb-1.4.2/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.855300 dbt-duckdb-1.5.0rc1/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)    13051 2023-04-19 20:36:09.855118 dbt-duckdb-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)    12744 2023-03-21 22:22:36.000000 dbt-duckdb-1.5.0rc1/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.846926 dbt-duckdb-1.5.0rc1/dbt/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.847184 dbt-duckdb-1.5.0rc1/dbt/adapters/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.849434 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       21 2023-04-19 20:35:31.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/buenavista.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3163 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 jwills     (501) staff       (20)     6057 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/credentials.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7866 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/environments.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7965 2023-03-26 18:59:50.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/glue.py
+-rw-r--r--   0 jwills     (501) staff       (20)     6984 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850216 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 jwills     (501) staff       (20)     1291 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)      589 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1669 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1034 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2050 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1141 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850359 dbt-duckdb-1.5.0rc1/dbt/include/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850641 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.851551 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/
+-rw-r--r--   0 jwills     (501) staff       (20)     7122 2023-03-21 22:22:36.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      950 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/catalog.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.852698 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 jwills     (501) staff       (20)     3916 2023-03-30 16:27:45.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     4633 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1417 2023-04-03 22:00:10.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      862 2023-03-27 04:56:30.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/snapshot_merge.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.854144 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/upstream.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.854936 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)    13051 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1551 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       63 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        4 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-04-19 20:36:09.855332 dbt-duckdb-1.5.0rc1/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1369 2023-04-19 20:35:31.000000 dbt-duckdb-1.5.0rc1/setup.py
```

### Comparing `dbt-duckdb-1.4.2/LICENSE` & `dbt-duckdb-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/PKG-INFO` & `dbt-duckdb-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.4.2
+Version: 1.5.0rc1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: glue
 License-File: LICENSE
```

### Comparing `dbt-duckdb-1.4.2/README.md` & `dbt-duckdb-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/buenavista.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/buenavista.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/connections.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/credentials.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/environments.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/environments.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/glue.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/glue.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/impl.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/__init__.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/excel.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/excel.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/relation.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/adapters/duckdb/utils.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/adapters.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/catalog.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/materializations/external.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/materializations/table.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/seed.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/snapshot_merge.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/datediff.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/dbt_duckdb.egg-info/PKG-INFO` & `dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.4.2
+Version: 1.5.0rc1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: glue
 License-File: LICENSE
```

### Comparing `dbt-duckdb-1.4.2/dbt_duckdb.egg-info/SOURCES.txt` & `dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.2/setup.py` & `dbt-duckdb-1.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,14 @@
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+dbt@gmail.com",
     url="https://github.com/jwills/dbt-duckdb",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-core~=1.4.0",
+        "dbt-core~=1.5.0rc1",
         "duckdb>=0.5.0",
     ],
     extras_require={
         "glue": ["boto3", "mypy-boto3-glue"],
     },
 )
```

