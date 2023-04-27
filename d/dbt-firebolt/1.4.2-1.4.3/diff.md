# Comparing `tmp/dbt_firebolt-1.4.2.tar.gz` & `tmp/dbt_firebolt-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dbt-firebolt/dbt-firebolt/dist/.tmp-xcyajm_u/dbt_firebolt-1.4.2.tar", last modified: Mon Apr 24 10:28:09 2023, max compression
+gzip compressed data, was "/home/runner/work/dbt-firebolt/dbt-firebolt/dist/.tmp-eolf6tlk/dbt_firebolt-1.4.3.tar", last modified: Thu Apr 27 13:56:14 2023, max compression
```

## Comparing `dbt_firebolt-1.4.2.tar` & `dbt_firebolt-1.4.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 10:27:59.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/dropif.sql
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/adapters/firebolt/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-27 13:56:04.000000 dbt_firebolt-1.4.3/dbt/adapters/firebolt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/adapters/firebolt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/adapters/firebolt/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/adapters/firebolt/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/adapters/firebolt/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/adapters/firebolt/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/dbt_external_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/dbt_external_tables/dropif.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt_firebolt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt_firebolt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt_firebolt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt_firebolt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt_firebolt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/dbt_firebolt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-27 13:55:50.000000 dbt_firebolt-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-27 13:56:14.000000 dbt_firebolt-1.4.3/setup.cfg
```

### Comparing `dbt_firebolt-1.4.2/LICENSE` & `dbt_firebolt-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/PKG-INFO` & `dbt_firebolt-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_firebolt
-Version: 1.4.2
+Version: 1.4.3
 Summary: The Firebolt adapter plugin for dbt (data build tool)
 Home-page: https://github.com/firebolt-db/dbt-firebolt
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/dbt-firebolt/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt_firebolt-1.4.2/README.md` & `dbt_firebolt-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/adapters/firebolt/column.py` & `dbt_firebolt-1.4.3/dbt/adapters/firebolt/column.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     def is_date(self) -> bool:
         return self.dtype.lower() == 'date'
 
     @classmethod
     def from_description(cls, name: str, raw_data_type: str) -> Column:
         if raw_data_type.startswith('ARRAY'):
             return cls(name, raw_data_type)
-        return Column.from_description(name, raw_data_type)
+        return super().from_description(name, raw_data_type)
```

### Comparing `dbt_firebolt-1.4.2/dbt/adapters/firebolt/connections.py` & `dbt_firebolt-1.4.3/dbt/adapters/firebolt/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/adapters/firebolt/impl.py` & `dbt_firebolt-1.4.3/dbt/adapters/firebolt/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/adapters/firebolt/relation.py` & `dbt_firebolt-1.4.3/dbt/adapters/firebolt/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/apply_grants.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/relation.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/catalog.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/merge.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/seed.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/table.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/view.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/listagg.sql` & `dbt_firebolt-1.4.3/dbt/include/firebolt/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/dbt_firebolt.egg-info/PKG-INFO` & `dbt_firebolt-1.4.3/dbt_firebolt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-firebolt
-Version: 1.4.2
+Version: 1.4.3
 Summary: The Firebolt adapter plugin for dbt (data build tool)
 Home-page: https://github.com/firebolt-db/dbt-firebolt
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/dbt-firebolt/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt_firebolt-1.4.2/dbt_firebolt.egg-info/SOURCES.txt` & `dbt_firebolt-1.4.3/dbt_firebolt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.2/setup.cfg` & `dbt_firebolt-1.4.3/setup.cfg`

 * *Files identical despite different names*

