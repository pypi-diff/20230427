# Comparing `tmp/sqlmesh-0.6.3.dev1.tar.gz` & `tmp/sqlmesh-0.6.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.6.3.dev1.tar", last modified: Wed Apr 26 23:19:10 2023, max compression
+gzip compressed data, was "sqlmesh-0.6.3.dev3.tar", last modified: Thu Apr 27 18:25:09 2023, max compression
```

## Comparing `sqlmesh-0.6.3.dev1.tar` & `sqlmesh-0.6.3.dev3.tar`

### file list

```diff
@@ -1,736 +1,736 @@
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.677892 sqlmesh-0.6.3.dev1/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.505922 sqlmesh-0.6.3.dev1/.circleci/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1872 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev1/.circleci/config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4414 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev1/.circleci/continue_config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/.dockerignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2152 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev1/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1900 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev1/.pre-commit-config.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      234 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev1/.readthedocs.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      135 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/Dockerfile.api
--rw-r--r--   0 eakmanrq   (501) staff       (20)      383 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/Dockerfile.app
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11346 2023-03-21 00:57:17.000000 sqlmesh-0.6.3.dev1/LICENSE
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1855 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2143 2023-04-26 23:19:10.678000 sqlmesh-0.6.3.dev1/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1192 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1008 2023-04-26 15:46:42.000000 sqlmesh-0.6.3.dev1/docker-compose.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.508209 sqlmesh-0.6.3.dev1/docs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.488369 sqlmesh-0.6.3.dev1/docs/_readthedocs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.508451 sqlmesh-0.6.3.dev1/docs/_readthedocs/html/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev1/docs/_readthedocs/html/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9965 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/docs/comparisons.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.510120 sqlmesh-0.6.3.dev1/docs/concepts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.510566 sqlmesh-0.6.3.dev1/docs/concepts/architecture/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1334 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/concepts/architecture/serialization.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1113 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6689 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev1/docs/concepts/audits.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3866 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/concepts/environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5952 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/docs/concepts/glossary.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       13 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/concepts/hooks.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3027 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/concepts/macros.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.511722 sqlmesh-0.6.3.dev1/docs/concepts/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9934 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/docs/concepts/models/model_kinds.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7859 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/docs/concepts/models/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev1/docs/concepts/models/python_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4938 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev1/docs/concepts/models/seed_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5356 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev1/docs/concepts/models/sql_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6637 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/docs/concepts/overview.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.511891 sqlmesh-0.6.3.dev1/docs/concepts/plans/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    43124 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8973 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/docs/concepts/plans.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/docs/concepts/tests.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      607 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/docs/development.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.513627 sqlmesh-0.6.3.dev1/docs/guides/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1943 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/docs/guides/connections.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1309 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/docs/guides/migrations.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10756 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev1/docs/guides/models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6133 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/docs/guides/multi_repo.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2142 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev1/docs/guides/projects.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.514895 sqlmesh-0.6.3.dev1/docs/guides/scheduling/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   740917 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   379880 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5648 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/guides/scheduling.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1854 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/docs/guides/testing.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5459 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/docs/index.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      297 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/docs/installation.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.516782 sqlmesh-0.6.3.dev1/docs/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2905 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/docs/integrations/airflow.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7801 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/docs/integrations/dbt.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24057 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/docs/integrations/engines.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      867 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/docs/integrations/github.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      217 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/docs/integrations/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      665 2023-03-28 15:29:23.000000 sqlmesh-0.6.3.dev1/docs/prerequisites.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10723 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/docs/quick_start.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.518378 sqlmesh-0.6.3.dev1/docs/reference/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6093 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/docs/reference/cli.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13607 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/docs/reference/configuration.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4579 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev1/docs/reference/notebook.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1127 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/reference/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       14 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/reference/python.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       16 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev1/docs/release_notes.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      122 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev1/docs/requirements.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3249 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/docs/sqlmesh.png
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.518586 sqlmesh-0.6.3.dev1/examples/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.519756 sqlmesh-0.6.3.dev1/examples/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1713 2023-04-08 22:07:58.000000 sqlmesh-0.6.3.dev1/examples/airflow/Dockerfile.template
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2164 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/examples/airflow/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)      942 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/airflow/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/airflow/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.519927 sqlmesh-0.6.3.dev1/examples/airflow/dags/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      263 2023-03-21 21:04:44.000000 sqlmesh-0.6.3.dev1/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3515 2023-04-08 22:07:58.000000 sqlmesh-0.6.3.dev1/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/airflow/requirements.txt
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.520403 sqlmesh-0.6.3.dev1/examples/airflow/spark_conf/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      872 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      151 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.489541 sqlmesh-0.6.3.dev1/examples/multi/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.520611 sqlmesh-0.6.3.dev1/examples/multi/repo_1/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.524751 sqlmesh-0.6.3.dev1/examples/multi/repo_1/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.525024 sqlmesh-0.6.3.dev1/examples/multi/repo_1/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.525513 sqlmesh-0.6.3.dev1/examples/multi/repo_1/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       63 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/models/a.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/models/b.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.525725 sqlmesh-0.6.3.dev1/examples/multi/repo_1/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_1/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.525828 sqlmesh-0.6.3.dev1/examples/multi/repo_2/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.526101 sqlmesh-0.6.3.dev1/examples/multi/repo_2/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.526361 sqlmesh-0.6.3.dev1/examples/multi/repo_2/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.526933 sqlmesh-0.6.3.dev1/examples/multi/repo_2/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       64 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/models/c.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/models/d.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.527075 sqlmesh-0.6.3.dev1/examples/multi/repo_2/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/examples/multi/repo_2/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.527537 sqlmesh-0.6.3.dev1/examples/sushi/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/sushi/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.527973 sqlmesh-0.6.3.dev1/examples/sushi/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      105 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/audits/items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      119 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/audits/order_items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      829 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.528248 sqlmesh-0.6.3.dev1/examples/sushi/data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-06 17:30:39.000000 sqlmesh-0.6.3.dev1/examples/sushi/data/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/sushi/helper.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.528639 sqlmesh-0.6.3.dev1/examples/sushi/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.528980 sqlmesh-0.6.3.dev1/examples/sushi/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/sushi/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      702 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.531122 sqlmesh-0.6.3.dev1/examples/sushi/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      916 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      204 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1910 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1911 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/order_items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/orders.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      346 2023-04-11 16:01:14.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      465 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      123 2023-02-17 23:03:10.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      691 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      197 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.531270 sqlmesh-0.6.3.dev1/examples/sushi/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.531421 sqlmesh-0.6.3.dev1/examples/sushi/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1459 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.532236 sqlmesh-0.6.3.dev1/examples/sushi_dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       15 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/.user.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.532475 sqlmesh-0.6.3.dev1/examples/sushi_dbt/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      507 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.532688 sqlmesh-0.6.3.dev1/examples/sushi_dbt/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.533623 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1125 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      182 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      309 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      752 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      186 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.490594 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.533756 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.533883 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.534119 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.534257 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.534344 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.534428 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.534510 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      783 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.535157 sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)       97 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.535302 sqlmesh-0.6.3.dev1/examples/sushi_dbt/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.535390 sqlmesh-0.6.3.dev1/examples/sushi_dbt/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.535561 sqlmesh-0.6.3.dev1/examples/wursthall/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.491297 sqlmesh-0.6.3.dev1/examples/wursthall/audits/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.535699 sqlmesh-0.6.3.dev1/examples/wursthall/audits/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      141 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.535923 sqlmesh-0.6.3.dev1/examples/wursthall/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      618 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev1/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.536167 sqlmesh-0.6.3.dev1/examples/wursthall/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.536779 sqlmesh-0.6.3.dev1/examples/wursthall/models/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      433 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      256 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3161 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      542 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.537462 sqlmesh-0.6.3.dev1/examples/wursthall/models/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1672 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      120 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3434 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      892 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.491781 sqlmesh-0.6.3.dev1/examples/wursthall/seeds/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.537609 sqlmesh-0.6.3.dev1/examples/wursthall/seeds/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7416 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.538026 sqlmesh-0.6.3.dev1/examples/wursthall/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      955 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2113 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/mkdocs.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.538170 sqlmesh-0.6.3.dev1/pdoc/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)     1153 2023-03-28 16:31:06.000000 sqlmesh-0.6.3.dev1/pdoc/cli.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.538417 sqlmesh-0.6.3.dev1/pdoc/templates/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      131 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.538774 sqlmesh-0.6.3.dev1/posts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.542322 sqlmesh-0.6.3.dev1/posts/virtual_data_environments/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   318753 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/posts/virtual_data_environments/change_categorization.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   274526 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/posts/virtual_data_environments/isolated_rigid_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   163619 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/posts/virtual_data_environments/partial_breaking.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   298971 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/posts/virtual_data_environments/stateful_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   366545 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev1/posts/virtual_data_environments/virtual_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)  1344487 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/posts/virtual_data_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18638 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/posts/virtual_data_environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      734 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/pytest.ini
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1393 2023-04-26 23:19:10.678484 sqlmesh-0.6.3.dev1/setup.cfg
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3158 2023-04-26 19:08:23.000000 sqlmesh-0.6.3.dev1/setup.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.547982 sqlmesh-0.6.3.dev1/sqlmesh/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        3 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/.airflowignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3950 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-04-26 23:19:10.000000 sqlmesh-0.6.3.dev1/sqlmesh/_version.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.553508 sqlmesh-0.6.3.dev1/sqlmesh/cli/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      898 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/cli/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4314 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/cli/example_project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9641 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/cli/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1433 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/cli/options.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.564366 sqlmesh-0.6.3.dev1/sqlmesh/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      586 2023-03-15 16:48:19.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/_typing.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.565139 sqlmesh-0.6.3.dev1/sqlmesh/core/audit/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      449 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1071 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8136 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.569332 sqlmesh-0.6.3.dev1/sqlmesh/core/config/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      668 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4412 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1001 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      940 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21184 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/connection.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3351 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1655 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5611 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/root.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8421 2023-04-26 18:37:27.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29390 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      735 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/constants.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    36130 2023-04-26 23:17:06.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8904 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/context_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17626 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/dialect.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.572629 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2626 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      762 2023-01-17 23:57:22.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29021 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4191 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4238 2023-04-14 22:30:56.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15694 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      402 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1939 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1971 2023-04-14 18:08:36.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2149 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6650 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1181 2023-03-31 20:18:23.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2658 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5638 2023-04-26 23:17:06.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1849 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      742 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/hooks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12673 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18920 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.573949 sqlmesh-0.6.3.dev1/sqlmesh/core/model/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      594 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1746 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1300 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2417 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    47685 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8168 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/kind.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13034 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/meta.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2017 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/model/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2314 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.574902 sqlmesh-0.6.3.dev1/sqlmesh/core/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      191 2022-12-27 18:08:03.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    22476 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/plan/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8125 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12623 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/renderer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15386 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20418 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.575809 sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      527 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    33750 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19248 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.576471 sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      692 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13382 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13144 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20682 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10834 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/test.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1412 2023-04-26 18:37:27.000000 sqlmesh-0.6.3.dev1/sqlmesh/core/user.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.579360 sqlmesh-0.6.3.dev1/sqlmesh/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       79 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9390 2023-04-14 22:30:56.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16746 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11231 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1762 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/column.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4771 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5087 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8044 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9806 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13257 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/package.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3701 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/profile.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4772 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      927 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3137 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/source.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13503 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/dbt/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.579673 sqlmesh-0.6.3.dev1/sqlmesh/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/engines/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4437 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev1/sqlmesh/engines/commands.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.579979 sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-03-22 20:32:25.000000 sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.580530 sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      148 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2571 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.580693 sqlmesh-0.6.3.dev1/sqlmesh/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.581296 sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2210 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1726 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1829 2023-01-18 17:26:59.000000 sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13754 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/magics.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.582281 sqlmesh-0.6.3.dev1/sqlmesh/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/migrations/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1749 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      103 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/migrations/v0002_remove_identify.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1183 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/migrations/v0003_move_batch_size.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      534 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/py.typed
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.582443 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.584325 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-05 17:38:29.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4020 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3830 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18819 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.585027 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-15 19:26:11.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2132 2023-03-22 20:54:22.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      868 2023-03-22 20:54:22.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8508 2023-03-22 20:33:52.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.592677 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1444 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6307 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2549 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      877 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1322 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1211 2023-01-20 20:10:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1340 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5222 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11104 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4400 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1292 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4139 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5213 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.595867 sqlmesh-0.6.3.dev1/sqlmesh/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4378 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3593 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7530 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      410 2022-12-30 00:03:50.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/conversions.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4329 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7549 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1244 2023-04-26 18:37:27.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16084 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15093 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1609 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/rich.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6487 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1419 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.548663 sqlmesh-0.6.3.dev1/sqlmesh.egg-info/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2143 2023-04-26 23:19:10.000000 sqlmesh-0.6.3.dev1/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21395 2023-04-26 23:19:10.000000 sqlmesh-0.6.3.dev1/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)        1 2023-04-26 23:19:10.000000 sqlmesh-0.6.3.dev1/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      142 2023-04-26 23:19:10.000000 sqlmesh-0.6.3.dev1/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      838 2023-04-26 23:19:10.000000 sqlmesh-0.6.3.dev1/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-04-26 23:19:10.000000 sqlmesh-0.6.3.dev1/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21020 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev1/sqlmesh.svg
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.596409 sqlmesh-0.6.3.dev1/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      285 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/common_fixtures.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4037 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/tests/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.600714 sqlmesh-0.6.3.dev1/tests/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/core/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.602427 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    27881 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1270 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1253 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2613 2023-01-17 20:15:22.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1569 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8036 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3191 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7073 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/tests/core/test_audit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6611 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/core/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      850 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/core/test_connection_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10197 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/test_context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2749 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/core/test_dialect.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      464 2022-12-28 16:53:44.000000 sqlmesh-0.6.3.dev1/tests/core/test_environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    26741 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/tests/core/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5880 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/test_macros.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25301 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/tests/core/test_model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15741 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/core/test_plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3862 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/core/test_plan_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4647 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/core/test_scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    32235 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/core/test_schema_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      857 2023-01-06 18:44:22.000000 sqlmesh-0.6.3.dev1/tests/core/test_seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    28498 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/core/test_snapshot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10299 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    23620 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/core/test_state_sync.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.602989 sqlmesh-0.6.3.dev1/tests/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-16 20:33:14.000000 sqlmesh-0.6.3.dev1/tests/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      739 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/tests/dbt/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2537 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/dbt/test_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13195 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/tests/dbt/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17095 2023-04-26 20:34:09.000000 sqlmesh-0.6.3.dev1/tests/dbt/test_transformation.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.603220 sqlmesh-0.6.3.dev1/tests/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/engines/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.603611 sqlmesh-0.6.3.dev1/tests/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      357 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/engines/spark/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1503 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.498393 sqlmesh-0.6.3.dev1/tests/fixtures/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.493821 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.604575 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.604825 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.493944 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1055 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.604940 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10264 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.605221 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.605987 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      334 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      863 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      196 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.497555 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.606138 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.606315 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.606581 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.607031 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1155 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      108 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.607200 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.607307 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.607432 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      540 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1250 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.607726 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       42 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.607929 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.608475 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.608648 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.609176 sqlmesh-0.6.3.dev1/tests/fixtures/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9823 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/tests/fixtures/migrations/environments.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25229 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.609529 sqlmesh-0.6.3.dev1/tests/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.620428 sqlmesh-0.6.3.dev1/tests/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/integrations/github/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.620826 sqlmesh-0.6.3.dev1/tests/integrations/github/fixtures/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      816 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      477 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.621006 sqlmesh-0.6.3.dev1/tests/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.622117 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1414 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.622685 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4442 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4392 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9857 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1345 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6222 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5944 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.625254 sqlmesh-0.6.3.dev1/tests/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1118 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/tests/utils/test_cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3580 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/utils/test_concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6430 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/utils/test_connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1381 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/utils/test_dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1818 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/utils/test_date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/utils/test_filesystem.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5516 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/utils/test_jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5790 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/utils/test_metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2501 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/utils/test_pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      518 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev1/tests/utils/test_pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2911 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev1/tests/utils/test_transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1194 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/tests/utils/test_yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.625487 sqlmesh-0.6.3.dev1/tests/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/tests/web/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16232 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/tests/web/test_main.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.625621 sqlmesh-0.6.3.dev1/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/web/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.630051 sqlmesh-0.6.3.dev1/web/client/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1104 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/.eslintrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)       94 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      129 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/.prettierignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      403 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/.prettierrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1076 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev1/web/client/index.html
--rw-r--r--   0 eakmanrq   (501) staff       (20)    37689 2023-04-26 15:46:39.000000 sqlmesh-0.6.3.dev1/web/client/openapi.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      330 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/orval.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)   408504 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/package-lock.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2389 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/package.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev1/web/client/playwright.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)       82 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/postcss.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.499230 sqlmesh-0.6.3.dev1/web/client/public/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.630311 sqlmesh-0.6.3.dev1/web/client/public/favicons/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2473 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.631066 sqlmesh-0.6.3.dev1/web/client/src/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.631739 sqlmesh-0.6.3.dev1/web/client/src/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1236 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/api/channels.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5243 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/src/api/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3247 2023-03-22 20:27:52.000000 sqlmesh-0.6.3.dev1/web/client/src/api/instance.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.499475 sqlmesh-0.6.3.dev1/web/client/src/assets/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.499587 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.634211 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74500 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74524 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74368 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73964 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    68940 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    67284 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74116 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73916 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.643487 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    55004 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56384 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57104 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    62320 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56652 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61688 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57680 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    53148 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57060 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56836 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61460 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    52820 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    59176 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    63876 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60768 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    81732 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60992 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    64792 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.644887 sqlmesh-0.6.3.dev1/web/client/src/context/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4126 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/src/context/context.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5719 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/src/context/editor.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      923 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/context/fileTree.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2284 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/context/lineage.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2661 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev1/web/client/src/context/plan.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1562 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/context/theme.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.645429 sqlmesh-0.6.3.dev1/web/client/src/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      308 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      817 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9555 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/src/index.css
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.499848 sqlmesh-0.6.3.dev1/web/client/src/library/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.501027 sqlmesh-0.6.3.dev1/web/client/src/library/components/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.645616 sqlmesh-0.6.3.dev1/web/client/src/library/components/banner/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1705 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.645996 sqlmesh-0.6.3.dev1/web/client/src/library/components/button/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4517 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.646349 sqlmesh-0.6.3.dev1/web/client/src/library/components/button/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3516 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.646552 sqlmesh-0.6.3.dev1/web/client/src/library/components/divider/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      856 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.646794 sqlmesh-0.6.3.dev1/web/client/src/library/components/divider/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      632 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.648879 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1992 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5437 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8518 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2718 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9819 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11419 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3796 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.649417 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5820 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5744 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1538 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.653040 sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10852 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6045 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2997 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      562 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.653420 sqlmesh-0.6.3.dev1/web/client/src/library/components/graph/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15931 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7045 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.653956 sqlmesh-0.6.3.dev1/web/client/src/library/components/ide/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4342 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4933 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    22356 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.654861 sqlmesh-0.6.3.dev1/web/client/src/library/components/input/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2087 2023-03-28 20:12:46.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      688 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.655100 sqlmesh-0.6.3.dev1/web/client/src/library/components/loading/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      486 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/loading/Loading.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.655942 sqlmesh-0.6.3.dev1/web/client/src/library/components/logo/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2292 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4637 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8042 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.656671 sqlmesh-0.6.3.dev1/web/client/src/library/components/modal/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1560 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1953 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1447 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.668529 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9269 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6775 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1312 2023-03-28 20:12:46.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10448 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4920 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15855 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9926 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12528 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3444 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2155 2023-03-22 20:27:52.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2599 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.668668 sqlmesh-0.6.3.dev1/web/client/src/library/components/progress/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      713 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.668837 sqlmesh-0.6.3.dev1/web/client/src/library/components/report/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1047 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/report/ReportTestsErrors.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.669349 sqlmesh-0.6.3.dev1/web/client/src/library/components/root/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      526 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1921 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      443 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.669695 sqlmesh-0.6.3.dev1/web/client/src/library/components/splitPane/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      788 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.669905 sqlmesh-0.6.3.dev1/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11713 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.670132 sqlmesh-0.6.3.dev1/web/client/src/library/components/toggle/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1453 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1197 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/main.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.671346 sqlmesh-0.6.3.dev1/web/client/src/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1647 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/models/artifact.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3472 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev1/web/client/src/models/directory.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4190 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/models/environment.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2190 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/client/src/models/file.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/models/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      766 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/models/initial.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      200 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/routes.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.671898 sqlmesh-0.6.3.dev1/web/client/src/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       35 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/web/client/src/tests/setup.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.672484 sqlmesh-0.6.3.dev1/web/client/src/types/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      467 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/types/enum.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      137 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev1/web/client/src/types/index.d.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.672924 sqlmesh-0.6.3.dev1/web/client/src/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4102 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev1/web/client/src/utils/index.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5245 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/utils/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.673102 sqlmesh-0.6.3.dev1/web/client/src/workers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      113 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/workers/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.673513 sqlmesh-0.6.3.dev1/web/client/src/workers/sqlglot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1105 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1578 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5879 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/client/tailwind.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.673696 sqlmesh-0.6.3.dev1/web/client/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      170 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/tests/initial.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1141 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/client/tsconfig.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1297 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev1/web/client/vite.config.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.675705 sqlmesh-0.6.3.dev1/web/server/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev1/web/server/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.675890 sqlmesh-0.6.3.dev1/web/server/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev1/web/server/api/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-26 23:19:10.677688 sqlmesh-0.6.3.dev1/web/server/api/endpoints/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      784 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4564 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/commands.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      819 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1858 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/directories.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      721 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/environments.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      637 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/events.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5383 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/files.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3283 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/lineage.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      962 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3635 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/server/api/endpoints/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3775 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev1/web/server/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/server/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5777 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev1/web/server/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      260 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev1/web/server/openapi.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2421 2023-04-26 15:46:39.000000 sqlmesh-0.6.3.dev1/web/server/settings.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev1/web/server/sse.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2461 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev1/web/server/utils.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      790 2023-04-26 18:37:32.000000 sqlmesh-0.6.3.dev1/web/server/watcher.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.102110 sqlmesh-0.6.3.dev3/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.916305 sqlmesh-0.6.3.dev3/.circleci/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1872 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev3/.circleci/config.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4414 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev3/.circleci/continue_config.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/.dockerignore
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2152 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev3/.gitignore
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1900 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      234 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev3/.readthedocs.yaml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      135 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/Dockerfile.api
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      383 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/Dockerfile.app
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    11346 2023-03-21 00:57:17.000000 sqlmesh-0.6.3.dev3/LICENSE
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1855 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/Makefile
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2143 2023-04-27 18:25:09.102263 sqlmesh-0.6.3.dev3/PKG-INFO
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1192 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/README.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1008 2023-04-27 17:19:12.000000 sqlmesh-0.6.3.dev3/docker-compose.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.919223 sqlmesh-0.6.3.dev3/docs/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.899449 sqlmesh-0.6.3.dev3/docs/_readthedocs/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.919503 sqlmesh-0.6.3.dev3/docs/_readthedocs/html/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev3/docs/_readthedocs/html/.keep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9965 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/docs/comparisons.md
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.921495 sqlmesh-0.6.3.dev3/docs/concepts/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.922041 sqlmesh-0.6.3.dev3/docs/concepts/architecture/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1334 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1113 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6689 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev3/docs/concepts/audits.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3866 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/concepts/environments.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5952 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/docs/concepts/glossary.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       13 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/concepts/hooks.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3027 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/concepts/macros.md
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.923436 sqlmesh-0.6.3.dev3/docs/concepts/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9934 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7859 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/docs/concepts/models/overview.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev3/docs/concepts/models/python_models.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4938 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev3/docs/concepts/models/seed_models.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5356 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev3/docs/concepts/models/sql_models.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6637 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/docs/concepts/overview.md
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.923633 sqlmesh-0.6.3.dev3/docs/concepts/plans/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    43124 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8973 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/docs/concepts/plans.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/docs/concepts/tests.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      607 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/docs/development.md
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.925428 sqlmesh-0.6.3.dev3/docs/guides/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1943 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/docs/guides/connections.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1309 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/docs/guides/migrations.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10756 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev3/docs/guides/models.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6133 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/docs/guides/multi_repo.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2142 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev3/docs/guides/projects.md
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.926642 sqlmesh-0.6.3.dev3/docs/guides/scheduling/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   740917 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   379880 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5648 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/guides/scheduling.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1854 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/docs/guides/testing.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5459 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/docs/index.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      297 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/docs/installation.md
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.928603 sqlmesh-0.6.3.dev3/docs/integrations/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2905 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/docs/integrations/airflow.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7801 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/docs/integrations/dbt.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    24057 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/docs/integrations/engines.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      867 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/docs/integrations/github.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      217 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/docs/integrations/overview.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      665 2023-03-28 15:29:23.000000 sqlmesh-0.6.3.dev3/docs/prerequisites.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10723 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/docs/quick_start.md
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.930072 sqlmesh-0.6.3.dev3/docs/reference/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6093 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/docs/reference/cli.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13607 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/docs/reference/configuration.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4579 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev3/docs/reference/notebook.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1127 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/reference/overview.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       14 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/reference/python.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       16 2023-03-27 03:14:49.000000 sqlmesh-0.6.3.dev3/docs/release_notes.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      122 2023-03-31 20:18:29.000000 sqlmesh-0.6.3.dev3/docs/requirements.txt
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3249 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/docs/sqlmesh.png
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.930288 sqlmesh-0.6.3.dev3/examples/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.931504 sqlmesh-0.6.3.dev3/examples/airflow/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1713 2023-04-08 22:07:58.000000 sqlmesh-0.6.3.dev3/examples/airflow/Dockerfile.template
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2164 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/examples/airflow/Makefile
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      942 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/airflow/README.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/airflow/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.931699 sqlmesh-0.6.3.dev3/examples/airflow/dags/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      263 2023-03-21 21:04:44.000000 sqlmesh-0.6.3.dev3/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3515 2023-04-08 22:07:58.000000 sqlmesh-0.6.3.dev3/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/airflow/requirements.txt
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.932350 sqlmesh-0.6.3.dev3/examples/airflow/spark_conf/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      872 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      151 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.900521 sqlmesh-0.6.3.dev3/examples/multi/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.932563 sqlmesh-0.6.3.dev3/examples/multi/repo_1/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.932723 sqlmesh-0.6.3.dev3/examples/multi/repo_1/audits/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.932897 sqlmesh-0.6.3.dev3/examples/multi/repo_1/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.937392 sqlmesh-0.6.3.dev3/examples/multi/repo_1/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       63 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.937642 sqlmesh-0.6.3.dev3/examples/multi/repo_1/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.937778 sqlmesh-0.6.3.dev3/examples/multi/repo_2/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.938073 sqlmesh-0.6.3.dev3/examples/multi/repo_2/audits/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      147 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.938362 sqlmesh-0.6.3.dev3/examples/multi/repo_2/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.938909 sqlmesh-0.6.3.dev3/examples/multi/repo_2/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       64 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.939106 sqlmesh-0.6.3.dev3/examples/multi/repo_2/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.939626 sqlmesh-0.6.3.dev3/examples/sushi/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/sushi/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.939971 sqlmesh-0.6.3.dev3/examples/sushi/audits/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      105 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/audits/items.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      119 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      829 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi/config.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.940176 sqlmesh-0.6.3.dev3/examples/sushi/data/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-06 17:30:39.000000 sqlmesh-0.6.3.dev3/examples/sushi/data/.keep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/sushi/helper.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.940359 sqlmesh-0.6.3.dev3/examples/sushi/hooks/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.940593 sqlmesh-0.6.3.dev3/examples/sushi/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/sushi/macros/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      702 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/macros/macros.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.942584 sqlmesh-0.6.3.dev3/examples/sushi/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      916 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      204 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/customers.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1910 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/items.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1911 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/order_items.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/orders.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      346 2023-04-11 16:01:14.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      465 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      123 2023-02-17 23:03:10.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      691 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      197 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.942715 sqlmesh-0.6.3.dev3/examples/sushi/seeds/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.942846 sqlmesh-0.6.3.dev3/examples/sushi/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1459 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.943655 sqlmesh-0.6.3.dev3/examples/sushi_dbt/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       15 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.943892 sqlmesh-0.6.3.dev3/examples/sushi_dbt/analyses/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/config.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      507 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.944106 sqlmesh-0.6.3.dev3/examples/sushi_dbt/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.945320 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1125 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      182 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      309 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      752 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      186 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.901556 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.945472 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.945629 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.945938 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.946157 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.946300 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.946405 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.946503 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      783 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.947274 sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       97 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.947416 sqlmesh-0.6.3.dev3/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.947504 sqlmesh-0.6.3.dev3/examples/sushi_dbt/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.947675 sqlmesh-0.6.3.dev3/examples/wursthall/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.902283 sqlmesh-0.6.3.dev3/examples/wursthall/audits/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.947807 sqlmesh-0.6.3.dev3/examples/wursthall/audits/db/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      141 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/config.yaml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.948046 sqlmesh-0.6.3.dev3/examples/wursthall/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      618 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev3/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.948265 sqlmesh-0.6.3.dev3/examples/wursthall/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.948868 sqlmesh-0.6.3.dev3/examples/wursthall/models/db/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      433 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      256 2023-04-27 17:28:43.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3161 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      542 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.949491 sqlmesh-0.6.3.dev3/examples/wursthall/models/src/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1672 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      120 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3434 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      892 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.902678 sqlmesh-0.6.3.dev3/examples/wursthall/seeds/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.949632 sqlmesh-0.6.3.dev3/examples/wursthall/seeds/src/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7416 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.949910 sqlmesh-0.6.3.dev3/examples/wursthall/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      955 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2113 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/mkdocs.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.950052 sqlmesh-0.6.3.dev3/pdoc/
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)     1153 2023-03-28 16:31:06.000000 sqlmesh-0.6.3.dev3/pdoc/cli.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.950288 sqlmesh-0.6.3.dev3/pdoc/templates/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      131 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.950512 sqlmesh-0.6.3.dev3/posts/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.956507 sqlmesh-0.6.3.dev3/posts/virtual_data_environments/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   318753 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   274526 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   163619 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   298971 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   366545 2023-04-19 01:45:56.000000 sqlmesh-0.6.3.dev3/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)  1344487 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    18638 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/posts/virtual_data_environments.md
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      734 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/pytest.ini
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1393 2023-04-27 18:25:09.102779 sqlmesh-0.6.3.dev3/setup.cfg
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3170 2023-04-27 18:23:39.000000 sqlmesh-0.6.3.dev3/setup.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.963553 sqlmesh-0.6.3.dev3/sqlmesh/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        3 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/.airflowignore
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3950 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-04-27 18:25:08.000000 sqlmesh-0.6.3.dev3/sqlmesh/_version.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.965217 sqlmesh-0.6.3.dev3/sqlmesh/cli/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      898 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/cli/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4314 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/cli/example_project.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9641 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/cli/main.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1433 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/cli/options.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.969720 sqlmesh-0.6.3.dev3/sqlmesh/core/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      586 2023-03-15 16:48:19.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/_typing.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.971323 sqlmesh-0.6.3.dev3/sqlmesh/core/audit/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      449 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1071 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8136 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.973338 sqlmesh-0.6.3.dev3/sqlmesh/core/config/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      668 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4412 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/base.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1001 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      940 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/common.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    21184 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/connection.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3351 2023-04-20 16:12:45.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/loader.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1655 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/model.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5611 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/root.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8421 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    29390 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/console.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      735 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/constants.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    36130 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/context.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8904 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/context_diff.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    17626 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/dialect.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.976616 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2626 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      762 2023-01-17 23:57:22.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    29358 2023-04-27 18:23:39.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4191 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4238 2023-04-14 22:30:56.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    15681 2023-04-27 18:23:39.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      402 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1939 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1971 2023-04-14 18:08:36.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2149 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6650 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1181 2023-03-31 20:18:23.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2658 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4763 2023-04-27 18:23:39.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1849 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/environment.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      742 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/hooks.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    12673 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/loader.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    18920 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/macros.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.983955 sqlmesh-0.6.3.dev3/sqlmesh/core/model/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      594 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1746 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/cache.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1300 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/common.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2417 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    47699 2023-04-27 18:23:39.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/definition.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8168 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/kind.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13034 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/meta.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2017 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/model/seed.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2314 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.984846 sqlmesh-0.6.3.dev3/sqlmesh/core/plan/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      191 2022-12-27 18:08:03.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    22476 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8125 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    12623 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/renderer.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    15386 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/scheduler.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    20418 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.985967 sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      527 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    33750 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    19247 2023-04-27 18:23:39.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.986724 sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      692 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13382 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13144 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    20682 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10834 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/test.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1412 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/core/user.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.991385 sqlmesh-0.6.3.dev3/sqlmesh/dbt/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       79 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9390 2023-04-14 22:30:56.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    16746 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    11231 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1762 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/column.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4771 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/common.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5087 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/context.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8044 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/loader.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9806 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/model.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13257 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/package.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3701 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/profile.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4772 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/project.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      927 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/seed.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3137 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/source.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13503 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/target.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/dbt/util.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.991753 sqlmesh-0.6.3.dev3/sqlmesh/engines/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/engines/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4437 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev3/sqlmesh/engines/commands.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.992282 sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-03-22 20:32:25.000000 sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.993148 sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      148 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2571 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.993331 sqlmesh-0.6.3.dev3/sqlmesh/integrations/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.993980 sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2210 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1726 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1829 2023-01-18 17:26:59.000000 sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13754 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/magics.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.994945 sqlmesh-0.6.3.dev3/sqlmesh/migrations/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1749 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      103 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1183 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/migrations/v0003_move_batch_size.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      534 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/py.typed
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.995119 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.997044 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-05 17:38:29.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4020 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3830 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    18819 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.997769 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-15 19:26:11.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2132 2023-03-22 20:54:22.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      868 2023-03-22 20:54:22.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8508 2023-03-22 20:33:52.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.006459 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1444 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6307 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2549 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      877 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1322 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1211 2023-01-20 20:10:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1340 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5222 2023-03-22 20:26:36.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    11104 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4400 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1292 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4139 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5213 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.009510 sqlmesh-0.6.3.dev3/sqlmesh/utils/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4378 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3593 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/cache.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7530 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      410 2022-12-30 00:03:50.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/conversions.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4329 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/dag.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7549 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/date.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1244 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/errors.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    16084 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/jinja.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    15093 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/pandas.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1609 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/rich.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6487 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1419 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.964272 sqlmesh-0.6.3.dev3/sqlmesh.egg-info/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2143 2023-04-27 18:25:08.000000 sqlmesh-0.6.3.dev3/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    21395 2023-04-27 18:25:08.000000 sqlmesh-0.6.3.dev3/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        1 2023-04-27 18:25:08.000000 sqlmesh-0.6.3.dev3/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      142 2023-04-27 18:25:08.000000 sqlmesh-0.6.3.dev3/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      850 2023-04-27 18:25:08.000000 sqlmesh-0.6.3.dev3/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-04-27 18:25:08.000000 sqlmesh-0.6.3.dev3/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    21020 2023-03-27 03:14:56.000000 sqlmesh-0.6.3.dev3/sqlmesh.svg
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.009986 sqlmesh-0.6.3.dev3/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      285 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/common_fixtures.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4037 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/tests/conftest.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.014579 sqlmesh-0.6.3.dev3/tests/core/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/core/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.016342 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    27881 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1270 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1253 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2613 2023-01-17 20:15:22.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1569 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8036 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3191 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7073 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/tests/core/test_audit.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6611 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/core/test_config.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      850 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/core/test_connection_config.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10197 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/test_context.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2749 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/core/test_dialect.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      464 2022-12-28 16:53:44.000000 sqlmesh-0.6.3.dev3/tests/core/test_environment.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    26741 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/core/test_integration.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5880 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/test_macros.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    25301 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/tests/core/test_model.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    15741 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/core/test_plan.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3862 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4647 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/core/test_scheduler.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    32235 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/core/test_schema_diff.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      857 2023-01-06 18:44:22.000000 sqlmesh-0.6.3.dev3/tests/core/test_seed.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    28498 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/core/test_snapshot.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10299 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    23620 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/core/test_state_sync.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.016914 sqlmesh-0.6.3.dev3/tests/dbt/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-16 20:33:14.000000 sqlmesh-0.6.3.dev3/tests/dbt/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      739 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/tests/dbt/conftest.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2537 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/dbt/test_adapter.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    13195 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/tests/dbt/test_config.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    17095 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/dbt/test_transformation.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.017078 sqlmesh-0.6.3.dev3/tests/engines/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/engines/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.017542 sqlmesh-0.6.3.dev3/tests/engines/spark/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/engines/spark/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      357 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/engines/spark/conftest.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1503 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.906211 sqlmesh-0.6.3.dev3/tests/fixtures/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.905018 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.018609 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.018764 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.905212 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1055 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.018885 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10264 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.019155 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.019861 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      334 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      863 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      196 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.905535 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.019993 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.020126 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.020367 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.030644 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1155 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      108 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.030800 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.030893 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.030988 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      540 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1250 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.031247 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       42 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.031389 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.031870 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.032041 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.032382 sqlmesh-0.6.3.dev3/tests/fixtures/migrations/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9823 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    25229 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.032709 sqlmesh-0.6.3.dev3/tests/integrations/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/integrations/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.032886 sqlmesh-0.6.3.dev3/tests/integrations/github/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/integrations/github/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.033131 sqlmesh-0.6.3.dev3/tests/integrations/github/fixtures/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      816 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      477 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.033270 sqlmesh-0.6.3.dev3/tests/schedulers/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/schedulers/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.034481 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1414 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.034932 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/operators/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4442 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4392 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9857 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1345 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6222 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5944 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.037088 sqlmesh-0.6.3.dev3/tests/utils/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/utils/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1118 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/tests/utils/test_cache.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3580 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/utils/test_concurrency.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6430 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/utils/test_connection_pool.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1381 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/utils/test_dag.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1818 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/utils/test_date.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/utils/test_filesystem.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5516 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/utils/test_jinja.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5790 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2501 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/utils/test_pandas.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      518 2022-12-05 19:41:13.000000 sqlmesh-0.6.3.dev3/tests/utils/test_pydantic.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2911 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev3/tests/utils/test_transactional_file.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1194 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/tests/utils/test_yaml.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.037530 sqlmesh-0.6.3.dev3/tests/web/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/tests/web/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    16232 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/tests/web/test_main.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.037746 sqlmesh-0.6.3.dev3/web/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/web/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.045303 sqlmesh-0.6.3.dev3/web/client/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1104 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/.eslintrc.js
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       94 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/.gitignore
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      129 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/.prettierignore
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      403 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/.prettierrc.js
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1076 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev3/web/client/index.html
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    37689 2023-04-27 17:30:24.000000 sqlmesh-0.6.3.dev3/web/client/openapi.json
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      330 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/orval.config.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)   408504 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/package-lock.json
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2389 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/package.json
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev3/web/client/playwright.config.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       82 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/postcss.config.js
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.906917 sqlmesh-0.6.3.dev3/web/client/public/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.045552 sqlmesh-0.6.3.dev3/web/client/public/favicons/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2473 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.046324 sqlmesh-0.6.3.dev3/web/client/src/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.047048 sqlmesh-0.6.3.dev3/web/client/src/api/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1236 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/api/channels.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5243 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/src/api/index.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3247 2023-03-22 20:27:52.000000 sqlmesh-0.6.3.dev3/web/client/src/api/instance.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.907132 sqlmesh-0.6.3.dev3/web/client/src/assets/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.907230 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.052684 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74500 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74524 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74368 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73964 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    68940 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    67284 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74116 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73916 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.058565 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    55004 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56384 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57104 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    62320 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56652 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61688 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57680 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    53148 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57060 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56836 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61460 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    52820 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    59176 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    63876 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60768 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    81732 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60992 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 eakmanrq   (501) staff       (20)    64792 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.059933 sqlmesh-0.6.3.dev3/web/client/src/context/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4126 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/src/context/context.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5719 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/src/context/editor.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      923 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/context/fileTree.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2284 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/client/src/context/lineage.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2661 2023-04-14 19:58:28.000000 sqlmesh-0.6.3.dev3/web/client/src/context/plan.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1562 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/context/theme.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.060385 sqlmesh-0.6.3.dev3/web/client/src/hooks/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      308 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      817 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9555 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/src/index.css
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.907454 sqlmesh-0.6.3.dev3/web/client/src/library/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:08.908652 sqlmesh-0.6.3.dev3/web/client/src/library/components/
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.060578 sqlmesh-0.6.3.dev3/web/client/src/library/components/banner/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1705 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.060833 sqlmesh-0.6.3.dev3/web/client/src/library/components/button/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4517 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.061128 sqlmesh-0.6.3.dev3/web/client/src/library/components/button/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3516 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.061338 sqlmesh-0.6.3.dev3/web/client/src/library/components/divider/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      856 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.061596 sqlmesh-0.6.3.dev3/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      632 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.063490 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1992 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-04-27 18:23:33.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8518 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2718 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9819 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    11419 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3527 2023-04-27 18:23:33.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.063909 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5820 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5744 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1538 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.064770 sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10852 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6045 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2997 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      562 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.065190 sqlmesh-0.6.3.dev3/web/client/src/library/components/graph/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    15931 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     7063 2023-04-27 18:23:33.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.065880 sqlmesh-0.6.3.dev3/web/client/src/library/components/ide/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4342 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4933 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    22356 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.078829 sqlmesh-0.6.3.dev3/web/client/src/library/components/input/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2087 2023-03-28 20:12:46.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      688 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.079331 sqlmesh-0.6.3.dev3/web/client/src/library/components/loading/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      486 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/loading/Loading.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.080558 sqlmesh-0.6.3.dev3/web/client/src/library/components/logo/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2292 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4637 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     8042 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.081146 sqlmesh-0.6.3.dev3/web/client/src/library/components/modal/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1560 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1953 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1447 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.083572 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9269 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     6775 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1312 2023-03-28 20:12:46.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    10448 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4920 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    15855 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     9926 2023-03-27 22:28:21.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    12528 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3444 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2155 2023-03-22 20:27:52.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2599 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.083706 sqlmesh-0.6.3.dev3/web/client/src/library/components/progress/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      713 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.083885 sqlmesh-0.6.3.dev3/web/client/src/library/components/report/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1047 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/report/ReportTestsErrors.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.084476 sqlmesh-0.6.3.dev3/web/client/src/library/components/root/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      526 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1921 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      443 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.084872 sqlmesh-0.6.3.dev3/web/client/src/library/components/splitPane/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      788 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.085120 sqlmesh-0.6.3.dev3/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)    11713 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.085286 sqlmesh-0.6.3.dev3/web/client/src/library/components/toggle/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1453 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1197 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/main.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.086701 sqlmesh-0.6.3.dev3/web/client/src/models/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1647 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/models/artifact.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3472 2023-04-06 22:49:28.000000 sqlmesh-0.6.3.dev3/web/client/src/models/directory.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4190 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/models/environment.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2190 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/client/src/models/file.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/models/index.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      766 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/models/initial.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      200 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/routes.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.087193 sqlmesh-0.6.3.dev3/web/client/src/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)       35 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/web/client/src/tests/setup.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.087611 sqlmesh-0.6.3.dev3/web/client/src/types/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      467 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/types/enum.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      137 2023-03-22 22:04:55.000000 sqlmesh-0.6.3.dev3/web/client/src/types/index.d.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.096283 sqlmesh-0.6.3.dev3/web/client/src/utils/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4102 2023-03-27 01:55:02.000000 sqlmesh-0.6.3.dev3/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5245 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/utils/index.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.096528 sqlmesh-0.6.3.dev3/web/client/src/workers/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      113 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/workers/index.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.096905 sqlmesh-0.6.3.dev3/web/client/src/workers/sqlglot/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1105 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1578 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5879 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/client/tailwind.config.js
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.097087 sqlmesh-0.6.3.dev3/web/client/tests/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      170 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/tests/initial.spec.ts
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1141 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/client/tsconfig.json
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1297 2023-04-17 00:43:26.000000 sqlmesh-0.6.3.dev3/web/client/vite.config.ts
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.099840 sqlmesh-0.6.3.dev3/web/server/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.6.3.dev3/web/server/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.100088 sqlmesh-0.6.3.dev3/web/server/api/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.6.3.dev3/web/server/api/__init__.py
+drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-27 18:25:09.101877 sqlmesh-0.6.3.dev3/web/server/api/endpoints/
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      784 2023-04-14 20:24:08.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     4564 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/commands.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      819 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/context.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1858 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/directories.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      721 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/environments.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      637 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/events.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5383 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/files.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3283 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      962 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/models.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3635 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/server/api/endpoints/plan.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     3775 2023-04-20 17:40:30.000000 sqlmesh-0.6.3.dev3/web/server/console.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/server/main.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     5777 2023-04-25 19:48:01.000000 sqlmesh-0.6.3.dev3/web/server/models.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      260 2023-04-04 21:33:39.000000 sqlmesh-0.6.3.dev3/web/server/openapi.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2421 2023-04-27 17:30:24.000000 sqlmesh-0.6.3.dev3/web/server/settings.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-03-17 21:52:31.000000 sqlmesh-0.6.3.dev3/web/server/sse.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)     2461 2023-04-19 01:45:57.000000 sqlmesh-0.6.3.dev3/web/server/utils.py
+-rw-r--r--   0 eakmanrq   (501) staff       (20)      790 2023-04-27 17:55:12.000000 sqlmesh-0.6.3.dev3/web/server/watcher.py
```

### Comparing `sqlmesh-0.6.3.dev1/.circleci/config.yml` & `sqlmesh-0.6.3.dev3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/.circleci/continue_config.yml` & `sqlmesh-0.6.3.dev3/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/.gitignore` & `sqlmesh-0.6.3.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/.pre-commit-config.yaml` & `sqlmesh-0.6.3.dev3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/LICENSE` & `sqlmesh-0.6.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/Makefile` & `sqlmesh-0.6.3.dev3/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/PKG-INFO` & `sqlmesh-0.6.3.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.3.dev1
+Version: 0.6.3.dev3
 Summary: UNKNOWN
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Description: ![SQLMesh logo](sqlmesh.svg)
```

### Comparing `sqlmesh-0.6.3.dev1/README.md` & `sqlmesh-0.6.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docker-compose.yml` & `sqlmesh-0.6.3.dev3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/comparisons.md` & `sqlmesh-0.6.3.dev3/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/architecture/serialization.md` & `sqlmesh-0.6.3.dev3/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.6.3.dev3/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/audits.md` & `sqlmesh-0.6.3.dev3/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/environments.md` & `sqlmesh-0.6.3.dev3/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/glossary.md` & `sqlmesh-0.6.3.dev3/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/macros.md` & `sqlmesh-0.6.3.dev3/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/models/model_kinds.md` & `sqlmesh-0.6.3.dev3/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/models/overview.md` & `sqlmesh-0.6.3.dev3/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/models/python_models.md` & `sqlmesh-0.6.3.dev3/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/models/seed_models.md` & `sqlmesh-0.6.3.dev3/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/models/sql_models.md` & `sqlmesh-0.6.3.dev3/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/overview.md` & `sqlmesh-0.6.3.dev3/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.6.3.dev3/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/plans.md` & `sqlmesh-0.6.3.dev3/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/concepts/tests.md` & `sqlmesh-0.6.3.dev3/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/development.md` & `sqlmesh-0.6.3.dev3/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/connections.md` & `sqlmesh-0.6.3.dev3/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/migrations.md` & `sqlmesh-0.6.3.dev3/docs/guides/migrations.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/models.md` & `sqlmesh-0.6.3.dev3/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/multi_repo.md` & `sqlmesh-0.6.3.dev3/docs/guides/multi_repo.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/projects.md` & `sqlmesh-0.6.3.dev3/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.6.3.dev3/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.6.3.dev3/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/scheduling.md` & `sqlmesh-0.6.3.dev3/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/guides/testing.md` & `sqlmesh-0.6.3.dev3/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/index.md` & `sqlmesh-0.6.3.dev3/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/integrations/airflow.md` & `sqlmesh-0.6.3.dev3/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/integrations/dbt.md` & `sqlmesh-0.6.3.dev3/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/integrations/engines.md` & `sqlmesh-0.6.3.dev3/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/integrations/github.md` & `sqlmesh-0.6.3.dev3/docs/integrations/github.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/prerequisites.md` & `sqlmesh-0.6.3.dev3/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/quick_start.md` & `sqlmesh-0.6.3.dev3/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/reference/cli.md` & `sqlmesh-0.6.3.dev3/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/reference/configuration.md` & `sqlmesh-0.6.3.dev3/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/reference/notebook.md` & `sqlmesh-0.6.3.dev3/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/reference/overview.md` & `sqlmesh-0.6.3.dev3/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/docs/sqlmesh.png` & `sqlmesh-0.6.3.dev3/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/airflow/Dockerfile.template` & `sqlmesh-0.6.3.dev3/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/airflow/Makefile` & `sqlmesh-0.6.3.dev3/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/airflow/README.md` & `sqlmesh-0.6.3.dev3/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.6.3.dev3/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.6.3.dev3/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/config.py` & `sqlmesh-0.6.3.dev3/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/helper.py` & `sqlmesh-0.6.3.dev3/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/macros/macros.py` & `sqlmesh-0.6.3.dev3/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.3.dev3/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/models/items.py` & `sqlmesh-0.6.3.dev3/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/models/order_items.py` & `sqlmesh-0.6.3.dev3/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/models/orders.py` & `sqlmesh-0.6.3.dev3/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.3.dev3/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.6.3.dev3/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.6.3.dev3/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/macros/macros.py` & `sqlmesh-0.6.3.dev3/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.6.3.dev3/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.6.3.dev3/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.6.3.dev3/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.6.3.dev3/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/models/src/shared.py` & `sqlmesh-0.6.3.dev3/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.6.3.dev3/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.6.3.dev3/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.6.3.dev3/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/mkdocs.yml` & `sqlmesh-0.6.3.dev3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/pdoc/cli.py` & `sqlmesh-0.6.3.dev3/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/posts/virtual_data_environments/change_categorization.png` & `sqlmesh-0.6.3.dev3/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/posts/virtual_data_environments/isolated_rigid_envs.png` & `sqlmesh-0.6.3.dev3/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/posts/virtual_data_environments/partial_breaking.png` & `sqlmesh-0.6.3.dev3/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/posts/virtual_data_environments/stateful_envs.png` & `sqlmesh-0.6.3.dev3/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/posts/virtual_data_environments/virtual_envs.png` & `sqlmesh-0.6.3.dev3/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/posts/virtual_data_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.6.3.dev3/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/posts/virtual_data_environments.md` & `sqlmesh-0.6.3.dev3/posts/virtual_data_environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/pytest.ini` & `sqlmesh-0.6.3.dev3/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/setup.cfg` & `sqlmesh-0.6.3.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/setup.py` & `sqlmesh-0.6.3.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             "databricks-sql-connector",
             "databricks-cli",
         ],
         "dev": [
             f"apache-airflow=={os.environ.get('AIRFLOW_VERSION', '2.3.3')}",
             "autoflake==1.7.7",
             "black==22.6.0",
-            "dbt-core",
+            "dbt-core<1.5.0",
             "Faker",
             "google-auth",
             "isort==5.10.1",
             "mkdocs-include-markdown-plugin==4.0.3",
             "mkdocs-material==9.0.5",
             "mypy~=1.0.0",
             "ipywidgets",
@@ -81,15 +81,15 @@
             "tenacity==8.1.0",
             "types-croniter",
             "types-dateparser",
             "types-pytz",
             "types-requests==2.28.8",
         ],
         "dbt": [
-            "dbt-core",
+            "dbt-core<1.5.0",
         ],
         "postgres": [
             "psycopg2",
         ],
         "redshift": [
             "redshift_connector",
         ],
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/cli/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/cli/example_project.py` & `sqlmesh-0.6.3.dev3/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/cli/main.py` & `sqlmesh-0.6.3.dev3/sqlmesh/cli/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/cli/options.py` & `sqlmesh-0.6.3.dev3/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/_typing.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/audit/definition.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/base.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/common.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/connection.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/loader.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/model.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/root.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/console.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/constants.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/context.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/context_diff.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/dialect.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 from __future__ import annotations
 
 import contextlib
 import itertools
 import logging
 import typing as t
+import uuid
 
 import pandas as pd
 from sqlglot import Dialect, exp
 from sqlglot.errors import ErrorLevel
 
 from sqlmesh.core.dialect import pandas_to_sql
 from sqlmesh.core.engine_adapter._typing import (
@@ -638,16 +639,16 @@
             )
         )
 
     def merge(
         self,
         target_table: TableName,
         source_table: QueryOrDF,
-        column_names: t.Iterable[str],
-        unique_key: t.Iterable[str],
+        column_names: t.Sequence[str],
+        unique_key: t.Sequence[str],
     ) -> None:
         on = exp.and_(
             *(
                 exp.EQ(
                     this=exp.column(part, TARGET_ALIAS),
                     expression=exp.column(part, SOURCE_ALIAS),
                 )
@@ -790,10 +791,21 @@
     ) -> t.List[DataObject]:
         """
         Returns all the data objects that exist in the given schema and optionally catalog.
         """
 
         raise NotImplementedError()
 
+    def _get_temp_table(
+        self,
+        table: TableName,
+    ) -> exp.Table:
+        """
+        Returns the name of the temp table that should be used for the given table name.
+        """
+        table = exp.to_table(table)
+        table.set("this", f"__temp_{table.name}_{uuid.uuid4().hex}")
+        return table
+
 
 class EngineAdapterWithIndexSupport(EngineAdapter):
     SUPPORTS_INDEXES = True
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/base_postgres.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import functools
 import logging
 import typing as t
-import uuid
 
 import pandas as pd
 from sqlglot import exp
 from sqlglot.errors import ErrorLevel
 from sqlglot.transforms import remove_precision_parameterized_types
 
 from sqlmesh.core.engine_adapter._typing import DF_TYPES, Query
@@ -140,20 +139,22 @@
     ) -> t.Tuple[BigQueryQueryResult, str]:
         """
         Loads a pandas dataframe into a temporary table in BigQuery. Returns the result of the load and the name of the
         temporary table. The temporary table will be deleted after 3 hours.
         """
         from google.cloud import bigquery
 
-        table = exp.to_table(table)
         precisionless_col_to_types = {
             col_name: remove_precision_parameterized_types(col_type)
             for col_name, col_type in columns_to_types.items()
         }
-        temp_table_name = f"{self.client.project}.{table.db}.__temp_{table.name}_{uuid.uuid4().hex}"
+
+        temp_table_name = ".".join(
+            [self.client.project, self._get_temp_table(table).sql(dialect=self.dialect)]
+        )
         schema = [
             bigquery.SchemaField(col_name, col_type.sql(dialect=self.dialect))
             for col_name, col_type in precisionless_col_to_types.items()
         ]
         bq_table = bigquery.Table(table_ref=temp_table_name, schema=schema)
         bq_table.expires = to_datetime("in 3 hours")
         self.client.create_table(bq_table)
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/engine_adapter/spark.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,50 +59,25 @@
         else:
             super().insert_append(table_name, query_or_df, columns_to_types, contains_json)
 
     def merge(
         self,
         target_table: TableName,
         source_table: QueryOrDF,
-        column_names: t.Iterable[str],
-        unique_key: t.Iterable[str],
+        column_names: t.Sequence[str],
+        unique_key: t.Sequence[str],
     ) -> None:
         if isinstance(source_table, PySparkDataFrame):
-            self._merge_pyspark_df(target_table, source_table, column_names, unique_key)
+            temp_view_name = self._get_temp_table(target_table).sql(dialect=self.dialect)
+            source_table.createOrReplaceTempView(temp_view_name)
+            query = exp.select(*column_names).from_(temp_view_name)
+            super().merge(target_table, query, column_names, unique_key)
         else:
             super().merge(target_table, source_table, column_names, unique_key)
 
-    def _merge_pyspark_df(
-        self,
-        target_table: TableName,
-        source_df: PySparkDataFrame,
-        column_names: t.Iterable[str],
-        unique_key: t.Iterable[str],
-    ) -> None:
-        """
-        Merge using DataFrames is only supported for Delta Tables using the Delta Table API.
-        It is not supported in Vanilla Spark. Iceberg only supports merge using SQL.
-        """
-        from delta.tables import DeltaTable  # type: ignore
-
-        if isinstance(target_table, exp.Table):
-            target_table = target_table.sql(dialect=self.dialect)
-        column_mapping = {f"target.`{col}`": f"source.`{col}`" for col in column_names}
-        (
-            DeltaTable.forName(self.spark, target_table)
-            .alias("target")
-            .merge(
-                source_df.alias("source"),
-                condition=" AND ".join([f"target.`{key}` = source.`{key}`" for key in unique_key]),
-            )
-            .whenMatchedUpdate(set=column_mapping)
-            .whenNotMatchedInsert(values=column_mapping)
-            .execute()
-        )
-
     def _insert_append_pandas_df(
         self,
         table_name: TableName,
         df: pd.DataFrame,
         columns_to_types: t.Optional[t.Dict[str, exp.DataType]] = None,
     ) -> None:
         self._insert_pyspark_df(table_name, self._ensure_pyspark_df(df), overwrite=False)
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/environment.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/hooks.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/loader.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/macros.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/cache.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/common.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/decorator.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/definition.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
     def depends_on(self) -> t.Set[str]:
         """All of the upstream dependencies referenced in the model's query, excluding self references.
 
         Returns:
             A list of all the upstream table names.
         """
         if self.depends_on_ is not None:
-            return self.depends_on_
+            return self.depends_on_ - {self.name}
 
         if self._depends_on is None:
             self._depends_on = _find_tables(self.render_query()) - {self.name}
         return self._depends_on
 
     @property
     def columns_to_types(self) -> t.Dict[str, exp.DataType]:
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/kind.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/meta.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/model/seed.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/notification_target.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/plan/definition.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/plan/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/renderer.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/scheduler.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/schema_diff.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/snapshot/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                         time_column=model.time_column,
                         columns_to_types=columns_to_types,
                     )
                 elif snapshot.is_incremental_by_unique_key_kind:
                     self.adapter.merge(
                         table_name,
                         query_or_df,
-                        column_names=columns_to_types.keys(),
+                        column_names=list(columns_to_types),
                         unique_key=model.unique_key,
                     )
                 else:
                     raise SQLMeshError(f"Unexpected SnapshotKind: {snapshot.model.kind}")
 
         for sql_statement in model.sql_statements:
             self.adapter.execute(sql_statement)
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/test.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/core/user.py` & `sqlmesh-0.6.3.dev3/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/adapter.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/basemodel.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/builtin.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/column.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/common.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/context.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/loader.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/model.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/package.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/package.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/profile.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/project.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/seed.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/source.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/dbt/target.py` & `sqlmesh-0.6.3.dev3/sqlmesh/dbt/target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/engines/commands.py` & `sqlmesh-0.6.3.dev3/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/app.py` & `sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.6.3.dev3/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.6.3.dev3/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/magics.py` & `sqlmesh-0.6.3.dev3/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.6.3.dev3/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/migrations/v0003_move_batch_size.py` & `sqlmesh-0.6.3.dev3/sqlmesh/migrations/v0003_move_batch_size.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py` & `sqlmesh-0.6.3.dev3/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/postgres.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.6.3.dev3/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/__init__.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/cache.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/concurrency.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/dag.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/date.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/errors.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/jinja.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/pandas.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/pydantic.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/rich.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh/utils/yaml.py` & `sqlmesh-0.6.3.dev3/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.6.3.dev3/sqlmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.6.3.dev1
+Version: 0.6.3.dev3
 Summary: UNKNOWN
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
 Description: ![SQLMesh logo](sqlmesh.svg)
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.6.3.dev3/sqlmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.6.3.dev3/sqlmesh.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 google-cloud-bigquery-storage
 
 [databricks]
 databricks-sql-connector
 databricks-cli
 
 [dbt]
-dbt-core
+dbt-core<1.5.0
 
 [dev]
 apache-airflow==2.3.3
 autoflake==1.7.7
 black==22.6.0
-dbt-core
+dbt-core<1.5.0
 Faker
 google-auth
 isort==5.10.1
 mkdocs-include-markdown-plugin==4.0.3
 mkdocs-material==9.0.5
 mypy~=1.0.0
 ipywidgets
```

### Comparing `sqlmesh-0.6.3.dev1/sqlmesh.svg` & `sqlmesh-0.6.3.dev3/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/conftest.py` & `sqlmesh-0.6.3.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_base_postgres.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_postgres.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.6.3.dev3/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_audit.py` & `sqlmesh-0.6.3.dev3/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_config.py` & `sqlmesh-0.6.3.dev3/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_connection_config.py` & `sqlmesh-0.6.3.dev3/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_context.py` & `sqlmesh-0.6.3.dev3/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_dialect.py` & `sqlmesh-0.6.3.dev3/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_integration.py` & `sqlmesh-0.6.3.dev3/tests/core/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_macros.py` & `sqlmesh-0.6.3.dev3/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_model.py` & `sqlmesh-0.6.3.dev3/tests/core/test_model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_plan.py` & `sqlmesh-0.6.3.dev3/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_plan_evaluator.py` & `sqlmesh-0.6.3.dev3/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_scheduler.py` & `sqlmesh-0.6.3.dev3/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_schema_diff.py` & `sqlmesh-0.6.3.dev3/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_seed.py` & `sqlmesh-0.6.3.dev3/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_snapshot.py` & `sqlmesh-0.6.3.dev3/tests/core/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.6.3.dev3/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/core/test_state_sync.py` & `sqlmesh-0.6.3.dev3/tests/core/test_state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/dbt/conftest.py` & `sqlmesh-0.6.3.dev3/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/dbt/test_adapter.py` & `sqlmesh-0.6.3.dev3/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/dbt/test_config.py` & `sqlmesh-0.6.3.dev3/tests/dbt/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/dbt/test_transformation.py` & `sqlmesh-0.6.3.dev3/tests/dbt/test_transformation.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/engines/spark/test_db_api.py` & `sqlmesh-0.6.3.dev3/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.6.3.dev3/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/migrations/environments.json` & `sqlmesh-0.6.3.dev3/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.6.3.dev3/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.6.3.dev3/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.6.3.dev3/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.6.3.dev3/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.6.3.dev3/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.6.3.dev3/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_cache.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_concurrency.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_connection_pool.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_dag.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_date.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_filesystem.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_jinja.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_metaprogramming.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_pandas.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_pydantic.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_transactional_file.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/utils/test_yaml.py` & `sqlmesh-0.6.3.dev3/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/tests/web/test_main.py` & `sqlmesh-0.6.3.dev3/tests/web/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/.eslintrc.js` & `sqlmesh-0.6.3.dev3/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/index.html` & `sqlmesh-0.6.3.dev3/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/openapi.json` & `sqlmesh-0.6.3.dev3/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/package-lock.json` & `sqlmesh-0.6.3.dev3/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/package.json` & `sqlmesh-0.6.3.dev3/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/playwright.config.ts` & `sqlmesh-0.6.3.dev3/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/public/favicons/favicon.ico` & `sqlmesh-0.6.3.dev3/web/client/public/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/api/channels.ts` & `sqlmesh-0.6.3.dev3/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/api/index.ts` & `sqlmesh-0.6.3.dev3/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/api/instance.ts` & `sqlmesh-0.6.3.dev3/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.6.3.dev3/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/context/context.ts` & `sqlmesh-0.6.3.dev3/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/context/editor.ts` & `sqlmesh-0.6.3.dev3/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/context/fileTree.ts` & `sqlmesh-0.6.3.dev3/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/context/lineage.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/context/lineage.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/context/plan.ts` & `sqlmesh-0.6.3.dev3/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/context/theme.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.6.3.dev3/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/index.css` & `sqlmesh-0.6.3.dev3/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/Editor.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import CodeEditor from './EditorCode'
 import EditorFooter from './EditorFooter'
 import EditorTabs from './EditorTabs'
 import EditorInspector from './EditorInspector'
 import './Editor.css'
 import EditorPreview from './EditorPreview'
 import { useStoreEditor } from '~/context/editor'
+import { useStoreLineage, useStoreReactFlow } from '@context/lineage'
+
 import clsx from 'clsx'
 
 export default function Editor(): JSX.Element {
   const files = useStoreFileTree(s => s.files)
   const selectedFile = useStoreFileTree(s => s.selectedFile)
 
   const tab = useStoreEditor(s => s.tab)
@@ -25,14 +27,17 @@
   const createTab = useStoreEditor(s => s.createTab)
   const addTab = useStoreEditor(s => s.addTab)
   const setDialects = useStoreEditor(s => s.setDialects)
   const setPreviewQuery = useStoreEditor(s => s.setPreviewQuery)
   const setPreviewConsole = useStoreEditor(s => s.setPreviewConsole)
   const setPreviewTable = useStoreEditor(s => s.setPreviewTable)
 
+  const clearActiveEdges = useStoreLineage(s => s.clearActiveEdges)
+  const clearNodesAndEdges = useStoreReactFlow(s => s.clearNodesAndEdges)
+
   const [isReadyEngine, setIsreadyEngine] = useState(false)
   const [direction, setDirection] = useState<'vertical' | 'horizontal'>(
     'vertical',
   )
 
   const handleEngineWorkerMessage = useCallback((e: MessageEvent): void => {
     if (e.data.topic === 'init') {
@@ -79,14 +84,16 @@
       if (storedTabsIds.includes(file.id)) {
         addTab(createTab(file))
       }
     })
   }, [files])
 
   useEffect(() => {
+    clearActiveEdges()
+    clearNodesAndEdges()
     setPreviewQuery(undefined)
     setPreviewTable(undefined)
     setPreviewConsole(undefined)
   }, [tab])
 
   useEffect(() => {
     if (selectedFile == null || tab?.file === selectedFile) return
```

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import { useMemo, type MouseEvent } from 'react'
 import { PlusIcon, XCircleIcon } from '@heroicons/react/24/solid'
 import { EnumSize, EnumVariant } from '~/types/enum'
 import { Button } from '../button/Button'
 import clsx from 'clsx'
 import { type EditorTab, useStoreEditor } from '~/context/editor'
-import { useStoreLineage, useStoreReactFlow } from '@context/lineage'
 
 export default function EditorTabs(): JSX.Element {
   const tabs = useStoreEditor(s => s.tabs)
   const selectTab = useStoreEditor(s => s.selectTab)
   const createTab = useStoreEditor(s => s.createTab)
 
   const [tabsLocal, tabsRemote] = useMemo(() => {
@@ -67,31 +66,26 @@
 }
 
 function Tab({ tab, title }: { tab: EditorTab; title: string }): JSX.Element {
   const activeTab = useStoreEditor(s => s.tab)
   const selectTab = useStoreEditor(s => s.selectTab)
   const closeTab = useStoreEditor(s => s.closeTab)
 
-  const clearActiveEdges = useStoreLineage(s => s.clearActiveEdges)
-  const clearNodesAndEdges = useStoreReactFlow(s => s.clearNodesAndEdges)
-
   function closeEditorTab(tab: EditorTab): void {
     closeTab(tab.file)
   }
 
   return (
     <li
       className={clsx(
         'inline-block py-1 pr-2 last-child:pr-0 overflow-hidden text-center overflow-ellipsis cursor-pointer',
       )}
       onClick={(e: MouseEvent) => {
         e.stopPropagation()
 
-        clearActiveEdges()
-        clearNodesAndEdges()
         selectTab(tab)
       }}
     >
       <span
         className={clsx(
           'flex border-2 justify-between items-center pl-2 pr-1 py-[0.125rem] min-w-[8rem] rounded-md group border-transparent border-r border-r-theme-darker dark:border-r-theme-lighter',
           tab.file.id === activeTab?.file.id
```

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/graph/Graph.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/graph/help.ts`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   isHighlighted?: boolean
   isInteractive?: boolean
   [key: string]: any
 }
 
 const elk = new ELK()
 
-const NODE_WIDTH = 172
+const NODE_WIDTH = 64
 const NODE_HEIGHT = 32
 
 export function getNodesAndEdges({
   lineage,
   highlightedNodes,
   models,
   nodes = [],
@@ -191,15 +191,15 @@
   )
 
   return modelNames.reduce((acc: Record<string, Node>, label: string) => {
     const node =
       current[label] ??
       createGraphNode({
         label,
-        width: NODE_WIDTH,
+        width: NODE_WIDTH + label.length * 8,
         height: NODE_HEIGHT + 32 * (models.get(label)?.columns?.length ?? 0),
       })
 
     node.data.isHighlighted = highlightedNodes.includes(label)
     node.data.isInteractive =
       isArrayNotEmpty(highlightedNodes) &&
       isFalse(highlightedNodes.includes(label))
```

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/report/ReportTestsErrors.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/report/ReportTestsErrors.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/main.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/models/artifact.ts` & `sqlmesh-0.6.3.dev3/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/models/directory.ts` & `sqlmesh-0.6.3.dev3/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/models/environment.ts` & `sqlmesh-0.6.3.dev3/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/models/file.ts` & `sqlmesh-0.6.3.dev3/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/models/initial.ts` & `sqlmesh-0.6.3.dev3/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/tests/utils.tsx` & `sqlmesh-0.6.3.dev3/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/utils/index.spec.ts` & `sqlmesh-0.6.3.dev3/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/utils/index.ts` & `sqlmesh-0.6.3.dev3/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.6.3.dev3/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.6.3.dev3/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/tailwind.config.js` & `sqlmesh-0.6.3.dev3/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/tsconfig.json` & `sqlmesh-0.6.3.dev3/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/client/vite.config.ts` & `sqlmesh-0.6.3.dev3/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/__init__.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/commands.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/context.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/directories.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/environments.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/events.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/files.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/lineage.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/models.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/api/endpoints/plan.py` & `sqlmesh-0.6.3.dev3/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/console.py` & `sqlmesh-0.6.3.dev3/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/main.py` & `sqlmesh-0.6.3.dev3/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/models.py` & `sqlmesh-0.6.3.dev3/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/settings.py` & `sqlmesh-0.6.3.dev3/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/sse.py` & `sqlmesh-0.6.3.dev3/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/utils.py` & `sqlmesh-0.6.3.dev3/web/server/utils.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.6.3.dev1/web/server/watcher.py` & `sqlmesh-0.6.3.dev3/web/server/watcher.py`

 * *Files identical despite different names*

