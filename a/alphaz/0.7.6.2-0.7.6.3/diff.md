# Comparing `tmp/alphaz-0.7.6.2.tar.gz` & `tmp/alphaz-0.7.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.6.2.tar", last modified: Wed Apr 26 18:21:26 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.6.3.tar", last modified: Thu Apr 27 10:12:19 2023, max compression
```

## Comparing `alphaz-0.7.6.2.tar` & `alphaz-0.7.6.3.tar`

### file list

```diff
@@ -1,397 +1,397 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.627025 alphaz-0.7.6.2/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-04-26 18:21:26.000000 alphaz-0.7.6.2/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-26 18:21:26.627025 alphaz-0.7.6.2/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.6.2/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.563025 alphaz-0.7.6.2/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/README.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      387 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.6.2/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.6.2/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.567025 alphaz-0.7.6.2/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.6.2/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.6.2/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.567025 alphaz-0.7.6.2/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.6.2/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.6.2/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.6.2/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.6.2/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.6.2/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6407 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1532 2023-04-26 12:36:19.000000 alphaz-0.7.6.2/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.567025 alphaz-0.7.6.2/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.6.2/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.6.2/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.6.2/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.6.2/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.6.2/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3324 2023-04-21 07:47:57.000000 alphaz-0.7.6.2/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.6.2/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.567025 alphaz-0.7.6.2/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.6.2/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.6.2/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.6.2/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.571025 alphaz-0.7.6.2/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.6.2/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.6.2/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.571025 alphaz-0.7.6.2/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.571025 alphaz-0.7.6.2/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.6.2/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.6.2/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.6.2/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.6.2/alphaz/documentations/docs/alpha_setup.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.571025 alphaz-0.7.6.2/alphaz/documentations/docs/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/authorizations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/cache.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2932 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/issues.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/methods.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/parameters.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/routes.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api/sqlalchemy.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/api_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.6.2/alphaz/documentations/docs/configuration.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.571025 alphaz-0.7.6.2/alphaz/documentations/docs/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/database/init.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/database/instantiate.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/database/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/database/model.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/database/relations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/database/schema.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/docs/database/update.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.6.2/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.6.2/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.571025 alphaz-0.7.6.2/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.571025 alphaz-0.7.6.2/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.555025 alphaz-0.7.6.2/alphaz/documentations/site/api/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/authorizations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/authorizations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/cache/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/cache/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27646 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/issues/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/issues/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/methods/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/methods/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/parameters/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/parameters/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/routes/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api/sqlalchemy/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api/sqlalchemy/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/api_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/api_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.559025 alphaz-0.7.6.2/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.575025 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.579025 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.579025 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.579025 alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.579025 alphaz-0.7.6.2/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.559025 alphaz-0.7.6.2/alphaz/documentations/site/database/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.579025 alphaz-0.7.6.2/alphaz/documentations/site/database/init/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23027 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/database/init/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.579025 alphaz-0.7.6.2/alphaz/documentations/site/database/instantiate/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/database/instantiate/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.579025 alphaz-0.7.6.2/alphaz/documentations/site/database/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/database/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.583025 alphaz-0.7.6.2/alphaz/documentations/site/database/model/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/database/model/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.583025 alphaz-0.7.6.2/alphaz/documentations/site/database/relations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/database/relations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.583025 alphaz-0.7.6.2/alphaz/documentations/site/database/schema/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/database/schema/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.583025 alphaz-0.7.6.2/alphaz/documentations/site/database/update/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/database/update/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.583025 alphaz-0.7.6.2/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.583025 alphaz-0.7.6.2/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    54137 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-26 18:21:25.000000 alphaz-0.7.6.2/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.6.2/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.6.2/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.587025 alphaz-0.7.6.2/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5785 2023-04-13 20:34:53.000000 alphaz-0.7.6.2/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13999 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.6.2/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5972 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.6.2/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6324 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.587025 alphaz-0.7.6.2/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.6.2/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.6.2/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.6.2/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.6.2/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.6.2/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.6.2/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.6.2/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.6.2/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.6.2/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-04-21 07:47:57.000000 alphaz-0.7.6.2/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.6.2/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6397 2023-04-13 20:34:53.000000 alphaz-0.7.6.2/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.6.2/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18517 2023-04-21 07:47:57.000000 alphaz-0.7.6.2/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9938 2023-04-21 07:47:57.000000 alphaz-0.7.6.2/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5503 2023-04-26 12:36:19.000000 alphaz-0.7.6.2/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.6.2/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.6.2/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7724 2023-04-26 18:21:23.000000 alphaz-0.7.6.2/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.591025 alphaz-0.7.6.2/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.6.2/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.6.2/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.6.2/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.6.2/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.6.2/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.591025 alphaz-0.7.6.2/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.595025 alphaz-0.7.6.2/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.6.2/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.6.2/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.6.2/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.6.2/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.595025 alphaz-0.7.6.2/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.6.2/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.595025 alphaz-0.7.6.2/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.6.2/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      884 2023-04-12 16:11:09.000000 alphaz-0.7.6.2/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.6.2/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.6.2/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14301 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14493 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/api/_reloader.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3776 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/api/_reloaders.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.6.2/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18786 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20174 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.6.2/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.6.2/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.595025 alphaz-0.7.6.2/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    26514 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.599025 alphaz-0.7.6.2/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.6.2/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.6.2/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.6.2/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.6.2/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.6.2/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    56515 2023-04-26 18:21:23.000000 alphaz-0.7.6.2/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.6.2/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4529 2023-04-21 13:36:09.000000 alphaz-0.7.6.2/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.6.2/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.6.2/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6699 2023-04-21 07:47:57.000000 alphaz-0.7.6.2/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.6.2/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.599025 alphaz-0.7.6.2/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.6.2/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.599025 alphaz-0.7.6.2/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.6.2/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.6.2/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14115 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.599025 alphaz-0.7.6.2/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.6.2/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.6.2/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.599025 alphaz-0.7.6.2/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.6.2/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27277 2023-04-18 09:00:04.000000 alphaz-0.7.6.2/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.599025 alphaz-0.7.6.2/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15952 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.6.2/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2100 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.6.2/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8011 2023-04-26 12:36:19.000000 alphaz-0.7.6.2/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3458 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4150 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.6.2/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14819 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7413 2023-04-21 07:47:57.000000 alphaz-0.7.6.2/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.6.2/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.6.2/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.6.2/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.6.2/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.6.2/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.6.2/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.6.2/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.603025 alphaz-0.7.6.2/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.611025 alphaz-0.7.6.2/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.6.2/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.559025 alphaz-0.7.6.2/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.619025 alphaz-0.7.6.2/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.6.2/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.2/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.6.2/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.6.2/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.6.2/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.6.2/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.6.2/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.623025 alphaz-0.7.6.2/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14226 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.6.2/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.6.2/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25295 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.627025 alphaz-0.7.6.2/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11553 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/utils/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.627025 alphaz-0.7.6.2/alphaz/utils/apm/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-04-21 13:36:09.000000 alphaz-0.7.6.2/alphaz/utils/apm/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-04-22 14:04:43.000000 alphaz-0.7.6.2/alphaz/utils/apm/ora.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.6.2/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.6.2/alphaz/utils/configuration.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.627025 alphaz-0.7.6.2/alphaz/utils/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13859 2023-04-21 07:47:58.000000 alphaz-0.7.6.2/alphaz/utils/database/init.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.6.2/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.6.2/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.6.2/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1653 2023-04-25 15:54:12.000000 alphaz-0.7.6.2/alphaz/utils/init_database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.6.2/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.6.2/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.6.2/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.6.2/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2023-04-26 18:21:23.000000 alphaz-0.7.6.2/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.6.2/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.6.2/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-26 18:21:26.567025 alphaz-0.7.6.2/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-26 18:21:26.000000 alphaz-0.7.6.2/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11365 2023-04-26 18:21:26.000000 alphaz-0.7.6.2/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-26 18:21:26.000000 alphaz-0.7.6.2/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-26 18:21:26.000000 alphaz-0.7.6.2/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-26 18:21:26.000000 alphaz-0.7.6.2/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-26 18:21:26.627025 alphaz-0.7.6.2/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-26 18:20:53.000000 alphaz-0.7.6.2/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.993398 alphaz-0.7.6.3/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-27 10:12:19.993398 alphaz-0.7.6.3/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.6.3/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.933398 alphaz-0.7.6.3/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/README.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      455 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.6.3/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.6.3/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.933398 alphaz-0.7.6.3/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.6.3/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.6.3/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.937398 alphaz-0.7.6.3/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.6.3/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3039 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3070 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.6.3/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7272 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.6.3/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6384 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1509 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.937398 alphaz-0.7.6.3/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.6.3/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2479 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2243 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4104 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.6.3/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3324 2023-04-21 07:47:57.000000 alphaz-0.7.6.3/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.6.3/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.937398 alphaz-0.7.6.3/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.6.3/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.6.3/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11572 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.937398 alphaz-0.7.6.3/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.6.3/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.6.3/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.937398 alphaz-0.7.6.3/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.941398 alphaz-0.7.6.3/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.6.3/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.6.3/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.6.3/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.6.3/alphaz/documentations/docs/alpha_setup.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.941398 alphaz-0.7.6.3/alphaz/documentations/docs/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/authorizations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/cache.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2931 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/issues.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/methods.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/parameters.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/routes.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api/sqlalchemy.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/api_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.6.3/alphaz/documentations/docs/configuration.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.941398 alphaz-0.7.6.3/alphaz/documentations/docs/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/documentations/docs/database/init.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/database/instantiate.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/database/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/database/model.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/database/relations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/database/schema.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/docs/database/update.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.6.3/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.6.3/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.6.3/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.941398 alphaz-0.7.6.3/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.941398 alphaz-0.7.6.3/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.941398 alphaz-0.7.6.3/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.929398 alphaz-0.7.6.3/alphaz/documentations/site/api/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/authorizations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/authorizations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/cache/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/cache/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27645 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/issues/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/issues/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/methods/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/methods/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/parameters/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/parameters/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/routes/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api/sqlalchemy/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/api/sqlalchemy/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/api_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/api_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.929398 alphaz-0.7.6.3/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.945398 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.949398 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.949398 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.949398 alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.949398 alphaz-0.7.6.3/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.929398 alphaz-0.7.6.3/alphaz/documentations/site/database/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.949398 alphaz-0.7.6.3/alphaz/documentations/site/database/init/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23029 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/database/init/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/database/instantiate/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/database/instantiate/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/database/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/database/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/database/model/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/database/model/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/database/relations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/database/relations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/database/schema/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/database/schema/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/database/update/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/database/update/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.953398 alphaz-0.7.6.3/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    54135 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-27 10:12:18.000000 alphaz-0.7.6.3/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.6.3/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.6.3/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.957398 alphaz-0.7.6.3/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5773 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13989 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.6.3/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5961 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.6.3/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6318 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.957398 alphaz-0.7.6.3/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.6.3/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.6.3/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.6.3/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6207 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3233 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1151 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13008 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.6.3/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11046 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-04-21 07:47:57.000000 alphaz-0.7.6.3/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.6.3/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6362 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2929 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18623 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9896 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5555 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.6.3/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4492 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7664 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.957398 alphaz-0.7.6.3/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.6.3/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1336 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1597 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3376 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.961398 alphaz-0.7.6.3/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.961398 alphaz-0.7.6.3/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.6.3/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.6.3/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.6.3/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.6.3/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.961398 alphaz-0.7.6.3/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      107 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.965398 alphaz-0.7.6.3/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.6.3/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      926 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.6.3/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.6.3/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14173 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14445 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/api/_reloader.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3717 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/api/_reloaders.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2219 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18705 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20124 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.6.3/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.6.3/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.965398 alphaz-0.7.6.3/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    26517 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-04-25 15:54:12.000000 alphaz-0.7.6.3/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.965398 alphaz-0.7.6.3/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.6.3/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.6.3/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9992 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.6.3/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.6.3/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    56477 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.6.3/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4529 2023-04-21 13:36:09.000000 alphaz-0.7.6.3/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9301 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.6.3/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6683 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.6.3/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.965398 alphaz-0.7.6.3/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.6.3/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.965398 alphaz-0.7.6.3/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.6.3/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.6.3/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14136 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.965398 alphaz-0.7.6.3/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.6.3/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.6.3/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      354 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27261 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15986 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.6.3/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2075 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2218 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-04-25 15:54:12.000000 alphaz-0.7.6.3/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8070 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3446 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-04-25 15:54:12.000000 alphaz-0.7.6.3/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4125 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4578 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14818 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7505 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2896 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.6.3/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.6.3/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.6.3/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.6.3/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.6.3/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.6.3/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.969398 alphaz-0.7.6.3/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.977398 alphaz-0.7.6.3/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.6.3/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.933398 alphaz-0.7.6.3/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.985398 alphaz-0.7.6.3/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.985398 alphaz-0.7.6.3/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.6.3/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.985398 alphaz-0.7.6.3/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.985398 alphaz-0.7.6.3/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.6.3/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.985398 alphaz-0.7.6.3/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.6.3/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.985398 alphaz-0.7.6.3/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.989398 alphaz-0.7.6.3/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.989398 alphaz-0.7.6.3/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.989398 alphaz-0.7.6.3/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.6.3/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.6.3/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.6.3/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.6.3/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.989398 alphaz-0.7.6.3/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14226 2023-04-25 15:54:12.000000 alphaz-0.7.6.3/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.6.3/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.6.3/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25295 2023-04-25 15:54:12.000000 alphaz-0.7.6.3/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.993398 alphaz-0.7.6.3/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       57 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11574 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/utils/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.993398 alphaz-0.7.6.3/alphaz/utils/apm/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-04-21 13:36:09.000000 alphaz-0.7.6.3/alphaz/utils/apm/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-04-22 14:04:43.000000 alphaz-0.7.6.3/alphaz/utils/apm/ora.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.6.3/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.6.3/alphaz/utils/configuration.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.993398 alphaz-0.7.6.3/alphaz/utils/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13818 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/utils/database/init.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.6.3/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.6.3/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1653 2023-04-25 15:54:12.000000 alphaz-0.7.6.3/alphaz/utils/init_database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.6.3/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.6.3/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23624 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.6.3/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2023-04-26 18:21:23.000000 alphaz-0.7.6.3/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.6.3/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3849 2023-04-27 10:12:16.000000 alphaz-0.7.6.3/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-27 10:12:19.933398 alphaz-0.7.6.3/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11365 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-27 10:12:19.000000 alphaz-0.7.6.3/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-27 10:12:19.993398 alphaz-0.7.6.3/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-27 10:11:42.000000 alphaz-0.7.6.3/setup.py
```

### Comparing `alphaz-0.7.6.2/MANIFEST.in` & `alphaz-0.7.6.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/PKG-INFO` & `alphaz-0.7.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.6.2
+Version: 0.7.6.3
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.6.2.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.6.3.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.6.2/README.md` & `alphaz-0.7.6.3/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/api.json` & `alphaz-0.7.6.3/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/api.py` & `alphaz-0.7.6.3/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/mails.py` & `alphaz-0.7.6.3/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/admin.py` & `alphaz-0.7.6.3/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/api.py` & `alphaz-0.7.6.3/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.6.3/alphaz/apis/routes/basic_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import List
+
 import uuid
 
 from ...models.database.tests import Test
 
 from ...utils.api import route, Parameter, ParameterMode
 from ...models.main import AlphaException
 from ...models.tests._test import TestInput
@@ -31,19 +31,19 @@
     "/test/parameters",
     methods=["GET", "POST"],
     route_log=False,
     parameters=[
         Parameter("value"),
         Parameter("options", options=["Y", "N", 1, 2]),
         Parameter("list", ptype=list),
-        Parameter("list_str", ptype=List[str]),
-        Parameter("list_int", ptype=List[int]),
-        Parameter("list_object", ptype=List[TestInput]),
-        Parameter("list_db_object", ptype=List[Test]),
-        Parameter("list_float", ptype=List[float]),
+        Parameter("list_str", ptype=list[str]),
+        Parameter("list_int", ptype=list[int]),
+        Parameter("list_object", ptype=list[TestInput]),
+        Parameter("list_db_object", ptype=list[Test]),
+        Parameter("list_float", ptype=list[float]),
         Parameter("list_default", ptype=list, default=[]),
         Parameter("dict", ptype=dict),
         Parameter("dict_default", ptype=dict, default={}),
         Parameter("string", ptype=str, max_size=100, min_size=5),
         Parameter("string_default", ptype=str, default=""),
         Parameter("integer", ptype=int),
         Parameter("integer_default", ptype=int, default=1),
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/database.py` & `alphaz-0.7.6.3/alphaz/apis/routes/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from ...utils.api import route, Parameter, ParameterMode
 
 from ...libs import logs_lib, database_lib
 
 from ...models.main import AlphaException
 
-from typing import List
 
 from core import core
 
 API = core.api
 DB = core.db
 log = core.get_logger("api")
 
@@ -17,16 +16,16 @@
 def get_schemas():
     return database_lib.get_schemas(**API.gets())
 
 
 @route(
     "/database/tables",
     parameters=[
-        Parameter("binds", ptype=List[str]),
-        Parameter("tables", ptype=List[str]),
+        Parameter("binds", ptype=list[str]),
+        Parameter("tables", ptype=list[str]),
     ],
     admin=True,
 )
 def liste_tables():
     return DB.get_tables_models(**API.gets())
 
 
@@ -57,16 +56,16 @@
     return core.db.drop_table(**API.gets())
 
 
 @route(
     "/database/init",
     admin=True,
     parameters=[
-        Parameter("binds", ptype=List[str]),
-        Parameter("tables", ptype=List[str]),
+        Parameter("binds", ptype=list[str]),
+        Parameter("tables", ptype=list[str]),
         Parameter("drop", ptype=bool, default=False),
         Parameter("truncate", ptype=bool, default=False),
         Parameter("force", ptype=bool, default=False),
         Parameter("create", ptype=bool, default=False),
         Parameter("init", ptype=bool, default=False),
     ],
 )
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/logs.py` & `alphaz-0.7.6.3/alphaz/apis/routes/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 def get_logs_files_names():
     log_directory = core.config.get("directories/logs")
     files = glob.glob(log_directory + os.sep + "*.log")
     return [os.path.basename(x) for x in files]
 
 
 def get_logs_content(
-    name: str = None, node: str = None, content: bool = False, single: bool = False
+    name: str | None = None,
+    node: str | None = None,
+    content: bool = False,
+    single: bool = False,
 ):
     current_node = platform.uname().node
     if node is not None and node.lower() != current_node.lower():
         url = f"http://{node}:{api.port}/logs/files"
 
         params = api.get_parameters()
         params["cluster"] = False
@@ -94,15 +97,17 @@
     return logs_content
 
 
 def get_log_content(name: str, content: bool = False):
     return get_logs_content(name, content)[name]
 
 
-def get_logs_content_cluster(name: str = None, node: str = None, content: bool = False):
+def get_logs_content_cluster(
+    name: str | None = None, node: str | None = None, content: bool = False
+):
     os_logs_content = get_logs_content(api["name"], node=node, content=api["content"])
 
     in_cluster = []
     if CLUSTERS is not None and type(CLUSTERS) is list and node is None:
         for clusters in CLUSTERS:
             if type(clusters) is not list or not platform.uname().node.lower() in [
                 x.lower() for x in clusters
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/mails.py` & `alphaz-0.7.6.3/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/main.py` & `alphaz-0.7.6.3/alphaz/apis/routes/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime, os, inspect, re, platform
-from typing import List
+
 
 from flask import request, send_from_directory
 
 from ...libs import test_lib, database_lib, api_lib, py_lib, files_lib, config_lib
 from ...utils.api import route, Parameter
 from ...models.main import AlphaException
 
@@ -229,15 +229,15 @@
     return config_lib.get_configs_key(**API.get_parameters())
 
 
 @route(
     "/mail",
     parameters=[
         Parameter("name", required=True),
-        Parameter("parameters", ptype=List[dict]),
+        Parameter("parameters", ptype=list[dict]),
     ],
     admin=True,
     methods=["POST"],
 )
 def mail_me():
     from ...libs import mail_lib
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/tests.py` & `alphaz-0.7.6.3/alphaz/apis/routes/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MODULES
 import sqlalchemy
-from typing import List
+
 
 # CORE
 from core import core
 
 # MODELS
 from ...models.database.users_definitions import Application
 from ...models.tests import Levels
@@ -30,15 +30,15 @@
         Parameter("names", ptype=list),
         Parameter("run", ptype=bool),
         Parameter("file_path", ptype=str),
         Parameter("coverage", ptype=str),
         Parameter("load_from_db", ptype=bool),
         Parameter("report", ptype=str),
         Parameter("coverage", ptype=str),
-        Parameter("levels", ptype=List[Levels], default=[]),
+        Parameter("levels", ptype=list[Levels], default=[]),
     ],
 )
 def get_tests():
     return test_lib.get_tests_auto(**API.gets())
 
 
 @route("/tests/coverage", parameters=[Parameter("file", required=True)])
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.6.3/alphaz/apis/routes/user_management/application_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,93 +1,96 @@
 from ....utils.api import route, api, Parameter, ParameterMode
 from ....models.database.users_definitions import Application
 from ....libs.user_management import application_management_lib
 
-from typing import List
 
 CATEGORY = "user-mgt"
 
+
 @route(
     "user-mgt/applications",
     logged=True,
     parameters=[
         Parameter("name", ptype=str, mode=ParameterMode.IN_LIKE, function=str.upper),
         Parameter("page_index", ptype=int),
         Parameter("page_size", ptype=int),
         Parameter("order_by", ptype=str, default="name"),
         Parameter("direction", ptype=str, default="asc"),
-        Parameter("columns", ptype=List[str]),
+        Parameter("columns", ptype=list[str]),
     ],
     methods=["GET"],
-    category=CATEGORY
+    category=CATEGORY,
 )
 def get_applications():
     return application_management_lib.get_applications(**api.get_parameters())
 
+
 @route(
     "user-mgt/applications/names",
     logged=True,
     parameters=[
         Parameter("name", ptype=str, mode=ParameterMode.IN_LIKE, function=str.upper)
     ],
     methods=["GET"],
-    category=CATEGORY
+    category=CATEGORY,
 )
 def get_applications_names():
     return application_management_lib.get_applications_names(**api.get_parameters())
 
-@route(
-    "user-mgt/applications/names-id",
-    logged=True,
-    category=CATEGORY
-)
+
+@route("user-mgt/applications/names-id", logged=True, category=CATEGORY)
 def get_applications_names_and_id():
-    return application_management_lib.get_applications_names_and_id(**api.get_parameters())
+    return application_management_lib.get_applications_names_and_id(
+        **api.get_parameters()
+    )
 
 
 @route(
     "user-mgt/application",
     logged=True,
     parameters=[
         Parameter("name", required=True),
     ],
-    methods=["GET"],category=CATEGORY
+    methods=["GET"],
+    category=CATEGORY,
 )
 def get_application():
     return application_management_lib.get_application(**api.get_parameters())
 
 
 @route(
     "user-mgt/application",
     logged=True,
     parameters=[
         Parameter("application", required=True, ptype=Application),
     ],
-    methods=["POST"],category=CATEGORY
+    methods=["POST"],
+    category=CATEGORY,
 )
 def create_application():
     return application_management_lib.create_application(**api.get_parameters())
 
 
 @route(
     "user-mgt/application",
     logged=True,
     parameters=[
         Parameter("application", required=True, ptype=Application),
     ],
-    methods=["PUT"],category=CATEGORY
+    methods=["PUT"],
+    category=CATEGORY,
 )
 def edit_application():
     return application_management_lib.edit_application(**api.get_parameters())
 
 
 @route(
     "user-mgt/application",
     logged=True,
     parameters=[
         Parameter("id", required=True, ptype=int),
     ],
-    methods=["DELETE"],category=CATEGORY
+    methods=["DELETE"],
+    category=CATEGORY,
 )
 def delete_application():
     return application_management_lib.delete_application(**api.get_parameters())
-
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.6.3/alphaz/apis/routes/user_management/permission_management.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 from ....utils.api import route, api, Parameter, ParameterMode
 from ....libs.user_management import permission_management_lib
 from ....models.database.users_definitions import Permission
 
-from typing import List
 
 CATEGORY = "user-mgt"
 
+
 @route(
     "user-mgt/permissions",
     logged=True,
     parameters=[
         Parameter("name", ptype=str, mode=ParameterMode.IN_LIKE, function=str.upper),
         Parameter("page_index", ptype=int),
         Parameter("page_size", ptype=int),
         Parameter("order_by", ptype=str, default="key"),
         Parameter("direction", ptype=str, default="asc"),
-        Parameter("columns", ptype=List[str]),
+        Parameter("columns", ptype=list[str]),
     ],
-    methods=["GET"],category=CATEGORY
+    methods=["GET"],
+    category=CATEGORY,
 )
 def get_permissions():
     return permission_management_lib.get_permissions(**api.get_parameters())
 
+
 @route(
     "user-mgt/permissions/names",
     logged=True,
     parameters=[
         Parameter("name", ptype=str, mode=ParameterMode.IN_LIKE, function=str.upper),
     ],
-    methods=["GET"],category=CATEGORY
+    methods=["GET"],
+    category=CATEGORY,
 )
 def get_permissions_names():
     return permission_management_lib.get_permissions_names(**api.get_parameters())
 
+
 @route(
     "user-mgt/permission",
     logged=True,
     parameters=[
         Parameter("name", required=True, ptype=str),
     ],
-    methods=["GET"],category=CATEGORY
+    methods=["GET"],
+    category=CATEGORY,
 )
 def get_permission():
     return permission_management_lib.get_permission(**api.get_parameters())
 
 
 @route(
     "user-mgt/permission",
     logged=True,
     parameters=[
         Parameter("permission", required=True, ptype=Permission),
     ],
-    methods=["POST"],category=CATEGORY
+    methods=["POST"],
+    category=CATEGORY,
 )
 def create_permission():
     return permission_management_lib.create_permission(**api.get_parameters())
 
 
 @route(
     "user-mgt/permission",
     logged=True,
     parameters=[
         Parameter("permission", required=True, ptype=Permission),
     ],
-    methods=["PUT"],category=CATEGORY
+    methods=["PUT"],
+    category=CATEGORY,
 )
 def edit_permission():
     return permission_management_lib.edit_permission(**api.get_parameters())
 
 
 @route(
     "user-mgt/permission",
     logged=True,
     parameters=[
         Parameter("key", required=True, ptype=str),
     ],
-    methods=["DELETE"],category=CATEGORY
+    methods=["DELETE"],
+    category=CATEGORY,
 )
 def delete_permission():
     return permission_management_lib.delete_permission(**api.get_parameters())
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.6.3/alphaz/apis/routes/user_management/role_management.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import List
 from ....utils.api import route, api, Parameter, ParameterMode
 from ....models.database.users_definitions import Role
 from ....libs.user_management import role_management_lib
 
 CATEGORY = "user-mgt"
 
 
@@ -37,47 +36,55 @@
 def get_roles_names():
     return role_management_lib.get_roles_names(**api.get_parameters())
 
 
 @route(
     "user-mgt/role",
     logged=True,
-    parameters=[Parameter("name", required=True),],
+    parameters=[
+        Parameter("name", required=True),
+    ],
     category=CATEGORY,
 )
 def get_role():
     return role_management_lib.get_role(**api.get_parameters())
 
 
 @route(
     "user-mgt/role",
     logged=True,
-    parameters=[Parameter("role", required=True, ptype=Role),],
+    parameters=[
+        Parameter("role", required=True, ptype=Role),
+    ],
     methods=["POST"],
     category=CATEGORY,
 )
 def create_role():
     return role_management_lib.create_role(**api.get_parameters())
 
 
 @route(
     "user-mgt/role",
     logged=True,
-    parameters=[Parameter("role", required=True, ptype=Role),],
+    parameters=[
+        Parameter("role", required=True, ptype=Role),
+    ],
     methods=["PUT"],
     category=CATEGORY,
 )
 def edit_role():
     return role_management_lib.edit_role(**api.get_parameters())
 
 
 @route(
     "user-mgt/role",
     logged=True,
-    parameters=[Parameter("name", required=True, ptype=str),],
+    parameters=[
+        Parameter("name", required=True, ptype=str),
+    ],
     methods=["DELETE"],
     category=CATEGORY,
 )
 def delete_role():
     return role_management_lib.delete_role(**api.get_parameters())
 
 
@@ -150,13 +157,15 @@
 def add_app_role():
     return role_management_lib.add_app_role(**api.get_parameters())
 
 
 @route(
     "user-mgt/role/application",
     logged=True,
-    parameters=[Parameter("role_name", required=True, ptype=str),],
+    parameters=[
+        Parameter("role_name", required=True, ptype=str),
+    ],
     methods=["DELETE"],
     category=CATEGORY,
 )
 def delete_app_role():
     return role_management_lib.delete_app_role(**api.get_parameters())
```

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.6.3/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/routes/users.py` & `alphaz-0.7.6.3/alphaz/apis/routes/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/tests.py` & `alphaz-0.7.6.3/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/users/ldap.py` & `alphaz-0.7.6.3/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/apis/users/users.py` & `alphaz-0.7.6.3/alphaz/apis/users/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+# MODULES
 import datetime, jwt, itertools
 import enum
-from enum import Enum
-
-from ...models.user import AlphaUser, AlphaUserSession
+from flask import request
 
-from ...libs import user_lib, secure_lib, json_lib, mail_lib
+# CORE
+from core import core, API, DB
 
+# MODELS
+from ...models.user import AlphaUser, AlphaUserSession
 from ...models.database.users_definitions import User, UserSession
-
 from ...models.main import AlphaException, EnumStr
 from ...models.api import AlphaRequest
 
-from core import core, API, DB
-
-from flask import request
+# LIBS
+from ...libs import user_lib, secure_lib, json_lib, mail_lib
 
 
 class LoginModes(EnumStr):
     LDAP = enum.auto()
     NO_CONFIRMATION = enum.auto()
 
 
@@ -28,14 +28,15 @@
 DATA_TO_JWT = {
     "id": "id",
     "username": "sub",
     "time": "iat",
     "permissions": "permissions",
 }
 
+
 # Serve for registration
 def try_register_user(
     mail, username, password, password_confirmation, validation=True, infos=""
 ):
     userByMail = user_lib.get_user_data_by_mail(mail)
     userByUsername = user_lib.get_user_data_by_username(username)
     validation = False if LOGIN_MODE == LoginModes.NO_CONFIRMATION.value else validation
@@ -283,15 +284,17 @@
             if not x in DATA_TO_JWT or x == "username"
         },
         "token": token,
         "valid_until": expire,
     }
 
 
-def try_su_login(admin_user_id: str = None, admin_user_name: str = None) -> AlphaUser:
+def try_su_login(
+    admin_user_id: str | None = None, admin_user_name: str | None = None
+) -> AlphaUser:
     user_data = try_login(
         admin_user_name if admin_user_name is not None else admin_user_id, None, su=True
     )
     API.admin_token = user_data["token"]
     return user_data
```

### Comparing `alphaz-0.7.6.2/alphaz/config/config.css` & `alphaz-0.7.6.3/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/config/config.html` & `alphaz-0.7.6.3/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/config/main_configuration.py` & `alphaz-0.7.6.3/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/config/page.py` & `alphaz-0.7.6.3/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/config/source.html` & `alphaz-0.7.6.3/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/config.json` & `alphaz-0.7.6.3/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/api/authorizations.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/api/authorizations.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/api/configuration.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/api/configuration.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```json
 "routes_no_log": ["//status", "//static", "//dashboard"],
 ```
 
 - models: In order to specify the **Flask-SqlAlchemy** models definitions paths
 
 ```json
-"models": ["models.databases"]
+"models": ["models.database"]
 ```
 
 - routes: In order to specify the routes definitions paths
 
 ```json
 "routes": ["apis.routes"]
 ```
```

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/api/main.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/api/main.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/api/methods.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/api/methods.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/api/parameters.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/api/parameters.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/api/routes.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/api/routes.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/api_database.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/api_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/database/init.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/database/init.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 The route **database/init** could be use to init the database or some tables.
 
 ```py 
 @route(
     "/database/init",
     admin=True,
     parameters=[
-        Parameter("binds", ptype=List[str]),
-        Parameter("tables", ptype=List[str]),
+        Parameter("binds", ptype=list[str]),
+        Parameter("tables", ptype=list[str]),
         Parameter("drop", ptype=bool, default=False),
         Parameter("truncate", ptype=bool, default=False),
         Parameter("force", ptype=bool, default=False),
         Parameter("create", ptype=bool, default=False),
     ],
 )
 ```
```

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/database/model.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/database/model.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/database/schema.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/database/schema.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/database/update.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/database/update.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/docs/index.md` & `alphaz-0.7.6.3/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/mkdocs.yml` & `alphaz-0.7.6.3/alphaz/documentations/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/404.html` & `alphaz-0.7.6.3/alphaz/documentations/site/404.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/alpha_admin/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/alpha_core/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/alpha_screens/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/alpha_setup/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/authorizations/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/authorizations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/cache/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/cache/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/configuration/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/configuration/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,15 @@
 <li>routes_no_log: In order to specify the routes where log must be ignored</li>
 </ul>
 <div class="highlight"><pre><span></span><code><span class="nt">&quot;routes_no_log&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;//status&quot;</span><span class="p">,</span> <span class="s2">&quot;//static&quot;</span><span class="p">,</span> <span class="s2">&quot;//dashboard&quot;</span><span class="p">],</span>
 </code></pre></div>
 <ul>
 <li>models: In order to specify the <strong>Flask-SqlAlchemy</strong> models definitions paths</li>
 </ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;models&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;models.databases&quot;</span><span class="p">]</span>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;models&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;models.database&quot;</span><span class="p">]</span>
 </code></pre></div>
 <ul>
 <li>routes: In order to specify the routes definitions paths</li>
 </ul>
 <div class="highlight"><pre><span></span><code><span class="nt">&quot;routes&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;apis.routes&quot;</span><span class="p">]</span>
 </code></pre></div>
 <ul>
```

#### html2text {}

```diff
@@ -60,15 +60,15 @@
 for further details on how to use it.
 **** Main ****
     * workers: In order to specify the numbers of workers
 "workers": 6
     * routes_no_log: In order to specify the routes where log must be ignored
 "routes_no_log": ["//status", "//static", "//dashboard"],
     * models: In order to specify the Flask-SqlAlchemy models definitions paths
-"models": ["models.databases"]
+"models": ["models.database"]
     * routes: In order to specify the routes definitions paths
 "routes": ["apis.routes"]
     * ssl: In order to activate ssl mode
 "ssl": false
     * threaded: In order to activate the threaded mode
 "threaded": false
     * config: In order to activate pass configuration to Flask api class
```

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/issues/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/issues/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/main/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/methods/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/methods/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/parameters/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/parameters/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/routes/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/routes/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api/sqlalchemy/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api/sqlalchemy/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/api_database/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/api_database/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.6.3/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/database/init/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/database/init/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -584,16 +584,16 @@
                 
                 <h1 id="route">Route</h1>
 <p>The route <strong>database/init</strong> could be use to init the database or some tables.</p>
 <div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span>
     <span class="s2">&quot;/database/init&quot;</span><span class="p">,</span>
     <span class="n">admin</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
     <span class="n">parameters</span><span class="o">=</span><span class="p">[</span>
-        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;binds&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]),</span>
-        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;tables&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]),</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;binds&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]),</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;tables&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]),</span>
         <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;drop&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
         <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;truncate&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
         <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;force&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
         <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
     <span class="p">],</span>
 <span class="p">)</span>
 </code></pre></div>
```

#### html2text {}

```diff
@@ -45,16 +45,16 @@
 
 ****** Route ******
 The route database/init could be use to init the database or some tables.
 @route(
     "/database/init",
     admin=True,
     parameters=[
-        Parameter("binds", ptype=List[str]),
-        Parameter("tables", ptype=List[str]),
+        Parameter("binds", ptype=list[str]),
+        Parameter("tables", ptype=list[str]),
         Parameter("drop", ptype=bool, default=False),
         Parameter("truncate", ptype=bool, default=False),
         Parameter("force", ptype=bool, default=False),
         Parameter("create", ptype=bool, default=False),
     ],
 )
 ****** Configuration ******
```

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/database/instantiate/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/database/instantiate/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/database/main/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/database/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/database/model/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/database/model/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/database/relations/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/database/relations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/database/schema/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/database/schema/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/database/update/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/database/update/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/documentation/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/index.html` & `alphaz-0.7.6.3/alphaz/documentations/site/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.6.3/alphaz/documentations/site/search/search_index.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983333333333333%*

 * *Differences: {"'docs'": "{63: {'text': 'The api is automatically configured from the api.jon file. See "*

 * *           'Configuration for further details on how to use it. Main workers: In order to specify '*

 * *           'the numbers of workers "workers" : 6 routes_no_log: In order to specify the routes '*

 * *           'where log must be ignored "routes_no_log" : [ "//status" , "//static" , "//dashboard" '*

 * *           '], models: In order to specify the Flask-SqlAlchemy models definitions paths "models" '*

 * *           ': [ "models […]*

```diff
@@ -321,20 +321,20 @@
         {
             "location": "api/cache/",
             "text": "A cache system is implemented, in order to use it you must specify the",
             "title": "Cache"
         },
         {
             "location": "api/configuration/",
-            "text": "The api is automatically configured from the api.jon file. See Configuration for further details on how to use it. Main workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false } Mails In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } } Auth In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } }, Reloader type In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\" Admin In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" }, Dashboard In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } }",
+            "text": "The api is automatically configured from the api.jon file. See Configuration for further details on how to use it. Main workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.database\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false } Mails In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } } Auth In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } }, Reloader type In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\" Admin In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" }, Dashboard In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } }",
             "title": "Configuration"
         },
         {
             "location": "api/configuration/#main",
-            "text": "workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false }",
+            "text": "workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.database\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false }",
             "title": "Main"
         },
         {
             "location": "api/configuration/#mails",
             "text": "In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } }",
             "title": "Mails"
         },
@@ -436,20 +436,20 @@
         {
             "location": "api/sqlalchemy/",
             "text": "If you specify a SqlAlchemy model as a type it will be automatically converted to the specified model. from core import core db = core . db class Logs ( db . Model , AlphaTable ): __tablename__ = 'LOGS' id = AlphaColumn ( Integer , nullable = False , primary_key = True ) name = AlphaColumn ( String , nullable = False ) @route ( \"logs\" , parameters = [ Parameter ( 'log' , ptype = Logs ) ]) def admin_logs (): db . add ( api [ 'log' ])",
             "title": "SqlAlchemy"
         },
         {
             "location": "database/init/",
-            "text": "Route The route database/init could be use to init the database or some tables. @route ( \"/database/init\" , admin = True , parameters = [ Parameter ( \"binds\" , ptype = List [ str ]), Parameter ( \"tables\" , ptype = List [ str ]), Parameter ( \"drop\" , ptype = bool , default = False ), Parameter ( \"truncate\" , ptype = bool , default = False ), Parameter ( \"force\" , ptype = bool , default = False ), Parameter ( \"create\" , ptype = bool , default = False ), ], ) Configuration Content of tables could be pre-defined in various ways: python : you have to specify the directory where the py files are defined using the init_database_dir_py parameter in your database configuration. For every table you want to fill you could specify objects which are models in this situation: from models.database.olca import TblGroups ini = { TblGroups : { \"objects\" : [ TblGroups . instantiate ( 2 , \"hidden\" , \"far fa-eye-slash\" , \"var(--ion-color-light)\" ), TblGroups . instantiate ( 3 , \"steps\" , \"fas fa-cogs\" , \"var(--ion-color-danger)\" ), TblGroups . instantiate ( 4 , \"materials\" , \"fas fa-cubes\" , \"var(--ion-color-primary)\" ), TblGroups . instantiate ( 5 , \"transports\" , \"fas fa-dolly-flatbed\" , \"var(--ion-color-secondary)\" ), TblGroups . instantiate ( 6 , \"powers\" , \"fas fa-lightbulb\" , \"var(--ion-color-warning)\" ), ] }, } json : you have to specify the directory where the json files are defined using the init_database_dir_json parameter in your database configuration. { \"sophisme\" : { \"headers\" : [ \"theme\" , \"sophisme\" , \"user\" , \"proposition\" ], \"values\" : [ [ 5 , 20 , 6 , 34 ], [ 5 , 7 , 1 , 35 ], [ 5 , 9 , 1 , 35 ] ] } } sql : you have to specify the directory where the sql files are defined using the init_database_dir_sql parameter in your database configuration. Here the code is directly executed, so it could have any valid sql structure.",
+            "text": "Route The route database/init could be use to init the database or some tables. @route ( \"/database/init\" , admin = True , parameters = [ Parameter ( \"binds\" , ptype = list [ str ]), Parameter ( \"tables\" , ptype = list [ str ]), Parameter ( \"drop\" , ptype = bool , default = False ), Parameter ( \"truncate\" , ptype = bool , default = False ), Parameter ( \"force\" , ptype = bool , default = False ), Parameter ( \"create\" , ptype = bool , default = False ), ], ) Configuration Content of tables could be pre-defined in various ways: python : you have to specify the directory where the py files are defined using the init_database_dir_py parameter in your database configuration. For every table you want to fill you could specify objects which are models in this situation: from models.database.olca import TblGroups ini = { TblGroups : { \"objects\" : [ TblGroups . instantiate ( 2 , \"hidden\" , \"far fa-eye-slash\" , \"var(--ion-color-light)\" ), TblGroups . instantiate ( 3 , \"steps\" , \"fas fa-cogs\" , \"var(--ion-color-danger)\" ), TblGroups . instantiate ( 4 , \"materials\" , \"fas fa-cubes\" , \"var(--ion-color-primary)\" ), TblGroups . instantiate ( 5 , \"transports\" , \"fas fa-dolly-flatbed\" , \"var(--ion-color-secondary)\" ), TblGroups . instantiate ( 6 , \"powers\" , \"fas fa-lightbulb\" , \"var(--ion-color-warning)\" ), ] }, } json : you have to specify the directory where the json files are defined using the init_database_dir_json parameter in your database configuration. { \"sophisme\" : { \"headers\" : [ \"theme\" , \"sophisme\" , \"user\" , \"proposition\" ], \"values\" : [ [ 5 , 20 , 6 , 34 ], [ 5 , 7 , 1 , 35 ], [ 5 , 9 , 1 , 35 ] ] } } sql : you have to specify the directory where the sql files are defined using the init_database_dir_sql parameter in your database configuration. Here the code is directly executed, so it could have any valid sql structure.",
             "title": "Init"
         },
         {
             "location": "database/init/#route",
-            "text": "The route database/init could be use to init the database or some tables. @route ( \"/database/init\" , admin = True , parameters = [ Parameter ( \"binds\" , ptype = List [ str ]), Parameter ( \"tables\" , ptype = List [ str ]), Parameter ( \"drop\" , ptype = bool , default = False ), Parameter ( \"truncate\" , ptype = bool , default = False ), Parameter ( \"force\" , ptype = bool , default = False ), Parameter ( \"create\" , ptype = bool , default = False ), ], )",
+            "text": "The route database/init could be use to init the database or some tables. @route ( \"/database/init\" , admin = True , parameters = [ Parameter ( \"binds\" , ptype = list [ str ]), Parameter ( \"tables\" , ptype = list [ str ]), Parameter ( \"drop\" , ptype = bool , default = False ), Parameter ( \"truncate\" , ptype = bool , default = False ), Parameter ( \"force\" , ptype = bool , default = False ), Parameter ( \"create\" , ptype = bool , default = False ), ], )",
             "title": "Route"
         },
         {
             "location": "database/init/#configuration",
             "text": "Content of tables could be pre-defined in various ways: python : you have to specify the directory where the py files are defined using the init_database_dir_py parameter in your database configuration. For every table you want to fill you could specify objects which are models in this situation: from models.database.olca import TblGroups ini = { TblGroups : { \"objects\" : [ TblGroups . instantiate ( 2 , \"hidden\" , \"far fa-eye-slash\" , \"var(--ion-color-light)\" ), TblGroups . instantiate ( 3 , \"steps\" , \"fas fa-cogs\" , \"var(--ion-color-danger)\" ), TblGroups . instantiate ( 4 , \"materials\" , \"fas fa-cubes\" , \"var(--ion-color-primary)\" ), TblGroups . instantiate ( 5 , \"transports\" , \"fas fa-dolly-flatbed\" , \"var(--ion-color-secondary)\" ), TblGroups . instantiate ( 6 , \"powers\" , \"fas fa-lightbulb\" , \"var(--ion-color-warning)\" ), ] }, } json : you have to specify the directory where the json files are defined using the init_database_dir_json parameter in your database configuration. { \"sophisme\" : { \"headers\" : [ \"theme\" , \"sophisme\" , \"user\" , \"proposition\" ], \"values\" : [ [ 5 , 20 , 6 , 34 ], [ 5 , 7 , 1 , 35 ], [ 5 , 9 , 1 , 35 ] ] } } sql : you have to specify the directory where the sql files are defined using the init_database_dir_sql parameter in your database configuration. Here the code is directly executed, so it could have any valid sql structure.",
             "title": "Configuration"
         },
```

### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.6.3/alphaz/documentations/site/sitemap.xml`

 * *Files 4% similar despite different names*

#### Comparing `alphaz-0.7.6.2/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.6.3/alphaz/documentations/site/sitemap.xml`

```diff
@@ -1,128 +1,128 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-26</lastmod>
+    <lastmod>2023-04-27</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `alphaz-0.7.6.2/alphaz/index.html` & `alphaz-0.7.6.3/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/api_lib.py` & `alphaz-0.7.6.3/alphaz/libs/api_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODULES
 import json, inspect, requests
-from xml.etree.ElementInclude import default_loader
 
 # UTILS
 from ..utils.api import ROUTES
 
 # MODELS
 from ..models.logger import AlphaLogger
 from ..models.api import ApiMethods
@@ -19,20 +18,20 @@
 
 MODULES = {}
 
 
 def get_api_answer(
     url: str,
     params: dict = {},
-    log: AlphaLogger = None,
+    log: AlphaLogger | None = None,
     no_log: bool = False,
     method: ApiMethods = ApiMethods.GET,
     requester=None,
     allow_none: bool = False,
-) -> ApiAnswer:
+) -> ApiAnswer | None:
     """Get data from api
 
     Args:
         url (str): [description]
         params (dict, optional): [description]. Defaults to {}.
         log (AlphaLogger, optional): [description]. Defaults to None.
         method (ApiMethods, optional): The request method. Defaults to GET.
@@ -115,19 +114,19 @@
             }
         )
 
 
 def get_api_data(
     url: str,
     params: dict = {},
-    log: AlphaLogger = None,
+    log: AlphaLogger | None = None,
     method: ApiMethods = ApiMethods.GET,
     data_only: bool = True,
     requester=None,
-) -> dict:
+) -> dict | ApiAnswer:
     """Get data from api
 
     Args:
         url (str): [description]
         params (dict, optional): [description]. Defaults to {}.
         log (AlphaLogger, optional): [description]. Defaults to None.
         method (ApiMethods, optional): The request method. Defaults to GET.
@@ -145,15 +144,15 @@
             f"Fail to get data from {url}: {answer.status} - {answer.status_description}"
         )
 
     return answer.data if data_only else answer
 
 
 def get_routes_infos(
-    log: AlphaLogger = None, categories=None, routes=None, reload_=False
+    log: AlphaLogger | None = None, categories=None, routes=None, reload_=False
 ) -> dict:
     """Get all apis routes with informations.
 
     Args:
         log ([AlphaLogger], optional): [description]. Defaults to None.
     Args:
         log ([AlphaLogger], optional): [description]. Defaults to None.
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/barcode_lib.py` & `alphaz-0.7.6.3/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/config_lib.py` & `alphaz-0.7.6.3/alphaz/libs/config_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime, os, re, configparser, pickle, json
-from typing import List
 
 CONFIG_FILE_EXTENSION = ".ini"
 
 from collections import OrderedDict
 
 from ..libs import converter_lib, json_lib, io_lib, dict_lib
 from ..models.database.structure import AlphaDatabase
@@ -449,15 +448,15 @@
         write_config_file(filename, dashboard, directory, upper_keys=True)
         return directory + os.sep + filename
     except Exception as ex:
         LOG.error(ex)
         return None
 
 
-def get_configs(config: str = None):
+def get_configs(config: str | None = None):
     from core import DB, LOG
     from ..models.database.main_definitions import Configs
 
     global CONFIGS
     configs = DB.select(Configs)
     configs_dict = {}
     for config in configs:
@@ -477,15 +476,15 @@
         dict_keys = dict_lib.get_nested_dict_from_list(keys)
         dict_lib.set_nested(dict_keys, keys, value)
         configs_dict = dict_lib.merge_dict(configs_dict, dict_keys)
     CONFIGS = configs_dict
     return configs_dict
 
 
-def get_configs_key(keys: List[str], config: str = None, default=None):
+def get_configs_key(keys: list[str], config: str | None = None, default=None):
     global CONFIGS
     if type(keys) == str:
         keys = keys.split(";")
     if CONFIGS is None or len(CONFIGS) == 0:
         CONFIGS = get_configs(config)
     value = dict_lib.get_nested(CONFIGS, [x.lower() for x in keys])
     return value if value is not None else default
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/converter_lib.py` & `alphaz-0.7.6.3/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/database_lib.py` & `alphaz-0.7.6.3/alphaz/libs/database_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # CORE
 from core import core
 
 # MODULES
 import re
-from typing import Dict, List, Union, Optional, Any
+from typing import Any
 
 # MODELS
 from ..models.main import AlphaException, AlphaCore
 
 # UTILS
 from ..utils.database import init as init_database_fct
 
 
 def init_databases(
     core: AlphaCore,
-    tables: List[str] | Dict[str, str] = None,
-    binds: List[str] = None,
+    tables: list[str] | dict[str, str] | None = None,
+    binds: list[str] | None = None,
     create: bool = False,
     drop: bool = False,
     truncate: bool = False,
     sqlite: bool = True,
     force: bool = True,
     init: bool = False,
 ):
     """Initialise les bases de données en fonction des paramètres fournis. Cette fonction est la principale et appelle les autres fonctions pour effectuer diverses tâches.
 
     Args:
         core (AlphaCore): objet Core contenant les informations de base et les configurations
-        tables (List[str] | Dict[str, str], optional): Liste ou dictionnaire des noms des tables à traiter. Defaults to None.
-        binds (List[str], optional): Liste des binds à traiter. Defaults to None.
+        tables (list[str] | dict[str, str], optional): Liste ou dictionnaire des noms des tables à traiter. Defaults to None.
+        binds (list[str], optional): Liste des binds à traiter. Defaults to None.
         create (bool, optional): Booléen indiquant si les tables doivent être créées. Defaults to False.
         drop (bool, optional): Booléen indiquant si les tables doivent être supprimées. Defaults to False.
         truncate (bool, optional):  Booléen indiquant si les tables doivent être vidées. Defaults to False.
         sqlite (bool, optional): Booléen indiquant si SQLite doit être utilisé. Defaults to True.
         force (bool, optional): Booléen indiquant si la configuration doit être forcée à 'local'. Defaults to True.
         init (bool, optional): Booléen indiquant si les fichiers d'initialisation doivent être traités. Defaults to False.
     """
@@ -72,15 +72,15 @@
 def get_table_content(
     bind: str,
     tablename: str,
     order_by: str,
     direction: str,
     page_index: int,
     page_size: int,
-    limit: int = None,
+    limit: int | None = None,
 ):
     model = core.db.get_table_model(tablename, bind)
     return core.db.select(
         model,
         page=page_index,
         per_page=page_size,
         order_by=order_by,
@@ -90,16 +90,16 @@
 
 
 def where_used(
     core: AlphaCore,
     data_type: str,
     value,
     bind: str,
-    column_name: Optional[str] = None,
-) -> Dict[str, Any]:
+    column_name: str | None = None,
+) -> dict[str, Any]:
     """
     Find where a value is used in columns of a certain data type.
 
     :param core: AlphaCore instance to work with.
     :param data_type: Data type to search for in columns.
     :param value: Value to search for in columns.
     :param bind: Bind name to work with.
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/date_lib.py` & `alphaz-0.7.6.3/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/dict_lib.py` & `alphaz-0.7.6.3/alphaz/libs/dict_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dictdiffer
-from typing import Iterable, List, Union
+from typing import Iterable
 
 
 def sort_dict(x, value=False, reverse=False):
     sorted_x = {
         x: y
         for x, y in sorted(
             x.items(), key=lambda kv: kv[1 if value else 0], reverse=reverse
@@ -23,15 +23,15 @@
     """
     out = {}
     for key in reversed(in_list):
         out = {key: out}
     return out
 
 
-def get_nested(data: dict, keys: List[str], ignore_case: bool = True):
+def get_nested(data: dict, keys: list[str], ignore_case: bool = True):
     if keys and data:
         element = keys[0].lower() if ignore_case else keys[0]
         if element:
             value = data.get(element)
             return value if len(keys) == 1 else get_nested(value, keys[1:])
 
 
@@ -74,15 +74,14 @@
         diff = dict(sorted(diff.items()))
 
     root = False
     if outputs is None:
         outputs, root = [], True
 
     for key, value in diff.items():
-
         if type(value) == list:
             is_diff = False
             for i, el in enumerate(value[::-1]):
                 sub_outputs = []
                 show_dict(el, level=level + 1, outputs=sub_outputs, show_none=show_none)
                 if len(sub_outputs) != 0:
                     outputs.extend(sub_outputs)
@@ -102,22 +101,22 @@
                 outputs.append("    " * level + f"-{key}:")
 
     if root:
         print("\n".join(outputs[::-1]))
 
 
 def compare_dicts(
-    d1: dict, d2: dict, ignore: list | dict = None, show: bool = False
-) -> dict:
+    d1: dict, d2: dict, ignore: list | dict | None = None, show: bool = False
+) -> dict | None:
     """Compare two dict, returns None if there is no difference
 
     Args:
         d1 (dict): _description_
         d2 (dict): _description_
-        ignore (list | dict, optional): List or dict of keys to ignore. Defaults to None.
+        ignore (list | dict, optional): list or dict of keys to ignore. Defaults to None.
         show (bool, optional): _description_. Defaults to False.
 
     Returns:
         dict: _description_
     """
     if d1 == d2:
         return None
@@ -174,15 +173,15 @@
     ):
         return None
     if len(res) == 0:
         return None
     return res
 
 
-def get_subdictionary(d: dict, keys: List[str] = None) -> dict:
+def get_subdictionary(d: dict, keys: list[str] | None = None) -> dict:
     if keys is None:
         keys = d.keys()  # use all keys by default
 
     if isinstance(d, dict):
         return {
             k: get_subdictionary(v, keys) if isinstance(v, (dict, list)) else v
             for k, v in d.items()
@@ -191,29 +190,28 @@
 
     elif isinstance(d, list):
         return [get_subdictionary(item, keys) for item in d]
 
     return d
 
 
-def get_nested_dictionary_keys(d: dict) -> List[str]:
+def get_nested_dictionary_keys(d: dict) -> list[str]:
     keys = []
     for k, v in d.items():
         keys.append(k)
         if isinstance(v, dict):
             keys.extend(get_nested_dictionary_keys(v))
     return set(keys)
 
 
-def dict_diff(dict_1: dict, dict2: dict) -> List[any]:
+def dict_diff(dict_1: dict, dict2: dict) -> list[any]:
     return [diff for diff in list(dictdiffer.diff(dict_1, dict2))]
 
 
-def get_dicts_diff(dict_1: Union[dict, List[dict]], dict_2: Union[dict, List[dict]]):
-
+def get_dicts_diff(dict_1: dict | list[dict], dict_2: dict | list[dict]):
     if isinstance(dict_1, dict):
         dict_1 = [dict_1]
 
     if isinstance(dict_2, dict):
         dict_2 = [dict_2]
 
     return [
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.6.3/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/events.py` & `alphaz-0.7.6.3/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/files_lib.py` & `alphaz-0.7.6.3/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/flask_lib.py` & `alphaz-0.7.6.3/alphaz/libs/flask_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 DB = core.db
 
 
 class AlphaModelView(ModelView):
     column_display_pk = True
 
 
-def load_views(binds: List[str], tables: List[str], log=None) -> List[ModelView]:
+def load_views(binds: list[str], tables: list[str], log=None) -> list[ModelView]:
     """[Load view from tables definitions module]
 
     Args:
         module (ModuleType): [description]
 
     Returns:
-        List[ModelView]: [description]
+        list[ModelView]: [description]
     """
     views = []
 
     for model in DB.get_tables_models(binds=binds, tables=tables):
         table_name = model.__tablename__
         bind = model.__bind_key__
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/img_lib.py` & `alphaz-0.7.6.3/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/io_lib.py` & `alphaz-0.7.6.3/alphaz/libs/io_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import requests, json, re, os, pickle, pathlib, datetime
 from lxml.html import fromstring
 from ..models.main import AlphaFile
 
-from typing import List
-
 
 def ensure_dir(file_path):
     directory = os.path.dirname(file_path)
     if directory != "" and not os.path.exists(directory):
         os.makedirs(directory)
 
 
@@ -93,15 +91,17 @@
             proxy = ":".join(
                 [i.xpath(".//td[1]/text()")[0], i.xpath(".//td[2]/text()")[0]]
             )
             proxies.add(proxy)
     return proxies
 
 
-def archive_object(object_to_save, filename: str, ext: str = None, log=None) -> None:
+def archive_object(
+    object_to_save, filename: str, ext: str | None = None, log=None
+) -> None:
     """Archive a Python object as a dump file
 
     Args:
         object_to_save ([type]): [Python object to save]
         filename (str): [output filename]
         ext (str, optional): [file extension]. Defaults to 'dmp'.
     """
@@ -115,15 +115,15 @@
         filename = filename + "." + ext
     with open(filename, "wb") as f:
         pickle.dump(object_to_save, f, protocol=pickle.HIGHEST_PROTOCOL)
     if log:
         log.info(f"Saved file {filename}")
 
 
-def unarchive_object(filename: str, ext: str = None, default: object = None):
+def unarchive_object(filename: str, ext: str | None = None, default: object = None):
     """[Unarchive a Python object from a dump file]
 
     Args:
         filename (str): [filename]
         ext (str, optional): [file extension]. Defaults to 'dmp'.
 
     Returns:
@@ -170,15 +170,15 @@
 
 
 def get_match(regex, txt):
     matchs = re.findall(regex, txt)
     return None if len(matchs) == 0 else matchs[0]
 
 
-def get_list_file(output) -> List[AlphaFile]:
+def get_list_file(output) -> list[AlphaFile]:
     files = []
     for line in output.split("\r\n" if "\r\n" in output else "\\r\\n"):
         if line.strip() == "":
             continue
 
         permission = get_match(r"[drwxr-]{10}\.?", line)
         if permission is None:
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/json_lib.py` & `alphaz-0.7.6.3/alphaz/libs/json_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import json, dataclasses, typing
+import json, dataclasses
 from flask_sqlalchemy.model import DefaultMeta
 from sqlalchemy.orm.attributes import instance_state
 from sqlalchemy import null
 
 from ..libs.time_lib import timer
 
 from ..models.database.row import Row
 
 
 def jsonify_database_models(
     model: DefaultMeta,
     first=False,
     relationship: bool = True,
-    disabled_relationships: typing.List[str] = None,
+    disabled_relationships: list[str] = None,
 ):
     """Convert a database model structure to json
 
     Args:
         model (DefaultMeta): database mode structure
         first (bool, optional): [description]. Defaults to False.
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/logs_lib.py` & `alphaz-0.7.6.3/alphaz/libs/logs_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+
 from core import core
 from ..models.database.main_definitions import Logs
 from ..models.main import AlphaException
 
 api = core.api
 DB = core.db
 
@@ -33,15 +34,15 @@
 
 
 def log_a_message(
     logger: str,
     criticality: str,
     message: str,
     level: int,
-    monitor: str = None,
+    monitor: str | None = None,
     log_in_db: bool = False,
 ):
     log = core.get_logger(logger)
     if log is None:
         raise AlphaException(f"No {logger=} found")
     if hasattr(log, criticality):
         getattr(log, criticality)(
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/mail_lib.py` & `alphaz-0.7.6.3/alphaz/libs/mail_lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import smtplib, socks, copy, json
-from typing import List
+
 
 import hashlib, re, os, datetime
 from flask import current_app
 from flask_mail import Message
 
 import uuid
 
@@ -11,264 +11,309 @@
 
 from . import string_lib
 from ..models.config._utils import get_mails_parameters
 
 from ..models.api import _utils
 
 # CORE
-from core import core 
+from core import core
 
-REQUIRED_PARAMETERS         = ['mail']
-KEY_SIGNATURE               = core.api.get_config("mails/key_signature") # '<alpha mail>' 
-MAIL_PARAMETERS_PATTERN     = "[[%s]]"
+REQUIRED_PARAMETERS = ["mail"]
+KEY_SIGNATURE = core.api.get_config("mails/key_signature")  # '<alpha mail>'
+MAIL_PARAMETERS_PATTERN = "[[%s]]"
 
 DB = core.db
 API = core.api
 
-def mail2(to_mails,subject,body,bodyHtml=None,attachments=[]):
+
+def mail2(to_mails, subject, body, bodyHtml=None, attachments=[]):
     import win32com.client as win32
-    outlook = win32.Dispatch('outlook.application')
+
+    outlook = win32.Dispatch("outlook.application")
     mail = outlook.CreateItem(0)
     mail.To = to_mails
     mail.Subject = subject
     mail.Body = body
-    mail.HTMLBody = bodyHtml if bodyHtml is not None else body #this field is optional
+    mail.HTMLBody = bodyHtml if bodyHtml is not None else body  # this field is optional
 
     # To attach a file to the email (optional):
     if len(attachments) != 0:
-    #attachment  = "Path to the attachment"
+        # attachment  = "Path to the attachment"
         for attachment in attachments:
             mail.Attachments.Add(attachment)
 
     mail.Send()
 
-def mail(to_mails,from_mails,proxy_host, proxy_port):
+
+def mail(to_mails, from_mails, proxy_host, proxy_port):
     receivers = [to_mails]
 
     message = """From: From Person <from@fromdomain.com>
     To: To Person <to@todomain.com>
     Subject: SMTP e-mail test
 
     This is a test e-mail message.
     """
-    
+
     if proxy_host is not None:
         socks.setdefaultproxy(socks.HTTP, proxy_host, proxy_port)
     socks.wrapmodule(smtplib)
 
     try:
-       smtpObj = smtplib.SMTP('SMTP.office365.com')
-       smtpObj.sendmail(from_mails, receivers, message)         
-       print ("Successfully sent email")
+        smtpObj = smtplib.SMTP("SMTP.office365.com")
+        smtpObj.sendmail(from_mails, receivers, message)
+        print("Successfully sent email")
     except Exception as ex:
-       print ("Error: unable to send email: ",ex)
-    
+        print("Error: unable to send email: ", ex)
+
+
 def get_mail_type(raw_mail_url):
-    if 'mail-content=' in raw_mail_url:
-        raw_mail_url = raw_mail_url.split('mail-content=')[1]
-    if '&' in raw_mail_url:
-        raw_mail_url = raw_mail_url.split('&')[0]
+    if "mail-content=" in raw_mail_url:
+        raw_mail_url = raw_mail_url.split("mail-content=")[1]
+    if "&" in raw_mail_url:
+        raw_mail_url = raw_mail_url.split("&")[0]
     return raw_mail_url
 
+
 """ MAILS """
-def get_mail_content(mail_root, mail_type,log):
+
+
+def get_mail_content(mail_root, mail_type, log):
     content = ""
     if not mail_root[-1] == os.sep:
         mail_root = mail_root + os.sep
 
-    raw         = mail_type.split('?')[0]
-    parameters  = {}
-    if len(mail_type.split('?')) != 1:
-        for el in mail_type.split('?')[1].split('&'):
-            key, value = el.split('=')[0], el.split('=')[1]
+    raw = mail_type.split("?")[0]
+    parameters = {}
+    if len(mail_type.split("?")) != 1:
+        for el in mail_type.split("?")[1].split("&"):
+            key, value = el.split("=")[0], el.split("=")[1]
             parameters[key] = value
 
     mail_path = mail_root + raw
 
     if os.path.exists(mail_path):
         with open(mail_path) as f:
-            content  = f.read()
+            content = f.read()
 
         for key, value in parameters.items():
-            file_name  = mail_root + value + '.html'
-            div_block  = r'<div id="%s">[^\<\>]*<\/div>'%key
-            regex_find = re.findall(div_block,content)
+            file_name = mail_root + value + ".html"
+            div_block = r'<div id="%s">[^\<\>]*<\/div>' % key
+            regex_find = re.findall(div_block, content)
 
             if len(regex_find) != 0:
                 result = regex_find[0]
             else:
-                log.error('Mail content is incorrect for %s, cannot div block by %s content (regex expression not matched: %s )'%(mail_path,file_name,div_block))
+                log.error(
+                    "Mail content is incorrect for %s, cannot div block by %s content (regex expression not matched: %s )"
+                    % (mail_path, file_name, div_block)
+                )
                 return None
 
             with open(file_name) as f:
-                div_content  = f.read()
-            content = content.replace(result,div_content)
+                div_content = f.read()
+            content = content.replace(result, div_content)
     else:
-        log.error('Cannot find mail content at %s'%mail_path)
+        log.error("Cannot find mail content at %s" % mail_path)
         return None
 
-    script_starts = [m.start() for m in re.finditer('<script', content)]
-    script_ends   = [m.start() for m in re.finditer('</script>', content)]
+    script_starts = [m.start() for m in re.finditer("<script", content)]
+    script_ends = [m.start() for m in re.finditer("</script>", content)]
 
     script_blocks = []
     for i in range(len(script_starts)):
-        script_blocks.append(content[script_starts[i]:script_ends[i] + len('</script>')])
+        script_blocks.append(
+            content[script_starts[i] : script_ends[i] + len("</script>")]
+        )
 
     for script_block in script_blocks:
-        content = content.replace(script_block,'')
+        content = content.replace(script_block, "")
 
-    with open(mail_root + os.sep + 'generated_mail.html','w') as f:
+    with open(mail_root + os.sep + "generated_mail.html", "w") as f:
         f.write(content)
 
     return content
 
+
 def get_mail_token(key):
-    salt        = "%ThisIsGolliath38Pepper$"
+    salt = "%ThisIsGolliath38Pepper$"
     hash_string = key + salt
-    hashed      = hashlib.sha256(hash_string.encode()).hexdigest()
+    hashed = hashlib.sha256(hash_string.encode()).hexdigest()
     return hashed
 
-def is_mail_token_valid(key,token):
+
+def is_mail_token_valid(key, token):
     hashed = get_mail_token(key)
     return hashed == token
 
-def get_title(content,default=''):
-    title_regex = r'<title[^>]*>([^<]+)</title>'
-    regex_find = re.findall(title_regex,content)
+
+def get_title(content, default=""):
+    title_regex = r"<title[^>]*>([^<]+)</title>"
+    regex_find = re.findall(title_regex, content)
 
     if len(regex_find) != 0:
         result = regex_find[0]
     else:
-        result = default if default is not None else ''
+        result = default if default is not None else ""
     return result
 
-def set_parameters(content,parameters):
+
+def set_parameters(content, parameters):
     for parameter, value in parameters.items():
         if value is not None:
-            content = content.replace(MAIL_PARAMETERS_PATTERN%parameter,str(value))
+            content = content.replace(MAIL_PARAMETERS_PATTERN % parameter, str(value))
     return content
 
+
 def add_mail_classic_parameter(parameters):
-    now     = datetime.datetime.now()
-    year    = now.year
-    month   = now.month
-    hour    = now.hour
-    minute  = now.minute
-    second  = now.second
+    now = datetime.datetime.now()
+    year = now.year
+    month = now.month
+    hour = now.hour
+    minute = now.minute
+    second = now.second
 
     classic_parameters = {
-        'year':year,
-        'month':month,
-        'hour':hour,
-        'minute':minute,
-        'second':second,
-        'uuid': str(uuid.uuid4()),
-        'mail_token': get_mail_token(parameters['mail'])
+        "year": year,
+        "month": month,
+        "hour": hour,
+        "minute": minute,
+        "second": second,
+        "uuid": str(uuid.uuid4()),
+        "mail_token": get_mail_token(parameters["mail"]),
     }
 
     for key, value in classic_parameters.items():
         if not key in parameters:
             parameters[key] = value
     return parameters
 
-def update_mail_content(content,mail_url,parameters,parameters_to_specify,log):
-    parameters_to_keep          = {}
+
+def update_mail_content(content, mail_url, parameters, parameters_to_specify, log):
+    parameters_to_keep = {}
     for required_parameter in REQUIRED_PARAMETERS:
         if not required_parameter in parameters.keys():
-            log.error('Missing parameter <%s> for sending mail !'%required_parameter)
+            log.error("Missing parameter <%s> for sending mail !" % required_parameter)
             return content, False, parameters_to_keep
 
-    parameters                  = add_mail_classic_parameter(parameters)
-    parameters['configuration'] = get_mail_type(mail_url)
+    parameters = add_mail_classic_parameter(parameters)
+    parameters["configuration"] = get_mail_type(mail_url)
 
     raw_parameters = copy.copy(parameters)
     for key, value in raw_parameters.items():
         for k, v in parameters.items():
-            if MAIL_PARAMETERS_PATTERN%key in str(v):
-                parameters[k] = v.replace(MAIL_PARAMETERS_PATTERN%key,value)
+            if MAIL_PARAMETERS_PATTERN % key in str(v):
+                parameters[k] = v.replace(MAIL_PARAMETERS_PATTERN % key, value)
 
     for key, value in parameters.items():
-        if MAIL_PARAMETERS_PATTERN%key in parameters_to_specify:
+        if MAIL_PARAMETERS_PATTERN % key in parameters_to_specify:
             parameters_to_keep[key] = value
 
-    content                     = set_parameters(content,parameters_to_keep)
+    content = set_parameters(content, parameters_to_keep)
 
-    parameters_not_specified    = list(set(get_mails_parameters(content)))
+    parameters_not_specified = list(set(get_mails_parameters(content)))
 
     if len(parameters_not_specified) != 0:
-        log.error('Missing parameters %s for mail "%s"'%(','.join(parameters_not_specified),mail_url))
+        log.error(
+            'Missing parameters %s for mail "%s"'
+            % (",".join(parameters_not_specified), mail_url)
+        )
         return content, False, parameters_to_keep
 
     """if not valid_signature:
         log.error('Invalid mail signature !')
         return False"""
 
     return content, True, parameters_to_keep
 
-def get_mail_content_for_parameters(mail_path,mail_url,parameters_list,log):
-    if not 'template' in mail_url:
-        mail_url = 'template.html?mail-content=' + mail_url
 
-    if log: 
-        log.debug('Getting mail at %s/%s'%(mail_path,mail_url))
+def get_mail_content_for_parameters(mail_path, mail_url, parameters_list, log):
+    if not "template" in mail_url:
+        mail_url = "template.html?mail-content=" + mail_url
+
+    if log:
+        log.debug("Getting mail at %s/%s" % (mail_path, mail_url))
 
-    content                 = get_mail_content(mail_path,mail_url,log)
+    content = get_mail_content(mail_path, mail_url, log)
     if content is None:
         return []
-    parameters_to_specify   = get_mails_parameters(content)
+    parameters_to_specify = get_mails_parameters(content)
 
-    #valid_signature         = KEY_SIGNATURE in str(content) 
+    # valid_signature         = KEY_SIGNATURE in str(content)
 
     mail_contents_list = []
-    for parameters in parameters_list:        
-        mail_contents_dict                      = {'content':None,'parameters':None,'valid':False}
-        out_content, valid, pars                = update_mail_content(content,mail_url,parameters,parameters_to_specify,log)
-        
-        mail_contents_dict['content']           = out_content
-        mail_contents_dict['parameters']        = pars
-        mail_contents_dict['raw_parameters']    = parameters
-        mail_contents_dict['valid']             = valid
+    for parameters in parameters_list:
+        mail_contents_dict = {"content": None, "parameters": None, "valid": False}
+        out_content, valid, pars = update_mail_content(
+            content, mail_url, parameters, parameters_to_specify, log
+        )
+
+        mail_contents_dict["content"] = out_content
+        mail_contents_dict["parameters"] = pars
+        mail_contents_dict["raw_parameters"] = parameters
+        mail_contents_dict["valid"] = valid
         mail_contents_list.append(mail_contents_dict)
     return mail_contents_list
 
-def __send_mail(mail_path,mail_type,parameters_list,sender,log,force:bool=False):
-    mail_contents_list = get_mail_content_for_parameters(mail_path,mail_type,parameters_list,log)
 
-    for config in mail_contents_list:        
-        if not force and is_mail_already_send(DB,mail_type,config['parameters'],log=log):
-            log.error('Mail already sent %s'%config)
+def __send_mail(
+    mail_path, mail_type, parameters_list, sender, log, force: bool = False
+):
+    mail_contents_list = get_mail_content_for_parameters(
+        mail_path, mail_type, parameters_list, log
+    )
+
+    for config in mail_contents_list:
+        if not force and is_mail_already_send(
+            DB, mail_type, config["parameters"], log=log
+        ):
+            log.error("Mail already sent %s" % config)
             return False
 
-        if is_blacklisted(DB,config['raw_parameters']['mail'],mail_type):
-            log.error('Mail adress <%s> blacklisted %s'%config['raw_parameters']['mail'])
+        if is_blacklisted(DB, config["raw_parameters"]["mail"], mail_type):
+            log.error(
+                "Mail adress <%s> blacklisted %s" % config["raw_parameters"]["mail"]
+            )
             return False
 
         # Send mail
-        msg     = Message(config['raw_parameters']['title'],
-                    sender=sender,
-                    recipients=[config['raw_parameters']['mail']])
-        msg.html = config['content']
+        msg = Message(
+            config["raw_parameters"]["title"],
+            sender=sender,
+            recipients=[config["raw_parameters"]["mail"]],
+        )
+        msg.html = config["content"]
         current_app.extensions["mail"].send(msg)
-        #api.mail.send(msg)
+        # api.mail.send(msg)
 
         # insert in history
-        mail_type   = get_mail_type(mail_type)
+        mail_type = get_mail_type(mail_type)
         if not force:
-            set_mail_history(DB,mail_type,config['raw_parameters']['uuid'],config['parameters'],log=log)
-        log.info('Sending mail to %s'%config['raw_parameters']['mail'])
+            set_mail_history(
+                DB,
+                mail_type,
+                config["raw_parameters"]["uuid"],
+                config["parameters"],
+                log=log,
+            )
+        log.info("Sending mail to %s" % config["raw_parameters"]["mail"])
     return True
 
-def send_mail(mail_config:str, parameters_list:List[dict]=None, sender=None, force:bool=False):
+
+def send_mail(
+    mail_config: str,
+    parameters_list: list[dict] = None,
+    sender=None,
+    force: bool = False,
+):
     # Configuration
     main_mail_config = API.get_config(["mails"])
     config = API.get_config(["mails", "configurations", mail_config])
     if config is None or type(config) != dict:
-        API.log.error(
-            f'Missing "{config}" mail configuration in "{API.config_path}"'
-        )
+        API.log.error(f'Missing "{config}" mail configuration in "{API.config_path}"')
         return False
 
     # Parameters
     root_config = copy.copy(main_mail_config["parameters"])
     for key, parameter in main_mail_config["parameters"].items():
         root_config[key] = parameter
 
@@ -310,54 +355,65 @@
         )
         _utils.merge_configuration(
             full_parameters, source_configuration=parameters, replace=True
         )
 
         full_parameters_list.append(full_parameters)
     mail_path = API.get_config("mails/path")
-    
+
     valid = __send_mail(
         mail_path=mail_path,
         mail_type=config["mail_type"],
         parameters_list=full_parameters_list,
         sender=sender,
         log=API.log,
-        force=force
+        force=force,
     )
     if not valid:
         API.set_error("mail_error")
     return valid
 
-def set_mail_history(db, mail_type,uuidValue,parameters,log=None):
-    mail_type           = get_mail_type(mail_type)
-    unique_parameters   = get_unique_parameters(parameters)
+
+def set_mail_history(db, mail_type, uuidValue, parameters, log=None):
+    mail_type = get_mail_type(mail_type)
+    unique_parameters = get_unique_parameters(parameters)
     return db.add(MailHistory(uuidValue, mail_type, unique_parameters, parameters))
 
+
 def get_unique_parameters(parameter):
     unique_parameters = {}
     for key, value in parameter.items():
-        if key[0:5] != 'page_': #TODO: check
+        if key[0:5] != "page_":  # TODO: check
             unique_parameters[key] = value
     return unique_parameters
 
-def is_mail_already_send(db,mail_type,parameters,log=None):
+
+def is_mail_already_send(db, mail_type, parameters, log=None):
     from ..models.database import main_definitions as defs
-    mail_type           = get_mail_type(mail_type)
-    unique_parameters   = get_unique_parameters(parameters)
 
-    results             = db.select(defs.MailHistory,filters=[
-        defs.MailHistory.mail_type==mail_type,
-        defs.MailHistory.parameters==json.dumps(unique_parameters)
-    ],json=True)
-    return len(results) != 0
+    mail_type = get_mail_type(mail_type)
+    unique_parameters = get_unique_parameters(parameters)
 
-def is_blacklisted(db,user_mail,mail_type,log=None):
-    from ..models.database import main_definitions as defs
-    mail_type   = get_mail_type(mail_type)
-    results             = db.select(defs.MailBlacklist,filters=[
-        defs.MailBlacklist.mail_type==mail_type,
-        defs.MailBlacklist.mail==user_mail
-    ],json=True)
+    results = db.select(
+        defs.MailHistory,
+        filters=[
+            defs.MailHistory.mail_type == mail_type,
+            defs.MailHistory.parameters == json.dumps(unique_parameters),
+        ],
+        json=True,
+    )
     return len(results) != 0
 
 
+def is_blacklisted(db, user_mail, mail_type, log=None):
+    from ..models.database import main_definitions as defs
 
+    mail_type = get_mail_type(mail_type)
+    results = db.select(
+        defs.MailBlacklist,
+        filters=[
+            defs.MailBlacklist.mail_type == mail_type,
+            defs.MailBlacklist.mail == user_mail,
+        ],
+        json=True,
+    )
+    return len(results) != 0
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/notifications_lib.py` & `alphaz-0.7.6.3/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/number_lib.py` & `alphaz-0.7.6.3/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/process_lib.py` & `alphaz-0.7.6.3/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/py_lib.py` & `alphaz-0.7.6.3/alphaz/libs/py_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import sys, imp, inspect, os, glob, re
-import typing
 
+from typing import OrderedDict
 from ..models.watcher import ModuleWatcher
-from typing import List, Dict, OrderedDict
 
 myself = lambda: inspect.stack()[1][3]
 
 
-def get_modules_infos(name: str = None, url: str = None, mode:str=None):
+def get_modules_infos(
+    name: str | None = None, url: str | None = None, mode: str = None
+):
     from importlib_metadata import version
     import pkgutil
 
     data = {}
     for item in pkgutil.iter_modules():
         if name is not None and name.lower() != item.name.lower():
             continue
-        if item.module_finder.path.endswith('.'):
+        if item.module_finder.path.endswith("."):
             continue
         try:
             data[item.name] = version(item.name)
         except:
             continue
 
     if url:
@@ -76,15 +77,15 @@
                 updates["local_down"].append(f"{key}=={data_url[key]}")
                 updates["distant_up"].append(f"{key}=={data[key]}")
 
         for key, items in updates.items():
             out[key] = " ".join(items)
         return out
     if mode == "requirements":
-        return '\n'.join([f"{x}=={y}"for x,y in data.items()])
+        return "\n".join([f"{x}=={y}" for x, y in data.items()])
     return data
 
 
 def myself(fct=None):
     name = inspect.stack()[1][3]
     if fct:
         name = fct(name)
@@ -181,16 +182,16 @@
 
 
 def filter_kwargs(fct, args: list = [], kwargs: dict = {}) -> dict:
     """Remove kwargs that are not in function kwargs
 
     Args:
         fct ([type]): [description]
-        args (List): [description]
-        kwargs (Dict): [description]
+        args (list): [description]
+        kwargs (dict): [description]
 
     Returns:
         [type]: [description]
     """
     fargs = inspect.getfullargspec(fct)
     kwargs = {x: y for x, y in kwargs.items() if x in fargs.args}
     return kwargs
@@ -240,21 +241,21 @@
 
 
 def sort_by_key(input_dict):
     return OrderedDict(sorted(input_dict.items(), key=lambda x: x[0]))
 
 
 def compare_dicts(
-    dict_obj_1, dict_obj_2, sub_elements: dict = None, ignore: List[str] = None
+    dict_obj_1, dict_obj_2, sub_elements: dict = None, ignore: list[str] = None
 ):
     if not sub_elements:
         sub_elements = {}
 
     level_dict = {}
-    
+
     if dict_obj_1 is None and dict_obj_2 is None:
         return None
     if dict_obj_1 is None or dict_obj_2 is None:
         list_keys = list(dict_obj_1.keys() if dict_obj_2 is None else dict_obj_2.keys())
     else:
         list_keys = list(set(dict_obj_1.keys()).union(set(dict_obj_2.keys())))
     list_keys.sort()
@@ -347,8 +348,8 @@
         iter(o)
         return True
     except:
         return False
 
 
 def is_list(o):
-    return type(o) == list or is_subtype(type(o), typing.List) or type(o) == tuple
+    return type(o) == list or is_subtype(type(o), list) or type(o) == tuple
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/scp_lib.py` & `alphaz-0.7.6.3/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/search_lib.py` & `alphaz-0.7.6.3/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/secure_lib.py` & `alphaz-0.7.6.3/alphaz/libs/secure_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import secrets
 from html import entities
 from bcrypt import hashpw, gensalt, checkpw
 from random import randint
-from typing import List, Union
+
 from base64 import (
     b64decode,
     b64encode,
     urlsafe_b64encode as b64e,
     urlsafe_b64decode as b64d,
 )
 
@@ -26,15 +26,15 @@
     Returns:
         The hashed password as a string.
     """
     password_hashed = hashpw(password.encode("utf-8"), gensalt())
     return password_hashed.decode("utf-8")
 
 
-def compare_passwords(password: str, hash_saved: str) -> bool:
+def compare_passwords(password: str | None, hash_saved: str) -> bool:
     """
     Compare a password to a saved hash to see if they match.
 
     Args:
         password: The password to compare.
         hash_saved: The saved hash to compare the password to.
 
@@ -54,15 +54,15 @@
 
     Returns:
         A URL-safe token as a string.
     """
     return secrets.token_urlsafe(45)
 
 
-def get_keys_numbers(key: str) -> list[int]:
+def get_keys_numbers(key: str) -> list[str]:
     """
     Get a list of the numbers that make up the sum of the ASCII values of the characters in the given key.
 
     Args:
         key: The key to process.
 
     Returns:
@@ -83,15 +83,15 @@
         key: A string representing the key to use for generating the cry operation code.
 
     Returns:
         A string representing the cry operation code.
     """
     keys_numbers = get_keys_numbers(key)
 
-    values: List[str] = []
+    values: list[str] = []
     for _ in range(5):
         value = "".join([str(randint(100, 999)) + x for x in keys_numbers])
         complement = "".join([str(9 - int(x)) for x in value[3:]])
         values.append(value + complement)
 
     return "-".join(values)
 
@@ -162,15 +162,15 @@
     return b64e(
         b"%b%b%b"
         % (salt, iterations.to_bytes(4, "big"), b64d(Fernet(key).encrypt(message)),)
     ).decode("utf-8")"""
 
 
 def password_encrypt(
-    message: Union[str, bytes], password: str, iterations: int = 100_000
+    message: str | bytes, password: str, iterations: int = 100_000
 ) -> str:
     """
     Encrypt a message with a password.
 
     Args:
         message: A byte string or a string to be encrypted.
         password: A string representing the password.
@@ -196,15 +196,15 @@
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
     key = _derive_key(password.encode(), salt, iterations)
     return Fernet(key).decrypt(token).decode("utf-8")
 """
 
 
-def password_decrypt(token: Union[str, bytes], password: str) -> bytes:
+def password_decrypt(token: str | bytes, password: str) -> bytes:
     """
     Decrypt a message with a password.
 
     Args:
         token: A byte string or a string representing the encrypted message.
         password: A string representing the password.
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/soap_lib.py` & `alphaz-0.7.6.3/alphaz/libs/soap_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-import requests, operator, time
-from requests import Session, get
-import os
+import operator, time
+from requests import Session
 from zeep import Client
 from zeep.transports import Transport
 
 proxies = {"http": "165.225.76.32:80", "https": "165.225.76.32:80"}
 
 cert_path = "merged-CA.pem"
 import operator
 import time
-from typing import Dict, Optional, Union
 
 from requests import Session
 from zeep import Client
 from zeep.transports import Transport
 
 
 def get_wsdl_response(
     base: str,
     wsdl: str,
     method: str,
-    parameters: Dict[str, str],
-    use_cert: Optional[bool] = False,
-    cert_path: Optional[str] = None,
-    use_proxy: Optional[bool] = False,
-    proxies: Optional[Dict[str, str]] = None,
-    log: Optional[object] = None,
-) -> Optional[Union[str, int, float]]:
+    parameters: dict[str, str],
+    use_cert: bool | None = False,
+    cert_path: str | None = None,
+    use_proxy: bool | None = False,
+    proxies: dict[str, str] | None = None,
+    log: object | None = None,
+) -> str | int | float | None:
     """
     Call a SOAP method and return the response.
 
     Args:
         base: The base URL for the SOAP service.
         wsdl: The path to the WSDL file.
         method: The name of the SOAP method to call.
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/ssh_lib.py` & `alphaz-0.7.6.3/alphaz/libs/ssh_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # MODULES
-from threading import current_thread
-import encodings, scp, re, datetime, os
-from typing import Dict, List
-
+import scp, re, datetime, os
 import warnings
 from cryptography.utils import CryptographyDeprecationWarning
 
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=CryptographyDeprecationWarning)
     import paramiko
 
@@ -34,15 +31,15 @@
         The standardized string.
     """
     if not isinstance(content, str):
         content = content.decode("utf-8")
     return content.replace("\\r\\n", "\n").replace("\\r\n", "\n").replace("\\t", "\t")
 
 
-def process_content(content: str, parameters: Dict[str, object] = None) -> str:
+def process_content(content: str, parameters: dict[str, object] | None = None) -> str:
     """
     Process the content of a string.
 
     If the string starts with "file:", the rest of the string is interpreted as a file path and the contents of the file
     are read and returned. If `parameters` is not None, the function replaces occurrences of "{{key}}" in the content
     string with the corresponding value in `parameters`.
 
@@ -123,30 +120,30 @@
         )
 
     def wait(self):
         ssh_stdin, ssh_stdout, ssh_stderr = self.ssh.exec_command("")
         while not ssh_stdout.channel.exit_status_ready():
             pass
 
-    def list_files(self, directory: str) -> List[AlphaFile]:
+    def list_files(self, directory: str) -> list[AlphaFile]:
         """[summary]
 
         Args:
             directory (str): [description]
 
         Returns:
-            List[AlphaFile]: [description]
+            list[AlphaFile]: [description]
         """
         output = self.execute_cmd(f"ls -l {directory}")
         files = io_lib.get_list_file(output)
         return files
 
     def list_files_names(
-        self, directory: str, pattern: str = None, hidden: bool = False
-    ) -> List[str]:
+        self, directory: str, pattern: str | None = None, hidden: bool = False
+    ) -> list[str]:
         cmd = "ls -l -f %s" % directory
         output = self.execute_cmd(cmd)
         lines = str(output).split()
         if pattern is not None:
             """filtered = []
             for line in lines:
                 matchs = re.findall(pattern,line)
@@ -159,28 +156,28 @@
                 x
                 for x in lines
                 if x.replace(".", "") != "" and (not "." in x or x.startswith("."))
             ]
         else:
             return [x for x in lines if x.replace(".", "") != "" and not "." in x]
 
-    def list_directories(self, directory: str) -> List[AlphaFile]:
+    def list_directories(self, directory: str) -> list[AlphaFile]:
         """[summary]
 
         Args:
             directory (str): [description]
 
         Returns:
-            List[AlphaFile]: [description]
+            list[AlphaFile]: [description]
         """
         output = self.execute_cmd("ls -l %s" % directory)
         directories = io_lib.get_list_file(output)
         return directories
 
-    def list_directories_names(self, directory: str, hidden: bool = False) -> List[str]:
+    def list_directories_names(self, directory: str, hidden: bool = False) -> list[str]:
         output = self.execute_cmd("ls -l -f %s" % directory)
         lines = str(output).split()
         if hidden:
             return [
                 x
                 for x in lines
                 if x.replace(".", "") != "" and (not "." in x or x.startswith("."))
@@ -194,32 +191,44 @@
         output = self.execute_cmd(f"cat {filepath}", decode=decode)
         return standardize_content(output) if escape_replace else output
 
     def is_file(self, filename: str):
         output = self.execute_cmd("test -f %s && echo 'y'" % filename)
         return "y" in output
 
-    def is_directory(self, path: str, group: str = None, user: str = None, mode=None):
+    def is_directory(
+        self,
+        path: str,
+        group: str | None = None,
+        user: str | None = None,
+        mode=None,
+    ):
         return self.is_dir(path=path, group=group, user=user, mode=mode)
 
-    def is_dir(self, path: str, group: str = None, user: str = None, mode=None):
+    def is_dir(
+        self,
+        path: str,
+        group: str | None = None,
+        user: str | None = None,
+        mode=None,
+    ):
         output = self.execute_cmd("test -d %s && echo 'y'" % path)
         if group is not None and not self.is_group(group, path):
             return False
         if user is not None and not self.is_user(user, path):
             return False
         if mode is not None and not self.is_mode(mode, path):
             return False
         return "y" in output
 
     def make_directory(
         self,
         path: str,
-        group: str = None,
-        user: str = None,
+        group: str | None = None,
+        user: str | None = None,
         mode=None,
         ensure_path: bool = True,
     ):
         options = ""
         if ensure_path:
             options = "-p"
         if not self.is_dir(path):
@@ -293,15 +302,15 @@
         content = process_content(content)
         original_content = self.get_file_content(path, decode=True)
         return content in original_content
 
     def restart_service(self, service: str):
         self.execute_cmd("sudo systemctl restart %s" % service)
 
-    def is_equal_to_file(self, content: str, path: str, mode: int = None):
+    def is_equal_to_file(self, content: str, path: str, mode: int | None = None):
         if not self.is_file(path):
             return False
 
         if mode is not None:
             self.change_mode(mode, path)
 
         content = process_content(content)
@@ -341,15 +350,15 @@
         return self.is_file(path)
 
     def write_to_file(
         self,
         content: str,
         path: str,
         ensure_path: bool = True,
-        parameters: Dict[str, object] = None,
+        parameters: dict[str, object] = None,
     ) -> bool:
         if ensure_path:
             self.make_directory(os.path.dirname(path))
 
         if content.startswith("file:"):  # TODO: remove
             content_path = content.replace("file:", "")
             self.scp.put(content_path, path)
@@ -385,26 +394,26 @@
         valid_version = eval(cmd)
         return valid_version
 
     def is_output(self, cmd: str):
         output = self.execute_cmd(cmd)
         return len(output.replace("\\n", "").replace("\\r", "").strip()) != 0
 
-    def is_found(self, cmd: str, greps: List[str] = []):
+    def is_found(self, cmd: str, greps: list[str] = []):
         if type(greps) == str:
             greps = [greps]
         cmd = cmd + " | " + " | ".join(['grep "%s"' % x for x in greps])
         output = self.execute_cmd(cmd, lines=True)
         if "illegal" in output[0]:
             return False
         if len(output) == 1 and output[0].strip() == "":
             return False
         return len(output) != 0
 
-    def get_pid(self, greps: List[str] = []):
+    def get_pid(self, greps: list[str] = []):
         if type(greps) == str:
             greps = [greps]
         cmd = "ps aux -P | " + " | ".join(['grep "%s"' % x for x in greps])
         output = self.execute_cmd(cmd, lines=True)
         if len(output) == 0:
             return None
         if len(output) == 1:
@@ -450,27 +459,27 @@
         cmd = "which python"
         output = self.execute_cmd(cmd)
         cmd = "python -c 'import %s'" % module
         output = self.execute_cmd(cmd)
         valid = not ("No module named " in output and module in output)
         return valid
 
-    def install_python_module(self, module: str, version: str = None):
+    def install_python_module(self, module: str, version: str | None = None):
         cmd = "which pip"
         output = self.execute_cmd(cmd)
         cmd = f"yes | pip install {module}{version}"
         output = self.execute_cmd(cmd)
         return not "error" in output
 
     def add_user(
         self,
         user: str,
-        description: str = None,
-        group: str = None,
-        password: str = None,
+        description: str | None = None,
+        group: str | None = None,
+        password: str | None = None,
     ):
         options = ""
         if description is not None:
             options += ' -c "%s"' % description
         cmd = "sudo useradd %s %s" % (options, user)
         self.execute_cmd(cmd)
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/string_lib.py` & `alphaz-0.7.6.3/alphaz/libs/string_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re, string, chardet, unicodedata, encodings, warnings
-from typing import Any, Dict, List, Tuple
 
 import hashlib
 
 
 def is_number(txt: str) -> bool:
     """
     Check if a string is a number.
@@ -59,15 +58,15 @@
 
     Returns:
         True if the string contains special characters, False otherwise.
     """
     return re.search(r"[@_!#$%^&*()<>?/\|}{~:]", test) is not None
 
 
-def get_words(txt: str) -> List[str]:
+def get_words(txt: str) -> list[str]:
     """
     Extract words from text and filter out noise.
 
     The function removes parentheses and their contents, and then filters out words that contain specific characters
     or are on a list of common but meaningless words.
 
     Args:
@@ -122,15 +121,15 @@
                 results[encoding_method] = txt.decode(encoding_method)
             except:
                 pass
     return results
 """
 
 
-def universal_decode(txt: bytes) -> Tuple[str, str]:
+def universal_decode(txt: bytes) -> tuple[str, str]:
     """
     Decode bytes using the detected encoding.
 
     This function attempts to decode the given bytes using the detected encoding,
     which is determined using the `detect` method from the `chardet` library.
 
     Args:
@@ -144,15 +143,15 @@
     try:
         result = txt.decode(encoding)
     except:
         pass
     return result, encoding
 
 
-def universal_decodes(txts: List[bytes]) -> Dict[str, str]:
+def universal_decodes(txts: list[bytes]) -> dict[str, str]:
     """
     Decode a list of bytes using the detected encoding for each.
 
     This function attempts to decode each of the given bytes using the detected encoding,
     which is determined using the `detect` method from the `chardet` library.
 
     Args:
@@ -254,16 +253,16 @@
             else:
                 d[i][j] = min(d[i - 1][j], d[i][j - 1], d[i - 1][j - 1]) + 1
 
     return d[m][n]
 
 
 def found_best_match(
-    word: str, words: List[str], threshold: float = None
-) -> Tuple[str, float]:
+    word: str, words: list[str], threshold: float = None
+) -> tuple[str, float]:
     """
     Find the word in a list of words that has the best match with a given word.
 
     The match is calculated as the ratio between the number of letters that match and the difference in length between
     the two words. The resulting match values are compared and the word with the highest match value is returned.
 
     Args:
@@ -284,15 +283,15 @@
     ]
     max_value = max(match_values)
     if threshold is not None and max_value < threshold:
         return None, max_value
     return words[match_values.index(max_value)], max_value
 
 
-def to_list(o: str) -> List[str]:
+def to_list(o: str) -> list[str]:
     """
     Convert a string representation of a list to a list of strings.
 
     The input string should be a comma-separated list of values, optionally enclosed in square brackets. String values
     may be enclosed in either single or double quotes.
 
     Args:
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/test_lib.py` & `alphaz-0.7.6.3/alphaz/libs/test_lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # MODULES
-from .. import os, defaultdict, List, Dict, timer
+from .. import os, defaultdict, timer
 
 # LIBS
 from . import io_lib, py_lib
 
 # MODELS
-from ..models.tests import TestGroup, AlphaTest, test, TestCategories, Levels
+from ..models.tests import TestGroup, AlphaTest, TestCategories, Levels
 
 # CORE
 from core import core
 
 LOG = core.get_logger("tests")
 
 CATEGORIES = {}
 
 
 def __group_parameters(
-    name: str = None,
-    names: List[str] = [],
-    group: str = None,
-    groups: List[str] = [],
-    category: str = None,
-    categories: List[str] = [],
+    name: str | None = None,
+    names: list[str] = [],
+    group: str | None = None,
+    groups: list[str] = [],
+    category: str | None = None,
+    categories: list[str] = [],
 ):
     categories = categories if categories is not None else []
     groups = groups if groups is not None else []
     names = names if names is not None else []
 
     if category is not None:
         categories.append(category)
@@ -37,19 +37,19 @@
     groups = [x.strip() for x in groups]
     names = [x.strip() for x in names]
     return categories, groups, names
 
 
 def process_test_categories(
     categories,
-    groups: List[str] = [],
-    names: List[str] = [],
-    levels: List[Levels] = [],
+    groups: list[str] = [],
+    names: list[str] = [],
+    levels: list[Levels] = [],
     run: bool = False,
-    coverage: str = None,
+    coverage: str | None = None,
     load_from_db: bool = True,
     stop: bool = True,
 ):
     subclasses = AlphaTest.__subclasses__()
     subclasses_by_module = defaultdict(list)
     for subclass in subclasses:
         module_name = subclass.__module__.split(".")[0]
@@ -79,33 +79,33 @@
     if run:
         test_categories.test_all(names, levels, stop=stop)
 
     return test_categories
 
 
 def get_tests_auto(
-    name: str = None,
-    names: List[str] = [],
-    group: str = None,
-    groups: List[str] = [],
-    category: str = None,
-    categories: List[str] = [],
-    file_path: str = None,
+    name: str | None = None,
+    names: list[str] = [],
+    group: str | None = None,
+    groups: list[str] = [],
+    category: str | None = None,
+    categories: list[str] = [],
+    file_path: str | None = None,
     run: bool = False,
     load_from_db: bool = False,
-    report: str = None,
-    coverage: str = None,
-    levels: List[Levels] = [],
+    report: str | None = None,
+    coverage: str | None = None,
+    levels: list[Levels] = [],
     stop: bool = True,
 ) -> TestCategories:
     """Get the TestCategories class, containings all required tests.
 
     Args:
-        tests_modules (List[str]): list of test modules path
-        tests_modules (List[str]): list of test modules path
+        tests_modules (list[str]): list of test modules path
+        tests_modules (list[str]): list of test modules path
         name (str, optional): the name of the test to select. Defaults to None.
         group (str, optional): the name of the group to select. Defaults to None.
         category (str, optional): the name of the category to select. Defaults to None.
 
     Returns:
         TestCategories: [description]
     """
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/time_lib.py` & `alphaz-0.7.6.3/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/libs/user_lib.py` & `alphaz-0.7.6.3/alphaz/libs/user_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from core import core
 
 DB = core.db
 
 # MODULES
 import datetime
 from sqlalchemy.orm import sessionmaker
-from typing import Optional
 
 # MODELS
 from ..models.user import AlphaUser
 from ..models.database import main_definitions as defs
 from ..models.database.users_definitions import User
 
 # LIBS
@@ -18,29 +17,29 @@
 
 
 def __get_user_data_by_identifier_and_password(
     identifier,
     password_attempt,
     identifier_type="username",
     no_password_check: bool = False,
-) -> Optional[AlphaUser]:
+) -> AlphaUser | None:
     user = __get_user_data(identifier, identifier_type.lower())
 
     if user is not None and password_attempt is not None:
         if no_password_check:
             return user
         valid_password = secure_lib.compare_passwords(password_attempt, user.password)
         if valid_password:
             return user
     return None
 
 
 def get_user_data_by_username_and_password(
     username, password_attempt
-) -> Optional[AlphaUser]:
+) -> AlphaUser | None:
     """Get user data from database by username.
 
     Args:
         mail ([type]): [description]
         password_attempt ([type]): [description]
 
     Returns:
@@ -49,15 +48,15 @@
     return __get_user_data_by_identifier_and_password(
         identifier=username,
         password_attempt=password_attempt,
         identifier_type="username",
     )
 
 
-def get_user_data_by_mail_and_password(mail, password_attempt) -> Optional[AlphaUser]:
+def get_user_data_by_mail_and_password(mail, password_attempt) -> AlphaUser | None:
     """Get user data from database by mail.
 
     Args:
         mail ([type]): [description]
         password_attempt ([type]): [description]
 
     Returns:
@@ -66,15 +65,15 @@
     return __get_user_data_by_identifier_and_password(
         identifier=mail, password_attempt=password_attempt, identifier_type="mail"
     )
 
 
 def get_user_data_from_login(
     login, password=None, no_password_check: bool = False
-) -> Optional[AlphaUser]:
+) -> AlphaUser | None:
     """Get user data from database either by mail or username.
 
     Args:
         login ([type]): [description]
         password ([type]): [description]
 
     Returns:
@@ -95,20 +94,19 @@
 
 def get_user_data_from_database(
     value,
     column,
     activity: bool = False,
     force_local: bool = False,
     scoped_session: bool = False,
-) -> Optional[dict]:
+) -> dict | None:
     """Get the user associated with given column."""
     user = None
-    user_api = DB.user_api + "/user/data"
 
-    if user_api is None or force_local:
+    if DB.user_api is None or force_local:
         if not scoped_session:
             user = DB.select(
                 User,
                 filters=[User.__dict__[column] == value],
                 first=True,
                 relationship=True,
                 # disabled_relationships=["notifications"],
@@ -156,54 +154,55 @@
                 scoped_session.rollback()
                 raise e
 
             finally:
                 # Fermer la session spécifique
                 scoped_session.close()
     else:
+        user_api = DB.user_api + "/user/data"
         user = api_lib.get_api_data(
             user_api,
             params={"value": value, "column": column, "activity": activity},
         )
     return user if user is not None else None
 
 
-def __get_user_data(value, column, activity: bool = False) -> Optional[AlphaUser]:
+def __get_user_data(value, column, activity: bool = False) -> AlphaUser | None:
     user = get_user_data_from_database(value, column, activity=activity)
     alpha_user = AlphaUser.auto_map_from_dict(user) if user is not None else None
     return alpha_user
 
 
-def get_user_data_by_id(user_id, activity: bool = False) -> Optional[AlphaUser]:
+def get_user_data_by_id(user_id, activity: bool = False) -> AlphaUser | None:
     if not string_lib.is_number(user_id):
         return None
     return __get_user_data(user_id, "id", activity=activity)
 
 
-def get_user_data_by_logged_token(token) -> Optional[AlphaUser]:
+def get_user_data_by_logged_token(token) -> AlphaUser | None:
     return __get_user_data(token, "token")
 
 
-def get_user_data_by_registration_token(token) -> Optional[AlphaUser]:
+def get_user_data_by_registration_token(token) -> AlphaUser | None:
     return __get_user_data(token, "registration_token")
 
 
-def get_user_data_by_password_reset_token(token) -> Optional[AlphaUser]:
+def get_user_data_by_password_reset_token(token) -> AlphaUser | None:
     return __get_user_data(token, "password_reset_token")
 
 
-def get_user_data_by_mail(mail) -> Optional[AlphaUser]:
+def get_user_data_by_mail(mail) -> AlphaUser | None:
     return __get_user_data(mail, "mail")
 
 
-def get_user_data_by_username(username, activity: bool = False) -> Optional[AlphaUser]:
+def get_user_data_by_username(username, activity: bool = False) -> AlphaUser | None:
     return __get_user_data(username, "username", activity=activity)
 
 
-def get_user_data_by_telegram_id(telegram_id) -> Optional[AlphaUser]:
+def get_user_data_by_telegram_id(telegram_id) -> AlphaUser | None:
     return __get_user_data(telegram_id, "telegram_id")
 
 
 def update_users():
     """Update all users."""
     # Set expired states if needed
     query = "UPDATE user SET role = 0 WHERE expire <= UTC_TIMESTAMP();"
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.6.3/alphaz/libs/user_management/application_management_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from alphaz.models.database.users_definitions import Application
 from core import core
-from typing import List
 
 
 DB = core.db
 LOG = core.get_logger("api")
 
 
 def get_applications(
     name: str,
     page_index: int,
     page_size: int,
     order_by: str,
     direction: str,
-    columns: List[str] = None,
+    columns: list[str] = None,
 ):
     return DB.select(
         Application,
         filters=[Application.name.like(name)],
         disabled_relationships=[Application.roles],
         page=page_index,
         per_page=page_size,
         order_by=order_by,
         order_by_direction=direction,
         columns=columns,
     )
 
-def get_applications_names(name:str):
+
+def get_applications_names(name: str):
     return DB.select(
         Application,
-        optional_filters={Application.name:{'like':name}},
+        optional_filters={Application.name: {"like": name}},
         unique=Application.name,
         distinct=Application.name,
-        order_by=Application.name.asc()
+        order_by=Application.name.asc(),
     )
 
+
 def get_applications_names_and_id():
     return DB.select(Application, columns=[Application.name, Application.id])
 
 
 def get_application(name: str):
     return DB.select(Application, filters=[Application.name == name], first=True)
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.6.3/alphaz/libs/user_management/permission_management_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from alphaz.models.database.users_definitions import Permission, Role
 from core import core
-from typing import List
 
 
 DB = core.db
 LOG = core.get_logger("api")
 
 
 def get_permissions(
     name: str,
     page_index: int,
     page_size: int,
     order_by: str,
     direction: str,
-    columns: List[str] = None,
+    columns: list[str] = None,
 ):
     permissions = DB.select(
         Permission,
         filters=[Permission.key.like(name)],
         page=page_index,
         per_page=page_size,
         order_by_direction=direction,
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.6.3/alphaz/libs/user_management/role_management_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 from sqlalchemy import distinct, or_
 from sqlalchemy.sql.expression import text
 from alphaz.models.database.users_definitions import (
     Role,
     RolePermission,
     UserRole,
     Application,
@@ -21,15 +19,15 @@
     name: str,
     application: str,
     permission: str,
     page_index: int,
     page_size: int,
     order_by: str,
     direction: str,
-) -> List[AlphaRole]:
+) -> list[AlphaRole]:
     query = (
         DB.session.query(Role)
         .distinct(Role.name)
         .outerjoin(Application, (Role.id_app == Application.id))
         .outerjoin(RolePermission, (Role.name == RolePermission.role_name))
     )
     if permission:
@@ -102,15 +100,18 @@
         )
     )
 
 
 def delete_user_role(user_id: int, role_name: str):
     return DB.delete(
         UserRole,
-        filters=[UserRole.user_id == user_id, UserRole.role_name == role_name,],
+        filters=[
+            UserRole.user_id == user_id,
+            UserRole.role_name == role_name,
+        ],
     )
 
 
 def add_user_role(user_id: int, role_name: str):
     return DB.add(
         UserRole(**{"user_id": user_id, "role_name": role_name, "activated": True})
     )
```

### Comparing `alphaz-0.7.6.2/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.6.3/alphaz/libs/user_management/user_management_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 import json
-from typing import List
+
 
 from sqlalchemy import or_, and_, outerjoin
 from alphaz.models.database.users_definitions import (
     User,
     UserRole,
     Role,
     RolePermission,
@@ -25,15 +25,15 @@
     application: str,
     role: str,
     permission: str,
     order_by: str,
     direction: str,
     page_index: int = 0,
     page_size: int = 200,
-) -> List[AlphaUser]:
+) -> list[AlphaUser]:
     query = (
         DB.session.query(User)
         .distinct(User.username)
         .outerjoin(UserRole, (UserRole.user_id == User.id))
         .outerjoin(Role, (UserRole.role_name == Role.name))
         .outerjoin(RolePermission, (RolePermission.role_name == Role.name))
         .outerjoin(Application, (Role.id_app == Application.id))
```

### Comparing `alphaz-0.7.6.2/alphaz/mails/Images/Background.png` & `alphaz-0.7.6.3/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.6.3/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.6.3/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.6.3/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/Mail.png` & `alphaz-0.7.6.3/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/Webmail.html` & `alphaz-0.7.6.3/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/debug.html` & `alphaz-0.7.6.3/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/mail.html` & `alphaz-0.7.6.3/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/password_reset.html` & `alphaz-0.7.6.3/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.6.3/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_answer.py` & `alphaz-0.7.6.3/alphaz/models/api/_answer.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,20 +3,20 @@
     field,
 )
 from ..main import _base
 
 
 @dataclass
 class ApiPagination(_base.AlphaDataclass):
-    total: int = None
-    total_pages: int = None
-    page: int = None
-    previous_page: int = None
-    next_page: int = None
-    per_page: int = None
+    total: int | None = None
+    total_pages: int | None = None
+    page: int | None = None
+    previous_page: int | None = None
+    next_page: int | None = None
+    per_page: int | None = None
 
 
 @dataclass
 class ApiAnswer(_base.AlphaDataclass):
     token_status: str = "success"
     status: str = "success"
     error: int = 0
```

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_colorations.py` & `alphaz-0.7.6.3/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_parameter.py` & `alphaz-0.7.6.3/alphaz/models/api/_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import json, datetime, dataclasses, re, typing, sqlalchemy, xmltodict
+import json, datetime, dataclasses, re, sqlalchemy, xmltodict
 
-from sqlalchemy.orm.base import object_mapper
-from sqlalchemy.orm.exc import UnmappedInstanceError
 from sqlalchemy.ext.declarative import DeclarativeMeta
 from sqlalchemy import inspect as inspect_sqlalchemy
 
 from flask import request
 from collections.abc import Callable
 
 from ..main import AlphaException
@@ -101,16 +99,16 @@
         ptype: type = str,
         private: bool = False,
         mode: ParameterMode = ParameterMode.NONE,
         override: bool = False,
         function: Callable = None,
         automap: bool = False,
         map_none: bool = False,
-        max_size: int = None,
-        min_size: int = None,
+        max_size: int | None = None,
+        min_size: int | None = None,
         separators: list = [",", ";"],
     ):
         """[summary]
 
         Args:
             name (str): [description]
             default ([type], optional): [description]. Defaults to None.
@@ -183,15 +181,15 @@
             self.is_value = True
         elif api_json is not None and self.name in api_json:
             self._value = api_json[self.name]
             self.is_value = True
         elif (
             self.name in args
             and self.name in dataDict
-            and (self.ptype == list or py_lib.is_subtype(self.ptype, typing.List))
+            and (self.ptype == list or py_lib.is_subtype(self.ptype, list))
             and (len(dataDict[self.name]) != 1)
         ):
             self._value = dataDict[self.name]
             self.is_value = True
         elif self.name in args:
             self._value = args.get(self.name)
             self.is_value = True
@@ -225,16 +223,16 @@
                     "parameter": self.name,
                     "size": len(self.value),
                     "value": self._value,
                     "min": self.min_size,
                 },
             )
 
-        # List
-        if self.ptype == list or py_lib.is_subtype(self.ptype, typing.List):
+        # list
+        if self.ptype == list or py_lib.is_subtype(self.ptype, list):
             is_empty = self._value is None or str(self._value).strip() == ""
             is_empty_value = all(not x in str(self._value) for x in [";", ",", "["])
 
             if is_empty:
                 self._value = self.default
             elif is_empty_value:
                 self._value = (
@@ -323,15 +321,15 @@
                 value = False
             else:
                 raise AlphaException(
                     f"Wrong value <{self._value}> for parameter <{self.name}> of type <bool>",
                 )
             self._value = value
 
-        if self.ptype == list or py_lib.is_subtype(self.ptype, typing.List):
+        if self.ptype == list or py_lib.is_subtype(self.ptype, list):
             if type(self._value) == str and str(self._value).strip() == "":
                 self._value = []
             elif type(self._value) == str:
                 try:
                     if (
                         len(str(self._value)) != 0
                         and str(self._value)[0] == "["
@@ -351,17 +349,17 @@
                     else:
                         self._value = [self._value]
                 except:
                     raise AlphaException(
                         f"Wrong value <{self._value}> for parameter <{self.name}> of type <list>"
                     )
 
-            if py_lib.is_subtype(self.ptype, typing.List[int]):
+            if py_lib.is_subtype(self.ptype, list[int]):
                 self._value = [int(x) for x in self._value]
-            if py_lib.is_subtype(self.ptype, typing.List[float]):
+            if py_lib.is_subtype(self.ptype, list[float]):
                 self._value = [float(x) for x in self._value]
 
             for val in self._value:
                 self.__check_options(val)
 
             if self.mode in [
                 ParameterMode.LIKE,
```

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_reloader.py` & `alphaz-0.7.6.3/alphaz/models/api/_reloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ".pytest_cache",
     ".mypy_cache",
 }
 
 
 def _iter_module_paths() -> t.Iterator[str]:
     """Find the filesystem paths associated with imported modules."""
-    # List is in case the value is modified by the app while updating.
+    # list is in case the value is modified by the app while updating.
     for module in list(sys.modules.values()):
         name = getattr(module, "__file__", None)
 
         if name is None or name.startswith(_ignore_always):
             continue
 
         while not os.path.isfile(name):
@@ -141,38 +141,38 @@
         dirs.add(os.path.dirname(name))
 
     _remove_by_pattern(dirs, exclude_patterns)
     return _find_common_roots(dirs)
 
 
 def _find_common_roots(paths: t.Iterable[str]) -> t.Iterable[str]:
-    root: t.Dict[str, dict] = {}
+    root: dict[str, dict] = {}
 
     for chunks in sorted((PurePath(x).parts for x in paths), key=len, reverse=True):
         node = root
 
         for chunk in chunks:
             node = node.setdefault(chunk, {})
 
         node.clear()
 
     rv = set()
 
-    def _walk(node: t.Mapping[str, dict], path: t.Tuple[str, ...]) -> None:
+    def _walk(node: t.Mapping[str, dict], path: tuple[str, ...]) -> None:
         for prefix, child in node.items():
             _walk(child, path + (prefix,))
 
         if not node:
             rv.add(os.path.join(*path))
 
     _walk(root, ())
     return rv
 
 
-def _get_args_for_reloading() -> t.List[str]:
+def _get_args_for_reloading() -> list[str]:
     """Determine how the script was executed, and return the args needed
     to execute it again in a new process.
     """
     rv = [sys.executable]
     py_script = sys.argv[0]
     args = sys.argv[1:]
     # Need to look at main module to determine how it was executed.
@@ -223,17 +223,17 @@
 
 
 class ReloaderLoop:
     name = ""
 
     def __init__(
         self,
-        extra_files: t.Optional[t.Iterable[str]] = None,
-        exclude_patterns: t.Optional[t.Iterable[str]] = None,
-        interval: t.Union[int, float] = 1,
+        extra_files: t.Iterable[str] | None = None,
+        exclude_patterns: t.Iterable[str] | None = None,
+        interval: int | float = 1,
     ) -> None:
         self.extra_files: t.Set[str] = {os.path.abspath(x) for x in extra_files or ()}
         self.exclude_patterns: t.Set[str] = set(exclude_patterns or ())
         self.interval = interval
 
     def __enter__(self) -> "ReloaderLoop":
         """Do any setup, then run one step of the watch to populate the
@@ -283,15 +283,15 @@
         _log("info", f" * Detected change in {filename!r}, reloading")
 
 
 class StatReloaderLoop(ReloaderLoop):
     name = "stat"
 
     def __enter__(self) -> ReloaderLoop:
-        self.mtimes: t.Dict[str, float] = {}
+        self.mtimes: dict[str, float] = {}
         return super().__enter__()
 
     def run_step(self) -> None:
         for name in _find_stat_paths(self.extra_files, self.exclude_patterns):
             try:
                 mtime = os.stat(name).st_mtime
             except OSError:
@@ -345,15 +345,15 @@
         # This is called inside an event handler, which means throwing
         # SystemExit has no effect.
         # https://github.com/gorakhargosh/watchdog/issues/294
         self.should_reload = True
         self.log_reload(filename)
 
     def __enter__(self) -> ReloaderLoop:
-        self.watches: t.Dict[str, t.Any] = {}
+        self.watches: dict[str, t.Any] = {}
         self.observer.start()
         return super().__enter__()
 
     def __exit__(self, exc_type, exc_val, exc_tb):  # type: ignore
         self.observer.stop()
         self.observer.join()
 
@@ -384,15 +384,15 @@
         for path in to_delete:
             watch = self.watches.pop(path, None)
 
             if watch is not None:
                 self.observer.unschedule(watch)
 
 
-reloader_loops: t.Dict[str, t.Type[ReloaderLoop]] = {
+reloader_loops: dict[str, t.Type[ReloaderLoop]] = {
     "stat": StatReloaderLoop,
     "watchdog": WatchdogReloaderLoop,
 }
 
 try:
     __import__("watchdog.observers")
 except ImportError:
@@ -418,17 +418,17 @@
     if not attributes[3] & termios.ECHO:
         attributes[3] |= termios.ECHO
         termios.tcsetattr(sys.stdin, termios.TCSANOW, attributes)
 
 
 def run_with_reloader(
     main_func: t.Callable[[], None],
-    extra_files: t.Optional[t.Iterable[str]] = None,
-    exclude_patterns: t.Optional[t.Iterable[str]] = None,
-    interval: t.Union[int, float] = 1,
+    extra_files: t.Iterable[str] | None = None,
+    exclude_patterns: t.Iterable[str] | None = None,
+    interval: int | float = 1,
     reloader_type: str = "auto",
 ) -> None:
     """Run the given function in an independent Python interpreter."""
     import signal
 
     signal.signal(signal.SIGTERM, lambda *args: sys.exit(0))
     reloader = reloader_loops[reloader_type](
```

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_reloaders.py` & `alphaz-0.7.6.3/alphaz/models/api/_reloaders.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # MODULES
-import os, configparser, datetime, copy, jwt, logging, re, itertools, sys, importlib, warnings, typing, traceback, time
-from typing import Dict, List
+import os, configparser, datetime, copy, jwt, logging, re, itertools, sys, importlib, warnings, traceback, time
 
 # WERKZEUG
 from werkzeug._reloader import reloader_loops, ReloaderLoop
 from ._reloader import _find_stat_paths
 
 DEBUGGED_FOLDERS = set()
 DEBUG = False
 
 
 class AlphaStatReloaderLoop(ReloaderLoop):
     name = "AlphaStatDebug"
     start_time = None
 
     def __enter__(self) -> ReloaderLoop:
-        self.mtimes: t.Dict[str, float] = {}
+        self.mtimes: t.dict[str, float] = {}
         return super().__enter__()
 
     def run_step(self) -> None:
         global DEBUGGED_FOLDERS
 
         for name in _find_stat_paths(self.extra_files, self.exclude_patterns):
             if DEBUG:
@@ -43,17 +42,17 @@
                 f.write("\n".join(DEBUGGED_FOLDERS))
 
 
 class AlphaReloaderLoop(ReloaderLoop):
     name = "AlphaStat"
 
     def __enter__(self) -> ReloaderLoop:
-        self.mtimes: typing.Dict[str, float] = {}
-        self.sizes: typing.Dict[str, float] = {}
-        self.stats: typing.Dict[str, object] = {}
+        self.mtimes: dict[str, float] = {}
+        self.sizes: dict[str, float] = {}
+        self.stats: dict[str, object] = {}
         return super().__enter__()
 
     def run_step(self) -> None:
         for name in itertools.chain(
             _find_stat_paths(self.extra_files, self.exclude_patterns)
         ):
             try:
@@ -95,15 +94,15 @@
                 )
 
 
 class AlphaMTimeReloaderLoop(ReloaderLoop):
     name = "AlphaMTimeSimpleStat"
 
     def __enter__(self) -> ReloaderLoop:
-        self.mtimes: t.Dict[str, float] = {}
+        self.mtimes: t.dict[str, float] = {}
         return super().__enter__()
 
     def run_step(self) -> None:
         for name in itertools.chain(
             _find_stat_paths(self.extra_files, self.exclude_patterns)
         ):
             try:
```

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_requests.py` & `alphaz-0.7.6.3/alphaz/models/api/_requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from flask import request, json
-from typing import *
 
 from ...libs.json_lib import load_json
 
 
 class AlphaRequest:
     @staticmethod
-    def get_gets() -> Dict[str, object]:
+    def get_gets() -> dict[str, object]:
         """returns GET value as a dict.
 
         Returns:
-            Dict[str, object]: [description]
+            dict[str, object]: [description]
         """
         return {x: y for x, y in request.args.items()}
 
     @staticmethod
     def get_json():
         data = {}  # TODO: modify
         try:
```

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_route.py` & `alphaz-0.7.6.3/alphaz/models/api/_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import datetime, os, copy, json
 import time
 import traceback
-from typing import List, Dict, Tuple
-import typing
 
 from flask import (
-    Flask,
     jsonify,
     request,
-    Response,
     make_response,
     render_template,
     send_from_directory,
 )
 
 from ...libs.time_lib import timer
 
@@ -95,15 +91,15 @@
     no_log = False
     ex = None
 
     def __init__(
         self,
         uuid: str,
         route: str,
-        parameters: List[Parameter],
+        parameters: list[Parameter],
         request_state,
         api,
         cache: bool = False,
         logged: bool = False,
         admin: bool = False,
         timeout=None,
         description: str = "",
@@ -148,15 +144,15 @@
 
         self.cache_dir = api.cache_dir
         self.log = api.log
         self.method = request_state.method
 
         self.init_return()
 
-        self.parameters: Dict[Parameter] = {y.name: copy.copy(y) for y in parameters}
+        self.parameters: dict[Parameter] = {y.name: copy.copy(y) for y in parameters}
         for parameter in self.parameters.values():
             try:
                 parameter.set_value(
                     self.method, self.dict, self.json, self.form, self.args
                 )
                 if parameter.name == "no_log":
                     self.no_log = parameter.value
@@ -260,24 +256,24 @@
         self.returned.status = str(status) if status is not None else "success"
         self.returned.status_description = (
             description
             if description is not None
             else description_from_status(self.returned.status)
         )
 
-    def get_status(self) -> Tuple[str, str]:
+    def get_status(self) -> tuple[str, str]:
         return (self.returned.status, self.returned.status_description)
 
     def timeout(self):
         self.returned.status = "timeout"
         self.returned.status_description = description_from_status(self.returned.status)
         self.returned.status_code = 524
         self.returned.error = 1
 
-    def access_denied(self, description: str = None):
+    def access_denied(self, description: str | None = None):
         self.returned.status = "unauthorized"
         self.returned.status_description = (
             description_from_status(self.returned.status)
             if description is None
             else description
         )
         self.returned.token_status = "denied"
@@ -295,16 +291,16 @@
         self.returned.status_description = description_from_status(self.returned.status)
         self.returned.token_status = "denied"
         self.returned.error = 1
         self.returned.status_code = 401
 
     def set_error(
         self,
-        status: typing.Union[str, AlphaException] = "error",
-        description: str = None,
+        status: str | AlphaException = "error",
+        description: str | None = None,
         warning: int = 0,
         error_code: int = 520,
         ex=None,
     ):
         log_fct = self.log.error if warning == 0 else self.log.warning
 
         if isinstance(status, AlphaException):
@@ -335,16 +331,16 @@
             else description_from_status(self.returned.status)
         )
         self.returned.error = 1 if warning == 0 else 0
         self.returned.warning = int(warning)
 
     def set_warning(
         self,
-        status: typing.Union[str, AlphaException] = "warning",
-        description: str = None,
+        status: str | AlphaException = "warning",
+        description: str | None = None,
     ):
         self.set_error(status=status, description=description, warning=1)
 
     def print(self, message):
         self.mode == "print"
         self.message = message
```

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_structures.py` & `alphaz-0.7.6.3/alphaz/models/api/_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODULES
-import os, jwt, itertools, sys, importlib, warnings, typing, traceback, time
-from typing import Dict, List
+import os, jwt, itertools, sys, importlib, warnings, traceback, time
 
 # WSGI
 from gevent.pywsgi import WSGIServer
 
 # WERKZEUG
 from werkzeug.debug import DebuggedApplication
 
@@ -42,15 +41,15 @@
 # LOCAL
 from . import _colorations
 from ._reloaders import reloader_loops
 from ._route import Route
 
 
 class AlphaFlask(Flask):
-    admin_token: str = None
+    admin_token: str | None = None
 
     def __init__(
         self,
         *args,
         config_name=None,
         configuration=None,
         root=None,
@@ -124,48 +123,48 @@
         if self.conf.get("routes_no_log"):
             _colorations.WerkzeugColorFilter.routes_exceptions = self.conf.get(
                 "routes_no_log"
             )
 
     def set_error(
         self,
-        status: typing.Union[str, AlphaException] = "error",
-        description: str = None,
+        status: str | AlphaException = "error",
+        description: str | None = None,
         warning: int = 0,
     ):
         self.get_current_route().set_error(
             status=status, description=description, warning=warning
         )
 
     def set_status(self, status="success", description=None):
         self.get_current_route().set_status(status=status, description=description)
 
-    def get_status(self) -> typing.Tuple[str, str]:
+    def get_status(self) -> tuple[str, str]:
         return self.get_current_route().get_status()
 
     def set_warning(
         self,
-        status: typing.Union[str, AlphaException] = "warning",
-        description: str = None,
+        status: str | AlphaException = "warning",
+        description: str | None = None,
     ):
         self.set_error(status=status, description=description, warning=1)
 
     def get_parameters(
         self,
         not_none: bool = False,
-        without: List[str] = None,
-        added: Dict[str, object] = None,
+        without: list[str] = None,
+        added: dict[str, object] = None,
         with_user_id: bool = False,
         with_user_permissions: bool = False,
         with_user: bool = False,
-    ) -> Dict[str, object]:
+    ) -> dict[str, object]:
         """Get non private route parameters values as a dict.
 
         Returns:
-            Dict[str, object]: [description]
+            dict[str, object]: [description]
         """
         route = self.get_current_route()
         parameters = route.parameters
         parameters_values = {
             x: y.value
             for x, y in parameters.items()
             if not y.private and (not not_none or y.value is not None)
@@ -189,20 +188,20 @@
                 user.permissions if user is not None else None
             )
         return parameters_values
 
     def gets(
         self,
         not_none: bool = False,
-        without: List[str] = None,
-        added: Dict[str, object] = None,
+        without: list[str] = None,
+        added: dict[str, object] = None,
         with_user_id: bool = False,
         with_user_permissions: bool = False,
         with_user: bool = False,
-    ) -> Dict[str, object]:
+    ) -> dict[str, object]:
         return self.get_parameters(**{x: y for x, y in locals().items() if x != "self"})
 
     def is_error(self) -> bool:
         return self.get_current_route().is_error()
 
     def is_warning(self) -> bool:
         return self.get_current_route().is_warning()
```

### Comparing `alphaz-0.7.6.2/alphaz/models/api/_utils.py` & `alphaz-0.7.6.3/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/config/_config.py` & `alphaz-0.7.6.3/alphaz/models/config/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os, json, inspect, copy, sys, socket, re, platform, getpass
 import numpy as np
-from typing import List, Dict
+
 from collections.abc import Iterable
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 
 from ...config.main_configuration import CONFIGURATION
 
 from ._utils import *
 
 from ..main._base import AlphaClass
 from ..main._exception import EXCEPTIONS
 from ..logger import AlphaLogger
 from ..main import AlphaException
 
-from ...libs import converter_lib, sql_lib, io_lib
+from ...libs import io_lib
 
 _CONFIGURATIONS = {}
 
 
 def replace_fct_matchs(string: str) -> str:
     if type(string) != str:
         return string
@@ -65,27 +65,27 @@
 
 class AlphaConfig(AlphaClass):
     __reserved = ["user", "configuration", "project", "ip", "platform"]
 
     def __init__(
         self,
         name: str = "config",
-        filepath: str = None,
-        root: str = None,
-        filename: str = None,
-        log: AlphaLogger = None,
-        configuration: str = None,
+        filepath: str | None = None,
+        root: str | None = None,
+        filename: str | None = None,
+        log: AlphaLogger | None = None,
+        configuration: str | None = None,
         data: dict = None,
         origin=None,
         core=None,
         core_configuration=None,
-        reserved: List[str] = [],
-        required: List[str] = [],
-        user: str = None,
-        default: str = None,
+        reserved: list[str] = [],
+        required: list[str] = [],
+        user: str | None = None,
+        default: str | None = None,
     ):
         if hasattr(self, "tmp"):
             return
 
         if default is not None and os.path.isfile(default):
             default_config = AlphaConfig(
                 f"default_{name}",
@@ -454,15 +454,15 @@
 
     def get(
         self,
         path=[],
         default=None,
         root: bool = True,
         force_exit: bool = False,
-        configuration: str = None,
+        configuration: str | None = None,
         type_=None,
         required: bool = False,
     ):
         value = self._get_parameter_path(path)
         if value is None and root:
             value = self._get_value_from_main_config(path, force_exit=force_exit)
         if type_ is not None:
@@ -710,15 +710,15 @@
 
     def __new__(cls):
         if not cls._instance:
             cls._instance = object.__new__(cls)
         return cls._instance
 
     def __init__(self):
-        self._configurations: Dict[str, AlphaConfig] = {}
+        self._configurations: dict[str, AlphaConfig] = {}
         if os.path.exists(self._name):
             loaded_configurations = io_lib.unarchive_object(self._name)
             if type(loaded_configurations) == dict:
                 for key, values in loaded_configurations.items():
                     if self._is_valid_configuration(values):
                         self._configurations[key] = values
 
@@ -776,15 +776,15 @@
                 }
                 for x in config.sub_configurations.values()
             },
         }
         try:
             self._configurations[key] = dataset
         except:
-            self._configurations: Dict[str, object] = {key: dataset}
+            self._configurations: dict[str, object] = {key: dataset}
         io_lib.archive_object(self._configurations, self._name)
 
     def is_configured(self, config) -> bool:
         path = config.get_key()
         return path in self._configurations
```

### Comparing `alphaz-0.7.6.2/alphaz/models/config/_utils.py` & `alphaz-0.7.6.3/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/database/main_definitions.py` & `alphaz-0.7.6.3/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/database/models.py` & `alphaz-0.7.6.3/alphaz/models/database/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import datetime, typing
+import datetime
 
 from sqlalchemy import (
     Table,
     Column,
     ForeignKey,
     Integer,
     String,
@@ -81,15 +81,15 @@
     def __str__(self):
         return repr(self)
 
     def __repr__(self):
         return repr(self)
 
     def to_json(
-        self, relationship: bool = True, disabled_relationships: typing.List[str] = None
+        self, relationship: bool = True, disabled_relationships: list[str] = None
     ):
         class_obj = self.__class__
         results_json = {}
 
         # if it is an AlphaTable
         if hasattr(class_obj, "schema"):
             schema = class_obj.get_schema(
@@ -109,19 +109,19 @@
     def init(self, kwargs: dict, not_none: bool = False):
         kwargs = {
             (x if type(x) == str else x.key): y
             for x, y in kwargs.items()
             if not not_none or (y is not None)
         }
         return self.__init__(**kwargs)
-    
+
     @classmethod
     def init_from_model(class_obj, model):
         columns = class_obj.get_columns()
-        kwargs = {x:y for x,y in model.__dict__.items() if x in columns}
+        kwargs = {x: y for x, y in model.__dict__.items() if x in columns}
         return class_obj(**kwargs)
 
     @classmethod
     def instantiate(class_obj, *args, **kwargs):
         """if type(values) == dict:
             return class_obj().init(**values)
         if values
@@ -137,15 +137,15 @@
             kwargs[column] = args[i]
         return class_obj(**kwargs)
 
     @classmethod
     def get_schema(
         class_obj,
         relationship: bool = True,
-        disabled_relationships: typing.List[str] = None,
+        disabled_relationships: list[str] = None,
     ):
         disabled_relationships = disabled_relationships or []
         """if (
             hasattr(class_obj, "schema")
             and class_obj.schema is not None
             and relationship
         ):
@@ -188,38 +188,38 @@
                     class_obj.set_attrib_listener,
                     retval=True,
                 )
             except Exception as ex:
                 continue  # TODO: modify
 
     @classmethod
-    def get_columns(class_obj) -> typing.List[str]:
+    def get_columns(class_obj) -> list[str]:
         columns_names = []
 
         for col in class_obj.__table__.columns:
             binary_expression = type(col.expression) is BinaryExpression
             if hasattr(col, "prop"):
                 column_property = isinstance(col.prop, ColumnProperty)
             if hasattr(col, "name"):
                 columns_names.append(col.name)
         return columns_names
 
     @classmethod
-    def get_table_model(class_obj) -> typing.Dict[str, str]:
+    def get_table_model(class_obj) -> dict[str, str]:
         columns_names = []
         columns = []
 
         for col in class_obj.__table__.columns:
             binary_expression = type(col.expression) is BinaryExpression
             if hasattr(col, "prop"):
                 column_property = isinstance(col.prop, ColumnProperty)
             if hasattr(col, "name"):
                 columns_names.append(col.name)
 
-        class_dict = {x:y for x,y in class_obj.__dict__.items()}
+        class_dict = {x: y for x, y in class_obj.__dict__.items()}
         for key, value in class_dict.items():
             if hasattr(value, "expression"):
                 if hasattr(value.expression, "name"):
                     if value.expression.name in columns_names:
                         if hasattr(value, "to_json"):
                             column_model = value.to_json()
                             if not hasattr(value, "_proxy_key"):
```

### Comparing `alphaz-0.7.6.2/alphaz/models/database/operators.py` & `alphaz-0.7.6.3/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/database/requests.py` & `alphaz-0.7.6.3/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/database/row.py` & `alphaz-0.7.6.3/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/database/structure.py` & `alphaz-0.7.6.3/alphaz/models/database/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # MODULES
-import enum, re, itertools, typing, datetime
+import enum, re, itertools, datetime
 import numpy as np
 from collections.abc import Iterable
-from typing import List, Optional, Dict
 from dataclasses import fields
 from time import sleep
 import logging
 
 # SQLALCHEMY
 from sqlalchemy import MetaData
 from sqlalchemy import inspect as inspect_sqlalchemy
@@ -47,18 +46,18 @@
         return datetime.datetime.now()
     return value
 
 
 def default_return(
     results,
     default=None,
-    columns: dict = None,
-    page: int = None,
-    per_page: int = None,
-    full_count: int = None,
+    columns: dict | None = None,
+    page: int | None = None,
+    per_page: int | None = None,
+    full_count: int | None = None,
     first: bool = False,
     pagination_mode: str = "raw",
 ):
     results = results if results is not None else default
     columns = (
         {}
         if columns is None
@@ -288,15 +287,15 @@
                     )
                     sleep(self.__retry_sleep_interval_sec__)
                     continue
                 else:
                     raise
 
 
-def convert_order_by_str(model, order_by: str, order_by_direction: str = None):
+def convert_order_by_str(model, order_by: str, order_by_direction: str | None = None):
     if model is None and order_by is not None and order_by_direction is not None:
         order_by = sqlalchemy.text(f"{order_by} {order_by_direction}")
     elif type(order_by) == str and order_by_direction is not None:
         relation = order_by
         if "." in order_by:
             order_by_split = order_by.split(".")
             relation = order_by_split[0]
@@ -367,18 +366,18 @@
     return str(element).upper() != "NULL"
 
 
 class AlphaDatabaseCore(SQLAlchemy):
     def __init__(
         self,
         *args,
-        name: Optional[str] = None,
-        log: Optional[AlphaLogger] = None,
+        name: str | None = None,
+        log: AlphaLogger | None = None,
         config=None,
-        timeout: Optional[int] = None,
+        timeout: int | None = None,
         main: bool = False,
         **kwargs,
     ):
         self.db_type: str = config.get("type", "oracle")
         self.user_api = config.get("user_api", None)
 
         """if type(cnx) == dict:
@@ -405,41 +404,41 @@
                                     autoflush=False,
                                     bind=engine))
             self._engine = engine
             self.Model = declarative_base()
             self.Model.query = session.query_property()
             self._session = session"""
 
-        self.name: Optional[str] = name
+        self.name: str | None = name
         self.main = main
 
         self.config = config
-        self.log: Optional[AlphaLogger] = log
+        self.log: AlphaLogger | None = log
 
         self.error = None
 
         self.query_str = None
         self.full_count = None
         self.pagination_mode = config.get("pagination_mode", "raw")
         self.mapping_mode = config.get("mapping_mode", MappingMode.AUTO1.value)
 
         self.models = []
 
-    def get_session(self, bind: Optional[str] = None):
+    def get_session(self, bind: str | None = None):
         return self.db.session if bind is None else self.get_engine(bind=bind)
 
-    def get_meta(self, bind: Optional[str] = None):
+    def get_meta(self, bind: str | None = None):
         engine = self.get_engine(bind=bind)
         meta = MetaData(engine)
         return meta
 
     def to_json(self):
         return py_lib.get_attributes(self)
 
-    def test(self, bind: Optional[str] = None, close=False):
+    def test(self, bind: str | None = None, close=False):
         """[Test the connection]
 
         Returns:
             [type]: [description]
         """
         engine = self.get_engine(bind=bind)
         output = False
@@ -472,15 +471,15 @@
         likes=None,
         sup=None,
     ):
         if query is None:
             query = model.query
 
         if columns is not None:
-            if type(columns) != list and type(columns) != List:
+            if type(columns) != list and type(columns) != list:
                 columns = [columns]
             ccs = []
             for column in columns:
                 """if type(column) != str:
                     ccs.append(column.key)
                 else:
                     ccs.append(column)"""
@@ -525,30 +524,30 @@
                     # TODO: modify
                     pass
         else:
             table_model.query.delete()
             self.commit()
 
     def execute(
-        self, query, values=None, commit=True, bind: Optional[str] = None, close=False
+        self, query, values=None, commit=True, bind: str | None = None, close=False
     ):
         return self.execute_query(query, values, commit=commit, bind=bind, close=close)
 
     def execute_many_query(
-        self, query, values=None, commit=True, bind: Optional[str] = None, close=False
+        self, query, values=None, commit=True, bind: str | None = None, close=False
     ):
         return self.execute_query(query, values, multi=True, bind=bind, commit=commit)
 
     def execute_query(
         self,
         query,
         values={},
         multi: bool = False,
         commit: bool = True,
-        bind: Optional[str] = None,
+        bind: str | None = None,
         close: bool = False,
     ) -> bool:
         if self.db_type == "sqlite":
             query = query.replace("%s", "?")
 
         engine = self.get_engine(bind=bind)
 
@@ -575,33 +574,31 @@
             if close:
                 self.session.close()
             return True
         except Exception as ex:
             self.log.error(ex)
             raise ex
 
-    def get(
-        self, query, values=None, unique=False, bind: Optional[str] = None, log=None
-    ):
+    def get(self, query, values=None, unique=False, bind: str | None = None, log=None):
         return self.get_query_results(
             query, values=values, unique=unique, bind=bind, log=log
         )
 
     def get_query_results(
         self,
         query,
         values=None,
         unique=False,
         log=None,
         bind=None,
         close=False,
         dataclass=None,
-        page: Optional[int] = None,
-        per_page: Optional[int] = None,
-        full_count_query: Optional[str] = None,
+        page: int | None = None,
+        per_page: int | None = None,
+        full_count_query: str | None = None,
     ):
         session = self.get_engine(self.app, bind)
 
         if self.db_type == "sqlite":
             query = query.replace("%s", "?")
 
         if log is None:
@@ -675,15 +672,15 @@
                 self.log.error(error_message)
         """
         if close:
             session.close()
 
         return rows
 
-    def get_blocked_queries(self, bind: Optional[str] = None):
+    def get_blocked_queries(self, bind: str | None = None):
         query = """SELECT SQL_TEXT
         FROM performance_schema.events_statements_history ESH,
             performance_schema.threads T
         WHERE ESH.THREAD_ID = T.THREAD_ID
         AND ESH.SQL_TEXT IS NOT NULL
         AND T.PROCESSLIST_ID = %s
         ORDER BY ESH.EVENT_ID LIMIT 10;"""
@@ -890,15 +887,15 @@
             return False
         for obj in objs:
             self.delete_obj(obj, commit=False)
         if commit:
             return self.commit(close=close)
         return True
 
-    def get_tables_names(self, bind: Optional[str] = None):
+    def get_tables_names(self, bind: str | None = None):
         return list(
             set(
                 [
                     x.__tablename__
                     for x in self.get_tables_models(
                         binds=[bind] if bind is not None else None
                     )
@@ -914,15 +911,15 @@
                     x.__bind_key__
                     for x in self.get_tables_models()
                     if getattr(x, "__bind_key__", None) is not None
                 ]
             )
         )
 
-    def get_table_model(self, table: str, bind: Optional[str] = None):
+    def get_table_model(self, table: str, bind: str | None = None):
         model = next(
             iter(
                 self.get_tables_models(
                     tables=[table], binds=[bind] if bind is not None else None
                 )
             ),
             None,
@@ -932,15 +929,15 @@
         return model
 
     def get_table_columns(self, table: str):
         model = self.get_table_model(table)
         return model._sa_class_manager.local_attrs
 
     def get_tables_models(
-        self, tables: List[str] = None, binds: List[str] = None
+        self, tables: list[str] = None, binds: list[str] = None
     ) -> list:
         if tables is not None:
             tables = [x.upper() for x in tables]
         if binds is not None:
             binds = [x.upper() for x in binds]
         models = self.__get_tables_models()
         registered_models = [
@@ -952,15 +949,15 @@
         return registered_models
 
     def __get_tables_models(self, force: bool = False):
         if len(self.models) == 0 or force:
             if hasattr(self.Model, "_decl_class_registry"):
                 registries = self.Model._decl_class_registry
                 registered_classes = [x for x in registries.values()]
-                registered_models: typing.Dict[str, DefaultMeta] = [
+                registered_models: dict[str, DefaultMeta] = [
                     x for x in registered_classes if isinstance(x, DefaultMeta)
                 ]
             else:
                 registered_models = [
                     x
                     for x in self.Model.registry._class_registry.values()
                     if hasattr(x, "__tablename__")
@@ -1020,24 +1017,24 @@
         json: bool = False,
         unique: InstrumentedAttribute = None,
         count: bool = False,
         order_by=None,
         order_by_direction=None,
         group_by=None,
         distinct=None,
-        limit: int = None,
-        columns: list | dict = None,
+        limit: int | None = None,
+        columns: list | dict | None = None,
         close=False,
         flush=False,
         schema=None,
         relationship=True,
-        disabled_relationships: typing.List[str] = None,
-        page: int = None,
-        per_page: int = None,
-        offset: int = None,
+        disabled_relationships: list[str] = None,
+        page: int | None = None,
+        per_page: int | None = None,
+        offset: int | None = None,
         dataclass=None,
         default=None,
     ):
         query = apply_jonctions(model, order_by)
 
         # model_name = inspect.getmro(model)[0].__name__
         # if self.db_type == "mysql": self.test(close=False)
@@ -1122,30 +1119,30 @@
         self,
         query,
         model=None,
         first: bool = False,
         json: bool = False,
         unique: InstrumentedAttribute = None,
         count: bool = False,
-        limit: int = None,
+        limit: int | None = None,
         filters: list = None,
         optional_filters: list = None,
         order_by=None,
         order_by_direction=None,
         close=False,
         flush=False,
         schema=None,
         relationship=True,
-        disabled_relationships: typing.List[str] = None,
-        page: int = None,
-        per_page: int = None,
-        offset: int = None,
+        disabled_relationships: list[str] = None,
+        page: int | None = None,
+        per_page: int | None = None,
+        offset: int | None = None,
         dataclass=None,
         default=None,
-        columns: dict = None,
+        columns: dict | None = None,
         distinct=None,
         group_by=None,
     ):
         if per_page is not None and page is None:
             page = 0
         if distinct is not None:
             query = (
@@ -1549,16 +1546,16 @@
 
         for entry in entries:
             session.merge(entry)
         session.commit()"""
 
     def init_all(
         self,
-        binds: List[str] = None,
-        tables: List[AlphaTable] = None,
+        binds: list[str] = None,
+        tables: list[AlphaTable] = None,
         drop: bool = False,
         create: bool = False,
         sqlite: bool = True,
         log=None,
     ):
         """if sqlite:
         binds = [
@@ -1609,20 +1606,20 @@
                     log.info(f"Drop tables from {bind=}: {tables_names_str}")
                 meta.drop_all(tables=tables)
             if create:
                 if log is not None:
                     log.info(f"Create tables from {bind=}: {tables_names_str}")
                 meta.create_all(tables=tables)
 
-    def create_table(self, table: str, bind: Optional[str] = None, drop: bool = False):
+    def create_table(self, table: str, bind: str | None = None, drop: bool = False):
         table_object = self.get_table_model(table, bind)
         if drop:
             try:
                 table_object.__table__.drop(self.engine)
             except:
                 pass
         table_object.__table__.create(self.engine)
         return True
 
-    def drop_table(self, table: str, bind: Optional[str] = None):
+    def drop_table(self, table: str, bind: str | None = None):
         table_object = self.get_table_model(table, bind)
         table_object.__table__.drop(self.db.engine)
```

### Comparing `alphaz-0.7.6.2/alphaz/models/database/tests.py` & `alphaz-0.7.6.3/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/database/users_definitions.py` & `alphaz-0.7.6.3/alphaz/models/database/users_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/database/utils.py` & `alphaz-0.7.6.3/alphaz/models/database/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import importlib, json, typing
+import importlib, json
 
 from marshmallow import Schema
 from marshmallow import fields as cfields
 from marshmallow_sqlalchemy import ModelConverter, fields
 
 from ...config.main_configuration import CONFIGURATION
 
@@ -29,15 +29,15 @@
     # Dynamic schema class creation
     properties = {"Meta": type("Meta", (object,), {"fields": columns})}
     schema = type(schema_name, (core.ma.Schema,), properties)
     return auto_schema
 
 
 def get_auto_schema(
-    model, relationship: bool = True, disabled_relationships: typing.List[str] = []
+    model, relationship: bool = True, disabled_relationships: list[str] = []
 ):
     from core import core
 
     if CONFIGURATION.DEBUG_SCHEMA:
         core.log.debug(f"Getting auto schema for <{model.__name__}>")
 
     properties = {
@@ -118,16 +118,16 @@
         content += f"l{level}-{tp[0]}-{tp[1]}_{sub_value}".replace("None", "a")
     return content
 
 
 def generate_schema(
     class_obj,
     relationship: bool = True,
-    disabled_relationships: typing.List[str] = None,
-    parents: typing.List[str] = None,
+    disabled_relationships: list[str] = None,
+    parents: list[str] = None,
 ):
     parents = parents or []
     disabled_relationships = disabled_relationships or []
     disabled_relationships = __pdr_list_to_dict(disabled_relationships)
     disabled_relationships_keys = __pdr_flat(disabled_relationships)
 
     # schema_key = "-".join([f"{x}:{str(y)}" for x, y in locals().items()])
@@ -170,15 +170,18 @@
             continue
 
         if hasattr(value, "visible") and getattr(value, "visible"):
             columns.append(key)
         elif hasattr(value, "entity") and relationship:
             skip, disabled_relationships_child = False, []
 
-            for (disabled_relationship, childs,) in disabled_relationships.items():
+            for (
+                disabled_relationship,
+                childs,
+            ) in disabled_relationships.items():
                 if skip:
                     continue
 
                 is_table = (
                     disabled_relationship[0] is None
                     or disabled_relationship[0] == class_obj.__tablename__
                 )
@@ -239,17 +242,17 @@
     return generated_schema
 
 
 def get_schema(
     class_obj,
     default: bool = False,
     relationship: bool = True,
-    disabled_relationships: typing.List[str] = None,
+    disabled_relationships: list[str] | None = None,
 ):
-    """ Get Schema for a model
+    """Get Schema for a model
 
     Args:
         class_obj ([type]): [description]
         parent ([type], optional): [description]. Defaults to None.
 
     Returns:
         [type]: [description]
```

### Comparing `alphaz-0.7.6.2/alphaz/models/database/views.py` & `alphaz-0.7.6.3/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/excel.py` & `alphaz-0.7.6.3/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/ftp.py` & `alphaz-0.7.6.3/alphaz/models/ftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import field
 import pysftp, ftplib, re
-from typing import List, Dict
 
 from core import core
 
 LOG = core.get_logger("ftp")
 
 
 class AlphaFtpFile:
@@ -114,15 +113,15 @@
         self.disconnect()
 
         if exc_type:
             print(f"exc_type: {exc_type}")
             print(f"exc_value: {exc_value}")
             print(f"exc_traceback: {exc_traceback}")
 
-    def list_dir(self, directory, contain=None, origin=None) -> List[AlphaFtpFile]:
+    def list_dir(self, directory, contain=None, origin=None) -> list[AlphaFtpFile]:
         files = []
 
         # Switch to a remote directory
         self.cnx.cwd(directory)  #'/home/gollnwnw'
 
         # Obtain structure of the remote directory '/var/www/vhosts'
         if self.sftp:
@@ -176,24 +175,24 @@
             self.files.append(ftp_file)
             self.index += 1
         except Exception as ex:
             if self.log:
                 self.log.error(ex)
 
     def write_file(
-        self, file_name: str, content: str, remote_directory: str = None
+        self, file_name: str, content: str, remote_directory: str | None = None
     ) -> bool:
         if remote_directory is not None and not self.is_dir(remote_directory):
             print(f"Go to {remote_directory}")
             self.cnx.cwd(remote_directory)
         with self.cnx.open(file_name, "w") as f:
             f.write(content)
         return True
 
-    def read_file(self, file_name: str, remote_directory: str = None) -> str:
+    def read_file(self, file_name: str, remote_directory: str | None = None) -> str:
         if remote_directory is not None and not self.is_dir(remote_directory):
             print(f"Go to {remote_directory}")
             self.cnx.cwd(remote_directory)
         with self.cnx.open(file_name, "r") as f:
             return f.read()
         return None
```

### Comparing `alphaz-0.7.6.2/alphaz/models/json/_converters.py` & `alphaz-0.7.6.3/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/logger/_colorations.py` & `alphaz-0.7.6.3/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/logger/_logger.py` & `alphaz-0.7.6.3/alphaz/models/logger/_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
             "monitor",
         ]
         return {x: self.__dict__[x] for x in keys if x in self.__dict__}
 
     def __init__(
         self,
         name: str,
-        filename: str = None,
-        root: str = None,
+        filename: str | None = None,
+        root: str | None = None,
         cmd_output: bool = True,
         level: str = "INFO",
         format_log: str = DEFAULT_FORMAT,
         date_format: str = DEFAUT_DATE_FORMAT,
         colors=None,
         log_in_db: bool = False,
         excludes=None,
@@ -158,15 +158,15 @@
 
     def _log(
         self,
         message: str,
         stack,
         stack_level: int,
         level: str = "INFO",
-        monitor: str = None,
+        monitor: str | None = None,
         log_in_db: bool = False,
         ex: Exception = None,
         enabled: bool = True,
     ):
         """
                 frame       = inspect.stack()[1]
         module      = inspect.getmodule(frame[0])
```

### Comparing `alphaz-0.7.6.2/alphaz/models/logger/_utils.py` & `alphaz-0.7.6.3/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/logs/main.log` & `alphaz-0.7.6.3/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/main/_base.py` & `alphaz-0.7.6.3/alphaz/models/main/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses, traceback
 import enum, inspect, operator, re, copy
 from dataclasses import dataclass, field, is_dataclass, _MISSING_TYPE, asdict
 from collections import OrderedDict
 
-from typing import Dict, Iterable, List, Optional, Tuple
+from typing import Iterable
 from typing_extensions import Annotated
 
 from ..logger import AlphaLogger
 from ...libs import py_lib, json_lib, string_lib
 
 from ._enum import MappingMode
 from ._exception import AlphaException
@@ -15,47 +15,47 @@
 FORCE_AUTO_MAP = True
 
 
 class AlphaMappingAttribute:
     def __init__(
         self,
         name: str,
-        key: str = None,
+        key: str | None = None,
         fct: object = None,
         required: bool = False,
         flat: bool = False,
     ):
         self.name = name
         self.key = key or name
         self.fct = fct
         self.required = required
         self.flat = flat
 
 
-def get_score_dict_best_match(score_dict: Dict[str, int]) -> str:
+def get_score_dict_best_match(score_dict: dict[str, int]) -> str:
     max_keys = [
         x
         for x, y in score_dict.items()
         if y == max(score_dict.items(), key=lambda k: k[1])[1]
     ]
     min_size = min(max_keys, key=len)
     best_matchs = [x for x in max_keys if len(x) == len(min_size)]
     if len(best_matchs) > 1:
         print(f"ERROR: multiple match {best_matchs}")
     return best_matchs[0]
 
 
 class AlphaClass:
-    def __init__(self, *args, log: AlphaLogger = None, **kwargs):
+    def __init__(self, *args, log: AlphaLogger | None = None, **kwargs):
         self.init_args: dict = {"args": args, "kwargs": kwargs}
         self.children: list = []
 
-        self.log: AlphaLogger = log
+        self.log = log
 
-        self.__piles: Dict[str, List[str]] = {}
+        self.__piles: dict[str, list[str]] = {}
 
     def make_child(self, child_cls, *args, **kwargs):
         if args is None:
             args = self.init_args["args"]
         if kwargs is None:
             kwargs = self.init_args["kwargs"]
         child = child_cls(self, *args, **kwargs)
@@ -63,16 +63,16 @@
         return child
 
     def get_attributes(self):
         return py_lib.get_attributes(self)
 
     def to_json(
         self,
-        columns: list = None,
-        rejected: list = None,
+        columns: list | None = None,
+        rejected: list | None = None,
         not_none: bool = False,
         not_empty: bool = False,
     ):
         d_rejected = ["_AlphaClass__piles", "init_args", "children", "log"]
         if rejected is not None:
             d_rejected.extend(rejected)
         dict_output = {}
@@ -127,15 +127,15 @@
 
     def critical(self, message, out=False, ex=None):
         self.__log(inspect.stack()[0][3], message=message, ex=ex, out=out)
         if out:
             exit()
 
     def map_from_inputs(
-        self, map_entries: List[AlphaMappingAttribute], inputs: Dict[str, object]
+        self, map_entries: list[AlphaMappingAttribute], inputs: dict[str, object]
     ):
         mapped = []
         for key in inputs:
             for mapping_attribute in map_entries:
                 if mapping_attribute.name in mapped:
                     continue
 
@@ -170,15 +170,15 @@
         return (
             False
             if value is None
             else ("Y" in str_val or "T" in str_val or "1" in str_val)
         )
 
 
-def identify(search_key: str, dict_keys: List[str], dataclass_type):
+def identify(search_key: str, dict_keys: list[str], dataclass_type):
     identified_k = None
     for dict_key in dict_keys:
         if search_key in dict_key or dict_key in search_key:
             identified_k = dict_key
             dict_keys.remove(identified_k)
             break
     score = 100
@@ -189,32 +189,32 @@
 
         if identified_k is None:
             # print(f"{dataclass_type}: Cannot find a match for {search_key}")
             return None, score
     return identified_k, score
 
 
-def get_association(key: str, associations: Dict[str, str] = {}):
+def get_association(key: str, associations: dict[str, str] = {}):
     associations = {
         x: y if type(associations[x]) != AlphaMappingAttribute else y.key
         for x, y in associations.items()
     }
     ass_matchs = [x for x, y in associations.items() if y == key]
 
     if len(ass_matchs) != 0:
         return ass_matchs[0]
     return None
 
 
 def full_identify(
     dataclass_type,
     dict_key: str,
-    fields_keys: List[str],
-    associations: Dict[str, str] = {},
-    no_match: List[str] = [],
+    fields_keys: list[str],
+    associations: dict[str, str] = {},
+    no_match: list[str] = [],
 ):
     patterns = {}
     required = False
 
     for x in fields_keys:
         if x in no_match:
             continue
@@ -266,48 +266,48 @@
 
     return identified_k, score
 
 
 @dataclass
 class AutoMapping(AlphaClass):
     dataclass_type: object
-    associations: Dict[str, str] = field(default_factory=lambda: {})
-    no_match: List[str] = field(default_factory=lambda: [])
+    associations: dict[str, str] = field(default_factory=lambda: {})
+    no_match: list[str] = field(default_factory=lambda: [])
 
-    object_fields: Dict[str, object] = field(default_factory=lambda: {})
-    dict_fields: Dict[str, object] = field(default_factory=lambda: {})
-    list_fields: Dict[str, object] = field(default_factory=lambda: {})
-    flat_fields: Dict[str, object] = field(default_factory=lambda: {})
-
-    identified_object_fields: Dict[str, object] = field(default_factory=lambda: {})
-    identified_dict_fields: Dict[str, object] = field(default_factory=lambda: {})
-    identified_list_fields: Dict[str, object] = field(default_factory=lambda: {})
-
-    matchs_object_fields: Dict[str, object] = field(default_factory=lambda: {})
-    matchs_dict_fields: Dict[str, object] = field(default_factory=lambda: {})
-    matchs_list_fields: Dict[str, object] = field(default_factory=lambda: {})
+    object_fields: dict[str, object] = field(default_factory=lambda: {})
+    dict_fields: dict[str, object] = field(default_factory=lambda: {})
+    list_fields: dict[str, object] = field(default_factory=lambda: {})
+    flat_fields: dict[str, object] = field(default_factory=lambda: {})
+
+    identified_object_fields: dict[str, object] = field(default_factory=lambda: {})
+    identified_dict_fields: dict[str, object] = field(default_factory=lambda: {})
+    identified_list_fields: dict[str, object] = field(default_factory=lambda: {})
+
+    matchs_object_fields: dict[str, object] = field(default_factory=lambda: {})
+    matchs_dict_fields: dict[str, object] = field(default_factory=lambda: {})
+    matchs_list_fields: dict[str, object] = field(default_factory=lambda: {})
 
-    already_assigned: List[str] = field(default_factory=lambda: [])
+    already_assigned: list[str] = field(default_factory=lambda: [])
 
     is_identified: bool = False
     flat: bool = False
 
     def __post_init__(self):
         self.__set_fields_types()
 
     def __set_fields_types(self):
         for x, y in self.dataclass_type.__dataclass_fields__.items():
-            if py_lib.is_subtype(y.type, List) or py_lib.is_subtype(y.type, list):
+            if py_lib.is_subtype(y.type, list) or py_lib.is_subtype(y.type, list):
                 self.list_fields[x] = y
             elif is_dataclass(y.type):
                 self.dict_fields[x] = y
             else:
                 self.object_fields[x] = y
 
-    def identify(self, dict_values: Dict[str, object]):
+    def identify(self, dict_values: dict[str, object]):
         dict_elements = {
             x: y for x, y in dict_values.items() if type(y) == dict or y is None
         }
         list_elements = {
             x: y for x, y in dict_values.items() if type(y) == list or y is None
         }
         other_elements = {
@@ -363,15 +363,15 @@
 
             for field_key, score_dict in matchs.items():
                 best_match = get_score_dict_best_match(score_dict)
                 if field_key in fields_dict:
                     identified_dict[best_match] = fields_dict[field_key]
                     identified.append(best_match)
 
-    def __identify_flat(self, dict_values: Dict[str, object]):
+    def __identify_flat(self, dict_values: dict[str, object]):
         identified = []
         for dict_key in dict_values.keys():
             identified_k = get_association(dict_key, self.associations)
             if identified_k is not None:
                 if not identified_k in self.matchs_object_fields:
                     self.matchs_object_fields[identified_k] = {}
                 self.matchs_object_fields[identified_k][dict_key] = 100
@@ -397,15 +397,15 @@
         for field_key, score_dict in self.matchs_object_fields.items():
             best_match = get_score_dict_best_match(score_dict)
             if field_key in self.object_fields:
                 self.identified_object_fields[best_match] = self.object_fields[
                     field_key
                 ]
 
-    def __map_flat(self, dict_values: Dict[str, object]):
+    def __map_flat(self, dict_values: dict[str, object]):
         if not self.is_identified:
             self.__identify_flat(dict_values)
 
         field_values = {}
         for (
             key,
             fd,
@@ -417,15 +417,15 @@
                 dict_values={
                     x: y for x, y in dict_values.items() if not x in field_values
                 }
             )
 
         return field_values
 
-    def map(self, dict_values: Dict[str, object]):
+    def map(self, dict_values: dict[str, object]):
         if self.flat:
             return self.__map_flat(dict_values)
 
         if not self.is_identified:
             self.identify(dict_values)
 
         field_values = {}
@@ -491,15 +491,15 @@
         try:
             return field_type(value)
         except:
             return value
 
 
 class AlphaDataclass(AlphaClass):
-    def get_fields_dict(self, keys: List[str] = None) -> dict:
+    def get_fields_dict(self, keys: list[str] = None) -> dict:
         dct = {}
         # dct['_tname'] = self.__class__.__name__
 
         for f in dataclasses.fields(self):
             f_type = f.type
             value = getattr(self, f.name)
             if hasattr(value, "get_fields_dict"):
@@ -509,15 +509,15 @@
             if keys is not None and f.name not in keys:
                 continue
             dct[f.name] = value
 
         return dct
 
     def compare(
-        self, other, attrs_list: List[str], attrs_eq: Dict[str, str] = None
+        self, other, attrs_list: list[str], attrs_eq: dict[str, str] = None
     ) -> bool:
         if not isinstance(other, self.__class__) and not issubclass(
             self.__class__, other.__class__
         ):
             raise AlphaException(
                 description=f"Cannot compare {self.__class__} object with {other.__class__} object"
             )
@@ -548,15 +548,15 @@
             else:
                 raise AlphaException(
                     description=f"{self.__class__.__name__} object has no attribute {attr}"
                 )
 
         return all(compared)
 
-    def check_attrs_not_none(self, attrs_list: List[str]) -> Optional[bool]:
+    def check_attrs_not_none(self, attrs_list: list[str]) -> bool | None:
         if attrs_list is None:
             return
 
         for attr in attrs_list:
             if hasattr(self, attr):
                 self_attr = getattr(self, attr)
                 if self_attr is None:
@@ -566,15 +566,15 @@
             else:
                 raise AlphaException(
                     description=f"{self.__class__.__name__} object has no attribute {attr}"
                 )
 
         return True
 
-    def check_attrs_none(self, attrs_list: List[str]) -> Optional[bool]:
+    def check_attrs_none(self, attrs_list: list[str]) -> bool | None:
         if attrs_list is None:
             return
 
         for attr in attrs_list:
             if hasattr(self, attr):
                 self_attr = getattr(self, attr)
                 if self_attr is not None:
@@ -584,15 +584,15 @@
             else:
                 raise AlphaException(
                     description=f"{self.__class__.__name__} object has no attribute {attr}"
                 )
 
         return True
 
-    def replace_empty_with_none(self, attrs_list: List[str]) -> Optional[bool]:
+    def replace_empty_with_none(self, attrs_list: list[str]) -> bool | None:
         if attrs_list is None:
             return
 
         for attr in attrs_list:
             if hasattr(self, attr):
                 self_attr = getattr(self, attr)
                 if self_attr == "":
@@ -600,15 +600,15 @@
             else:
                 raise AlphaException(
                     description=f"{self.__class__.__name__} object has no attribute {attr}"
                 )
 
         return True
 
-    def check_attributes_max_lenght(self, attrs_list: List[Tuple[str, int]]):
+    def check_attributes_max_lenght(self, attrs_list: list[tuple[str, int]]):
         if attrs_list is None:
             return
 
         for attr, max_length in attrs_list:
             if hasattr(self, attr):
                 self_attr = getattr(self, attr)
                 if self_attr is not None and len(self_attr) > max_length:
@@ -620,28 +620,28 @@
                     description=f"{self.__class__.__name__} object has no {attr=}"
                 )
 
         return True
 
     def update_from_auto_map_from_dict(
         self,
-        dict_values: Dict[str, object],
-        associations: Dict[str, str] = {},
-        no_match: List[str] = [],
+        dict_values: dict[str, object],
+        associations: dict[str, str] = {},
+        no_match: list[str] = [],
         flat: bool = False,
     ):
         instance = self.auto_map_from_dict(
             dict_values, associations, no_match, flat=flat
         )
 
         for key, fd in instance.__dict__.items():
             if fd is not None:
                 setattr(self, key, fd)
 
-    def flatten(self, parent: str = None):
+    def flatten(self, parent: str | None = None):
         output = {}
         for key, field in self.__dataclass_fields__.items():
             if not key in self.__dict__:
                 value = field.default
             else:
                 value = self.__dict__[key]
             value_key = f"{parent}.{key}" if parent is not None else key
@@ -680,17 +680,17 @@
             for f in dataclasses.fields(dataclass_type)
             if (init_only and f.init) or not init_only
         ]
 
     @classmethod
     def auto_map_from_dict(
         dataclass_type,
-        dict_values: Dict[str, object],
-        associations: Dict[str, str] = {},
-        no_match: List[str] = [],
+        dict_values: dict[str, object],
+        associations: dict[str, str] = {},
+        no_match: list[str] = [],
         flat: bool = False,
     ):
         global DATACLASS_AUTO_MAP_MATCHS, FORCE_AUTO_MAP
         if dict_values is None:
             return dataclass_type()
 
         dataclass_name = str(dataclass_type).split(".")[-1].replace("'>", "")
@@ -745,21 +745,21 @@
             print(f"Failed to map {dataclass_type} with: {json_values}")
             print(ex)
             obj = None
         return obj
 
     @classmethod
     def map_from_dict(
-        dataclass_type, dict_value: Dict[str, object], automap: bool = False
+        dataclass_type, dict_value: dict[str, object], automap: bool = False
     ):
         if automap and hasattr(dataclass_type, "auto_map_from_dict"):
             return dataclass_type.auto_map_from_dict(dict_values=dict_value)
 
         if (
-            not py_lib.is_subtype(type(dict_value), Dict)
+            not py_lib.is_subtype(type(dict_value), dict)
             and not py_lib.is_subtype(type(dict_value), dict)
             and not type(dict_value) == dict
         ):
             return None
         if dict_value is None:
             return None
 
@@ -770,15 +770,15 @@
 
             field = dataclass_type.__dataclass_fields__[key]
             field_type = field.type
 
             if not field.init:
                 continue
 
-            if py_lib.is_subtype(field_type, List) or py_lib.is_subtype(
+            if py_lib.is_subtype(field_type, list) or py_lib.is_subtype(
                 field_type, list
             ):
                 field_values[key] = []
                 if value is not None:
                     field_values[key] = [
                         convert_value_from_field(
                             py_lib.get_subtype(field_type), v, automap=automap
```

### Comparing `alphaz-0.7.6.2/alphaz/models/main/_core/_core.py` & `alphaz-0.7.6.3/alphaz/models/main/_core/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MODULES
 import os, sys, warnings, logging
-from typing import List, Dict
+
 
 from sqlalchemy import exc as sqlalchemy_exc
 
 with warnings.catch_warnings():
     from flask_marshmallow import Marshmallow
 from flask_cors import CORS
 
@@ -42,47 +42,47 @@
     def __init__(self, file: str, level: int = 0, *args, **kwargs):
         super().__init__(log=None)
 
         self.root: str = _get_relative_path(file, level=level)
 
         self.root_alpha = os.path.dirname(__file__).split("models")[0]
 
-        self.config: AlphaConfig = None
+        self.config: AlphaConfig | None = None
 
         self.initiated: bool = False
-        self.loggers: Dict[str, AlphaLogger] = {}
+        self.loggers: dict[str, AlphaLogger] = {}
 
-        self.ma: Marshmallow = None
-        self._db: AlphaDatabase = None
-        self.api: AlphaFlask = None
+        self.ma: Marshmallow | None = None
+        self._db: AlphaDatabase | None = None
+        self.api: AlphaFlask | None = None
 
-        self._models_sources: List[str] = []
+        self._models_sources: list[str] = []
         self.databases_models: list = []
 
         configuration = (
             None
             if not CONFIGURATION.CONFIGURATION_ENV_NAME in os.environ
             else os.environ[CONFIGURATION.CONFIGURATION_ENV_NAME].lower().strip()
         )
-        self.configuration: str = configuration
-        self.configuration_name: str = configuration
+        self.configuration: str | None = configuration
+        self.configuration_name: str | None = configuration
 
         self.config: AlphaConfig = AlphaConfig(
             CONFIGURATION.MAIN_CONFIGURATION_NAME,
             root=self.root,
             configuration=configuration,
             core=self,
             # default=f"{self.root_alpha}{os.sep}{CONFIGURATION.DEFAULT_CONFIG_FILEPATH}.json"
         )
         """ignored_warnings = self.config.get("ignored_warnings", [])
         for ignored_warning in ignored_warnings:
             warnings.filterwarnings("ignore", message=ignored_warning)"""
 
         self.logger_root = self.config.get("directories/logs", required=True)
-        self.log: AlphaLogger = None
+        self.log: AlphaLogger | None = None
 
         self.__set_loggers()
         self.__configure_databases()
 
     @property
     def db(self):
         self.prepare_api(self.configuration)
@@ -409,22 +409,22 @@
             if self.config is None:
                 print("ERROR: Configuration need to be initialized")
                 exit()
 
     def get_data_directory(self):
         return self.config.get("directories/data", required=True)
 
-    def save(self, object_to_save: object, filename: str, ext: str = None):
+    def save(self, object_to_save: object, filename: str, ext: str | None = None):
         filename = (
             filename
             if os.sep in filename
             else self.config.get("directories/tmp") + os.sep + filename
         )
         io_lib.archive_object(object_to_save=object_to_save, filename=filename, ext=ext)
 
-    def load(self, filename: str, ext: str = None, default: object = None):
+    def load(self, filename: str, ext: str | None = None, default: object = None):
         filename = (
             filename
             if os.sep in filename
             else self.config.get("directories/tmp") + os.sep + filename
         )
         return io_lib.unarchive_object(filename=filename, ext=ext, default=default)
```

### Comparing `alphaz-0.7.6.2/alphaz/models/main/_exception.py` & `alphaz-0.7.6.3/alphaz/models/main/_exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import re, traceback
 
-from typing import Dict
-
 EXCEPTIONS = {}
 
 
 def get_message_from_name(name):
     if type(name) != str:
         name = str(name)
     name = name.replace("_", " ")
@@ -14,15 +12,15 @@
 
 class AlphaException(Exception):
     def __init__(
         self,
         name="exception",
         warning: bool = False,
         description=None,
-        parameters: Dict[str, object] = {},
+        parameters: dict[str, object] = {},
         ex: Exception = None,
         traces_levels: int = 10,
     ):
         self.name = name if name is not None else "exception"
         self.warning = 1 if warning else 0
         if isinstance(name, Exception):
             self.name = "exception"
```

### Comparing `alphaz-0.7.6.2/alphaz/models/main/_request.py` & `alphaz-0.7.6.3/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/main/_singleton.py` & `alphaz-0.7.6.3/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/models/request.py` & `alphaz-0.7.6.3/alphaz/models/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODULES
 import requests
-from typing import Dict, Optional
 
 # ALPHAZ
 from alphaz.models.config import AlphaConfig
 
 # CORE
 from core import core
 
@@ -35,15 +34,15 @@
             A string representing the URL for the given route.
         """
         if not route.startswith("/"):
             route = "/" + route
         protocol = "https" if self.config.get("ssl") else "http"
         return f"{protocol}://{self.host}{route}"
 
-    def post(self, route: str, data: Optional[Dict] = None) -> Optional[str]:
+    def post(self, route: str, data: dict | None = None) -> str | None:
         """
         Send a POST request to the given route.
 
         Args:
             route: The route to send the POST request to.
             data: The data to include in the POST request (optional).
```

### Comparing `alphaz-0.7.6.2/alphaz/models/tests/_category.py` & `alphaz-0.7.6.3/alphaz/models/tests/_category.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 from ..tests import Levels
 from ..database.main_definitions import Tests
 
 # LOCAL
 from ._group import TestGroup
 
 # CORE
-from ... import Dict, List, timer
+from ... import timer
 
 from core import core
 
 
 class TestCategory:
     def __init__(self, category):
         self.category = category
         self.status: bool = True
-        self.groups: Dict[str, TestGroup] = {}
+        self.groups: dict[str, TestGroup] = {}
 
     def add_test_group(self, testGroup: TestGroup):
         self.groups[testGroup.name] = testGroup
 
     def test_all(
-        self, names: List[str] = None, levels: List[Levels] = [], stop: bool = True
+        self,
+        names: list[str] | None = None,
+        levels: list[Levels] = [],
+        stop: bool = True,
     ) -> bool:
         for test_group in self.groups.values():
             if not test_group.test_all(names, levels):
                 self.status = False
                 if stop:
                     break
         return self.status
@@ -58,27 +61,30 @@
 
 def truncate_time(number: float):
     return int(number * 100) / 100
 
 
 class TestCategories:
     def __init__(self):
-        self.categories: Dict[str, TestCategory] = {}
+        self.categories: dict[str, TestCategory] = {}
         self.status: bool = True
 
     def add_test_group(self, test_group: TestGroup):
         if not test_group.category in self.categories:
             self.categories[test_group.category] = TestCategory(test_group.category)
 
         self.categories[test_group.category].add_test_group(test_group)
 
         self.categories = dict_lib.sort_dict(self.categories)
 
     def test_all(
-        self, names: List[str] = None, levels: List[Levels] = [], stop: bool = True
+        self,
+        names: list[str] | None = None,
+        levels: list[Levels] = [],
+        stop: bool = True,
     ) -> bool:
         stopped = False
         for category in self.categories.values():
             if stopped:
                 break
             for test_group in category.groups.values():
                 if stopped:
@@ -111,15 +117,15 @@
                         ),
                         None,
                     )
 
                     if test_db is not None:
                         test.update_from_database(test_db)
 
-    def report(self, file_path: str = None) -> str:
+    def report(self, file_path: str | None = None) -> str:
         contents = []
         space = "   "
         c_space = "      "
         g_space = "         "
 
         failed, success, times = [], [], 0
         l_content = []
```

### Comparing `alphaz-0.7.6.2/alphaz/models/tests/_group.py` & `alphaz-0.7.6.3/alphaz/models/tests/_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 
 # MODELS
 from ..tests import Levels
 from ..database.main_definitions import Tests
 
 # LOCAL
-from ... import Dict, List, OrderedDict, timer
+from ... import OrderedDict, timer
 from ._method import TestMethod
 from ._wrappers import TEST_METHOD_NAME
 
 # CORE
 from core import core
 
 
@@ -67,15 +67,15 @@
                 test.update_from_database(test_db)
 
     def test(self, name: str):
         if name in self.tests:
             self.tests[name].test(coverage=self.coverage)
 
     def test_all(
-        self, names: List[str] = None, levels: List[Levels] = [], stop: bool = True
+        self, names: list[str] = None, levels: list[Levels] = [], stop: bool = True
     ) -> bool:
         tests = self.tests
         if names is not None and len(names) != 0:
             tests = {x: y for x, y in tests.items() if x in names}
         if levels is not None and len(levels) != 0:
             tests = {x: y for x, y in tests.items() if y.level.name in levels}
```

### Comparing `alphaz-0.7.6.2/alphaz/models/tests/_method.py` & `alphaz-0.7.6.3/alphaz/models/tests/_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODULES
-import datetime, re
-import typing
+import datetime
 
 # MODELS
 from ..database.main_definitions import Tests
 
 # LIBS
 from ...libs import number_lib
 
@@ -46,15 +45,15 @@
         self.level = level
 
         self.status: bool = None
         self.start_time: datetime.datetime = None
         self.end_time: datetime.datetime = None
         self.elapsed: int = 0
         self.last_run_elapsed = None
-        self.coverages: typing.Dict[str, object] = {}
+        self.coverages: dict[str, object] = {}
 
         self.ex: Exception = None
 
     def test(self, classTest=None, coverage: bool = False):
         if classTest is None:
             classTest = self.classTest()
```

### Comparing `alphaz-0.7.6.2/alphaz/models/tests/_save.py` & `alphaz-0.7.6.3/alphaz/models/tests/_save.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         Set the root directory for saving files.
 
         Args:
             root: The new root directory to use for saving files.
         """
         self.root = root
 
-    def get_file_path(self, filename: str, class_name: str = None) -> str:
+    def get_file_path(self, filename: str, class_name: str | None = None) -> str:
         """
         Get the file path for a given filename and class name.
 
         Args:
             filename: The name of the file to get the path for.
             class_name: The name of the class to save the file under.
```

### Comparing `alphaz-0.7.6.2/alphaz/models/tests/_test.py` & `alphaz-0.7.6.3/alphaz/models/tests/_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MODULES
 import traceback, inspect, trace, sys, os
-from typing import List, Dict
+
 from dataclasses import copy, dataclass
 import pandas as pd
 
 # CORE
 from core import core
 
 # LIBS
@@ -24,16 +24,16 @@
 
 class AlphaTest:
     _test = True
     category = ""
     index = 0
     current_test_name = ""
 
-    outputs: Dict[str, bool] = {}
-    coverages: Dict[str, object] = {}
+    outputs: dict[str, bool] = {}
+    coverages: dict[str, object] = {}
 
     def __init__(self):
         self.begin_class()
 
     def begin_class(self):
         pass
 
@@ -41,16 +41,16 @@
         pass
 
     def end(self):
         pass
 
     def init_tables(
         self,
-        tables: List[str],
-        binds: List[str] = None,
+        tables: list[str],
+        binds: list[str] | None = None,
         truncate: bool = False,
         drop: bool = False,
         create: bool = False,
         init: bool = True,
     ):
         database_lib.init_databases(
             core=core,
@@ -89,130 +89,130 @@
             self.coverages[name] = tracer.results()
         if self.output is not None:
             status = self.output
 
         return status
 
     def reverse(self) -> bool:
-        self.__reverse_output()
+        return self.__reverse_output()
 
     def __reverse_output(self) -> bool:
         self.output = not self.output
         return self.output
 
     def _set_output(self, status) -> bool:
         if self.output is not None:
             self.output = status and self.output
         else:
             self.output = status
         return status
 
-    def _assert(self, status, conditions: List[bool] = [], msg: str = "") -> bool:
+    def _assert(self, status, conditions: list[bool] = [], msg: str = "") -> bool:
         if len(conditions) != 0 and type(conditions) == list:
             status = status and all(conditions)
         return self._set_output(status)
 
     def assert_array_equal(
-        self, a, b, conditions: List[bool] = [], msg: str = ""
+        self, a, b, conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         status = len(a) == len(b)
         if status:
             for i in range(len(a)):
                 if a[i] != b[i]:
                     status = False
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: <{a}> and <{b}> are not equals"
             )
         return self._assert(status, conditions)
 
-    def assert_is_not_none(self, a, conditions: List[bool] = [], msg: str = "") -> bool:
+    def assert_is_not_none(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
         status = a is not None
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value is None")
         return self._assert(status, conditions)
 
-    def assert_is_none(self, a, conditions: List[bool] = [], msg: str = "") -> bool:
+    def assert_is_none(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
         status = a is None
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value is not None")
         return self._assert(status, conditions)
 
     def assert_is_empty(
-        self, a, conditions: List[bool] = [], msg: str = "", attribute=None
+        self, a, conditions: list[bool] = [], msg: str = "", attribute=None
     ) -> bool:
         status = self.assert_is_not_empty(
             a, conditions=conditions, attribute=attribute, msg=msg
         )
         if status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value is not empty")
         return self.__reverse_output()
 
     def assert_are_keys_in_model_attributes(
-        self, a, model, attributes=[], conditions: List[bool] = [], msg: str = ""
+        self, a, model, attributes=[], conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         status = self.assert_are_keys_in_models_attributes(
             a, [model], attributes=attributes, conditions=conditions
         )
         return status
 
     def assert_are_keys_in_models_attributes(
-        self, a, models, attributes=[], conditions: List[bool] = [], msg: str = ""
+        self, a, models, attributes=[], conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         self.assert_is_not_none(a, msg=msg)
         for model in models:
             attributes.extend(list(model.get_schema()._declared_fields.keys()))
         attributes = list(set(attributes))
         key_in = {x: x in attributes for x in a.keys()}
         status = all(key_in.values())
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: missing keys in model: {','.join([x for x, y in key_in.items() if not y])}"
             )
         return self._assert(status, conditions)
 
     def assert_has_model_attributes(
-        self, a, model, conditions: List[bool] = [], msg: str = ""
+        self, a, model, conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         self.assert_is_not_none(a, msg=msg)
         fields = list(model.get_schema()._declared_fields.keys())
         if not hasattr(a, "keys"):
             return self._assert(False, conditions)
         key_in = {x: x in a.keys() for x in fields}
         status = all(key_in.values())
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: missing model keys: {','.join([x for x, y in key_in.items() if not y])}"
             )
         return self._assert(status, conditions)
 
-    def assert_is_true(self, a, conditions: List[bool] = [], msg: str = "") -> bool:
+    def assert_is_true(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
         status = a
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value {a} is not True")
         return self._assert(status, conditions)
 
-    def assert_is_false(self, a, conditions: List[bool] = [], msg: str = "") -> bool:
+    def assert_is_false(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
         status = a
         if status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value {a} is not False")
         return self._assert(not status, conditions)
 
     def assert_contains(
-        self, container, element, conditions: List[bool] = [], msg: str = ""
+        self, container, element, conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         status = element in container
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: {container=} does not contain {element=}"
             )
         return self._assert(status, conditions)
 
     def assert_is_not_empty(
-        self, a, conditions: List[bool] = [], msg: str = "", attribute=None
+        self, a, conditions: list[bool] = [], msg: str = "", attribute=None
     ) -> bool:
         if attribute is not None:
             if not hasattr(a, attribute):
                 LOG.info(
                     f"{self.current_test_name} {msg} - Object of type <{type(a)}> does not have an attribute named <{attribute}>"
                 )
             status = a is not None and not len(getattr(a, attribute)) == 0
@@ -220,66 +220,66 @@
             status = a is not None and not a.empty
         else:
             status = a is not None and len(a) != 0
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value is None")
         return self._assert(status, conditions)
 
-    def assert_is_dict(self, a, conditions: List[bool] = [], msg: str = "") -> bool:
+    def assert_is_dict(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
         status = type(a) == dict
         if not type(a) == dict:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value is not a dict")
         return self._assert(status, conditions)
 
-    def assert_is_dict_not_empty(self, a, conditions: List[bool] = [], msg: str = ""):
+    def assert_is_dict_not_empty(self, a, conditions: list[bool] = [], msg: str = ""):
         self.assert_is_dict(a, msg=msg)
         status = self.assert_is_not_empty(a, msg=msg)
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: dict {a} is empty")
         return self._assert(status, conditions)
 
     def assert_is_dict_with_key(
-        self, a, key, conditions: List[bool] = [], msg: str = ""
+        self, a, key, conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         self.assert_is_dict(a, msg=msg)
         status = key in a
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: dict has not key {key}")
         return self._assert(status, conditions)
 
     def assert_is_dict_with_key_not_empty(
-        self, a, key, conditions: List[bool] = [], msg: str = ""
+        self, a, key, conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         self.assert_is_not_none(a, msg=msg)
         self.assert_is_dict_with_key(a, key, msg=msg)
         status = self.assert_is_not_empty(a, msg=msg)
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: dict {a} has no empty key {key}"
             )
         return self._assert(status, conditions)
 
     def assert_is_dict_with_key_with_value(
-        self, a, key, value, conditions: List[bool] = [], msg: str = ""
+        self, a, key, value, conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         status = self.assert_is_dict_with_key_not_empty(a, key, msg=msg)
         if status:
             status = self.assert_equal(a[key], value, msg=msg)
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: {a} does not contains a {key=} with {value=}"
             )
         return self._assert(status, conditions)
 
     def assert_equal(
         self,
         a,
         b,
-        ignore: list | dict = None,
-        conditions: List[bool] = [],
+        ignore: list | dict | None = None,
+        conditions: list[bool] = [],
         msg: str = "",
     ) -> bool:
         if isinstance(a, list) and isinstance(b, list) and len(a) == 0 and len(b) == 0:
             return True
         if (
             isinstance(a, list)
             and isinstance(b, list)
@@ -317,15 +317,15 @@
                 )
         return self._assert(status, conditions)
 
     def assert_in_str(
         self,
         a: str,
         b: str,
-        conditions: List[bool] = [],
+        conditions: list[bool] = [],
         msg: str = "",
     ) -> bool:
         for e in [a, b]:
             if type(e) != str:
                 LOG.info(
                     f"{self.current_test_name} {msg} - Assert: {e} type is not str"
                 )
@@ -337,43 +337,43 @@
             )
         return self._assert(status, conditions)
 
     def assert_not_equal(
         self,
         a,
         b,
-        ignore: list | dict = None,
-        conditions: List[bool] = [],
+        ignore: list | dict | None = None,
+        conditions: list[bool] = [],
         msg: str = "",
     ) -> bool:
         status = a != b
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: {a} and {b} are equals")
         return self._assert(status, conditions)
 
     def assert_length(
         self,
         a,
         length,
-        conditions: List[bool] = [],
+        conditions: list[bool] = [],
         msg: str = "",
         strict: bool = False,
     ) -> bool:
         status_not_none = self.assert_is_not_none(a, msg=msg)
         status = len(a) == length
         if strict:
             status = status and len(a) != 0
         if not status and status_not_none:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: length {len(a)} is not the {length} expected"
             )
         return self._assert(status, conditions)
 
     def assert_transaction(
-        self, tr, conditions: List[bool] = [], msg: str = ""
+        self, tr, conditions: list[bool] = [], msg: str = ""
     ) -> bool:
         status_not_none = self.assert_is_not_none(tr, msg=msg)
         status = tr is not None and tr != "timeout"
         if not status and status_not_none:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: object if not a transaction"
             )
```

### Comparing `alphaz-0.7.6.2/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.6.3/alphaz/models/tests/_wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-from typing import List, Dict, Callable, Any
+from typing import Callable, Any
 from pathlib import Path
 
 # LOCALS
 from ...apis.users.users import try_su_login, logout_su
 from ..main import AlphaException
 from ...models.tests import AlphaTest
 from ...libs import dict_lib
@@ -15,15 +15,18 @@
 
 LOG = core.get_logger("tests")
 
 TEST_METHOD_NAME = "test_alpha_in"
 
 
 def call_function(
-    fct: Callable, obj: object, args: List = None, kwargs: Dict[str, object] = None
+    fct: Callable,
+    obj: object,
+    args: list | None = None,
+    kwargs: dict[str, object] | None = None,
 ) -> Any:
     """
     Call a function with arguments and return its output.
 
     Args:
         fct: The function to call.
         obj: The object to pass as the first argument if the function is a method.
@@ -45,29 +48,29 @@
         return fct(*args, **kwargs)
 
 
 def test(
     mandatory: bool = False,
     save: bool = False,
     save_ext: str = ".ast",
-    save_path: Path = None,
-    begin: Callable = None,
-    end: Callable = None,
-    save_post_process: Callable = None,
+    save_path: Path | None = None,
+    begin: Callable | None = None,
+    end: Callable | None = None,
+    save_post_process: Callable | None = None,
     return_diff: bool = False,
-    begin_args: list = None,
-    begin_kwargs: Dict[str, Any] = None,
-    end_args: list = None,
-    end_kwargs: Dict[str, Any] = None,
-    description: str = None,
+    begin_args: list | None = None,
+    begin_kwargs: dict[str, Any] | None = None,
+    end_args: list | None = None,
+    end_kwargs: dict[str, Any] | None = None,
+    description: str | None = None,
     stop: bool = True,
     disable: bool = False,
     level: Levels = Levels.MEDIUM,
-    admin_user_id: str = None,
-    admin_user_name: str = None,
+    admin_user_id: str | None = None,
+    admin_user_name: str | None = None,
 ) -> Callable:
     """
     Decorator used to mark a test function to be run.
 
     The test function should be a method of a class which inherits from `unittest.TestCase`.
     The decorator wraps the function in another function which performs various pre- and post-processing.
```

### Comparing `alphaz-0.7.6.2/alphaz/models/user.py` & `alphaz-0.7.6.3/alphaz/models/user.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,77 +2,76 @@
 from datetime import datetime
 
 from .main import (
     AlphaDataclass,
     AlphaMappingAttribute,
     dataclass,
     field,
-    List,
 )
 
 from alphaz.libs import json_lib
 
 
 @dataclass
 class AlphaApplication(AlphaDataclass):
     id: int
     name: str
-    description: str = None
+    description: str | None = None
 
 
 @dataclass
 class AlphaPermission(AlphaDataclass):
     key: str
     activated: bool
-    description: str = None
-    update_date: datetime = None
+    description: str | None = None
+    update_date: datetime | None = None
 
 
 @dataclass
 class AlphaRole(AlphaDataclass):
     name: str
     activated: bool
     id_app: int
     app: AlphaApplication
-    description: str = None
+    description: str | None = None
 
-    permissions: List[AlphaPermission] = field(default_factory=lambda: [])
+    permissions: list[AlphaPermission] = field(default_factory=lambda: [])
 
 
 @dataclass
 class AlphaUserRole(AlphaDataclass):
     user_id: int
     role_name: str
     role: AlphaRole
     activated: bool
 
 
 @dataclass
 class AlphaUser(AlphaDataclass):
     id: int
     username: str
-    last_activity: datetime = None
-    mail: str = None
+    last_activity: datetime | None = None
+    mail: str | None = None
     role: int = -1
-    password: str = None
+    password: str | None = None
 
     infos: dict = field(default_factory=lambda: {})
-    roles: List[AlphaRole] = field(default_factory=lambda: [])
-    permissions: List[str] = field(default_factory=lambda: [])
+    roles: list[AlphaRole] = field(default_factory=lambda: [])
+    permissions: list[str] = field(default_factory=lambda: [])
 
-    registration_token: str = None
-    pass_reset_token_exp: str = None
+    registration_token: str | None = None
+    pass_reset_token_exp: str | None = None
 
-    registration_code: str = None
-    expire: str = None
+    registration_code: str | None = None
+    expire: str | None = None
 
-    telegram_id: str = None
-    pass_reset_token: str = None
+    telegram_id: str | None = None
+    pass_reset_token: str | None = None
 
-    date_registred: str = None
+    date_registred: str | None = None
 
     def __post_init__(self):
         permissions = [
             [x.key for x in y.permissions if x is not None and x.activated]
             for y in self.roles
             if y is not None and y.activated
         ]
@@ -107,18 +106,17 @@
 
 @dataclass
 class AlphaUserSession(AlphaDataclass):
     user_id: int
     token: str
     ip: int
     expire: datetime
-    update_date: datetime = None
+    update_date: datetime | None = None
 
 
 @dataclass
 class AlphaRolePermission(AlphaDataclass):
     role_name: str
     role: AlphaRole
     permission_key: str
     permission: AlphaPermission
     activated: bool
-
```

### Comparing `alphaz-0.7.6.2/alphaz/models/watcher.py` & `alphaz-0.7.6.3/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/pocs/main.py` & `alphaz-0.7.6.3/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/run.py` & `alphaz-0.7.6.3/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/src/alpha.png` & `alphaz-0.7.6.3/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/src/configs/loggers.json` & `alphaz-0.7.6.3/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/stitch/Core.py` & `alphaz-0.7.6.3/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/stitch/stitch.py` & `alphaz-0.7.6.3/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.6.3/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.6.3/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/css/home.css` & `alphaz-0.7.6.3/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.6.3/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.6.3/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.6.3/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.6.3/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.6.3/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.6.3/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.6.3/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.6.3/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/home.html` & `alphaz-0.7.6.3/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/templates/logs.html` & `alphaz-0.7.6.3/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/test.py` & `alphaz-0.7.6.3/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/tests/api.py` & `alphaz-0.7.6.3/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/tests/basic_test.py` & `alphaz-0.7.6.3/alphaz/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/tests/configurations.py` & `alphaz-0.7.6.3/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/tests/database.py` & `alphaz-0.7.6.3/alphaz/tests/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/tests/utils.py` & `alphaz-0.7.6.3/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/api.py` & `alphaz-0.7.6.3/alphaz/utils/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import traceback
 
-from typing import List, Dict, Union
+
 from flask import (
     jsonify,
     make_response,
     request,
     send_file,
     send_from_directory,
     abort,
@@ -56,30 +56,30 @@
     ADMIN_USER_NAME_PRIVATE,
 ]
 
 
 default_parameters_names = [p.name for p in default_parameters]
 
 
-def get_pagination_parameters(pagination: int = None):
+def get_pagination_parameters(pagination: int | None = None):
     if type(pagination) == bool:
         return [
             Parameter("page", ptype=int, default=0),
             Parameter("per_page", ptype=int),
         ]
     else:
         return [
             Parameter("page", ptype=int, default=0),
             Parameter("per_page", ptype=int, default=pagination),
         ]
 
 
 def _process_parameters(
-    path: str, parameters: List[Parameter], pagination: int = None
-) -> List[Parameter]:
+    path: str, parameters: list[Parameter], pagination: int | None = None
+) -> list[Parameter]:
     parameters = [] if parameters is None else parameters
     overrides = []
     for i, parameter in enumerate(parameters):
         if type(parameter) == str:
             parameter = Parameter(parameter)
             parameters[i] = parameter
         if parameter.name in default_parameters_names:
@@ -104,27 +104,27 @@
         )
     output_parameter.extend(parameters)
     return output_parameter
 
 
 def route(
     path,
-    parameters: List[Parameter] = None,
+    parameters: list[Parameter] | None = None,
     methods=["GET"],
     cache: bool = False,
     logged: bool = False,
     admin: bool = False,
-    timeout: int = None,
-    category: str = None,
-    description: str = None,
-    mode: str = None,
+    timeout: int | None = None,
+    category: str | None = None,
+    description: str | None = None,
+    mode: str | None = None,
     route_log: bool = True,
-    access_strings: Union[List[str], List[Enum]] = [],
-    access_error_message: str = None,
-    pagination: int = None,
+    access_strings: list[str] | list[Enum] = [],
+    access_error_message: str | None = None,
+    pagination: int | None = None,
 ):
     path = "/" + path if path[0] != "/" else path
 
     parameters = _process_parameters(path, parameters, pagination=pagination)
 
     def api_in(func):
         api.add_url_rule(path, methods=methods, view_func=func, endpoint=func.__name__)
```

### Comparing `alphaz-0.7.6.2/alphaz/utils/apm/ora.py` & `alphaz-0.7.6.3/alphaz/utils/apm/ora.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/configuration.py` & `alphaz-0.7.6.3/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/database/init.py` & `alphaz-0.7.6.3/alphaz/utils/database/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MODULES
 import glob, os, importlib, re, json
-from typing import Dict, List, Union, Optional, Any
+
 
 # MODELS
 from ...models.main import AlphaException, AlphaCore
 
 
 def __get_module_path(file_path: str) -> str:
     """
@@ -24,23 +24,23 @@
     if module_path[0] == ".":
         module_path = module_path[1:]
 
     return module_path
 
 
 def __process_python_file(
-    core: AlphaCore, bind: str, file_path: str, tables: List[str]
+    core: AlphaCore, bind: str, file_path: str, tables: list[str]
 ) -> None:
     """
     Process a Python file for database initialization.
 
     :param core: AlphaCore instance to work with.
     :param bind: Bind name to work with.
     :param file_path: Path to the Python file containing the database initialization configuration.
-    :param tables: List of table names to process, None for all tables.
+    :param tables: list of table names to process, None for all tables.
     :raises AlphaException: If there is any issue with the provided configuration or file.
     """
     module_path = __get_module_path(file_path)
 
     module = importlib.import_module(module_path)
 
     if not hasattr(module, "ini"):
@@ -53,23 +53,23 @@
         )
 
     for real_table_name, conf in ini.items():
         __process_table(core, bind, real_table_name, tables, file_path, conf)
 
 
 def __process_json_file(
-    core: AlphaCore, bind: str, file_path: str, tables: List[str]
+    core: AlphaCore, bind: str, file_path: str, tables: list[str]
 ) -> None:
     """
     Process a JSON file for database initialization.
 
     :param core: AlphaCore instance to work with.
     :param bind: Bind name to work with.
     :param file_path: Path to the JSON file containing the database initialization configuration.
-    :param tables: List of table names to process, None for all tables.
+    :param tables: list of table names to process, None for all tables.
     :raises AlphaException: If there is any issue with the provided configuration or file.
     """
     try:
         data = {}
         if os.path.exists(file_path):
             with open(file_path, encoding="utf-8") as json_data_file:
                 data = json.load(json_data_file)
@@ -101,25 +101,25 @@
                 core.db.log.error(f"Error with init of {file_path=}", ex=ex)
 
 
 def __process_table(
     core: AlphaCore,
     bind: str,
     table_name: str,
-    tables: List[str],
+    tables: list[str],
     file_path: str,
     conf: dict,
 ) -> None:
     """
     Process a table based on the provided configuration.
 
     :param core: AlphaCore instance to work with.
     :param bind: Bind name to work with.
     :param table_name: Name of the table to process.
-    :param tables: List of table names to process, None for all tables.
+    :param tables: list of table names to process, None for all tables.
     :param file_path: Path to the file containing the database initialization configuration.
     :param conf: Configuration for the table.
     """
     if tables is not None and table_name.upper() not in [x.upper() for x in tables]:
         return
 
     if type(table_name) != str and hasattr(table_name, "__tablename__"):
@@ -169,28 +169,28 @@
 
 def __process_headers_values(
     core: AlphaCore,
     file_path: str,
     bind: str,
     table_name: str,
     table,
-    headers: List[str],
-    values: List[Union[str, dict]],
+    headers: list[str],
+    values: list[str | dict],
     data_type: str = "alpha",
 ) -> None:
     """
     Process headers and values for a given table.
 
     :param core: AlphaCore instance to work with.
     :param file_path: Path to the file containing the database initialization configuration.
     :param bind: Bind name to work with.
     :param table_name: Name of the table to process.
     :param table: Table object to process.
-    :param headers: List of header names.
-    :param values: List of values for the table.
+    :param headers: list of header names.
+    :param values: list of values for the table.
     :param data_type: Type of data being processed (default is "alpha").
     :raises ValueError: If an invalid data_type is provided.
     """
     if not isinstance(values, list):
         core.log.error(
             f'In file {file_path} "values" key from {table_name=} and {bind=} must be of type <list>'
         )
@@ -209,27 +209,27 @@
 
 
 def __extract_entries(
     core: AlphaCore,
     file_path: str,
     bind: str,
     table_name: str,
-    values: List[Union[str, dict]],
+    values: list[str | dict],
     data_type: str,
-) -> List[List[str]]:
+) -> list[list[str]]:
     """
     Extract entries from the given values based on the data type.
 
     :param core: AlphaCore instance to work with.
     :param file_path: Path to the file containing the database initialization configuration.
     :param bind: Bind name to work with.
     :param table_name: Name of the table to process.
-    :param values: List of values for the table.
+    :param values: list of values for the table.
     :param data_type: Type of data being processed.
-    :return: List of extracted entries.
+    :return: list of extracted entries.
     :raises ValueError: If an invalid data_type is provided.
     """
     entries = []
 
     for entry in values:
         if data_type == "alpha":
             if not isinstance(entry, list):
@@ -254,46 +254,46 @@
     return entries
 
 
 def __process_databases_init(
     core: AlphaCore,
     bind: str,
     file_path: str,
-    tables: List[str] = None,
+    tables: list[str] | None = None,
     file_type: str = "py",
 ) -> None:
     """
     Process database initialization based on the given file type (Python, JSON, or SQL).
 
     :param core: AlphaCore instance to work with.
     :param bind: Bind name to work with.
     :param file_path: Path to the file containing the database initialization configuration.
-    :param tables: List of table names to process, None for all tables.
+    :param tables: list of table names to process, None for all tables.
     :param file_type: Type of file to process (default is "py").
     :raises AlphaException: If there is any issue with the provided configuration or file.
     """
     if file_type == "py":
         __process_python_file(core, bind, file_path, tables)
     elif file_type == "json":
         __process_json_file(core, bind, file_path, tables)
     elif file_type == "sql":
         __process_sql_file(core, bind, file_path)
     else:
         raise ValueError(f"Unsupported file type '{file_type}'")
 
 
 def process_init_files(
-    core: AlphaCore, binds: List[str], tables: List[str], init_databases_config: dict
+    core: AlphaCore, binds: list[str], tables: list[str], init_databases_config: dict
 ):
     """Charge les fichiers d'initialisation en fonction des types de fichiers et du répertoire d'initialisation spécifié pour chaque type.
 
     Args:
         core (AlphaCore): objet Core contenant les informations de base et les configurations
-        binds (List[str]): Liste des binds à traiter
-        tables (List[str]):  Liste ou dictionnaire des noms des tables à traiter. Defaults to None.
+        binds (list[str]): Liste des binds à traiter
+        tables (list[str]):  Liste ou dictionnaire des noms des tables à traiter. Defaults to None.
         init_databases_config (dict): Dictionnaire de configuration d'initialisation normalisé avec les clés en majuscules
     """
     ini_types = {
         "json": {"key": "init_database_dir_json", "pattern": "*.json"},
         "py": {"key": "init_database_dir_py", "pattern": "*.py"},
         "sql": {"key": "init_database_dir_sql", "pattern": "*.sql"},
     }
@@ -317,67 +317,67 @@
 
             for file_path in files:
                 __process_databases_init(
                     core, bind, file_path, tables, file_type=ini_type
                 )
 
 
-def __normalize_tables(tables: List[str] | Dict[str, str]) -> List[str]:
+def __normalize_tables(tables: list[str] | dict[str, str]) -> list[str]:
     """Normalise le paramètre 'tables' pour s'assurer qu'il est sous la forme d'un dictionnaire avec les noms des tables en majuscules.
 
     Args:
-        tables (List[str]): Liste ou dictionnaire des noms des tables à traiter
+        tables (list[str]): Liste ou dictionnaire des noms des tables à traiter
 
     Returns:
-        List[str] | Dict[str, str]: _description_
+        list[str] | dict[str, str, optional: _description_
     """
     if tables is not None:
         return (
             {x.upper(): None for x in tables}
             if type(tables) == list
             else {x.upper(): y for x, y in tables.items()}
         )
     return tables
 
 
-def __normalize_and_check_binds(binds: List[str], core: AlphaCore) -> List[str]:
+def __normalize_and_check_binds(binds: list[str], core: AlphaCore) -> list[str]:
     """Normalise le paramètre 'binds' et vérifie que les binds sont valides.
 
     Args:
-        binds (List[str]): Liste des binds à traiter
+        binds (list[str]): Liste des binds à traiter
         core (AlphaCore): objet Core contenant les informations de base et les configurations
 
     Raises:
         AlphaException: _description_
 
     Returns:
-        List[str]: Liste contenant la liste des binds normalisés et la liste des binds récupérés depuis l'objet Core
+        list[str]: Liste contenant la liste des binds normalisés et la liste des binds récupérés depuis l'objet Core
     """
     db_binds = core.db.get_all_binds()
     binds = [bind.upper() for bind in binds] if binds is not None else db_binds
     if len(binds) != len(db_binds):
         for bind in binds:
             if not bind in db_binds:
                 raise AlphaException(f"Cannot find {bind=}")
     return binds
 
 
-def __get_normalized_init_config(core: AlphaCore) -> Dict[str, dict]:
+def __get_normalized_init_config(core: AlphaCore) -> dict[str, dict]:
     """Récupère et normalise la configuration d'initialisation des bases de données.
 
     Args:
         core (AlphaCore): objet Core contenant les informations de base et les configurations
 
     Raises:
         AlphaException: _description_
 
     Returns:
-        Dict[str, dict]: Dictionnaire de configuration d'initialisation normalisé avec les clés en majuscules
+        dict[str, dict]: Dictionnaire de configuration d'initialisation normalisé avec les clés en majuscules
     """
-    init_databases_config = core.config.get("databases")
+    init_databases_config: dict = core.config.get("databases")
     if init_databases_config is None:
         raise AlphaException(
             "No initialisation configuration has been set in <databases> entry"
         )
     return {x.upper(): y for x, y in init_databases_config.items()}
```

### Comparing `alphaz-0.7.6.2/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.6.3/alphaz/utils/database_to_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from timeit import default_timer as timer
 from datetime import timedelta
 
 from datetime import datetime
 from alphaz.models.main import (
     AlphaDataclass, 
     dataclass,
-    List
+    list
 )
 
 @dataclass
 class {class_name}(AlphaDataclass):
 {fields}
 
-def load_{table_name_lower}(limit:int=None) -> List[{class_name}]:
+def load_{table_name_lower}(limit:int=None) -> list[{class_name}]:
     print("Loading table {table_name} ...")
     start = timer()
     from core import core
     DB = core.db
 
     raw_results = DB.get_query_results("select * from {table_name}" + ("" if not limit else " LIMIT " + str(limit)), bind="{bind}")
     end = timer()
```

### Comparing `alphaz-0.7.6.2/alphaz/utils/decorators.py` & `alphaz-0.7.6.3/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/ensure.py` & `alphaz-0.7.6.3/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/init_database.py` & `alphaz-0.7.6.3/alphaz/utils/init_database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/mep.py` & `alphaz-0.7.6.3/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/screens.py` & `alphaz-0.7.6.3/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/selectionMenu.py` & `alphaz-0.7.6.3/alphaz/utils/selectionMenu.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,263 +1,303 @@
-'''
+"""
 Created on 24 juin 2018
 
 @author: aurele
-'''
+"""
 import re, os, copy, traceback
 
 from ..libs.converter_lib import to_int
 from ..libs import py_lib, io_lib
 from .logger import AlphaLogger
 
+
 def reload_modules():
     reload_path = os.getcwd()
-    #print('Reload modules at %s'%reload_path)
+    # print('Reload modules at %s'%reload_path)
     py_lib.reload_modules(reload_path)
-    reload_path = os.sep.join(os.path.dirname(os.path.abspath(__file__)).split(os.sep)[:-1])
-    #print('Reload modules at %s'%reload_path)
+    reload_path = os.sep.join(
+        os.path.dirname(os.path.abspath(__file__)).split(os.sep)[:-1]
+    )
+    # print('Reload modules at %s'%reload_path)
     py_lib.reload_modules(reload_path)
 
+
 def replace_name(name):
-    return name.lower().replace(' ','_')
+    return name.lower().replace(" ", "_")
 
-class SelectionMenu():
-    name            = None
-    save_directory  = None
-    level           = 0
-    commands        = []
-    selected        = []
-    selected_history= []
-    record          = False
-    in_command      = False
-    sequence        = []
 
-    def __init__(self, name, parameters, save_directory, config_file=None, config_folder='config/menus',log=None):
+class SelectionMenu:
+    name = None
+    save_directory = None
+    level = 0
+    commands = []
+    selected = []
+    selected_history = []
+    record = False
+    in_command = False
+    sequence = []
+
+    def __init__(
+        self,
+        name,
+        parameters,
+        save_directory,
+        config_file=None,
+        config_folder="config/menus",
+        log=None,
+    ):
         if log is None:
             log = core.get_logger()
 
-        self.name           = name
+        self.name = name
         self.save_directory = save_directory
 
-        self.parameters     = parameters        
-        self.returnValue    = None
+        self.parameters = parameters
+        self.returnValue = None
 
-        self.exit           = False
-        self.log            = log
+        self.exit = False
+        self.log = log
+
+        self.config_folder = config_folder
+        self.config_file = config_file
 
-        self.config_folder  = config_folder
-        self.config_file    = config_file
-        
         self.load_default_values()
-        
-    def debug_print(self,string):
+
+    def debug_print(self, string):
         if self.get_value("debug_menu"):
-            print(__name__,string)
-        
+            print(__name__, string)
+
     def run(self):
         while not self.exit:
             self.level = 0
             self.execute(self.parameters)
         return self.returnValue
-        
-    def execute(self,conf):
+
+    def execute(self, conf):
         conf = copy.copy(conf)
 
         if type(conf) == list:
             for sub_conf in conf:
                 self.execute(sub_conf)
             return
 
         conf = self.convert_parameters(conf)
 
-        if 'command' in conf:
+        if "command" in conf:
             self.in_command = True
 
         try:
             reload_modules()
 
-            if "before" in conf:        self.execute(conf["before"])
+            if "before" in conf:
+                self.execute(conf["before"])
 
             # BETWEEN
-            if 'set' in conf:
-                for key, value in conf['set'].items():
-                    self.set_value(key, value) #,convert=self.get_parameter_value(config,'convert'))
-
-            if 'switch' in conf:
-                if type(conf['switch']) == dict:
-                    for key in conf['switch']:
+            if "set" in conf:
+                for key, value in conf["set"].items():
+                    self.set_value(
+                        key, value
+                    )  # ,convert=self.get_parameter_value(config,'convert'))
+
+            if "switch" in conf:
+                if type(conf["switch"]) == dict:
+                    for key in conf["switch"]:
                         self.switch_value(key)
                 else:
-                    self.switch_value(conf['switch'])
+                    self.switch_value(conf["switch"])
 
             self.functions_evaluate(conf)
             self.printEvaluate(conf)
 
             if "input" in conf:
-                value                                       = input("\nValue: ")
-                self.set_value(conf['set'], self.convert_value(value,convert=self.get_parameter_value(conf,'convert')) )
+                value = input("\nValue: ")
+                self.set_value(
+                    conf["set"],
+                    self.convert_value(
+                        value, convert=self.get_parameter_value(conf, "convert")
+                    ),
+                )
 
             if "quit" in conf or "exit" in conf:
-                self.exit                                   = True
+                self.exit = True
 
             # set returning value
-            if 'return' in conf:
-                self.returnValue                            = self.convert_value(conf['return'])
+            if "return" in conf:
+                self.returnValue = self.convert_value(conf["return"])
 
             # SELECTIONS
-            
-            if "selections" in conf:    
+
+            if "selections" in conf:
                 self.level += 1
                 self.select(conf["selections"])
 
-            if "after" in conf:         self.execute(conf["after"]) 
+            if "after" in conf:
+                self.execute(conf["after"])
 
             if "selections" in conf:
                 if len(self.selected) >= 1:
                     self.selected = self.selected[:-1]
-                self.level -=1
+                self.level -= 1
 
             if "pause" in conf:
-                input('Press enter to continue ...')
+                input("Press enter to continue ...")
         except:
-            text    = traceback.format_exc()
-            print('ERROR:\n\n',str(text))
+            text = traceback.format_exc()
+            print("ERROR:\n\n", str(text))
 
         """if self.get_parameter_value(executingConfig,'bypass') is not None:
             conf                                      = executingConfig  
         else:
             conf                                      = self.select(executingConfig)"""
-             
-        #self.valueEvaluate(conf)
-              
-        ### SELECTION MENU  
+
+        # self.valueEvaluate(conf)
+
+        ### SELECTION MENU
         """if 'selection' in MODE:
             selectionValues                             = self.get_parameter_value(conf,'selection_values')
             multiple                                    = 'selections'  in MODE
             key_mode                                    = 'key'         in MODE
             #             selectionValues = self.get_parameter_value(conf,'selection_values')
             if selectionValues is not None:
                 newConfig                               = self.get_config_from_values(conf,selectionValues,multiple=multiple,key_mode=key_mode)
             else:
                 newConfig                               = conf['selection_config']"""
-           
-        if 'command' in conf:
+
+        if "command" in conf:
             self.in_command = False
 
-    def select(self,selections_config):
-        selections_config       = copy.copy(selections_config)
+    def select(self, selections_config):
+        selections_config = copy.copy(selections_config)
 
-        commands_selections     = self.get_commands()
-        formatStr               = '{:7} {:40} {:30} {}'
-        header                  = '   '*self.level
+        commands_selections = self.get_commands()
+        formatStr = "{:7} {:40} {:30} {}"
+        header = "   " * self.level
 
-        conf     = {}
+        conf = {}
         selected = None
         while selected is None:
-            self.debug_print('      VALUES:\n%s'%str('\n'.join(["   {:20}:{}".format(x,y) for x,y in self.values.items()])))
-            i                       = 0
-            selections              = {x['key']:x for x in commands_selections if 'key' in x}
-        
-            select_list             = copy.copy(commands_selections)
+            self.debug_print(
+                "      VALUES:\n%s"
+                % str(
+                    "\n".join(
+                        ["   {:20}:{}".format(x, y) for x, y in self.values.items()]
+                    )
+                )
+            )
+            i = 0
+            selections = {x["key"]: x for x in commands_selections if "key" in x}
+
+            select_list = copy.copy(commands_selections)
             select_list.extend(self.selected)
             select_list.extend(selections_config)
 
             for conf in select_list:
                 if type(conf) == dict:
                     if "txt_selection" in conf:
-                        print(conf['txt_selection'])
+                        print(conf["txt_selection"])
                         continue
 
-                    desc                = self.get_string(conf,'description')
-                    name                = self.get_string(conf,'name')
+                    desc = self.get_string(conf, "description")
+                    name = self.get_string(conf, "name")
 
                     if "header" in conf:
-                        print("\n"+header+formatStr.format("","== " + conf['header'] + " ==","",desc)+"\n")
+                        print(
+                            "\n"
+                            + header
+                            + formatStr.format(
+                                "", "== " + conf["header"] + " ==", "", desc
+                            )
+                            + "\n"
+                        )
                         continue
 
-                    #activate            = conf['mode'] == 'activate' if 'mode' in conf.keys() else False
-                    #self.debug_print("name - select configuration: %s"%conf)
+                    # activate            = conf['mode'] == 'activate' if 'mode' in conf.keys() else False
+                    # self.debug_print("name - select configuration: %s"%conf)
 
-                    #self.valueEvaluate(conf,start=True)
-                    #self.functions_evaluate(conf,start=True)
+                    # self.valueEvaluate(conf,start=True)
+                    # self.functions_evaluate(conf,start=True)
+
+                    key = conf["key"] if "key" in conf.keys() else str(i)
 
-                    key                 = conf['key'] if 'key' in conf.keys() else str(i)
-                    
                     # DEFAULT VALUE
-                    #if not self.get_parameter_value(conf, 'no_default'):
-                    default         = "" if not 'name' in conf else self.get_value(conf['name'])
-                    if default is None and 'value' in conf:
-                        default     = conf['value']
+                    # if not self.get_parameter_value(conf, 'no_default'):
+                    default = "" if not "name" in conf else self.get_value(conf["name"])
+                    if default is None and "value" in conf:
+                        default = conf["value"]
                     elif default is None:
-                        default     = ""
+                        default = ""
 
                     if type(default) == bool:
-                        switch      = 'switch' in conf.keys()
+                        switch = "switch" in conf.keys()
                         if switch:
-                            default = 'ON' if default else 'OFF'
+                            default = "ON" if default else "OFF"
                         else:
                             default = "Y" if default else "N"
 
                     """if 'mode' in conf.keys() and conf['mode'] == 'activate':
                         default = str(key) in str(default).split(',')"""
-                                                                    
+
                     show = True
-                    if 'show' in conf.keys():
-                        show            = conf['show']
-                        vshow           = self.get_value(show)
-                        show            = vshow if vshow is not None else show
-                        
+                    if "show" in conf.keys():
+                        show = conf["show"]
+                        vshow = self.get_value(show)
+                        show = vshow if vshow is not None else show
 
-                    txt = formatStr.format(str(key),name,str(default),desc)
+                    txt = formatStr.format(str(key), name, str(default), desc)
                     if not key in self.commands:
                         txt = header + txt
-                    conf['txt_menu'] = txt
+                    conf["txt_menu"] = txt
                     if show:
                         print(txt)
-                    
+
                     self.printEvaluate(conf)
-                    
-                    selections[key]     = conf
 
-                    if not 'key' in conf:
+                    selections[key] = conf
+
+                    if not "key" in conf:
                         i += 1
                 else:
-                    selections[str(i)]     = {"set":{'selected': conf},"txt_menu":header + formatStr.format(str(i),conf,"","")}
-                    print(selections[str(i)]['txt_menu'])
+                    selections[str(i)] = {
+                        "set": {"selected": conf},
+                        "txt_menu": header + formatStr.format(str(i), conf, "", ""),
+                    }
+                    print(selections[str(i)]["txt_menu"])
                     i += 1
 
             if len(self.sequence) != 0:
-                selection       = self.sequence[0]
-                self.sequence   = self.sequence[1:]
+                selection = self.sequence[0]
+                self.sequence = self.sequence[1:]
             else:
-                selection            = input("\nSelection > ").lower()
+                selection = input("\nSelection > ").lower()
 
-            is_command           = re.match("(^[^0-9]+$)", str(selection))
+            is_command = re.match("(^[^0-9]+$)", str(selection))
             if is_command:
-                commands            = [x['key'] for x in select_list if 'key' in x]
+                commands = [x["key"] for x in select_list if "key" in x]
 
                 if selection in commands:
-                    conf            = [x for x in select_list if 'key' in x and x['key'] == selection][0]
+                    conf = [
+                        x for x in select_list if "key" in x and x["key"] == selection
+                    ][0]
                 else:
-                    commandFounds   = 0
+                    commandFounds = 0
                     for command in commands:
-                        m           = re.match("("+selection+"[^0-9]+$)", command.lower())
+                        m = re.match("(" + selection + "[^0-9]+$)", command.lower())
                         if m:
-                            selection  = m.groups()[0]
+                            selection = m.groups()[0]
                             commandFounds += 1
-                            
+
                     if commandFounds != 1:
-                        print('\n>>>> ERROR: command not recognized be more specific !')
+                        print("\n>>>> ERROR: command not recognized be more specific !")
                         continue
                     else:
-                        conf          = selections[selection]
+                        conf = selections[selection]
             else:
                 if not selection in selections.keys():
                     continue
-                
+
                 """if activate:    
                     activated_values = str(self.values[conf['set']]).split(',')
                     
                     if str(selection) in activated_values:
                         activated_values.remove(str(selection))
                         self.values[conf['set']] = ','.join(activated_values)
                     else:
@@ -266,283 +306,353 @@
                         
                     print('SELECTED: %s'%self.values[conf['set']])
                     continue
                 else:"""
                 conf = selections[selection]
 
             selected = True
-        
-        sel = {'key':selection}
 
-        if 'txt_menu' in conf:
-            sel['txt_selection'] = conf['txt_menu']
+        sel = {"key": selection}
+
+        if "txt_menu" in conf:
+            sel["txt_selection"] = conf["txt_menu"]
         self.selected.append(sel)
 
-        if not self.in_command and not 'command' in conf:
-            print('\n                > Save action: %s\n'%str(conf))
+        if not self.in_command and not "command" in conf:
+            print("\n                > Save action: %s\n" % str(conf))
             self.selected_history.append(sel)
         else:
-            print('\n                > Not in command\n')
+            print("\n                > Not in command\n")
 
         self.execute(conf)
 
     def get_commands(self):
         selections = [
-            {'header':"COMMANDS"},
+            {"header": "COMMANDS"},
             {
-                'key': 'mo', 'name': 'Modes',
+                "key": "mo",
+                "name": "Modes",
                 "selections": [
-                    {'key':'dm',"value":False,'switch':'debug_menu','name':'Debug menu','description':"Turn ON/OFF the menu debug mode"},
-                    {'key':'d',"value":False,'name':'Debug','switch':'debug','description':"Turn ON/OFF the debug mode"},
-                ]
+                    {
+                        "key": "dm",
+                        "value": False,
+                        "switch": "debug_menu",
+                        "name": "Debug menu",
+                        "description": "Turn ON/OFF the menu debug mode",
+                    },
+                    {
+                        "key": "d",
+                        "value": False,
+                        "name": "Debug",
+                        "switch": "debug",
+                        "description": "Turn ON/OFF the debug mode",
+                    },
+                ],
             },
             {
-                'key':'c','name':'Configuration','description':"Configuration menu",
+                "key": "c",
+                "name": "Configuration",
+                "description": "Configuration menu",
                 "selections": [
-                    {'key':'s','function':self.save_config,'name':'Save configuration','description':"Save the current configuration"},
-                    {'key':'r','function':self.reset_config,'name':'Reset configuration','description':"Reset the current configuration"},
-                ]
+                    {
+                        "key": "s",
+                        "function": self.save_config,
+                        "name": "Save configuration",
+                        "description": "Save the current configuration",
+                    },
+                    {
+                        "key": "r",
+                        "function": self.reset_config,
+                        "name": "Reset configuration",
+                        "description": "Reset the current configuration",
+                    },
+                ],
             },
             {
-                'key':'m',
-                'name':'Memorize','description':"Memorize the last selection",
+                "key": "m",
+                "name": "Memorize",
+                "description": "Memorize the last selection",
                 "selections": [
-                    {'name':'memorize','description':'Memorize actions','set':{'memorize_action':'memorize'}},
-                    {'name':'view','description':'View memorized actions','set':{'memorize_action':'view'}},
-                    {'name':'reset','description':'Reset memorized actions action','set':{'memorize_action':'reset'}},
+                    {
+                        "name": "memorize",
+                        "description": "Memorize actions",
+                        "set": {"memorize_action": "memorize"},
+                    },
+                    {
+                        "name": "view",
+                        "description": "View memorized actions",
+                        "set": {"memorize_action": "view"},
+                    },
+                    {
+                        "name": "reset",
+                        "description": "Reset memorized actions action",
+                        "set": {"memorize_action": "reset"},
+                    },
                 ],
                 "after": {
-                    "function":{
-                        'method':self.memorize,"kwargs":{'action':'{{memorize_action}}'}
+                    "function": {
+                        "method": self.memorize,
+                        "kwargs": {"action": "{{memorize_action}}"},
                     }
-                }
+                },
+            },
+            {
+                "key": "e",
+                "function": self.execute_memorize,
+                "name": "Execute",
+                "description": "Execute the last selection",
+            },
+            {
+                "key": "v",
+                "name": "Values",
+                "function": self.show_values,
+                "description": "Show values",
+            },
+            {
+                "key": "r",
+                "name": "Reload",
+                "description": "Reload modules",
+                "function": reload_modules,
             },
-            {'key':'e',"function":self.execute_memorize,'name':'Execute','description':"Execute the last selection"},
-            {'key':'v','name':'Values','function':self.show_values,'description':'Show values'},
-            {'key':'r','name':'Reload','description':"Reload modules","function":reload_modules},
-            {'key':'b','name':'Back','description':"Go back"},
-            {'key':'q','function':self.quit,'name':'Quit','description':"Quit the menu"},
-            {'header':"SELECTIONS"},
+            {"key": "b", "name": "Back", "description": "Go back"},
+            {
+                "key": "q",
+                "function": self.quit,
+                "name": "Quit",
+                "description": "Quit the menu",
+            },
+            {"header": "SELECTIONS"},
         ]
 
         self.commands = []
         for s in selections:
-            if 'value' in s and 'name' in s and replace_name(s['name']) not in self.values:
-                self.set_value(s['name'], s['value'])
-            if 'key' in s:
-                self.commands.append(s['key'])
-            s['command'] = True
+            if (
+                "value" in s
+                and "name" in s
+                and replace_name(s["name"]) not in self.values
+            ):
+                self.set_value(s["name"], s["value"])
+            if "key" in s:
+                self.commands.append(s["key"])
+            s["command"] = True
 
         return selections
 
-    def set_value(self,name,value,convert=True):
-        name                = replace_name(name)
-        self.values[name]   = self.convert_value(value) if convert else value
-        self.debug_print('   Set value %s to %s'%(name,self.values[name]))
-        print('   Set value %s to %s'%(name,self.values[name]))
+    def set_value(self, name, value, convert=True):
+        name = replace_name(name)
+        self.values[name] = self.convert_value(value) if convert else value
+        self.debug_print("   Set value %s to %s" % (name, self.values[name]))
+        print("   Set value %s to %s" % (name, self.values[name]))
 
-    def switch_value(self,name):
+    def switch_value(self, name):
         name = replace_name(name)
         if name in self.values and type(self.values[name]) == bool:
-            self.debug_print('   Switch value %s from %s to %s'%(name,self.values[name],not self.values[name]))
+            self.debug_print(
+                "   Switch value %s from %s to %s"
+                % (name, self.values[name], not self.values[name])
+            )
             self.values[name] = not self.values[name]
 
-    def functions_evaluate(self,conf):
+    def functions_evaluate(self, conf):
         functions_config = []
-        if 'function' in conf:
-            functions_config.append(conf['function'])
-        if 'functions' in conf:
-            functions_config.extend(conf['functions'])
+        if "function" in conf:
+            functions_config.append(conf["function"])
+        if "functions" in conf:
+            functions_config.extend(conf["functions"])
 
         if len(functions_config) != 0:
             for config in functions_config:
                 args, kwargs = [], {}
                 if type(config) == dict:
-                    if 'args' in config.keys():
-                        raw_args                                    = config['args']
-                        args                                        = self.convert_list(raw_args)
-                    if  'kwargs' in config.keys():
-                        raw_kwargs                                  = config['kwargs']
-                        kwargs                                      = self.convert_dict(raw_kwargs)
-                    
-                    if 'method' in config.keys():
-                        fct                                         = config['method']
-                        fct                                         = self.convert_value(fct) if type(fct) == str else fct
+                    if "args" in config.keys():
+                        raw_args = config["args"]
+                        args = self.convert_list(raw_args)
+                    if "kwargs" in config.keys():
+                        raw_kwargs = config["kwargs"]
+                        kwargs = self.convert_dict(raw_kwargs)
+
+                    if "method" in config.keys():
+                        fct = config["method"]
+                        fct = self.convert_value(fct) if type(fct) == str else fct
                 else:
                     fct = config
 
                 if fct is not None:
-                    self.debug_print('Exec fct %s with args %s and kwargs %s'%(fct,args,kwargs))
-                    print('Exec fct %s with args %s and kwargs %s'%(fct,args,kwargs))
-                    functionReturn = fct(*args,**kwargs)
-                    print('      return: %s'%(functionReturn))
-                    self.set_value('returned',functionReturn,convert=False)
+                    self.debug_print(
+                        "Exec fct %s with args %s and kwargs %s" % (fct, args, kwargs)
+                    )
+                    print(
+                        "Exec fct %s with args %s and kwargs %s" % (fct, args, kwargs)
+                    )
+                    functionReturn = fct(*args, **kwargs)
+                    print("      return: %s" % (functionReturn))
+                    self.set_value("returned", functionReturn, convert=False)
 
-                    if type(config) == dict and 'name' in config:
-                        self.set_value(config['name'],functionReturn)
-        
-    def convert_list(self,args):
+                    if type(config) == dict and "name" in config:
+                        self.set_value(config["name"], functionReturn)
+
+    def convert_list(self, args):
         convertedArgs = []
         for value in args:
             convertedArgs.append(self.convert_value(value))
         return convertedArgs
 
-    def convert_dict(self,args):
+    def convert_dict(self, args):
         convertedArgs = {}
         for key, value in args.items():
             convertedArgs[key] = self.convert_value(value)
         return convertedArgs
 
-    def convert_value(self,rawValue,convert=None):
+    def convert_value(self, rawValue, convert=None):
         value = copy.copy(rawValue)
-        
+
         if type(rawValue) == dict:
             for key, v in rawValue.items():
                 value[self.convert_value(key)] = self.convert_value(v)
             return value
         if type(rawValue) == list:
             new_list = []
             for v in rawValue:
                 new_list.append(self.convert_value(v))
             return new_list
 
-        # List
+        # list
         elementList = False
-        regex   = "\[\d+\]"
-        m       = re.search(regex, str(rawValue))
+        regex = "\[\d+\]"
+        m = re.search(regex, str(rawValue))
         if m is not None:
-            group       = m.group(0)
-            positionRaw = group.replace('[','').replace(']','')
-            position    = self.convert_value(positionRaw,convert=int)
-            rawValue    = rawValue.replace(group,'')
+            group = m.group(0)
+            positionRaw = group.replace("[", "").replace("]", "")
+            position = self.convert_value(positionRaw, convert=int)
+            rawValue = rawValue.replace(group, "")
             elementList = True
 
         # Range
-        regex   = "\[[\d*]:[\d*]\]"
-        m       = re.search(regex, str(rawValue))
+        regex = "\[[\d*]:[\d*]\]"
+        m = re.search(regex, str(rawValue))
         if m is not None:
-            values  = m.group(0).replace('[','').replace(']','').split(':')
-            v1      = self.convert_value(values[0],convert=int)
-            v2      = self.convert_value(values[1],convert=int)
-            value   = range(v1,v2)
+            values = m.group(0).replace("[", "").replace("]", "").split(":")
+            v1 = self.convert_value(values[0], convert=int)
+            v2 = self.convert_value(values[1], convert=int)
+            value = range(v1, v2)
             return value
-        
+
         # Call dynamically a method from this class
-        if "self." in str(rawValue) and rawValue.replace('self','') in dir(self):
+        if "self." in str(rawValue) and rawValue.replace("self", "") in dir(self):
             value = getattr(self, rawValue)
-        
+
         value = self.convert_parameters(value)
 
-        #if elementList:
+        # if elementList:
         #    print("%s > %s %s"%(rawValue,value,self.values.keys()))
 
         if elementList:
             value = value[position]
-                
+
         if convert == int:
             convertion, ok = to_int(value)
             if ok:
                 value = convertion
 
         return value
 
-    def convert_parameters(self,value):
+    def convert_parameters(self, value):
         if type(value) != str:
             return value
 
         for key, val in self.values.items():
-            if '{{%s}}'%key == str(value):
+            if "{{%s}}" % key == str(value):
                 return val
-            if '{{%s}}'%key in str(value):
-                value = value.replace('{{%s}}'%key,str(val))
+            if "{{%s}}" % key in str(value):
+                value = value.replace("{{%s}}" % key, str(val))
         return value
 
     def quit(self):
-        print('   QUIT')
+        print("   QUIT")
         self.exit = True
-            
-    def get_value(self,name):
+
+    def get_value(self, name):
         name = replace_name(name)
         if not name in self.values.keys():
             return None
         return self.convert_value(self.values[name])
-    
-    def is_parameter(self,conf,name):
+
+    def is_parameter(self, conf, name):
         for key, value in conf.items():
             if replace_name(key) == name:
                 return self.convert_value(value)
         return replace_name(name) in conf.keys()
 
-    def get_parameter_value(self,conf,name):
+    def get_parameter_value(self, conf, name):
         name = replace_name(name)
-        if self.is_parameter(conf,name):
+        if self.is_parameter(conf, name):
             for key, value in conf.items():
                 if replace_name(key) == name:
                     return self.convert_value(value)
         return None
-            
-    def get_string(self,conf,name):
+
+    def get_string(self, conf, name):
         key = replace_name(name)
         if key in conf.keys():
             return self.format_string(conf[name])
-        return ''
+        return ""
 
-    def format_string(self,conf):
+    def format_string(self, conf):
         if type(conf) == str:
             return conf
-        args = self.convert_dict(conf['values']).values()
-        return conf['str'].format(*args)
-                
+        args = self.convert_dict(conf["values"]).values()
+        return conf["str"].format(*args)
+
     def save_config(self):
         filename = self.save_directory + os.sep + self.name
-        io_lib.archive_object(self.values,filename)
+        io_lib.archive_object(self.values, filename)
 
     def reset_config(self):
         self.values = {}
         self.save_config()
 
-    def memorize(self,action=None):
-        if action == 'view':
+    def memorize(self, action=None):
+        if action == "view":
             for selection in self.selected_history:
                 print(selection)
         elif action == "memorize":
-            self.values['memorized_selection'] = self.selected_history
+            self.values["memorized_selection"] = self.selected_history
             self.save_config()
-        elif action == 'reset':
+        elif action == "reset":
             self.selected_history = []
 
     def execute_memorize(self):
-        self.sequence = [x['key'] for x in self.selected_history]
+        self.sequence = [x["key"] for x in self.selected_history]
 
     def load_default_values(self):
-        defaults            = {}
-        filename            = self.save_directory + os.sep + self.name
+        defaults = {}
+        filename = self.save_directory + os.sep + self.name
 
-        values              = None
+        values = None
         try:
-            values          = io_lib.unarchive_object(filename)
+            values = io_lib.unarchive_object(filename)
         except:
-            print('ERROR with configuration file')
+            print("ERROR with configuration file")
 
         if values is not None:
-            defaults        = values
+            defaults = values
         else:
             self.log.error("No default values are specified")
 
-        self.values         = defaults
-        self.defaultskeys   = list(defaults.keys())
+        self.values = defaults
+        self.defaultskeys = list(defaults.keys())
+
+        if "memorized_selection" in self.values:
+            self.selected_history = self.values["memorized_selection"]
 
-        if 'memorized_selection' in self.values:
-            self.selected_history = self.values['memorized_selection']
-        
     def show_values(self):
         for key, value in self.values.items():
             print(f"Menu values: {key}: {value}")
 
-    def printEvaluate(self,conf):
+    def printEvaluate(self, conf):
         pass
         """
         key                                             = 'print'
 
         parameters                                      = conf.keys()
         ### PRINT
         if key in parameters:
@@ -550,15 +660,15 @@
             print("\nOUTPUT: " + output + "\n")
             
         key                                             = 'infos'
         if key in parameters:
             output                                      = self.format_string(conf[key])
             print(output + "\n")
         """
-                            
+
     """def get_config_from_values(self,valuesConfig,values,multiple=False,key_mode=False):
         parameters = valuesConfig.keys()
         
         choices = {}
         i = 0
         if not type(values) == dict:
             for value in values:
@@ -577,8 +687,8 @@
             if key_mode:
                 subConfig['set_key']    = True 
             if multiple:
                 subConfig['mode']       = 'activate'
 
             conf[value] = subConfig
             self.debug_print("sub configuration %s"%subConfig.keys())
-        return conf"""
+        return conf"""
```

### Comparing `alphaz-0.7.6.2/alphaz/utils/tasks.py` & `alphaz-0.7.6.3/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/tests.py` & `alphaz-0.7.6.3/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/time.py` & `alphaz-0.7.6.3/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/alphaz/utils/transactions.py` & `alphaz-0.7.6.3/alphaz/utils/transactions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,131 @@
 from threading import Thread, Event
 import os, datetime, uuid, time, math, ast
-from typing import List, Dict
 
 from alphaz.models.database.structure import AlphaDatabase
 from alphaz.models.main import AlphaClass, AlphaTransaction
 
 from ..libs import transactions_lib
 
 from core import core
 
-LOG = core.get_logger('requests')
+LOG = core.get_logger("requests")
 DB = core.db
 
-class TransactionsThread(Thread):    # PowerCounter class
-    def __init__(self, function, 
-            message_types:List[str] = [], 
-            database: AlphaDatabase = DB, 
-            interval: int = 2,
-            timeout: int = 0, 
-            pool_size:int = 20, 
-            answer_lifetime = 3600,
-            args = [], 
-            kwargs = {}
-        ):
 
+class TransactionsThread(Thread):  # PowerCounter class
+    def __init__(
+        self,
+        function,
+        message_types: list[str] = [],
+        database: AlphaDatabase = DB,
+        interval: int = 2,
+        timeout: int = 0,
+        pool_size: int = 20,
+        answer_lifetime: int = 3600,
+        args: list | None = None,
+        kwargs: dict | None = None,
+    ):
         Thread.__init__(self)
 
         self.function = function
-        self.message_types:List[str]  = message_types
+        self.message_types: list[str] = message_types
         self.database: AlphaDatabase = database
-        self.interval:str = interval
+        self.interval = interval
         self.timeout = timeout
-        self.pool_size:int = pool_size
-        self.answer_lifetime: int = answer_lifetime
-        self.args:list = args
-        self.kwargs:dict = kwargs
+        self.pool_size = pool_size
+        self.answer_lifetime = answer_lifetime
+        self.args = args if args is not None else []
+        self.kwargs = kwargs if kwargs is not None else []
 
         self.started: Event = Event()
-        self.running: Event= Event()
-        self.finished: Event = Event()        
+        self.running: Event = Event()
+        self.finished: Event = Event()
 
     def ensure(self):
         if not self.started.is_set() and not self.running.is_set():
             self.start()
 
     def run(self):
         self.started.set()
 
         count = 0
         offset = 0
         elapsed = 0
         dts = datetime.datetime.now()
-        while not self.finished.is_set() and (self.timeout <= 0 or elapsed < self.timeout):
+        while not self.finished.is_set() and (
+            self.timeout <= 0 or elapsed < self.timeout
+        ):
             dt = datetime.datetime.now()
-            
+
             if not self.running.is_set():
                 self.running.set()
 
             if count == 0:
-                #secs = (math.ceil(dt) - dt).total_seconds()
+                # secs = (math.ceil(dt) - dt).total_seconds()
                 secs = 0
             else:
                 secs = self.interval - offset
-                
+
             self.finished.wait(secs)
             if not self.finished.is_set():
                 t = time.time()
 
                 self.process()
 
                 offset = time.time() - t
                 count += 1
-            
+
             elapsed = (dt - dts).total_seconds()
 
         if self.timeout > 0 and elapsed > self.timeout:
             LOG.info("Thread reachs its limit")
         else:
             LOG.info("Thread ended")
 
     def process(self):
-        requests = transactions_lib.get_requests(self.database, message_types=self.message_types, limit=self.pool_size)
+        requests = transactions_lib.get_requests(
+            self.database, message_types=self.message_types, limit=self.pool_size
+        )
 
         if len(requests) == 0:
             return
 
         requests = [AlphaTransaction(x) for x in requests]
 
-        LOG.info(f'Processing {len(requests)} requests ...')
+        LOG.info(f"Processing {len(requests)} requests ...")
 
-        uuids   = []
+        uuids = []
         for request in requests:
-            answer = ''
+            answer = ""
             try:
                 uuid = request.uuid
                 parameters = request.message
                 uuids.append(uuid)
-                LOG.debug('REQUEST: \n\n'+str(parameters)+'\n')
+                LOG.debug("REQUEST: \n\n" + str(parameters) + "\n")
 
                 if type(parameters) is not dict:
-                    LOG.error('Answer is of the wrong type')
+                    LOG.error("Answer is of the wrong type")
                     continue
 
                 answer = self.function(request, *self.args, **self.kwargs)
-                        
+
                 if answer is not None:
-                    answer            = str(answer)
-                    LOG.debug('Sending answer: '+answer)
+                    answer = str(answer)
+                    LOG.debug("Sending answer: " + answer)
             except Exception as ex:
-                LOG.error("Cannot send answser",ex=ex)
+                LOG.error("Cannot send answser", ex=ex)
             finally:
-                transactions_lib.send_answer(self.database, uuid, answer, 
-                    message_type=str(request.message_type), answer_lifetime=self.answer_lifetime)
+                transactions_lib.send_answer(
+                    self.database,
+                    uuid,
+                    answer,
+                    message_type=str(request.message_type),
+                    answer_lifetime=self.answer_lifetime,
+                )
 
         transactions_lib.delete_requests(self.database, uuids)
 
     def cancel(self):
         self.finished.set()
         self.started.clear()
-        self.running.clear()
+        self.running.clear()
```

### Comparing `alphaz-0.7.6.2/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.6.3/alphaz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.6.2
+Version: 0.7.6.3
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.6.2.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.6.3.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.6.2/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.6.3/alphaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.6.2/setup.py` & `alphaz-0.7.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.6.2"
+version = "0.7.6.3"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
```

