# Comparing `tmp/lnhub_rest-0.9.2.tar.gz` & `tmp/lnhub_rest-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.9.2.tar", last modified: Tue Apr 25 12:03:01 2023, max compression
+gzip compressed data, was "lnhub_rest-0.9.3.tar", last modified: Thu Apr 27 04:23:40 2023, max compression
```

## Comparing `lnhub_rest-0.9.2.tar` & `lnhub_rest-0.9.3.tar`

### file list

```diff
@@ -1,123 +1,201 @@
--rw-r--r--   0        0        0     1259 2023-04-21 01:42:24.519599 lnhub_rest-0.9.2/.dockerignore
--rw-r--r--   0        0        0     3274 2023-04-25 10:03:44.980051 lnhub_rest-0.9.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     5044 2023-04-24 14:19:00.543169 lnhub_rest-0.9.2/.github/workflows/google-cloudrun-docker-prod.yml
--rw-r--r--   0        0        0     5050 2023-04-24 14:19:00.543667 lnhub_rest-0.9.2/.github/workflows/google-cloudrun-docker-staging.yml
--rw-r--r--   0        0        0      133 2023-04-21 01:42:24.520239 lnhub_rest-0.9.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-04-21 01:42:24.520334 lnhub_rest-0.9.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1212 2023-04-21 01:42:24.520401 lnhub_rest-0.9.2/.gitignore
--rw-r--r--   0        0        0       73 2023-04-21 01:42:24.520472 lnhub_rest-0.9.2/.gitmodules
--rw-r--r--   0        0        0     1772 2023-04-21 01:42:24.520543 lnhub_rest-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-04-21 01:42:24.520628 lnhub_rest-0.9.2/Dockerfile
--rw-r--r--   0        0        0     2442 2023-04-25 10:03:44.980353 lnhub_rest-0.9.2/README.md
--rw-r--r--   0        0        0     1680 2023-04-25 10:03:44.980643 lnhub_rest-0.9.2/docs/00-migrate.ipynb
--rw-r--r--   0        0        0     1189 2023-04-21 01:42:24.520930 lnhub_rest-0.9.2/docs/01-checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0     4487 2023-04-21 01:42:24.521176 lnhub_rest-0.9.2/docs/02-account/02-create-account.ipynb
--rw-r--r--   0        0        0     5566 2023-04-21 01:42:24.521235 lnhub_rest-0.9.2/docs/02-account/03-update-account.ipynb
--rw-r--r--   0        0        0     6111 2023-04-24 13:04:10.866202 lnhub_rest-0.9.2/docs/02-account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9088 2023-04-21 01:42:24.521405 lnhub_rest-0.9.2/docs/02-account/05-rls.ipynb
--rw-r--r--   0        0        0    11211 2023-04-21 01:42:24.521521 lnhub_rest-0.9.2/docs/03-instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5293 2023-04-23 13:16:18.288701 lnhub_rest-0.9.2/docs/03-instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6498 2023-04-24 13:04:10.866445 lnhub_rest-0.9.2/docs/03-instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     8667 2023-04-23 13:16:18.289081 lnhub_rest-0.9.2/docs/03-instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     7001 2023-04-21 01:42:24.521829 lnhub_rest-0.9.2/docs/03-instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19423 2023-04-21 01:42:24.521892 lnhub_rest-0.9.2/docs/03-instance/06-rls.ipynb
--rw-r--r--   0        0        0     3870 2023-04-21 01:42:24.521998 lnhub_rest-0.9.2/docs/04-storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9837 2023-04-21 01:42:24.522057 lnhub_rest-0.9.2/docs/04-storage/02-rls.ipynb
--rw-r--r--   0        0        0     3894 2023-04-21 01:42:24.522164 lnhub_rest-0.9.2/docs/05-organization/01-create-organization.ipynb
--rw-r--r--   0        0        0     4749 2023-04-24 13:04:10.866810 lnhub_rest-0.9.2/docs/05-organization/02-manage-members.ipynb
--rw-r--r--   0        0        0     5892 2023-04-21 01:42:24.522293 lnhub_rest-0.9.2/docs/05-organization/03-rls.ipynb
--rw-r--r--   0        0        0     5310 2023-04-25 10:03:44.980748 lnhub_rest-0.9.2/docs/06-integration/01-signup-signin.ipynb
--rw-r--r--   0        0        0      125 2023-04-21 01:42:24.522348 lnhub_rest-0.9.2/docs/README.md
--rw-r--r--   0        0        0    23525 2023-04-25 12:02:44.399723 lnhub_rest-0.9.2/docs/changelog.md
--rw-r--r--   0        0        0      520 2023-04-21 01:42:24.522540 lnhub_rest-0.9.2/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-04-21 01:42:24.522624 lnhub_rest-0.9.2/docs/notes/index.md
--rw-r--r--   0        0        0    26418 2023-04-21 01:42:24.522736 lnhub_rest-0.9.2/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0      137 2023-04-21 01:42:24.522803 lnhub_rest-0.9.2/lamin-project.yaml
-drwxr-xr-x   0        0        0        0 2023-04-21 01:42:24.522825 lnhub_rest-0.9.2/lndb/
--rw-r--r--   0        0        0      157 2023-04-25 12:02:44.399839 lnhub_rest-0.9.2/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     7054 2023-04-25 10:03:44.981726 lnhub_rest-0.9.2/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       64 2023-04-21 01:42:24.523094 lnhub_rest-0.9.2/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0     1026 2023-04-21 01:42:24.523153 lnhub_rest-0.9.2/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1094 2023-04-22 05:34:46.604175 lnhub_rest-0.9.2/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1722 2023-04-21 01:42:24.523279 lnhub_rest-0.9.2/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0     1260 2023-04-25 10:03:44.982321 lnhub_rest-0.9.2/lnhub_rest/_ci.py
--rw-r--r--   0        0        0     5726 2023-04-21 01:42:24.523408 lnhub_rest-0.9.2/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0     1620 2023-04-25 10:03:44.982735 lnhub_rest-0.9.2/lnhub_rest/config.py
--rw-r--r--   0        0        0       42 2023-04-21 01:42:24.523491 lnhub_rest-0.9.2/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      285 2023-04-21 01:42:24.523581 lnhub_rest-0.9.2/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     2542 2023-04-21 01:42:24.523640 lnhub_rest-0.9.2/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-04-21 01:42:24.523697 lnhub_rest-0.9.2/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      739 2023-04-21 01:42:24.523756 lnhub_rest-0.9.2/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3325 2023-04-21 01:42:24.523826 lnhub_rest-0.9.2/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1423 2023-04-21 01:42:24.523885 lnhub_rest-0.9.2/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-04-21 01:42:24.523968 lnhub_rest-0.9.2/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     3056 2023-04-24 13:04:10.868306 lnhub_rest-0.9.2/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-04-21 01:42:24.524108 lnhub_rest-0.9.2/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-21 01:42:24.524172 lnhub_rest-0.9.2/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1284 2023-04-21 01:42:24.524255 lnhub_rest-0.9.2/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6751 2023-04-22 05:34:46.604597 lnhub_rest-0.9.2/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1532 2023-04-21 01:42:24.524381 lnhub_rest-0.9.2/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1067 2023-04-21 01:42:24.524440 lnhub_rest-0.9.2/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       32 2023-04-21 01:42:24.524537 lnhub_rest-0.9.2/lnhub_rest/core/member/__init__.py
--rw-r--r--   0        0        0     2078 2023-04-21 01:42:24.524605 lnhub_rest-0.9.2/lnhub_rest/core/member/_crud.py
--rw-r--r--   0        0        0       80 2023-04-21 01:42:24.524878 lnhub_rest-0.9.2/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     2861 2023-04-21 01:42:24.524964 lnhub_rest-0.9.2/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-04-21 01:42:24.525036 lnhub_rest-0.9.2/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      796 2023-04-25 10:03:44.982856 lnhub_rest-0.9.2/lnhub_rest/main.py
--rw-r--r--   0        0        0       39 2023-04-21 01:42:24.525187 lnhub_rest-0.9.2/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      199 2023-04-25 10:03:44.982972 lnhub_rest-0.9.2/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     1968 2023-04-25 10:03:44.983078 lnhub_rest-0.9.2/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      198 2023-04-21 01:42:24.525421 lnhub_rest-0.9.2/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     4661 2023-04-24 13:04:10.868534 lnhub_rest-0.9.2/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-04-21 01:42:24.525553 lnhub_rest-0.9.2/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0      791 2023-04-25 11:58:18.953834 lnhub_rest-0.9.2/lnhub_rest/routers/collaborator.py
--rw-r--r--   0        0        0      408 2023-04-21 01:42:24.525616 lnhub_rest-0.9.2/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     5233 2023-04-24 13:04:10.868748 lnhub_rest-0.9.2/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     2617 2023-04-21 01:42:24.525777 lnhub_rest-0.9.2/lnhub_rest/routers/organization.py
--rw-r--r--   0        0        0     1074 2023-04-21 01:42:24.525865 lnhub_rest-0.9.2/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      249 2023-04-21 01:42:24.525973 lnhub_rest-0.9.2/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     4986 2023-04-21 01:42:24.526054 lnhub_rest-0.9.2/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-04-21 01:42:24.526129 lnhub_rest-0.9.2/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      262 2023-04-21 01:42:24.526196 lnhub_rest-0.9.2/lnhub_rest/schema/_type.py
--rw-r--r--   0        0        0      252 2023-04-21 01:42:24.526266 lnhub_rest-0.9.2/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-04-21 01:42:24.526334 lnhub_rest-0.9.2/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-04-21 01:42:24.526396 lnhub_rest-0.9.2/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       40 2023-04-25 10:03:44.983212 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-21 01:42:24.526564 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/clone.py
--rw-r--r--   0        0        0     3033 2023-04-25 10:03:44.983454 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-04-21 01:42:24.527088 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0     1319 2023-04-21 01:42:24.527185 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1667 2023-04-21 01:42:24.527276 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0       39 2023-04-21 01:42:24.527356 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-04-21 01:42:24.527507 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-04-21 01:42:24.527601 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      214 2023-04-21 01:42:24.527688 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0      192 2023-04-21 01:42:24.527766 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
--rw-r--r--   0        0        0     7619 2023-04-21 01:42:24.527838 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1408 2023-04-21 01:42:24.527910 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0      880 2023-04-21 01:42:24.527983 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
--rw-r--r--   0        0        0       33 2023-04-21 01:42:24.528050 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-04-21 01:42:24.528131 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0     5258 2023-04-25 10:03:44.983595 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/testing.py
--rw-r--r--   0        0        0     9882 2023-04-21 01:42:24.528495 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-04-21 01:42:24.528568 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-04-21 01:42:24.528650 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-04-21 01:42:24.528720 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      542 2023-04-21 01:42:24.528778 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0     1199 2023-04-21 01:42:24.528837 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
--rw-r--r--   0        0        0      733 2023-04-21 01:42:24.528898 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
--rw-r--r--   0        0        0     5143 2023-04-21 01:42:24.528990 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
--rw-r--r--   0        0        0      593 2023-04-21 01:42:24.529057 lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
--rw-r--r--   0        0        0       60 2023-04-21 01:42:24.529115 lnhub_rest-0.9.2/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0       13 2023-04-21 01:42:24.529203 lnhub_rest-0.9.2/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-04-21 01:42:24.529270 lnhub_rest-0.9.2/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      352 2023-04-21 01:42:24.529325 lnhub_rest-0.9.2/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-04-21 01:42:24.529386 lnhub_rest-0.9.2/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3820 2023-04-21 01:42:24.529455 lnhub_rest-0.9.2/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1714 2023-04-25 10:03:44.984104 lnhub_rest-0.9.2/noxfile.py
--rw-r--r--   0        0        0     1368 2023-04-25 10:03:44.984473 lnhub_rest-0.9.2/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-04-21 01:42:24.529709 lnhub_rest-0.9.2/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-04-21 01:42:24.529811 lnhub_rest-0.9.2/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-04-21 01:42:24.529893 lnhub_rest-0.9.2/supabase/config.toml
--rw-r--r--   0        0        0     1212 2023-04-25 10:03:44.984830 lnhub_rest-0.9.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 lnhub_rest-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.9.3/.dockerignore
+-rw-r--r--   0        0        0     3274 2023-04-25 15:29:32.846604 lnhub_rest-0.9.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5044 2023-04-25 15:29:32.846743 lnhub_rest-0.9.3/.github/workflows/google-cloudrun-docker-prod.yml
+-rw-r--r--   0        0        0     5050 2023-04-25 15:29:32.846865 lnhub_rest-0.9.3/.github/workflows/google-cloudrun-docker-staging.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.9.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.9.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.9.3/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.9.3/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.9.3/Dockerfile
+-rw-r--r--   0        0        0     2442 2023-04-25 15:29:32.847024 lnhub_rest-0.9.3/README.md
+-rw-r--r--   0        0        0     1680 2023-04-27 03:39:31.402324 lnhub_rest-0.9.3/docs/00-migrate.ipynb
+-rw-r--r--   0        0        0     1189 2023-04-27 03:39:31.402860 lnhub_rest-0.9.3/docs/01-checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0     4487 2023-04-27 03:39:31.414955 lnhub_rest-0.9.3/docs/02-account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5566 2023-04-27 03:39:31.419067 lnhub_rest-0.9.3/docs/02-account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6111 2023-04-27 03:39:31.418992 lnhub_rest-0.9.3/docs/02-account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9088 2023-04-27 03:39:31.419398 lnhub_rest-0.9.3/docs/02-account/05-rls.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-27 04:21:53.504972 lnhub_rest-0.9.3/docs/03-instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5293 2023-04-27 03:39:31.415575 lnhub_rest-0.9.3/docs/03-instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6498 2023-04-27 03:39:31.417147 lnhub_rest-0.9.3/docs/03-instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8667 2023-04-27 03:39:31.417306 lnhub_rest-0.9.3/docs/03-instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     7001 2023-04-27 03:39:31.420904 lnhub_rest-0.9.3/docs/03-instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19423 2023-04-27 03:39:31.401299 lnhub_rest-0.9.3/docs/03-instance/06-rls.ipynb
+-rw-r--r--   0        0        0     3990 2023-04-27 04:21:53.505189 lnhub_rest-0.9.3/docs/04-storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9837 2023-04-27 03:39:31.421340 lnhub_rest-0.9.3/docs/04-storage/02-rls.ipynb
+-rw-r--r--   0        0        0     3894 2023-04-27 03:39:31.415314 lnhub_rest-0.9.3/docs/05-organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     4749 2023-04-27 03:39:31.413247 lnhub_rest-0.9.3/docs/05-organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5892 2023-04-27 03:39:31.413014 lnhub_rest-0.9.3/docs/05-organization/03-rls.ipynb
+-rw-r--r--   0        0        0     5310 2023-04-27 03:39:31.417221 lnhub_rest-0.9.3/docs/06-integration/01-signup-signin.ipynb
+-rw-r--r--   0        0        0      125 2023-04-18 16:52:57.348114 lnhub_rest-0.9.3/docs/README.md
+-rw-r--r--   0        0        0    23668 2023-04-27 04:22:49.840295 lnhub_rest-0.9.3/docs/changelog.md
+-rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.9.3/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.9.3/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.9.3/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.9.3/lamin-project.yaml
+-rw-r--r--   0        0        0     3832 2023-04-18 16:53:14.549682 lnhub_rest-0.9.3/lndb/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.9.3/lndb/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.9.3/lndb/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.9.3/lndb/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-25 15:29:40.845175 lnhub_rest-0.9.3/lndb/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.9.3/lndb/LICENSE
+-rw-r--r--   0        0        0      173 2023-04-18 16:53:14.549987 lnhub_rest-0.9.3/lndb/README.md
+-rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.9.3/lndb/docs/api.md
+-rw-r--r--   0        0        0    47755 2023-04-27 03:47:05.803728 lnhub_rest-0.9.3/lndb/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.9.3/lndb/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.9.3/lndb/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-04-18 16:53:14.550717 lnhub_rest-0.9.3/lndb/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-04-18 16:53:14.551192 lnhub_rest-0.9.3/lndb/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-25 15:29:40.845949 lnhub_rest-0.9.3/lndb/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.9.3/lndb/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-18 16:53:14.551375 lnhub_rest-0.9.3/lndb/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-18 16:53:14.551472 lnhub_rest-0.9.3/lndb/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-18 16:53:14.551612 lnhub_rest-0.9.3/lndb/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10370 2023-04-27 04:20:38.053396 lnhub_rest-0.9.3/lndb/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-25 15:29:40.846776 lnhub_rest-0.9.3/lndb/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-25 15:29:40.846861 lnhub_rest-0.9.3/lndb/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-25 15:29:40.846961 lnhub_rest-0.9.3/lndb/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-04-18 16:53:14.552137 lnhub_rest-0.9.3/lndb/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-25 15:29:40.847226 lnhub_rest-0.9.3/lndb/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.9.3/lndb/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-25 15:29:40.847416 lnhub_rest-0.9.3/lndb/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.9.3/lndb/docs/index.md
+-rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.9.3/lndb/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-27 03:47:05.803990 lnhub_rest-0.9.3/lndb/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-25 15:29:40.847751 lnhub_rest-0.9.3/lndb/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.9.3/lndb/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-18 16:53:14.553281 lnhub_rest-0.9.3/lndb/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-25 15:29:40.847842 lnhub_rest-0.9.3/lndb/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-18 16:53:14.553610 lnhub_rest-0.9.3/lndb/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-18 16:53:14.553765 lnhub_rest-0.9.3/lndb/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-25 15:29:40.848070 lnhub_rest-0.9.3/lndb/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-04-27 03:52:24.150379 lnhub_rest-0.9.3/lndb/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6485 2023-04-27 03:49:23.883095 lnhub_rest-0.9.3/lndb/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-18 16:53:14.554421 lnhub_rest-0.9.3/lndb/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-18 16:53:14.554545 lnhub_rest-0.9.3/lndb/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-25 15:29:40.848442 lnhub_rest-0.9.3/lndb/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-25 15:29:40.848595 lnhub_rest-0.9.3/lndb/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.9.3/lndb/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-25 15:29:40.848722 lnhub_rest-0.9.3/lndb/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-18 16:53:14.554944 lnhub_rest-0.9.3/lndb/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      803 2023-04-27 04:20:38.053795 lnhub_rest-0.9.3/lndb/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.9.3/lndb/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-25 15:29:40.849016 lnhub_rest-0.9.3/lndb/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 21:34:53.593994 lnhub_rest-0.9.3/lndb/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.9.3/lndb/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.9.3/lndb/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-25 15:29:40.849262 lnhub_rest-0.9.3/lndb/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-18 16:53:14.555545 lnhub_rest-0.9.3/lndb/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-04-18 16:53:14.555802 lnhub_rest-0.9.3/lndb/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-18 16:53:14.555956 lnhub_rest-0.9.3/lndb/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.9.3/lndb/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.9.3/lndb/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-18 16:53:14.556103 lnhub_rest-0.9.3/lndb/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-04-27 03:49:23.883399 lnhub_rest-0.9.3/lndb/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-04-18 16:53:14.556382 lnhub_rest-0.9.3/lndb/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.9.3/lndb/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-18 16:53:14.556505 lnhub_rest-0.9.3/lndb/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.9.3/lndb/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-04-18 16:53:14.556633 lnhub_rest-0.9.3/lndb/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-25 15:29:40.849676 lnhub_rest-0.9.3/lndb/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-25 15:29:40.849829 lnhub_rest-0.9.3/lndb/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.9.3/lndb/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-18 16:53:14.557004 lnhub_rest-0.9.3/lndb/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-18 16:53:14.557144 lnhub_rest-0.9.3/lndb/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.9.3/lndb/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-04-27 03:52:24.153553 lnhub_rest-0.9.3/lndb/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-18 16:53:14.557417 lnhub_rest-0.9.3/lndb/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.9.3/lndb/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.9.3/lndb/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-18 16:53:14.557535 lnhub_rest-0.9.3/lndb/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-27 04:20:38.053974 lnhub_rest-0.9.3/lndb/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-18 16:53:14.557862 lnhub_rest-0.9.3/lndb/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.9.3/lndb/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:53:14.558657 lnhub_rest-0.9.3/lndb/tests/test_notebooks.py
+-rw-r--r--   0        0        0      157 2023-04-27 04:22:10.385439 lnhub_rest-0.9.3/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     7054 2023-04-25 15:29:32.854635 lnhub_rest-0.9.3/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.9.3/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0     1026 2023-01-15 12:17:52.330665 lnhub_rest-0.9.3/lnhub_rest/_assets/_instances.py
+-rw-r--r--   0        0        0     1094 2023-04-22 04:59:42.149916 lnhub_rest-0.9.3/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.9.3/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0     1260 2023-04-25 15:29:32.854787 lnhub_rest-0.9.3/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5726 2023-04-19 15:57:22.490723 lnhub_rest-0.9.3/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0     1620 2023-04-25 15:29:32.854908 lnhub_rest-0.9.3/lnhub_rest/config.py
+-rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.9.3/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.9.3/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2542 2023-04-21 10:12:34.724799 lnhub_rest-0.9.3/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.9.3/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      739 2023-04-19 15:57:22.491329 lnhub_rest-0.9.3/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3325 2023-04-19 15:57:22.491711 lnhub_rest-0.9.3/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1423 2023-04-19 15:57:22.491949 lnhub_rest-0.9.3/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.9.3/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     3056 2023-04-25 15:29:32.855696 lnhub_rest-0.9.3/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.9.3/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.9.3/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1284 2023-04-19 15:57:22.492340 lnhub_rest-0.9.3/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6096 2023-04-27 04:21:53.505412 lnhub_rest-0.9.3/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1532 2023-04-19 15:57:22.492860 lnhub_rest-0.9.3/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1067 2023-04-19 15:57:22.493104 lnhub_rest-0.9.3/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.9.3/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.9.3/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.9.3/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     3230 2023-04-27 04:21:53.505588 lnhub_rest-0.9.3/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.9.3/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      796 2023-04-25 15:29:32.855942 lnhub_rest-0.9.3/lnhub_rest/main.py
+-rw-r--r--   0        0        0       39 2023-04-19 15:57:22.493742 lnhub_rest-0.9.3/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      199 2023-04-25 15:29:32.856194 lnhub_rest-0.9.3/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     1968 2023-04-25 15:29:32.856453 lnhub_rest-0.9.3/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      198 2023-04-18 16:02:04.950703 lnhub_rest-0.9.3/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4661 2023-04-25 15:29:32.856734 lnhub_rest-0.9.3/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.9.3/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0      779 2023-04-27 04:21:53.505758 lnhub_rest-0.9.3/lnhub_rest/routers/collaborator.py
+-rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.9.3/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     5233 2023-04-25 15:29:32.856998 lnhub_rest-0.9.3/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.9.3/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1074 2023-04-19 15:57:22.494317 lnhub_rest-0.9.3/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.9.3/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.9.3/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.9.3/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.9.3/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.9.3/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.9.3/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.9.3/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       40 2023-04-25 15:29:32.857365 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     3033 2023-04-25 15:29:32.857603 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0     5258 2023-04-25 15:29:32.857771 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     9882 2023-04-18 16:52:57.349405 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-04-18 16:52:57.349781 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.9.3/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.9.3/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.9.3/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.9.3/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.9.3/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3820 2023-04-19 15:57:22.494545 lnhub_rest-0.9.3/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1714 2023-04-25 15:29:32.857902 lnhub_rest-0.9.3/noxfile.py
+-rw-r--r--   0        0        0     1368 2023-04-25 15:29:32.858048 lnhub_rest-0.9.3/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.9.3/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.9.3/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.9.3/supabase/config.toml
+-rw-r--r--   0        0        0     1212 2023-04-25 15:29:32.858221 lnhub_rest-0.9.3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 lnhub_rest-0.9.3/PKG-INFO
```

### Comparing `lnhub_rest-0.9.2/.dockerignore` & `lnhub_rest-0.9.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/.github/workflows/build.yml` & `lnhub_rest-0.9.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/.github/workflows/google-cloudrun-docker-prod.yml` & `lnhub_rest-0.9.3/.github/workflows/google-cloudrun-docker-prod.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/.github/workflows/google-cloudrun-docker-staging.yml` & `lnhub_rest-0.9.3/.github/workflows/google-cloudrun-docker-staging.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/.gitignore` & `lnhub_rest-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/.pre-commit-config.yaml` & `lnhub_rest-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/README.md` & `lnhub_rest-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/00-migrate.ipynb` & `lnhub_rest-0.9.3/docs/00-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/01-checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.9.3/docs/01-checks/01-check-break-lndb.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/02-account/02-create-account.ipynb` & `lnhub_rest-0.9.3/docs/02-account/02-create-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/02-account/03-update-account.ipynb` & `lnhub_rest-0.9.3/docs/02-account/03-update-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/02-account/04-fetch-account.ipynb` & `lnhub_rest-0.9.3/docs/02-account/04-fetch-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/02-account/05-rls.ipynb` & `lnhub_rest-0.9.3/docs/02-account/05-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/03-instance/01-init-instance.ipynb` & `lnhub_rest-0.9.3/docs/03-instance/01-init-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996646341463414%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, 'from lnhub_rest.core.storage._add_storage import "*

 * *            "validate_storage_root_arg\\n')], delete: [4]}}, 36: {'source': ['# actually happens "*

 * *            'during add_storage\\n\', \'validate_storage_root_arg("test/")\\n\', '*

 * *            '\'validate_storage_root_arg("gs://test")\\n\', '*

 * *            '\'validate_storage_root_arg("gs://test")\']}}'}*

```diff
@@ -22,16 +22,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.storage._add_storage import validate_root_arg\n",
                 "from lnhub_rest.core.instance._init_instance import (\n",
                 "    validate_db_arg,\n",
                 "    validate_schema_arg,\n",
-                "    validate_storage_arg,\n",
                 ")\n",
+                "from lnhub_rest.core.storage._add_storage import validate_storage_root_arg\n",
                 "from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth\n",
                 "from lnhub_rest.core.instance import init_instance, delete_instance\n",
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest._clean_ci import delete_ci_instances\n",
                 "import sqlmodel as sqm\n",
                 "from lnhub_rest.schema import Instance, Account, Storage\n",
                 "from lnhub_rest.main import client\n",
@@ -388,22 +388,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# test typos in schema string\n",
-                "validate_storage_arg(\"test/\")\n",
-                "# test errors during validation\n",
-                "validate_storage_arg(\"gs://test\")\n",
-                "# test errors for hub-only instances\n",
-                "validate_root_arg(\"gs://test\")\n",
-                "with pytest.raises(ValueError):\n",
-                "    validate_root_arg(\"23jf://test\")"
+                "# actually happens during add_storage\n",
+                "validate_storage_root_arg(\"test/\")\n",
+                "validate_storage_root_arg(\"gs://test\")\n",
+                "validate_storage_root_arg(\"gs://test\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `lnhub_rest-0.9.2/docs/03-instance/02-load-instance.ipynb` & `lnhub_rest-0.9.3/docs/03-instance/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/03-instance/03-update-instance.ipynb` & `lnhub_rest-0.9.3/docs/03-instance/03-update-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/03-instance/04-delete-instance.ipynb` & `lnhub_rest-0.9.3/docs/03-instance/04-delete-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/03-instance/05-fetch-instance.ipynb` & `lnhub_rest-0.9.3/docs/03-instance/05-fetch-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/03-instance/06-rls.ipynb` & `lnhub_rest-0.9.3/docs/03-instance/06-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/04-storage/01-add-storage.ipynb` & `lnhub_rest-0.9.3/docs/04-storage/01-add-storage.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'cells'": "{insert: [(1, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['Alse see validation in init_instance.'])]))]}"}*

```diff
@@ -4,14 +4,21 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Test add storage"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Alse see validation in init_instance."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest.core.storage import add_storage\n",
```

### Comparing `lnhub_rest-0.9.2/docs/04-storage/02-rls.ipynb` & `lnhub_rest-0.9.3/docs/04-storage/02-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/05-organization/01-create-organization.ipynb` & `lnhub_rest-0.9.3/docs/05-organization/01-create-organization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/05-organization/02-manage-members.ipynb` & `lnhub_rest-0.9.3/docs/05-organization/02-manage-members.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/05-organization/03-rls.ipynb` & `lnhub_rest-0.9.3/docs/05-organization/03-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/06-integration/01-signup-signin.ipynb` & `lnhub_rest-0.9.3/docs/06-integration/01-signup-signin.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/changelog.md` & `lnhub_rest-0.9.3/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-✨Add is_collaborator endpoint | [191](https://github.com/laminlabs/lnhub-rest/pull/191) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.9.2
+✨ Allow local storage locations | [194](https://github.com/laminlabs/lnhub-rest/pull/194) | [falexwolf](https://github.com/falexwolf) | 2023-04-27 | 0.9.3
+✨ Add `is_collaborator` endpoint | [191](https://github.com/laminlabs/lnhub-rest/pull/191) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.9.2
 👷 Refactor environment management  | [180](https://github.com/laminlabs/lnhub-rest/pull/180) | [lawrlee](https://github.com/lawrlee) | 2023-04-24 |
-🔖  Staging version 0.9.0 | [170](https://github.com/laminlabs/lnhub-rest/pull/170) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.9.1
+🔖 Staging version 0.9.0 | [170](https://github.com/laminlabs/lnhub-rest/pull/170) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.9.1
 🎨 Redesign acct-instances endpoint | [190](https://github.com/laminlabs/lnhub-rest/pull/190) | [bpenteado](https://github.com/bpenteado) | 2023-04-23 |
 ✨ Create add-collaborator endpoint | [189](https://github.com/laminlabs/lnhub-rest/pull/189) | [bpenteado](https://github.com/bpenteado) | 2023-04-23 |
 🎨 Enrich account organizations endpoint | [188](https://github.com/laminlabs/lnhub-rest/pull/188) | [bpenteado](https://github.com/bpenteado) | 2023-04-23 |
-🍱  Add schema module `lamin1` | [187](https://github.com/laminlabs/lnhub-rest/pull/187) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.8.2
-:children_crossing: Ask for postgresql instead of postgres | [186](https://github.com/laminlabs/lnhub-rest/pull/186) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 |
+🍱 Add schema module `lamin1` | [187](https://github.com/laminlabs/lnhub-rest/pull/187) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.8.2
+🚸 Ask for postgresql instead of postgres | [186](https://github.com/laminlabs/lnhub-rest/pull/186) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 |
 👷 Run tests on staging | [179](https://github.com/laminlabs/lnhub-rest/pull/179) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 ✅ Decouple tests from lndb-related objects | [184](https://github.com/laminlabs/lnhub-rest/pull/184) | [bpenteado](https://github.com/bpenteado) | 2023-04-20 |
 💚 Fix tests | [178](https://github.com/laminlabs/lnhub-rest/pull/178) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 🚚 Rename folders in docs | [177](https://github.com/laminlabs/lnhub-rest/pull/177) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 🏗️ Clean up historical migrations & remove cloning from production for migrations testing | [175](https://github.com/laminlabs/lnhub-rest/pull/175) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 🏗️ Fix local development setup | [174](https://github.com/laminlabs/lnhub-rest/pull/174) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 | 0.8.1
 🗃️ Fix RLS for storage table | [173](https://github.com/laminlabs/lnhub-rest/pull/173) | [fredericenard](https://github.com/fredericenard) | 2023-04-18 |
```

### Comparing `lnhub_rest-0.9.2/docs/migrations.md` & `lnhub_rest-0.9.3/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.9.3/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/__main__.py` & `lnhub_rest-0.9.3/lnhub_rest/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/_assets/_instances.py` & `lnhub_rest-0.9.3/lnhub_rest/_assets/_instances.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.9.3/lnhub_rest/_assets/_schemas.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.9.3/lnhub_rest/_check_breaks_lndb.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/_ci.py` & `lnhub_rest-0.9.3/lnhub_rest/_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.9.3/lnhub_rest/_clean_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/config.py` & `lnhub_rest-0.9.3/lnhub_rest/config.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.9.3/lnhub_rest/core/account/_create_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.9.3/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.9.3/lnhub_rest/core/account/_delete_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.9.3/lnhub_rest/core/account/_signup_signin.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.9.3/lnhub_rest/core/account/_update_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/collaborator/_crud.py` & `lnhub_rest-0.9.3/lnhub_rest/core/collaborator/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.9.3/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.9.3/lnhub_rest/core/instance/_delete_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.9.3/lnhub_rest/core/instance/_init_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Initializing an instance.
 
 This functionality will at first only be accessible through Python API client & CLI.
 
 We might also enable it from the UI.
 """
-from pathlib import Path
 from typing import Mapping, Optional
 from uuid import UUID, uuid4
 
 from postgrest.exceptions import APIError
 
 from lnhub_rest import check_breaks_lndb_and_error
 from lnhub_rest._assets import schemas as known_schema_names
@@ -39,15 +38,15 @@
     hub = connect_hub_with_auth(
         email=_email, password=_password, access_token=_access_token
     )
     check_breaks_lndb_and_error(hub)  # assumes that only called from within lndb
     try:
         # validate input arguments
         schema_str = validate_schema_arg(schema)
-        # validate_storage_arg(storage)  # needs improvement! happens in add_storage
+        # storage is validated in add_storage
         validate_db_arg(db)
 
         # get account
         account = sb_select_account_by_handle(owner, hub)
         if account is None:
             return "account-not-exists"
 
@@ -120,34 +119,14 @@
             validated_schema.append(name)
             to_be_validated.remove(name)
     if len(to_be_validated) != 0:
         raise ValueError(f"Unkown schema module name(s): {to_be_validated}")
     return ",".join(validated_schema)
 
 
-# todo: improve this function
-# also see _add_storage.validate_root_arg which errors
-# upon non gs non-s3
-def validate_storage_arg(storage: str) -> None:
-    # google cloud or AWS
-    # for instances that are stored on the hub,
-    # this is a requirement
-    if storage.startswith(("gs://", "s3://")):
-        return None
-    else:
-        try:
-            # try creating a path
-            _ = Path(storage)
-            return None
-        except Exception:
-            raise ValueError(
-                "`storage` is neither a valid local, a Google Cloud nor an S3 path."
-            )
-
-
 def validate_db_arg(db: Optional[str]) -> None:
     if db is not None:
         if db.startswith("postgres") and not db.startswith("postgresql"):
             raise ValueError(
                 "Please follow the SQLAlchemy convention of prefixing the connection"
                 " string with 'postgresql://' instead of 'postgres://'"
             )
```

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.9.3/lnhub_rest/core/instance/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.9.3/lnhub_rest/core/instance/_update_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/member/_crud.py` & `lnhub_rest-0.9.3/lnhub_rest/core/member/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.9.3/lnhub_rest/core/storage/_add_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from typing import Optional, Tuple
 from uuid import UUID, uuid4
 
 from lnhub_rest import check_breaks_lndb_and_error
 from lnhub_rest.core.storage._crud import sb_insert_storage, sb_select_storage_by_root
 from lnhub_rest.orm._sbclient import connect_hub_with_auth
 from lnhub_rest.utils._id import base62
@@ -14,15 +15,15 @@
     from botocore.exceptions import ClientError
 
     from lnhub_rest.core.account._crud import sb_select_account_by_handle
 
     hub = connect_hub_with_auth(access_token=_access_token)
     try:
         check_breaks_lndb_and_error(hub)  # assumes that only called from within lndb
-        validate_root_arg(root)
+        validate_storage_root_arg(root)
         # get account
         account = sb_select_account_by_handle(account_handle, hub)
 
         # check if storage exists already
         storage = sb_select_storage_by_root(root, hub)
         if storage is not None:
             return storage["id"], None
@@ -52,17 +53,27 @@
             return None, "bucket-does-not-exists"
         else:
             return None, exception.response["Error"]["Message"]
     finally:
         hub.auth.sign_out()
 
 
-def validate_root_arg(root: str) -> None:
-    if not root.startswith(("s3://", "gs://")):
-        raise ValueError("Only accept s3 and Google Cloud buckets.")
+def validate_storage_root_arg(storage_root: str) -> None:
+    if storage_root.endswith("/"):
+        raise ValueError("Pass settings.storage.root_as_str rather than path")
+    if storage_root.startswith(("gs://", "s3://")):
+        return None
+    else:  # local path
+        try:
+            _ = Path(storage_root)
+            return None
+        except Exception:
+            raise ValueError(
+                "`storage` is neither a valid local, a Google Cloud nor an S3 path."
+            )
 
 
 def get_storage_region(storage_root: str) -> Optional[str]:
     storage_root_str = str(storage_root)
     storage_region = None
 
     if storage_root_str.startswith("s3://"):
```

### Comparing `lnhub_rest-0.9.2/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.9.3/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/main.py` & `lnhub_rest-0.9.3/lnhub_rest/main.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.9.3/lnhub_rest/orm/_sbclient.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/routers/account.py` & `lnhub_rest-0.9.3/lnhub_rest/routers/account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/routers/ci.py` & `lnhub_rest-0.9.3/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/routers/collaborator.py` & `lnhub_rest-0.9.3/lnhub_rest/routers/collaborator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Union
 
 from fastapi import APIRouter, Header
 
 from lnhub_rest.core.collaborator._crud import sb_select_collaborator
-from .utils import (
-    extract_access_token,
-    get_supabase_client,
-)
+
+from .utils import extract_access_token, get_supabase_client
 
 router = APIRouter(prefix="/instance/collaborator")
 
 
 @router.get("/{account_handle}/{name}")
 def is_collaborator(
     instance_id: str,
```

### Comparing `lnhub_rest-0.9.2/lnhub_rest/routers/instance.py` & `lnhub_rest-0.9.3/lnhub_rest/routers/instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/routers/organization.py` & `lnhub_rest-0.9.3/lnhub_rest/routers/organization.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/routers/utils.py` & `lnhub_rest-0.9.3/lnhub_rest/routers/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/_core.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/alembic.ini` & `lnhub_rest-0.9.3/lnhub_rest/schema/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/clone.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/testing.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/testing.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py` & `lnhub_rest-0.9.3/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/lnhub_rest/utils/_test.py` & `lnhub_rest-0.9.3/lnhub_rest/utils/_test.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/noxfile.py` & `lnhub_rest-0.9.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/pyproject.toml` & `lnhub_rest-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/supabase/config.toml` & `lnhub_rest-0.9.3/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/tests/test_notebooks.py` & `lnhub_rest-0.9.3/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.2/PKG-INFO` & `lnhub_rest-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.9.2
+Version: 0.9.3
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: supabase==1.0.2
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
```

