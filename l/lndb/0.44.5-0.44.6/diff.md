# Comparing `tmp/lndb-0.44.5.tar.gz` & `tmp/lndb-0.44.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.44.5.tar", last modified: Wed Apr 26 03:54:37 2023, max compression
+gzip compressed data, was "lndb-0.44.6.tar", last modified: Thu Apr 27 17:05:47 2023, max compression
```

## Comparing `lndb-0.44.5.tar` & `lndb-0.44.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     3832 2023-04-21 13:18:34.631639 lndb-0.44.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-21 13:18:34.631707 lndb-0.44.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-21 13:18:34.631769 lndb-0.44.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-04-21 13:18:34.631841 lndb-0.44.5/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-24 06:41:18.770060 lndb-0.44.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-04-21 13:18:34.632006 lndb-0.44.5/LICENSE
--rw-r--r--   0        0        0      173 2023-04-21 13:18:34.632071 lndb-0.44.5/README.md
--rw-r--r--   0        0        0       52 2023-04-21 13:18:34.632182 lndb-0.44.5/docs/api.md
--rw-r--r--   0        0        0    47755 2023-04-25 20:36:08.721067 lndb-0.44.5/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-04-21 13:18:34.632486 lndb-0.44.5/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-04-21 13:18:34.632563 lndb-0.44.5/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-04-21 13:18:34.632642 lndb-0.44.5/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-04-21 13:18:34.632695 lndb-0.44.5/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-24 06:41:18.770918 lndb-0.44.5/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-04-21 13:18:34.632807 lndb-0.44.5/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-21 13:18:34.632917 lndb-0.44.5/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-21 13:18:34.633000 lndb-0.44.5/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-21 13:18:34.633102 lndb-0.44.5/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11110 2023-04-21 13:18:34.633175 lndb-0.44.5/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5355 2023-04-21 13:18:34.633258 lndb-0.44.5/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6390 2023-04-24 06:41:18.771249 lndb-0.44.5/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3746 2023-04-24 12:01:41.554380 lndb-0.44.5/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-04-21 13:18:34.633441 lndb-0.44.5/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-21 13:18:34.633502 lndb-0.44.5/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-04-21 13:18:34.633563 lndb-0.44.5/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-24 06:41:18.771572 lndb-0.44.5/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-04-21 13:18:34.633686 lndb-0.44.5/docs/index.md
--rw-r--r--   0        0        0      118 2023-04-21 13:18:34.633747 lndb-0.44.5/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-25 20:36:22.476938 lndb-0.44.5/lndb/__init__.py
--rw-r--r--   0        0        0     4507 2023-04-21 13:18:34.633901 lndb-0.44.5/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-04-21 13:18:34.633976 lndb-0.44.5/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-21 13:18:34.634041 lndb-0.44.5/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-25 20:35:43.603247 lndb-0.44.5/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-21 13:18:34.634153 lndb-0.44.5/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-21 13:18:34.634210 lndb-0.44.5/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-25 12:02:07.055852 lndb-0.44.5/lndb/_info.py
--rw-r--r--   0        0        0     6051 2023-04-21 13:18:34.634337 lndb-0.44.5/lndb/_init_instance.py
--rw-r--r--   0        0        0     4003 2023-04-21 13:18:34.634409 lndb-0.44.5/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-21 13:18:34.634486 lndb-0.44.5/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-21 13:18:34.634548 lndb-0.44.5/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-25 12:02:07.056289 lndb-0.44.5/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-24 06:41:18.772725 lndb-0.44.5/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-04-21 13:18:34.634765 lndb-0.44.5/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-25 12:02:07.056619 lndb-0.44.5/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-21 13:18:34.634902 lndb-0.44.5/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      700 2023-04-21 13:18:34.634957 lndb-0.44.5/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-04-21 13:18:34.635011 lndb-0.44.5/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-24 06:41:18.772972 lndb-0.44.5/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-21 13:18:34.635125 lndb-0.44.5/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-04-21 13:18:34.635180 lndb-0.44.5/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-04-21 13:18:34.635232 lndb-0.44.5/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-21 13:18:34.635297 lndb-0.44.5/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-21 13:18:34.635390 lndb-0.44.5/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-04-21 13:18:34.635455 lndb-0.44.5/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-21 13:18:34.635521 lndb-0.44.5/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-04-21 13:18:34.635580 lndb-0.44.5/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-04-21 13:18:34.635632 lndb-0.44.5/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-21 13:18:34.635702 lndb-0.44.5/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8764 2023-04-21 13:18:34.635786 lndb-0.44.5/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-04-21 13:18:34.635856 lndb-0.44.5/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-04-21 13:18:34.636120 lndb-0.44.5/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-21 13:18:34.636185 lndb-0.44.5/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-04-21 13:18:34.636245 lndb-0.44.5/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-04-21 13:18:34.636316 lndb-0.44.5/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-24 06:41:18.773287 lndb-0.44.5/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-24 06:41:18.773542 lndb-0.44.5/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-04-21 13:18:34.636532 lndb-0.44.5/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-21 13:18:34.636604 lndb-0.44.5/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-21 13:18:34.636702 lndb-0.44.5/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-04-21 13:18:34.636748 lndb-0.44.5/lndb/test/_env.py
--rw-r--r--   0        0        0     3870 2023-04-21 13:18:34.636808 lndb-0.44.5/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-21 13:18:34.636877 lndb-0.44.5/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-04-21 13:18:34.636938 lndb-0.44.5/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-04-21 13:18:34.636995 lndb-0.44.5/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-21 13:18:34.637059 lndb-0.44.5/noxfile.py
--rw-r--r--   0        0        0     1396 2023-04-25 12:07:23.777541 lndb-0.44.5/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-21 13:18:34.637215 lndb-0.44.5/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-04-21 13:18:34.637282 lndb-0.44.5/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-21 13:18:34.637338 lndb-0.44.5/tests/test_notebooks.py
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.5/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-04-10 14:26:28.783318 lndb-0.44.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-15 08:56:55.830020 lndb-0.44.6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-15 08:56:55.830119 lndb-0.44.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-03-15 08:56:55.830224 lndb-0.44.6/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-24 09:27:00.933000 lndb-0.44.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-15 08:56:55.830520 lndb-0.44.6/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 05:09:16.038571 lndb-0.44.6/README.md
+-rw-r--r--   0        0        0       52 2023-03-15 08:56:55.830736 lndb-0.44.6/docs/api.md
+-rw-r--r--   0        0        0    48038 2023-04-27 17:04:52.978133 lndb-0.44.6/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-15 08:56:55.831086 lndb-0.44.6/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-15 08:56:55.831186 lndb-0.44.6/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-27 05:09:16.039131 lndb-0.44.6/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-27 05:09:16.039234 lndb-0.44.6/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-22 15:24:35.393597 lndb-0.44.6/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-15 08:56:55.831660 lndb-0.44.6/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-10 14:26:28.783932 lndb-0.44.6/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-10 14:26:28.784059 lndb-0.44.6/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-03-27 05:09:16.039598 lndb-0.44.6/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10238 2023-04-27 10:15:48.138286 lndb-0.44.6/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     6419 2023-04-27 10:15:48.138461 lndb-0.44.6/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-24 09:27:00.941223 lndb-0.44.6/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-26 05:23:05.373464 lndb-0.44.6/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-27 05:09:16.039994 lndb-0.44.6/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-21 03:09:31.419101 lndb-0.44.6/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-03-15 08:56:55.832700 lndb-0.44.6/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-22 15:24:35.394504 lndb-0.44.6/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-03-15 08:56:55.832922 lndb-0.44.6/docs/index.md
+-rw-r--r--   0        0        0      118 2023-03-15 08:56:55.833018 lndb-0.44.6/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-27 17:04:10.694916 lndb-0.44.6/lndb/__init__.py
+-rw-r--r--   0        0        0     4697 2023-04-27 17:03:55.795190 lndb-0.44.6/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-03-15 08:56:55.833550 lndb-0.44.6/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 14:26:28.784379 lndb-0.44.6/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-27 10:15:48.138789 lndb-0.44.6/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-10 14:26:28.784709 lndb-0.44.6/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-10 14:26:28.784835 lndb-0.44.6/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-26 05:23:05.375280 lndb-0.44.6/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-04-27 10:15:48.139549 lndb-0.44.6/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6729 2023-04-27 10:15:48.140360 lndb-0.44.6/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-10 14:26:28.785194 lndb-0.44.6/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-10 14:26:28.785299 lndb-0.44.6/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-26 05:23:05.375597 lndb-0.44.6/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-22 15:24:35.395863 lndb-0.44.6/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-03-15 08:56:55.834680 lndb-0.44.6/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-26 05:23:05.375756 lndb-0.44.6/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-10 14:26:28.785570 lndb-0.44.6/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      803 2023-04-27 10:15:48.140662 lndb-0.44.6/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-03-15 08:56:55.834857 lndb-0.44.6/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-24 09:27:00.946199 lndb-0.44.6/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-19 06:33:40.117765 lndb-0.44.6/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-03-15 08:56:55.835145 lndb-0.44.6/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-03-15 08:56:55.835215 lndb-0.44.6/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-21 03:09:31.420591 lndb-0.44.6/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-10 14:26:28.785901 lndb-0.44.6/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-28 04:03:47.769616 lndb-0.44.6/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-10 14:26:28.786021 lndb-0.44.6/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-03-15 08:56:55.835748 lndb-0.44.6/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-03-15 08:56:55.835829 lndb-0.44.6/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-10 14:26:28.786141 lndb-0.44.6/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-04-27 10:15:48.140982 lndb-0.44.6/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-27 05:09:16.041820 lndb-0.44.6/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-03-15 08:56:55.836258 lndb-0.44.6/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-10 14:26:28.786361 lndb-0.44.6/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-03-15 08:56:55.836438 lndb-0.44.6/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-20 10:25:09.955595 lndb-0.44.6/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-23 05:23:25.735656 lndb-0.44.6/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-24 09:27:00.951105 lndb-0.44.6/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-03-15 08:56:55.836803 lndb-0.44.6/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-10 14:26:28.786692 lndb-0.44.6/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-10 14:26:28.786816 lndb-0.44.6/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-03-15 08:56:55.837137 lndb-0.44.6/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-04-27 10:15:48.141161 lndb-0.44.6/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-10 14:26:28.787063 lndb-0.44.6/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-03-15 08:56:55.837581 lndb-0.44.6/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-03-15 08:56:55.837695 lndb-0.44.6/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 14:26:28.787186 lndb-0.44.6/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-27 10:15:48.141448 lndb-0.44.6/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 14:26:28.787386 lndb-0.44.6/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-15 08:56:55.838152 lndb-0.44.6/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:24:58.325988 lndb-0.44.6/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.6/PKG-INFO
```

### Comparing `lndb-0.44.5/.github/workflows/build.yml` & `lndb-0.44.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/.github/workflows/latest-changes.yml` & `lndb-0.44.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/.gitignore` & `lndb-0.44.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/.pre-commit-config.yaml` & `lndb-0.44.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/LICENSE` & `lndb-0.44.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/changelog.md` & `lndb-0.44.6/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚑 Fix load | [372](https://github.com/laminlabs/lndb/pull/372) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-27 | 0.44.6
+✨ Add `--storage` arg to `lamin load` | [370](https://github.com/laminlabs/lndb/pull/370) | [falexwolf](https://github.com/falexwolf) | 2023-04-27 |
 ⬆️ Upgrade lnhub-rest | [369](https://github.com/laminlabs/lndb/pull/369) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.44.5
 ✨ Allow to set additional fsspec kwargs for cloud instances | [366](https://github.com/laminlabs/lndb/pull/366) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 | 0.44.4
 ⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
 🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
 🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
```

### Comparing `lndb-0.44.5/docs/faq/check-synchronization.ipynb` & `lndb-0.44.6/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/faq/clone.ipynb` & `lndb-0.44.6/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.44.6/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/faq/manage-migrations.ipynb` & `lndb-0.44.6/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/faq/switch-environment.ipynb` & `lndb-0.44.6/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.44.6/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/faq/test-migrations-unit.ipynb` & `lndb-0.44.6/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/guide/01-setup-user.ipynb` & `lndb-0.44.6/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/guide/02-init-instance.ipynb` & `lndb-0.44.6/docs/guide/02-init-instance.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9696137338538654%*

 * *Differences: {"'cells'": '{2: {\'source\': [\'We already set up a user account for "testuser1@lamin.ai" and '*

 * *            "chose handle `testuser1`.']}, 4: {'source': ['## Local database & storage']}, 6: "*

 * *            '{\'source\': [\'ln.setup.init(storage="./mydata")  # CLI: lamin init --storage '*

 * *            "./mydata']}, 7: {delete: ['attachments']}, 9: {'source': {insert: [(3, 'assert "*

 * *            'ln.setup.settings.storage.root.as_posix() == '*

 * *            'Path("mydata").resolve().as_posix()\\n\'), (4, \'assert '*

 * * […]*

```diff
@@ -20,15 +20,15 @@
                 "from pathlib import Path"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Assume we already setup a user account for \"testuser1@lamin.ai\" and chose handle `testuser1`."
+                "We already set up a user account for \"testuser1@lamin.ai\" and chose handle `testuser1`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -36,45 +36,34 @@
                 "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Init a local instance"
+                "## Local database & storage"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### SQLite"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "!lamin init --storage ./mydata\n",
-                "```"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"./mydata\")"
+                "ln.setup.init(storage=\"./mydata\")  # CLI: lamin init --storage ./mydata"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This automatically assigns an instance name that equals the name of the storage root along with a few other settings:"
             ]
         },
         {
@@ -95,19 +84,30 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "assert ln.setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.name == \"mydata\"\n",
+                "assert ln.setup.settings.storage.root.as_posix() == Path(\"mydata\").resolve().as_posix()\n",
+                "assert ln.setup.settings.storage.cache_dir is None\n",
                 "assert (\n",
-                "    ln.setup.settings.instance.storage.root.as_posix()\n",
-                "    == Path(\"mydata\").absolute().as_posix()\n",
-                ")\n",
-                "assert ln.setup.settings.instance.storage.cache_dir is None"
+                "    ln.setup.settings.instance.db\n",
+                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/mydata.lndb\"\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "If you want to register it on the hub at lamin.ai, call:\n",
+                "```\n",
+                "ln.setup.register()\n",
+                "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Postgres"
@@ -126,15 +126,15 @@
                 "pgurl = setup_local_test_postgres()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The connection string for postgres looks like this (we created it above):"
+                "A connection string for postgres looks like this:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -173,75 +173,56 @@
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.dialect == \"postgresql\"\n",
                 "assert ln.setup.settings.instance.db == pgurl\n",
                 "assert (\n",
                 "    ln.setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"mydatapg\").absolute().as_posix()\n",
                 ")\n",
-                "assert ln.setup.settings.instance.storage.cache_dir is None"
+                "assert ln.setup.settings.instance.storage.cache_dir is None\n",
+                "\n",
+                "!lamin delete pgtest\n",
+                "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "!lamin delete pgtest\n",
-                "!docker stop pgtest && docker rm pgtest"
+                "### Custom instance name"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Provide a custom instance name"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": [
                 "pgurl = setup_local_test_postgres()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Instead of having the instance name be auto-determined from storage or database, you can provide a custom name for the instance:\n",
-                "```\n",
-                "!lamin init --storage mystorage --name \"mydata\" --db $PGURL\n",
-                "```"
+                "Instead of having the instance name be auto-determined from `storage` or `db`, you can provide a custom name:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"mystorage\", name=\"mydata2\", db=pgurl)"
+                "ln.setup.init(\n",
+                "    storage=\"./mystorage\", name=\"mydata2\", db=pgurl\n",
+                ")  # CLI: lamin init --storage ./mystorage --name \"mydata\" --db {pgurl}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -279,18 +260,15 @@
                 "### AWS"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You need to have access to AWS S3 via `awscli configure`.\n",
-                "```\n",
-                "!lamin init --storage \"s3://lndb-setup-ci\"\n",
-                "```"
+                "You need to have access to AWS S3 via `awscli configure`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let us look at the special case of an sqlite instance:"
@@ -298,15 +276,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"s3://lndb-setup-ci\")"
+                "ln.setup.init(\n",
+                "    storage=\"s3://lndb-setup-ci\"\n",
+                ")  # CLI: lamin init --storage \"s3://lndb-setup-ci\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -331,39 +311,33 @@
             "source": [
                 "ln.setup.settings.instance._sqlite_file_local"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "assert ln.setup.settings.instance.storage.is_cloud == True\n",
-                "assert str(ln.setup.settings.instance.storage.root) == \"s3://lndb-setup-ci/\"\n",
-                "assert ln.setup.settings.instance.storage.region == \"us-east-1\"\n",
-                "assert (\n",
-                "    str(ln.setup.settings.instance._sqlite_file)\n",
-                "    == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
+                "# test\n",
+                "assert ln.setup.settings.storage.is_cloud == True\n",
+                "assert str(ln.setup.settings.storage.root) == \"s3://lndb-setup-ci/\"\n",
+                "assert ln.setup.settings.storage.region == \"us-east-1\"\n",
+                "assert (\n",
+                "    str(ln.setup.settings.instance._sqlite_file)\n",
+                "    == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
+                ")\n",
+                "\n",
                 "# do the same for an S3 bucket in Europe\n",
                 "ln.setup.init(storage=\"s3://lndb-setup-ci-eu-central-1\", name=\"lndb-setup-ci-europe\")\n",
-                "assert ln.setup.settings.instance.storage.region == \"eu-central-1\"\n",
+                "assert ln.setup.settings.storage.region == \"eu-central-1\"\n",
                 "assert ln.setup.settings.instance.name == \"lndb-setup-ci-europe\"\n",
                 "assert (\n",
                 "    str(ln.setup.settings.instance._sqlite_file)\n",
                 "    == \"s3://lndb-setup-ci-eu-central-1/lndb-setup-ci-europe.lndb\"\n",
                 ")\n",
                 "ln.setup.delete(\"lndb-setup-ci-europe\")"
             ]
@@ -404,62 +378,30 @@
             },
             "outputs": [],
             "source": [
                 "ln.setup.delete(\"lndb-setup-ci-us\")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Register a local instance on the hub"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pgurl = setup_local_test_postgres(name=\"pgtest-registered\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "!lamin init --storage ./mydatapg --name pgtest-registered --hub\n",
-                "```"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.init(storage=\"s3://lndb-setup-ci\", db=pgurl)"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# this should move up in this guide\n",
+                "pgurl = setup_local_test_postgres(name=\"pgtest-registered\")\n",
+                "ln.setup.init(storage=\"s3://lndb-setup-ci\", db=pgurl)\n",
                 "ln.setup.register()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Re-initializing an existing instance"
+                "## Re-initialize an existing instance"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Assume we accidentally `init` an existing instance, it will be loaded:"
@@ -471,24 +413,21 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert ln.setup.init(storage=\"mydata\") == \"migrate-unnecessary\""
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "For now, only assert the type."
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "assert type(ln.setup.settings.storage.id)"
             ]
         }
     ],
     "metadata": {
```

### Comparing `lndb-0.44.5/docs/guide/03-load-instance.ipynb` & `lndb-0.44.6/docs/guide/03-load-instance.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9873748110355254%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'from pathlib import Path\\n'), (1, 'import "*

 * *            "pytest\\n')], delete: [1]}}, 5: {'cell_type': 'code', 'id': 'e7ecc665', 'source': "*

 * *            '[\'ln.setup.load("mydata")  # CLI: lamin load mydata\'], \'execution_count\': None, '*

 * *            "'outputs': []}, 6: {'id': '2276e0be', 'metadata': {replace: OrderedDict([('tags', "*

 * *            "['hide-cell'])])}, 'source': ['assert settings.instance.storage.is_cloud == "*

 * *            'False\\n\', \'assert settin […]*

```diff
@@ -9,20 +9,31 @@
             "source": [
                 "# Load & close an instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "5fd65a65-5c34-462e-a980-a5aed1a2713f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "!lamin close"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
+                "from pathlib import Path\n",
+                "import pytest\n",
                 "import lamindb as ln\n",
-                "import os\n",
                 "from lamindb.setup import settings\n",
                 "from lndb.dev._settings_store import instance_settings_file"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1be836bb",
@@ -36,31 +47,21 @@
             "id": "a5c94e19",
             "metadata": {},
             "source": [
                 "If the user is the instance owner, just load the instance by name:"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "e292c512",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "!lamin load mydata\n",
-                "```"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "id": "e7ecc665",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.load(\"mydata\")"
+                "ln.setup.load(\"mydata\")  # CLI: lamin load mydata"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2276e0be",
             "metadata": {
@@ -68,17 +69,48 @@
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "assert settings.instance.storage.is_cloud == False\n",
                 "assert settings.instance.name == \"mydata\"\n",
-                "assert settings.instance.storage.root.as_posix() == f\"{os.getcwd()}/mydata\"\n",
+                "assert (\n",
+                "    settings.instance.storage.root.as_posix() == Path(\"./mydata\").resolve().as_posix()\n",
+                ")\n",
+                "assert settings.instance.storage.cache_dir is None\n",
+                "assert (\n",
+                "    settings.instance.db\n",
+                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/mydata.lndb\"\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ac0d2b30",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# assume we move the storage location\n",
+                "!mv mydata mydata_new_loc\n",
+                "with pytest.raises(\n",
+                "    RuntimeError\n",
+                "):  # triggers because it does not find the SQLite file anymore\n",
+                "    ln.setup.load(\"mydata\")\n",
+                "# now account for the new storage location\n",
+                "ln.setup.load(\"mydata\", storage=\"./mydata_new_loc\")\n",
+                "assert (\n",
+                "    settings.instance.storage.root.as_posix()\n",
+                "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
+                ")\n",
                 "assert settings.instance.storage.cache_dir is None\n",
-                "assert settings.instance.db == f\"sqlite:///{os.getcwd()}/mydata/mydata.lndb\""
+                "assert (\n",
+                "    settings.instance.db\n",
+                "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/mydata.lndb\"\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4f179b5b",
             "metadata": {
```

### Comparing `lndb-0.44.5/docs/guide/04-set-storage.ipynb` & `lndb-0.44.6/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/guide/05-schema-modules.ipynb` & `lndb-0.44.6/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/guide/06-info.ipynb` & `lndb-0.44.6/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/guide/07-delete.ipynb` & `lndb-0.44.6/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/docs/guide/migrate.md` & `lndb-0.44.6/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/__init__.py` & `lndb-0.44.6/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.44.5"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.6"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.44.5/lndb/__main__.py` & `lndb-0.44.6/lndb/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .dev._settings_user import user_description as user
 
 signup_help = "First time sign up."
 login_help = "Log in an already-signed-up user."
 init_help = "Init & config instance with db & storage."
 load_help = "Load instance by name."
 set_storage_help = "Set storage used by an instance."
+load_storage_help = "Load the instance with an updated default storage."
 info_help = "Show current instance information."
 close_help = "Close instance."
 migr_help = "Manage migrations."
 delete_help = "Delete an instance."
 register_help = (
     "Register instance on hub (local instances are not automatically registered)."
 )
@@ -39,36 +40,37 @@
 aa = login.add_argument
 aa(
     "user",
     type=str,
     metavar="user",
     help="Email or user handle. Email is needed at first login.",
 )  # noqa
-aa("--password", type=str, metavar="s", default=None, help=user.password)
+aa("--password", type=str, metavar="pw", default=None, help=user.password)
 
 # init instance
 init = subparsers.add_parser("init", help=init_help)
 aa = init.add_argument
 aa("--storage", type=str, metavar="s", help=instance.storage_root)
-aa("--db", type=str, metavar="s", default=None, help=instance.db)
-aa("--schema", type=str, metavar="s", default=None, help=instance.schema)
-aa("--name", type=str, metavar="s", default=None, help=instance.name)
+aa("--db", type=str, metavar="d", default=None, help=instance.db)
+aa("--schema", type=str, metavar="schema", default=None, help=instance.schema)
+aa("--name", type=str, metavar="n", default=None, help=instance.name)
 
 # load instance
 load = subparsers.add_parser("load", help=load_help)
 aa = load.add_argument
 instance_help = """
 The instance identifier can the instance name (owner is
 current user), handle/name, or the URL: https://lamin.ai/handle/name."""
-aa("instance", type=str, metavar="s", default=None, help=instance_help)
+aa("instance", type=str, metavar="i", default=None, help=instance_help)
+aa("--storage", type=str, metavar="s", default=None, help=load_storage_help)
 
 # delete instance
 delete_parser = subparsers.add_parser("delete", help=delete_help)
 aa = delete_parser.add_argument
-aa("instance", type=str, metavar="s", default=None, help=instance.name)
+aa("instance", type=str, metavar="i", default=None, help=instance.name)
 
 # show instance info
 info_parser = subparsers.add_parser("info", help=info_help)
 
 # set storage
 set_storage_parser = subparsers.add_parser("set", help=set_storage_help)
 aa = set_storage_parser.add_argument
@@ -113,14 +115,15 @@
             schema=args.schema,
             name=args.name,
         )
         return process_result(result)
     elif args.command == "load":
         result = _init_instance.load(
             identifier=args.instance,
+            storage=args.storage,
         )
         return process_result(result)
     elif args.command == "close":
         return close_instance()
     elif args.command == "register":
         return register()
     elif args.command == "delete":
```

### Comparing `lndb-0.44.5/lndb/_check_instance_setup.py` & `lndb-0.44.6/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_close.py` & `lndb-0.44.6/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_delete.py` & `lndb-0.44.6/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_init_instance.py` & `lndb-0.44.6/lndb/_init_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import importlib
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
 from lnhub_rest.core.instance._init_instance import init_instance as init_instance_hub
-from lnhub_rest.core.instance._init_instance import (
-    validate_db_arg,
-    validate_schema_arg,
-    validate_storage_arg,
+from lnhub_rest.core.instance._init_instance import validate_db_arg, validate_schema_arg
+from lnhub_rest.core.storage._add_storage import (
+    get_storage_region,
+    validate_storage_root_arg,
 )
-from lnhub_rest.core.storage._add_storage import get_storage_region
 from pydantic import PostgresDsn
 
 from lndb.dev.upath import UPath
 
 from ._load_instance import load, load_from_isettings
 from ._settings import settings
 from .dev import InstanceSettings
@@ -88,15 +87,15 @@
         db: {}
         schema: {}
     """
     assert settings.user.id  # check user is logged in
     owner = settings.user.handle
 
     schema = validate_schema_arg(schema)
-    validate_storage_arg(str(storage))  # needs improvement!
+    validate_storage_root_arg(str(storage))
     validate_db_arg(db)
 
     name_str = infer_instance_name(storage=storage, name=name, db=db)
     # test whether instance exists by trying to load it
     message = load(f"{owner}/{name_str}", _log_error_message=False, migrate=_migrate)
     if message != "instance-not-reachable":
         return message
```

### Comparing `lndb-0.44.5/lndb/_load_instance.py` & `lndb-0.44.6/lndb/_load_instance.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 import os
-from typing import Optional
+from pathlib import Path
+from typing import Optional, Union
 
+import sqlmodel as sqm
 from lamin_logger import logger
 from lnhub_rest.core.instance._load_instance import (
     load_instance as load_instance_from_hub,
 )
 
+from lndb.dev.upath import UPath
+
 from ._settings import InstanceSettings, settings
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
+from .dev._storage import StorageSettings
 
 
 def load(
     identifier: str,
     *,
     migrate: Optional[bool] = None,
+    storage: Optional[Union[str, Path, UPath]] = None,
     _log_error_message: bool = True,
     _access_token: Optional[str] = None,
 ) -> Optional[str]:
     """Load existing instance.
 
     Args:
-        identifier: The instance identifier can the instance name (owner is
+        identifier: `str` - The instance identifier can the instance name (owner is
             current user), handle/name, or the URL: https://lamin.ai/handle/name.
-        migrate: Whether to auto-migrate or not.
+        storage: `Optional[PathLike] = None` - Load the instance with an
+            updated default storage.
+        migrate: `Optional[bool] = None` - Whether to auto-migrate or not.
 
     Returns:
-        - migrate-failed if migration failed
-        - migrate-success if migration was successful
-        - migrate-unnecessary if migration was not required
+        - "migrate-failed" if migration failed
+        - "migrate-success" if migration was successful
+        - "migrate-unnecessary" if migration was not required
     """
     owner, name = get_owner_name_from_identifier(identifier)
 
     hub_result = load_instance_from_hub(
         owner=owner, name=name, _access_token=_access_token
     )
     # if hub_result is not a string, it means it made a request
     # that successfully returned metadata
     if not isinstance(hub_result, str):
-        instance, storage = hub_result
+        instance_result, storage_result = hub_result
         isettings = InstanceSettings(
             owner=owner,
             name=name,
-            storage_root=storage.root,
-            storage_region=storage.region,
-            db=instance.db,
-            schema=instance.schema_str,
+            storage_root=storage_result.root,
+            storage_region=storage_result.region,
+            db=instance_result.db,
+            schema=instance_result.schema_str,
         )
     else:
         settings_file = instance_settings_file(name, owner)
         if settings_file.exists():
             logger.info(f"Found cached instance metadata: {settings_file}")
             isettings = load_instance_settings(settings_file)
         else:
@@ -57,14 +65,23 @@
                 logger.error(
                     f"Instance {owner}/{name} neither loadable from hub nor local"
                     " cache. Check whether instance exists and you have access:"
                     f" https://lamin.ai/{owner}/{name}?tab=collaborators"
                 )
             return "instance-not-reachable"
 
+    if storage is not None:
+        update_isettings_with_storage(isettings, storage)
+
+    if not isettings.storage.root.exists():
+        raise RuntimeError(
+            f"Storage root does not exist: {isettings.storage.root}\n"
+            "Please amend by passing --storage <my-storage-root>"
+        )
+
     check, msg = isettings._is_db_setup()
     if not check:
         if _log_error_message:
             raise RuntimeError(msg)
         else:
             logger.warning(
                 "Instance metadata exists, but DB might have been corrupted or deleted."
@@ -73,14 +90,15 @@
             return "instance-not-reachable"
 
     message = load_from_isettings(isettings, migrate)
 
     if not message == "migrate-failed":
         os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
 
+    logger.success(f"Loaded instance: {isettings.owner}/{isettings.name}")
     return message
 
 
 def get_owner_name_from_identifier(identifier: str):
     if "/" in identifier:
         if identifier.startswith("https://lamin.ai/"):
             identifier = identifier.replace("https://lamin.ai/", "")
@@ -101,18 +119,63 @@
     isettings: InstanceSettings,
     migrate: Optional[bool] = None,
 ):
     from ._init_instance import persist_settings_load_schema, register, reload_lamindb
     from ._migrate import check_deploy_migration
     from .dev._setup_knowledge import load_bionty_versions
 
-    logger.info(f"Loading instance: {isettings.owner}/{isettings.name}")
     persist_settings_load_schema(isettings)
     message = check_deploy_migration(
         usettings=settings.user, isettings=isettings, attempt_deploy=migrate
     )
     if message == "migrate-failed":
         return message
     register(isettings, settings.user)
     load_bionty_versions(isettings)
     reload_lamindb()
     return message
+
+
+def update_isettings_with_storage(
+    isettings: InstanceSettings, storage: Union[str, Path, UPath]
+) -> None:
+    isettings._persist()  # this is temporary for import of lnschema_core
+    ssettings = StorageSettings(storage, instance_settings=isettings)
+    if ssettings.is_cloud:
+        try:  # triggering ssettings.id makes a lookup in the storage table
+            logger.success(f"Loaded storage: {ssettings.id} / {ssettings.root_as_str}")
+        except RuntimeError:
+            raise RuntimeError(
+                "Storage not registered!\n"
+                "Load instance without the `storage` arg and register storage root: "
+                f"`lamin set storage --storage {storage}`"
+            )
+    else:
+        # local storage
+        # assumption is you want to merely update the storage location
+        from lnschema_core import Storage
+
+        isettings._storage = ssettings  # need this here already
+        if isettings.dialect == "sqlite":
+            isettings._engine = sqm.create_engine(isettings.db)
+            with sqm.Session(isettings.engine) as session:
+                storage = session.exec(
+                    sqm.select(Storage).where(Storage.root == ssettings.root_as_str)
+                ).one_or_none()
+            if storage is None:
+                with sqm.Session(isettings.engine) as session:
+                    storage_record = session.exec(sqm.select(Storage)).one()
+                    storage_record.root = ssettings.root_as_str
+                    session.add(storage_record)
+                    session.commit()
+                    session.refresh(storage_record)
+                logger.success(
+                    f"Updated storage root {storage_record.id} to"
+                    f" {ssettings.root_as_str}"
+                )
+        else:
+            raise RuntimeError(
+                "Cannot currently not update local storage of sqlite upon load. Use"
+                " `lamin set --storage`"
+            )
+    # update isettings in place
+    isettings._storage = ssettings
```

### Comparing `lndb-0.44.5/lndb/_migrate/alembic.ini` & `lndb-0.44.6/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_migrate/core.py` & `lndb-0.44.6/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_migrate/deploy.py` & `lndb-0.44.6/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_migrate/env.py` & `lndb-0.44.6/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_migrate/utils.py` & `lndb-0.44.6/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_register_instance.py` & `lndb-0.44.6/lndb/_register_instance.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 def register():
     """Register an instance on the hub."""
     isettings = settings.instance
     result = init_instance_hub(
         owner=isettings.owner,
         name=isettings.name,
         storage=isettings.storage.root_as_str,
-        db=isettings.db,
+        db=isettings.db if isettings.dialect != "sqlite" else None,
         schema=isettings._schema_str,
     )
     if result == "instance-exists-already":
-        logger.info("Instance already registered")
+        logger.info("Instance was already registered")
     elif isinstance(result, str):
         raise RuntimeError(f"Creating instance on hub failed:\n{result}")
-    logger.success("Instance registered")
+    else:
+        logger.success(f"Instance registered: https://lamin.ai/{isettings.identifier}")
```

### Comparing `lndb-0.44.5/lndb/_schema.py` & `lndb-0.44.6/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_set.py` & `lndb-0.44.6/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_settings.py` & `lndb-0.44.6/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/_setup_user.py` & `lndb-0.44.6/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/__init__.py` & `lndb-0.44.6/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_clone.py` & `lndb-0.44.6/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_db.py` & `lndb-0.44.6/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_deprecated.py` & `lndb-0.44.6/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_exclusion.py` & `lndb-0.44.6/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_settings_instance.py` & `lndb-0.44.6/lndb/dev/_settings_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from lamin_logger import logger
 from pydantic import PostgresDsn
 from sqlalchemy.future import Engine
 
 from ._exclusion import empty_locker, get_locker
 from ._settings_save import save_instance_settings
 from ._settings_store import current_instance_settings_file, instance_settings_file
-from ._storage import Storage
+from ._storage import StorageSettings
 from .upath import UPath
 
 # leave commented out until we understand more how to deal with
 # migrations in redun
 # https://stackoverflow.com/questions/2614984/sqlite-sqlalchemy-how-to-enforce-foreign-keys
 # foreign key constraints for sqlite3
 # from sqlite3 import Connection as SQLite3Connection
@@ -40,15 +40,15 @@
         storage_root: Union[str, Path, UPath],  # storage location on cloud
         storage_region: Optional[str] = None,
         db: Optional[PostgresDsn] = None,  # DB URI
         schema: Optional[str] = None,  # comma-separated string of schema names
     ):
         self._owner: str = owner
         self._name: str = name
-        self._storage: Storage = Storage(
+        self._storage: StorageSettings = StorageSettings(
             storage_root, instance_settings=self, region=storage_region
         )
         self._db: Optional[str] = db
         self._schema_str: Optional[str] = schema
         self._engine: Engine = sqm.create_engine(self.db)
 
     def __repr__(self):
@@ -168,15 +168,15 @@
     def _cloud_sqlite_locker(self):
         if self.is_cloud_sqlite:
             return get_locker()
         else:
             return empty_locker
 
     @property
-    def storage(self) -> Storage:
+    def storage(self) -> StorageSettings:
         """Low-level access to storage location."""
         return self._storage
 
     @property
     def is_remote(self) -> bool:
         """Boolean indicating if an instance has no local component."""
         if not self.storage.is_cloud:
@@ -214,21 +214,24 @@
 
         settings._instance_settings = self
 
     def _is_db_setup(self, mute: bool = False) -> Tuple[bool, str]:
         """Is the database available and initialized as LaminDB?"""
         if not self._is_db_reachable(mute=mute):
             if self.dialect == "sqlite":
-                return False, f"SQLite file {self._sqlite_file} does not exist"
+                return (
+                    False,
+                    f"SQLite file {self._sqlite_file} does not exist! It should be in"
+                    f" the storage root: {self.storage.root}",
+                )
             else:
                 return False, f"Connection {self.db} not reachable"
-        # cannot import lnschema_core here, yet!
 
         with self.engine.connect() as conn:
-            try:
+            try:  # cannot import lnschema_core here, need to use plain SQL
                 result = conn.execute(sa.text("select * from version_yvzi")).first()
             except Exception as e:
                 return False, f"Your DB is not initialized: {e}"
             if result is None:
                 return False, "Your DB is not initialized: version_yvzi has no row"
         return True, ""
```

### Comparing `lndb-0.44.5/lndb/dev/_settings_load.py` & `lndb-0.44.6/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_settings_save.py` & `lndb-0.44.6/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_settings_store.py` & `lndb-0.44.6/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_settings_user.py` & `lndb-0.44.6/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_setup_knowledge.py` & `lndb-0.44.6/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_setup_schema.py` & `lndb-0.44.6/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/_storage.py` & `lndb-0.44.6/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/dev/upath.py` & `lndb-0.44.6/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/lndb/test/_migrations_e2e.py` & `lndb-0.44.6/lndb/test/_migrations_e2e.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from subprocess import run
 from typing import Optional
 
 from lamin_logger import logger
 from lnhub_rest._assets import instances as test_instances
-from lnhub_rest.core.instance._init_instance import (
-    validate_db_arg,
-    validate_schema_arg,
-    validate_storage_arg,
-)
+from lnhub_rest.core.instance._init_instance import validate_db_arg, validate_schema_arg
+from lnhub_rest.core.storage._add_storage import validate_storage_root_arg
 
 from lndb._init_instance import infer_instance_name, init
 from lndb._settings import settings
 from lndb.dev import setup_local_test_sqlite_file
 from lndb.dev._clone import clone_test
 from lndb.dev._settings_instance import InstanceSettings
 
@@ -70,15 +67,15 @@
         storage: Storage (for SQLite instances).
         name: Instance name.
         schema: The schema string.
         n_rows: Number of rows per table to clone.
         kill_docker: Kill the docker container.
     """
     schema = validate_schema_arg(schema)
-    validate_storage_arg(str(storage))  # needs improvement!
+    validate_storage_root_arg(str(storage))  # needs improvement!
     validate_db_arg(db)
     logger.info(f"Will attempt to migrate these schemas beyond core: {schema}")
     name_str = infer_instance_name(storage=storage, name=name, db=db)
     # get settings, but not from load, as we don't want to trigger loading the instance
     src_settings = InstanceSettings(
         storage_root=storage if storage is not None else "pgtest",
         db=db,
```

### Comparing `lndb-0.44.5/lndb/test/_migrations_unit.py` & `lndb-0.44.6/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/noxfile.py` & `lndb-0.44.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/pyproject.toml` & `lndb-0.44.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.2",
+    "lnhub_rest==0.9.3",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.28.0",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
```

### Comparing `lndb-0.44.5/tests/test_bionty.py` & `lndb-0.44.6/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/tests/test_init_instance.py` & `lndb-0.44.6/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.5/PKG-INFO` & `lndb-0.44.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.44.5
+Version: 0.44.6
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.9.2
+Requires-Dist: lnhub_rest==0.9.3
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
 Requires-Dist: cloudpathlib
 Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
```

