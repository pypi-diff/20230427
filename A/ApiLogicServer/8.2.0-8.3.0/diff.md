# Comparing `tmp/ApiLogicServer-8.2.0.tar.gz` & `tmp/ApiLogicServer-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApiLogicServer-8.2.0.tar", last modified: Fri Apr 14 03:21:29 2023, max compression
+gzip compressed data, was "ApiLogicServer-8.3.0.tar", last modified: Thu Apr 27 02:31:19 2023, max compression
```

## Comparing `ApiLogicServer-8.2.0.tar` & `ApiLogicServer-8.3.0.tar`

### file list

```diff
@@ -1,757 +1,762 @@
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.860473 ApiLogicServer-8.2.0/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.659819 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/
--rw-r--r--   0 val        (502) staff       (20)    15205 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    53439 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/SOURCES.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/dependency_links.txt
--rw-r--r--   0 val        (502) staff       (20)       66 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/entry_points.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/not-zip-safe
--rw-r--r--   0 val        (502) staff       (20)      583 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/requires.txt
--rw-r--r--   0 val        (502) staff       (20)       21 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/ApiLogicServer.egg-info/top_level.txt
--rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/LICENSE
--rw-r--r--   0 val        (502) staff       (20)      679 2023-01-26 02:30:48.000000 ApiLogicServer-8.2.0/MANIFEST.in
--rw-r--r--   0 val        (502) staff       (20)    15205 2023-04-14 03:21:29.860255 ApiLogicServer-8.2.0/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    14216 2023-04-14 01:21:42.000000 ApiLogicServer-8.2.0/README.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.663331 ApiLogicServer-8.2.0/api_logic_server_cli/
--rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.2.0/api_logic_server_cli/Todo_models.py.py
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    58487 2023-04-14 01:20:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/api_logic_server.py
--rw-r--r--   0 val        (502) staff       (20)      153 2023-04-14 01:23:53.000000 ApiLogicServer-8.2.0/api_logic_server_cli/api_logic_server_info.yaml
--rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.2.0/api_logic_server_cli/cli.py
--rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.2.0/api_logic_server_cli/cli_args_base.py
--rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.2.0/api_logic_server_cli/cli_args_project.py
--rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.666784 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.673303 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5300 2023-02-26 23:03:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    13492 2023-03-16 03:50:38.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     5290 2023-02-05 02:48:17.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
--rw-r--r--   0 val        (502) staff       (20)    11423 2023-03-16 03:50:23.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py
--rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/model_creation_services.py
--rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.675893 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
--rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.676101 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
--rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
--rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
--rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
--rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
--rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
--rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
--rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.651943 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.679082 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
--rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
--rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
--rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
--rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.750210 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
--rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
--rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.754345 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
--rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.760320 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.760957 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/
--rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
--rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.761512 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
--rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
--rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.761688 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
--rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.652258 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.652296 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.762008 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.762315 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
--rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
--rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
--rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
--rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
--rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/create_admin.sh
--rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/fab_config.py
--rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/home.js
--rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js
--rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/ui_admin_creator.py
--rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/uri_info.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.773689 ApiLogicServer-8.2.0/api_logic_server_cli/database/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/authentication.sqlite
--rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/classicmodels.sqlite
--rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/new.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/nw-gold-plus.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/nw.sqlite
--rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/table_filters_tests.sqlite
--rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/table_filters_tests.yml
--rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/table_filters_tests_nw.yml
--rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/table_filters_tests_nw_1.yml
--rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/table_filters_tests_typical.yml
--rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.2.0/api_logic_server_cli/database/todos.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.791767 ApiLogicServer-8.2.0/api_logic_server_cli/docs/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1251 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/API-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     2647 2022-12-29 01:51:24.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/API.md
--rw-r--r--   0 val        (502) staff       (20)     3222 2022-12-21 16:33:05.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Admin-Customization.md
--rw-r--r--   0 val        (502) staff       (20)    18275 2023-03-10 04:52:51.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Admin-Tour.md
--rw-r--r--   0 val        (502) staff       (20)      384 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Architecture-What-Is.md
--rw-r--r--   0 val        (502) staff       (20)    12713 2022-11-22 02:48:15.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Architecture.md
--rw-r--r--   0 val        (502) staff       (20)    61944 2022-10-11 03:42:54.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Behave-Logic-Report.md
--rw-r--r--   0 val        (502) staff       (20)     3838 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Behave.md
--rw-r--r--   0 val        (502) staff       (20)     1994 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Create-ApiLogicProject.md
--rw-r--r--   0 val        (502) staff       (20)     5319 2022-12-21 20:29:28.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Classes.md
--rw-r--r--   0 val        (502) staff       (20)     2660 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Customization.md
--rw-r--r--   0 val        (502) staff       (20)     1114 2023-01-27 04:14:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Examples.md
--rw-r--r--   0 val        (502) staff       (20)      970 2022-10-03 02:15:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Keys.md
--rw-r--r--   0 val        (502) staff       (20)     3898 2023-01-06 02:59:38.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Multi.md
--rw-r--r--   0 val        (502) staff       (20)    13193 2023-03-12 01:14:31.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Database-Connectivity.md
--rw-r--r--   0 val        (502) staff       (20)     1241 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Execute.md
--rw-r--r--   0 val        (502) staff       (20)     3273 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/FAQ-Frameworks.md
--rw-r--r--   0 val        (502) staff       (20)      527 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/FAQ-Low-Code.md
--rw-r--r--   0 val        (502) staff       (20)     7036 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/FAQ-RETE.md
--rw-r--r--   0 val        (502) staff       (20)     1851 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/IDE-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     7532 2023-01-20 15:50:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/IDE-Execute.md
--rw-r--r--   0 val        (502) staff       (20)     6368 2023-02-04 01:50:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Eval-x.md
--rw-r--r--   0 val        (502) staff       (20)     8093 2023-01-09 21:17:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Eval.md
--rw-r--r--   0 val        (502) staff       (20)     3390 2023-02-03 23:28:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Express-x.md
--rw-r--r--   0 val        (502) staff       (20)     3539 2022-08-23 15:56:25.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Express.md
--rw-r--r--   0 val        (502) staff       (20)      566 2022-11-30 17:57:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-psycopg2.md
--rw-r--r--   0 val        (502) staff       (20)      977 2022-11-17 04:40:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-pyodbc.md
--rw-r--r--   0 val        (502) staff       (20)     7135 2022-09-18 04:42:29.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install.md
--rw-r--r--   0 val        (502) staff       (20)    13448 2023-02-05 02:54:14.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Internals-CLI.md
--rw-r--r--   0 val        (502) staff       (20)     6504 2022-12-01 16:51:37.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Internals.md
--rw-r--r--   0 val        (502) staff       (20)     3258 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic-Operation.md
--rw-r--r--   0 val        (502) staff       (20)    14729 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)    10325 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic-Why.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic.md
--rw-r--r--   0 val        (502) staff       (20)     4205 2022-08-28 15:23:33.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Manage-GitHub.md
--rw-r--r--   0 val        (502) staff       (20)     3796 2022-12-28 03:43:06.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Builders.md
--rw-r--r--   0 val        (502) staff       (20)     1957 2022-12-22 04:40:03.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-DevOps.md
--rw-r--r--   0 val        (502) staff       (20)     1930 2023-01-31 22:36:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Env.md
--rw-r--r--   0 val        (502) staff       (20)     4936 2022-11-24 20:38:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Execution.md
--rw-r--r--   0 val        (502) staff       (20)     2446 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Rebuild.md
--rw-r--r--   0 val        (502) staff       (20)     2104 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Structure.md
--rw-r--r--   0 val        (502) staff       (20)      773 2022-09-18 04:42:29.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Sample-Database.md
--rw-r--r--   0 val        (502) staff       (20)     2227 2023-02-14 23:54:00.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Activation.md
--rw-------   0 val        (502) staff       (20)     1585 2023-01-21 01:47:08.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Authentication-Provider.md
--rw-------   0 val        (502) staff       (20)     1470 2023-01-21 02:17:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Authentication.md
--rw-r--r--   0 val        (502) staff       (20)     1922 2023-01-06 17:06:26.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Authorization.md
--rw-r--r--   0 val        (502) staff       (20)     5277 2023-01-21 01:31:32.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Overview.md
--rw-r--r--   0 val        (502) staff       (20)      155 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech--Notes.md
--rw-r--r--   0 val        (502) staff       (20)      237 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-4GL.md
--rw-r--r--   0 val        (502) staff       (20)     7081 2022-11-24 00:40:19.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-CodeSpaces.md
--rw-r--r--   0 val        (502) staff       (20)     3053 2022-12-06 21:43:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
--rw-r--r--   0 val        (502) staff       (20)     3174 2022-12-06 18:38:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     5693 2022-12-05 19:50:10.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Conference.md
--rw-r--r--   0 val        (502) staff       (20)     3385 2022-11-07 18:45:42.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Docker.md
--rw-r--r--   0 val        (502) staff       (20)      815 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Install-Python.md
--rw-r--r--   0 val        (502) staff       (20)     1049 2022-10-03 16:52:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Proven.md
--rw-r--r--   0 val        (502) staff       (20)     2679 2022-12-07 04:30:27.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Python-311.md
--rw-r--r--   0 val        (502) staff       (20)     3728 2023-01-12 06:40:15.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Python.md
--rw-r--r--   0 val        (502) staff       (20)     3019 2022-10-21 23:29:01.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-m1.md
--rw-r--r--   0 val        (502) staff       (20)     1644 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-mkdocs-material.md
--rw-r--r--   0 val        (502) staff       (20)    12291 2022-10-08 18:23:10.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Troubleshooting.md
--rw-r--r--   0 val        (502) staff       (20)    15277 2023-04-14 03:21:29.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     6697 2022-12-02 18:42:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Working-With-Docker.md
--rw-r--r--   0 val        (502) staff       (20)     4031 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.792079 ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-08-30 03:14:41.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.792581 ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/images/
--rw-r--r--   0 val        (502) staff       (20)     2362 2022-08-29 00:06:15.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/images/bulb-icon.svg
--rw-r--r--   0 val        (502) staff       (20)     3482 2022-08-30 03:46:01.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/images/lightbulb.svg
--rw-r--r--   0 val        (502) staff       (20)    15440 2023-02-06 03:49:29.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/index.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.792908 ApiLogicServer-8.2.0/api_logic_server_cli/docs/stylesheets/
--rw-r--r--   0 val        (502) staff       (20)      634 2022-08-30 03:44:15.000000 ApiLogicServer-8.2.0/api_logic_server_cli/docs/stylesheets/extra.css
--rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.2.0/api_logic_server_cli/extended_builder.py
--rw-r--r--   0 val        (502) staff       (20)     1014 2023-03-08 16:58:33.000000 ApiLogicServer-8.2.0/api_logic_server_cli/logging.yml
--rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/models.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.796832 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-02-14 05:32:37.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.797788 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.798227 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.800024 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1116 2022-04-03 03:00:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml
--rw-r--r--   0 val        (502) staff       (20)     2433 2022-04-03 03:00:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.800752 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.801767 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     1984 2023-02-05 02:50:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api/customize_api.py
--rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api/expose_api_models.py
--rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api/json_encoder.py
--rw-r--r--   0 val        (502) staff       (20)    18245 2023-04-13 16:36:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api_logic_server_run.py
--rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.802757 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.803494 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/
--rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/env.py
--rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/readme.md
--rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.803673 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/versions/
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
--rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic.ini
--rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/bind_databases.py
--rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/default.env
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.803951 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.805233 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/
--rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
--rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
--rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
--rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
--rw-r--r--   0 val        (502) staff       (20)     1483 2023-04-13 02:03:37.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.805507 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/logic/
--rw-r--r--   0 val        (502) staff       (20)      870 2023-01-23 01:01:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/mypy.ini
--rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
--rw-r--r--   0 val        (502) staff       (20)     7111 2023-02-06 23:07:59.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/run.ps1
--rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/run.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.806150 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.807017 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.809771 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.810353 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.810591 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.653812 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.811493 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.811788 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
--rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.812497 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/notes_temp/
--rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
--rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
--rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.813548 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.813851 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/authentication.py
--rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/authorization.py
--rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.814136 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/templates/
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/templates/index.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.814311 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.814806 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
--rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.814960 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.815319 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.815959 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
--rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
--rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.816715 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/basic/
--rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/basic/server_test.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.817242 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.817611 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
--rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/admin/home.js
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.817872 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.819573 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.820799 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.820938 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/templates/
--rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/templates/content.html
--rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/util.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.822663 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/
--rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/py.py
--rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
--rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
--rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
--rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
--rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.823402 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 18:56:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.823752 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/api/
--rw-r--r--   0 val        (502) staff       (20)     8711 2023-02-13 15:35:11.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.824763 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/database/
--rw-r--r--   0 val        (502) staff       (20)     1752 2023-03-11 01:10:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/database/db_debug.py
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.825044 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/logic/
--rw-r--r--   0 val        (502) staff       (20)    10506 2023-03-10 18:58:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)      305 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.825318 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/security/
--rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.825628 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.825719 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.826281 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
--rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
--rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
--rw-r--r--   0 val        (502) staff       (20)      321 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.827201 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
--rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
--rw-r--r--   0 val        (502) staff       (20)     3989 2023-01-14 03:30:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.827449 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
--rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.828942 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
--rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
--rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
--rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.829840 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.831756 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
--rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
--rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
--rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
--rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
--rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
--rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
--rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.831925 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/
--rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.832967 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)    16965 2023-03-11 01:27:45.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
--rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.833255 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.834885 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.836245 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.836391 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw_no_cust/
--rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.837993 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.839725 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.839981 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.842447 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
--rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
--rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
--rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
--rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
--rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.842905 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     5986 2023-04-13 16:51:25.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.844436 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.845420 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.845560 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
--rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
--rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.847015 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.847275 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
--rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
--rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
--rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
--rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
--rw-r--r--   0 val        (502) staff       (20)    21134 2023-04-14 00:57:12.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/sample_db.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.848772 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
--rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.850974 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    21696 2023-03-12 04:54:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
--rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.852632 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
--rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
--rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.853091 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
--rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.854104 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.856008 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
--rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.857013 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
--rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
--rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
--rwxr-xr-x   0 val        (502) staff       (20)    17212 2023-03-12 01:12:46.000000 ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-14 03:21:29.859712 ApiLogicServer-8.2.0/api_logic_server_cli/templates/
--rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.2.0/api_logic_server_cli/templates/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.2.0/api_logic_server_cli/templates/app_fiddle.md
--rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.2.0/api_logic_server_cli/templates/app_fiddle.txt
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/templates/index.html
--rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/templates/login_endpoint.txt
--rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.2.0/api_logic_server_cli/templates/login_endpoint_imports.txt
--rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.2.0/api_logic_server_cli/ui_basic_web_app_run.py
--rw-r--r--   0 val        (502) staff       (20)       38 2023-04-14 03:21:29.860526 ApiLogicServer-8.2.0/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)     3519 2023-03-04 19:39:20.000000 ApiLogicServer-8.2.0/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.975350 ApiLogicServer-8.3.0/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.780486 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/
+-rw-r--r--   0 val        (502) staff       (20)    15305 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    53720 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (502) staff       (20)       66 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/entry_points.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/not-zip-safe
+-rw-r--r--   0 val        (502) staff       (20)      585 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/requires.txt
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/top_level.txt
+-rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/LICENSE
+-rw-r--r--   0 val        (502) staff       (20)      732 2023-04-23 23:14:50.000000 ApiLogicServer-8.3.0/MANIFEST.in
+-rw-r--r--   0 val        (502) staff       (20)    15305 2023-04-27 02:31:19.975074 ApiLogicServer-8.3.0/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    14316 2023-04-27 02:26:34.000000 ApiLogicServer-8.3.0/README.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.782317 ApiLogicServer-8.3.0/api_logic_server_cli/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    59835 2023-04-27 02:26:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/api_logic_server.py
+-rw-r--r--   0 val        (502) staff       (20)      120 2023-04-27 00:54:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/api_logic_server_info.yaml
+-rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/cli.py
+-rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_base.py
+-rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_project.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.785729 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.790357 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5300 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    13492 2023-03-16 03:50:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5290 2023-02-05 02:48:17.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
+-rw-r--r--   0 val        (502) staff       (20)    11423 2023-03-16 03:50:23.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py
+-rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/model_creation_services.py
+-rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.792257 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
+-rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.792420 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
+-rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
+-rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
+-rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
+-rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
+-rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
+-rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
+-rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.773537 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.794801 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
+-rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
+-rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
+-rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
+-rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.856172 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
+-rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
+-rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.860277 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
+-rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.866214 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.866774 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/
+-rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
+-rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.867252 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
+-rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.867395 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
+-rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.773843 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.773891 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.867702 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.868091 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
+-rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
+-rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
+-rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
+-rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
+-rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/create_admin.sh
+-rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/fab_config.py
+-rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/home.js
+-rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js
+-rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/ui_admin_creator.py
+-rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/uri_info.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.882951 ApiLogicServer-8.3.0/api_logic_server_cli/database/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/authentication.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/classicmodels.sqlite
+-rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/new.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold-plus.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/nw.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests.yml
+-rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests_nw.yml
+-rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests_nw_1.yml
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests_typical.yml
+-rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/todos.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.903399 ApiLogicServer-8.3.0/api_logic_server_cli/docs/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1251 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/API-Customize.md
+-rw-r--r--   0 val        (502) staff       (20)     2647 2022-12-29 01:51:24.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/API.md
+-rw-r--r--   0 val        (502) staff       (20)     3222 2022-12-21 16:33:05.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Customization.md
+-rw-r--r--   0 val        (502) staff       (20)    18275 2023-03-10 04:52:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Tour.md
+-rw-r--r--   0 val        (502) staff       (20)      384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Architecture-What-Is.md
+-rw-r--r--   0 val        (502) staff       (20)    12713 2022-11-22 02:48:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Architecture.md
+-rw-r--r--   0 val        (502) staff       (20)    61944 2022-10-11 03:42:54.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave-Logic-Report.md
+-rw-r--r--   0 val        (502) staff       (20)     3838 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave.md
+-rw-r--r--   0 val        (502) staff       (20)     1994 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Create-ApiLogicProject.md
+-rw-r--r--   0 val        (502) staff       (20)     5319 2022-12-21 20:29:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Classes.md
+-rw-r--r--   0 val        (502) staff       (20)     2660 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Customization.md
+-rw-r--r--   0 val        (502) staff       (20)     1114 2023-01-27 04:14:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Examples.md
+-rw-r--r--   0 val        (502) staff       (20)      970 2022-10-03 02:15:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Keys.md
+-rw-r--r--   0 val        (502) staff       (20)     3898 2023-01-06 02:59:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Multi.md
+-rw-r--r--   0 val        (502) staff       (20)    13193 2023-03-12 01:14:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Database-Connectivity.md
+-rw-r--r--   0 val        (502) staff       (20)     1241 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Execute.md
+-rw-r--r--   0 val        (502) staff       (20)     3273 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Frameworks.md
+-rw-r--r--   0 val        (502) staff       (20)      527 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Low-Code.md
+-rw-r--r--   0 val        (502) staff       (20)     7036 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-RETE.md
+-rw-r--r--   0 val        (502) staff       (20)     1851 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Customize.md
+-rw-r--r--   0 val        (502) staff       (20)     7532 2023-01-20 15:50:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Execute.md
+-rw-r--r--   0 val        (502) staff       (20)     6368 2023-02-04 01:50:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval-x.md
+-rw-r--r--   0 val        (502) staff       (20)     8093 2023-01-09 21:17:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval.md
+-rw-r--r--   0 val        (502) staff       (20)     3390 2023-02-03 23:28:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express-x.md
+-rw-r--r--   0 val        (502) staff       (20)     3539 2022-08-23 15:56:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express.md
+-rw-r--r--   0 val        (502) staff       (20)      566 2022-11-30 17:57:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-psycopg2.md
+-rw-r--r--   0 val        (502) staff       (20)      977 2022-11-17 04:40:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-pyodbc.md
+-rw-r--r--   0 val        (502) staff       (20)     7135 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install.md
+-rw-r--r--   0 val        (502) staff       (20)    13448 2023-02-05 02:54:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals-CLI.md
+-rw-r--r--   0 val        (502) staff       (20)     6504 2022-12-01 16:51:37.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals.md
+-rw-r--r--   0 val        (502) staff       (20)     3258 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Operation.md
+-rw-r--r--   0 val        (502) staff       (20)    14729 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)    10325 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Why.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic.md
+-rw-r--r--   0 val        (502) staff       (20)     4205 2022-08-28 15:23:33.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Manage-GitHub.md
+-rw-r--r--   0 val        (502) staff       (20)     3796 2022-12-28 03:43:06.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Builders.md
+-rw-r--r--   0 val        (502) staff       (20)     1957 2022-12-22 04:40:03.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-DevOps.md
+-rw-r--r--   0 val        (502) staff       (20)     1930 2023-01-31 22:36:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Env.md
+-rw-r--r--   0 val        (502) staff       (20)     4936 2022-11-24 20:38:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Execution.md
+-rw-r--r--   0 val        (502) staff       (20)     2446 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Rebuild.md
+-rw-r--r--   0 val        (502) staff       (20)     2104 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Structure.md
+-rw-r--r--   0 val        (502) staff       (20)      773 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Sample-Database.md
+-rw-r--r--   0 val        (502) staff       (20)     2227 2023-02-14 23:54:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Activation.md
+-rw-------   0 val        (502) staff       (20)     1585 2023-01-21 01:47:08.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication-Provider.md
+-rw-------   0 val        (502) staff       (20)     1470 2023-01-21 02:17:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication.md
+-rw-r--r--   0 val        (502) staff       (20)     1922 2023-01-06 17:06:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authorization.md
+-rw-r--r--   0 val        (502) staff       (20)     5277 2023-01-21 01:31:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Overview.md
+-rw-r--r--   0 val        (502) staff       (20)      155 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech--Notes.md
+-rw-r--r--   0 val        (502) staff       (20)      237 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-4GL.md
+-rw-r--r--   0 val        (502) staff       (20)     7081 2022-11-24 00:40:19.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-CodeSpaces.md
+-rw-r--r--   0 val        (502) staff       (20)     3053 2022-12-06 21:43:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
+-rw-r--r--   0 val        (502) staff       (20)     3174 2022-12-06 18:38:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)     5693 2022-12-05 19:50:10.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference.md
+-rw-r--r--   0 val        (502) staff       (20)     3385 2022-11-07 18:45:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Docker.md
+-rw-r--r--   0 val        (502) staff       (20)      815 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Install-Python.md
+-rw-r--r--   0 val        (502) staff       (20)     1049 2022-10-03 16:52:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Proven.md
+-rw-r--r--   0 val        (502) staff       (20)     2679 2022-12-07 04:30:27.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python-311.md
+-rw-r--r--   0 val        (502) staff       (20)     3728 2023-01-12 06:40:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python.md
+-rw-r--r--   0 val        (502) staff       (20)     3019 2022-10-21 23:29:01.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-m1.md
+-rw-r--r--   0 val        (502) staff       (20)     1644 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-mkdocs-material.md
+-rw-r--r--   0 val        (502) staff       (20)    12291 2022-10-08 18:23:10.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Troubleshooting.md
+-rw-r--r--   0 val        (502) staff       (20)    15277 2023-04-27 02:31:04.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)     6697 2022-12-02 18:42:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-With-Docker.md
+-rw-r--r--   0 val        (502) staff       (20)     4031 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.903819 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-08-30 03:14:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.904412 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/
+-rw-r--r--   0 val        (502) staff       (20)     2362 2022-08-29 00:06:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/bulb-icon.svg
+-rw-r--r--   0 val        (502) staff       (20)     3482 2022-08-30 03:46:01.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/lightbulb.svg
+-rw-r--r--   0 val        (502) staff       (20)    15440 2023-02-06 03:49:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/index.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.904763 ApiLogicServer-8.3.0/api_logic_server_cli/docs/stylesheets/
+-rw-r--r--   0 val        (502) staff       (20)      634 2022-08-30 03:44:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/stylesheets/extra.css
+-rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/extended_builder.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.906796 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/
+-rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
+-rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/configZZ.py
+-rw-r--r--   0 val        (502) staff       (20)       63 2022-10-01 16:17:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/db_typesZZ.txt
+-rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/modelsZZ.py
+-rw-r--r--   0 val        (502) staff       (20)      888 2023-04-23 22:57:22.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/nw_virtual_attrs.py
+-rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
+-rw-r--r--   0 val        (502) staff       (20)     1006 2023-04-21 23:18:04.000000 ApiLogicServer-8.3.0/api_logic_server_cli/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.911444 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-04-26 02:43:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.912474 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.912741 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.914735 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1116 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml
+-rw-r--r--   0 val        (502) staff       (20)     2433 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.915174 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.916445 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     2053 2023-04-26 02:48:17.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/customize_api.py
+-rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/expose_api_models.py
+-rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/json_encoder.py
+-rw-r--r--   0 val        (502) staff       (20)     2527 2023-04-26 02:40:27.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/readme_customize_api.md
+-rw-r--r--   0 val        (502) staff       (20)    18289 2023-04-22 14:56:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api_logic_server_run.py
+-rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.917436 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.918970 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/
+-rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/env.py
+-rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/readme.md
+-rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.919361 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/versions/
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic.ini
+-rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/bind_databases.py
+-rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/default.env
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.919722 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.921036 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/
+-rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
+-rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
+-rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
+-rw-r--r--   0 val        (502) staff       (20)     1475 2023-04-21 23:01:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.922139 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/
+-rw-r--r--   0 val        (502) staff       (20)      592 2023-04-26 02:47:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)     5953 2023-04-27 00:49:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
+-rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/mypy.ini
+-rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
+-rw-r--r--   0 val        (502) staff       (20)     6894 2023-04-27 00:54:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.ps1
+-rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.922829 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.923535 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.925711 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.926325 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.926631 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.775495 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.927682 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.927945 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
+-rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.928739 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/
+-rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
+-rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
+-rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.929581 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.929855 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authentication.py
+-rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authorization.py
+-rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.930378 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/templates/
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/templates/index.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.930634 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.931218 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
+-rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.931396 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.931760 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.932472 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
+-rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
+-rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.933277 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/basic/server_test.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.933874 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.934310 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
+-rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/home.js
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.934619 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.936701 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.938129 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.938284 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/templates/
+-rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/templates/content.html
+-rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/util.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.939792 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/
+-rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/py.py
+-rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
+-rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
+-rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
+-rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.940341 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.940575 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/api/
+-rw-r--r--   0 val        (502) staff       (20)     8711 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.941426 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/
+-rw-r--r--   0 val        (502) staff       (20)     2662 2023-04-24 23:31:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/db_debug.py
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.941687 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/logic/
+-rw-r--r--   0 val        (502) staff       (20)    10650 2023-04-23 00:10:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)      305 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.941991 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/security/
+-rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.942239 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.942342 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.943075 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
+-rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
+-rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
+-rw-r--r--   0 val        (502) staff       (20)      473 2023-04-23 23:42:07.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.944594 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
+-rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
+-rw-r--r--   0 val        (502) staff       (20)     4722 2023-04-23 23:41:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.944950 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
+-rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.947665 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
+-rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
+-rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
+-rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.948338 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.949990 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
+-rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
+-rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
+-rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
+-rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
+-rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
+-rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
+-rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.950173 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/
+-rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.951135 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)    17259 2023-04-24 23:38:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
+-rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.951407 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.953186 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.954941 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.955125 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw_no_cust/
+-rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.956541 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.958105 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.958369 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.960784 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
+-rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
+-rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
+-rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
+-rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
+-rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.961315 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     5986 2023-04-13 16:51:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.962889 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.963858 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.963995 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
+-rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
+-rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.965403 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.965656 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
+-rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
+-rw-r--r--   0 val        (502) staff       (20)    21134 2023-04-14 00:57:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/sample_db.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.967172 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.968964 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21696 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
+-rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.970082 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
+-rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
+-rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.970470 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
+-rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.971398 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.972559 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
+-rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.973099 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
+-rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
+-rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
+-rwxr-xr-x   0 val        (502) staff       (20)    17212 2023-03-12 01:12:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.974759 ApiLogicServer-8.3.0/api_logic_server_cli/templates/
+-rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.md
+-rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.txt
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/index.html
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/login_endpoint.txt
+-rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/login_endpoint_imports.txt
+-rw-r--r--   0 val        (502) staff       (20)       38 2023-04-27 02:31:19.975387 ApiLogicServer-8.3.0/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)     3521 2023-04-26 19:16:06.000000 ApiLogicServer-8.3.0/setup.py
```

### Comparing `ApiLogicServer-8.2.0/ApiLogicServer.egg-info/PKG-INFO` & `ApiLogicServer-8.3.0/ApiLogicServer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.2.0
+Version: 8.3.0
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -263,14 +263,16 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
+
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
 04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships (Issue 65)
 
 03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4 
 
 03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3
```

### Comparing `ApiLogicServer-8.2.0/ApiLogicServer.egg-info/SOURCES.txt` & `ApiLogicServer-8.3.0/ApiLogicServer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,22 @@
 ApiLogicServer.egg-info/PKG-INFO
 ApiLogicServer.egg-info/SOURCES.txt
 ApiLogicServer.egg-info/dependency_links.txt
 ApiLogicServer.egg-info/entry_points.txt
 ApiLogicServer.egg-info/not-zip-safe
 ApiLogicServer.egg-info/requires.txt
 ApiLogicServer.egg-info/top_level.txt
-api_logic_server_cli/Todo_models.py.py
 api_logic_server_cli/__init__.py
 api_logic_server_cli/api_logic_server.py
 api_logic_server_cli/api_logic_server_info.yaml
 api_logic_server_cli/cli.py
 api_logic_server_cli/cli_args_base.py
 api_logic_server_cli/cli_args_project.py
-api_logic_server_cli/config.py
 api_logic_server_cli/extended_builder.py
 api_logic_server_cli/logging.yml
-api_logic_server_cli/models.py
-api_logic_server_cli/ui_basic_web_app_run.py
 api_logic_server_cli/create_from_model/.DS_Store
 api_logic_server_cli/create_from_model/__init__.py
 api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
 api_logic_server_cli/create_from_model/api_logic_server_utils.py
 api_logic_server_cli/create_from_model/model_creation_services.py
 api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
 api_logic_server_cli/create_from_model/ui_admin_creator.py
@@ -401,14 +397,20 @@
 api_logic_server_cli/docs/Working-With-Docker.md
 api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
 api_logic_server_cli/docs/index.md
 api_logic_server_cli/docs/assets/.DS_Store
 api_logic_server_cli/docs/assets/images/bulb-icon.svg
 api_logic_server_cli/docs/assets/images/lightbulb.svg
 api_logic_server_cli/docs/stylesheets/extra.css
+api_logic_server_cli/fragments/Todo_modelsZZ.py.py
+api_logic_server_cli/fragments/configZZ.py
+api_logic_server_cli/fragments/db_typesZZ.txt
+api_logic_server_cli/fragments/modelsZZ.py
+api_logic_server_cli/fragments/nw_virtual_attrs.py
+api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
 api_logic_server_cli/project_prototype/.DS_Store
 api_logic_server_cli/project_prototype/.gitignore
 api_logic_server_cli/project_prototype/api_logic_server_run.py
 api_logic_server_cli/project_prototype/config.py
 api_logic_server_cli/project_prototype/default.env
 api_logic_server_cli/project_prototype/logging.yml
 api_logic_server_cli/project_prototype/mypy.ini
@@ -430,28 +432,30 @@
 api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
 api_logic_server_cli/project_prototype/.vscode/launch.json
 api_logic_server_cli/project_prototype/.vscode/settings.json
 api_logic_server_cli/project_prototype/api/__init__.py
 api_logic_server_cli/project_prototype/api/customize_api.py
 api_logic_server_cli/project_prototype/api/expose_api_models.py
 api_logic_server_cli/project_prototype/api/json_encoder.py
+api_logic_server_cli/project_prototype/api/readme_customize_api.md
 api_logic_server_cli/project_prototype/database/__init__.py
 api_logic_server_cli/project_prototype/database/alembic.ini
 api_logic_server_cli/project_prototype/database/bind_databases.py
 api_logic_server_cli/project_prototype/database/customize_models.py
 api_logic_server_cli/project_prototype/database/alembic/env.py
 api_logic_server_cli/project_prototype/database/alembic/readme.md
 api_logic_server_cli/project_prototype/database/alembic/script.py.mako
 api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
 api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
 api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
 api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
 api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
 api_logic_server_cli/project_prototype/devops/docker/build_image.sh
 api_logic_server_cli/project_prototype/logic/declare_logic.py
+api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
 api_logic_server_cli/project_prototype/security/.DS_Store
 api_logic_server_cli/project_prototype/security/__init__.py
 api_logic_server_cli/project_prototype/security/declare_security.py
 api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
 api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
 api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
 api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
```

### Comparing `ApiLogicServer-8.2.0/ApiLogicServer.egg-info/requires.txt` & `ApiLogicServer-8.3.0/ApiLogicServer.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 SQLAlchemy-Utils==0.38.2
 Werkzeug==2.2.3
 logicbankutils==0.6.0
 inflect==5.0.2
 itsdangerous==2.1.2
 Jinja2==3.1.2
 MarkupSafe==2.1.1
-safrs>=3.0
+safrs>=3.0.2
 Flask-Admin==1.5.7
 Flask-Cors==3.0.0
 Flask==2.2.2
 Flask-JWT-Extended==4.4.4
 Flask-Login==0.6.2
 Flask-OpenID==1.3.0
 python-dotenv==0.15.0
 email-validator==1.1.1
-LogicBank>=1.08.03
+LogicBank>=1.08.04
 PyMySQL==1.0.2
 cryptography==36.0.1
 requests==2.27.1
 gunicorn==20.1.0
 psycopg2-binary==2.9.5
 dotmap==1.3.25
 WTForms==2.3.3
```

### Comparing `ApiLogicServer-8.2.0/LICENSE` & `ApiLogicServer-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/MANIFEST.in` & `ApiLogicServer-8.3.0/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -3,10 +3,11 @@
 recursive-include api_logic_server_cli/project_prototype_nw_no_cust *.*
 recursive-include api_logic_server_cli/project_tutorial *.*
 recursive-include api_logic_server_cli/sqlacodegen_wrapper *.*
 recursive-include api_logic_server_cli/create_from_model *.*
 recursive-include api_logic_server_cli/database *.*
 recursive-include api_logic_server_cli/templates *.*
 recursive-include api_logic_server_cli/docs *.*
+recursive-include api_logic_server_cli/fragments *.*
 include api_logic_server_cli/api_logic_server_info.yaml
 include api_logic_server_cli/login_endpoint.txt
 include api_logic_server_cli/logging.yml
```

### Comparing `ApiLogicServer-8.2.0/PKG-INFO` & `ApiLogicServer-8.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.2.0
+Version: 8.3.0
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -263,14 +263,16 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
+
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
 04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships (Issue 65)
 
 03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4 
 
 03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3
```

### Comparing `ApiLogicServer-8.2.0/README.md` & `ApiLogicServer-8.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,16 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
+
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
 04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships (Issue 65)
 
 03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4 
 
 03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/Todo_models.py.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/api_logic_server.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/api_logic_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
         * api/expose_api_models.py for a safrs api  - using introspected models.py
     * Special provisions for NW Sample, to show customizations.
     * See end for key module map quick links...
 
 Called from api_logic_server_cli.py, by instantiating the ProjectRun object.
 '''
 
-__version__ = "08.02.00"
+__version__ = "08.03.00"
 recent_changes = \
     f'\n\nRecent Changes:\n' +\
+    "\t04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, readme updates, LogicBank 1.8.4 \n"\
     "\t04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65) \n"\
     "\t04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships \n"\
     "\t03/23/2023 - 08.01.15: cloud debug additions, issue 59, 62-4, table filters \n"\
     "\t03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3 \n"\
     "\t02/15/2023 - 08.00.01: Declarative Authorization and Authentication, Werkzeug==2.2.3 \n"\
     "\t01/10/2023 - 07.00.04: Portable projects, server_proxy  \n"\
     "\t01/06/2023 - 07.00.00: Multi-db, sqlite test dbs, tests run, security prototype, env config  \n"\
@@ -77,22 +78,28 @@
     return str(python_path)
 
 current_path = os.path.abspath(os.path.dirname(__file__))
 with open(f'{get_api_logic_server_dir()}/logging.yml','rt') as f:
         config=yaml.safe_load(f.read())
         f.close()
 logging.config.dictConfig(config)
-log=logging.getLogger(__name__)
+log = logging.getLogger(__name__)
 debug_value = os.getenv('APILOGICSERVER_DEBUG')
 if debug_value is not None:
     debug_value = debug_value.upper()
     if debug_value.startswith("F") or debug_value.startswith("N"):
         log.setLevel(logging.INFO)
     else:
         log.setLevel(logging.DEBUG)
+        logging.getLogger('create_from_model.api_logic_server_utils').setLevel(logging.DEBUG)
+        logging.getLogger('sqlacodegen_wrapper.sqlacodegen.sqlacodegen.codegen').setLevel(logging.DEBUG)
+        logging.getLogger('api_logic_server_cli.sqlacodegen_wrapper.sqlacodegen_wrapper').setLevel(logging.DEBUG)
+        logging.getLogger('create_from_model.model_creation_services').setLevel(logging.DEBUG)
+        
+
 
 # log.debug("sys.path.append(get_api_logic_server_dir())\n",get_api_logic_server_dir())
 sys.path.append(get_api_logic_server_dir())  # e.g, on Docker: export PATH="/home/api_logic_server/api_logic_server_cli"
 api_logic_server_path = os.path.dirname(get_api_logic_server_dir())  # e.g: export PATH="/home/api_logic_server"
 sys.path.append(api_logic_server_path)
 from create_from_model.model_creation_services import ModelCreationServices
 
@@ -387,29 +394,40 @@
     result = name
     if result.startswith("~"):
         result = str(Path.home()) + result[1:]
     return result
 
 
 def fix_database_models(project_directory: str, db_types: str, nw_db_status: str):
-    """ injecting <db_types file> into database/models.py, fix nw cascade delete """
+    """ injecting <db_types file> into database/models.py, fix nw cascade delete, jsonapi_attr """
     models_file_name = f'{project_directory}/database/models.py'
     if db_types is not None and db_types != "":
         log.debug(f'.. .. ..Injecting file {db_types} into database/models.py')
         with open(db_types, 'r') as file:
             db_types_data = file.read()
         create_utils.insert_lines_at(lines=db_types_data,
                                     at="(typically via --db_types)",
                                     file_name=models_file_name)
     if nw_db_status in ["nw", "nw+", "nw-"]:
         log.debug(f'.. .. ..Setting cascade delete for sample database database/models.py')
         create_utils.replace_string_in_file(in_file=models_file_name,
             search_for="OrderDetailList = relationship('OrderDetail', cascade_backrefs=True, backref='Order')",
             replace_with="OrderDetailList = relationship('OrderDetail', cascade='all, delete', cascade_backrefs=True, backref='Order')  # manual fix")
-
+"""         if not "include_exclude" in project_directory and False:  #
+            log.debug(f'.. .. ..And Employee Virtual Attributes')
+            nw_virtuals_attrs_file_name = Path(get_api_logic_server_dir()).\
+                                        joinpath('fragments/nw_virtual_attrs.py')
+            with open(nw_virtuals_attrs_file_name, 'r') as file:
+                nw_virtual_attrs = file.read()
+            nw_virtuals_attrs = nw_virtual_attrs[8:]  # first line was for IDE no errors
+            create_utils.insert_lines_at(lines=nw_virtuals_attrs,
+                                        at="OrderList = relationship('Order', cascade_backrefs=True, backref='Employee')",
+                                        file_name=models_file_name,
+                                        after=True)
+ """
 
 def final_project_fixup(msg, project) -> str:
     """
     * fix ports/hosts, 
     * inject project names/dates, 
     * update info file
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/cli.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/cli.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/cli_args_base.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_base.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/cli_args_project.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_project.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/config.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/configZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/model_creation_services.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/model_creation_services.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/create_admin.sh` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/create_admin.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/fab_config.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/fab_config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/home.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/ui_admin_creator.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/ui_admin_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/create_from_model/uri_info.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/uri_info.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/authentication.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/authentication.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/classicmodels.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/classicmodels.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/new.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/new.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/nw-gold-plus.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold-plus.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/nw-gold.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/nw.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/nw.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/table_filters_tests.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/database/todos.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/database/todos.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/API-Customize.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/API-Customize.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/API.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/API.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Admin-Customization.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Customization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Admin-Tour.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Tour.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Architecture.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Architecture.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Behave-Logic-Report.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave-Logic-Report.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Behave.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Create-ApiLogicProject.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Create-ApiLogicProject.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Classes.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Classes.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Customization.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Customization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Examples.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Examples.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Keys.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Keys.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Data-Model-Multi.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Multi.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Database-Connectivity.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Database-Connectivity.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Execute.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Execute.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/FAQ-Frameworks.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Frameworks.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/FAQ-Low-Code.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Low-Code.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/FAQ-RETE.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-RETE.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/IDE-Customize.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Customize.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/IDE-Execute.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Execute.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Eval-x.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval-x.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Eval.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Express-x.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express-x.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-Express.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-psycopg2.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-psycopg2.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install-pyodbc.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-pyodbc.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Install.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Internals-CLI.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals-CLI.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Internals.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic-Operation.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Operation.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic-Tutorial.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic-Why.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Why.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Logic.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Manage-GitHub.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Manage-GitHub.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Builders.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Builders.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-DevOps.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-DevOps.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Env.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Env.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Execution.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Execution.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Rebuild.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Rebuild.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Project-Structure.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Structure.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Sample-Database.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Sample-Database.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Activation.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Activation.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Authentication-Provider.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication-Provider.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Authentication.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Authorization.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authorization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Security-Overview.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Overview.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-CodeSpaces.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-CodeSpaces.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Conference.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Docker.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Docker.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Install-Python.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Install-Python.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Proven.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Proven.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Python-311.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python-311.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-Python.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-m1.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-m1.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tech-mkdocs-material.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-mkdocs-material.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Troubleshooting.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Troubleshooting.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Tutorial.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Working-With-Docker.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-With-Docker.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/images/bulb-icon.svg` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/bulb-icon.svg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/assets/images/lightbulb.svg` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/lightbulb.svg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/index.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/index.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/docs/stylesheets/extra.css` & `ApiLogicServer-8.3.0/api_logic_server_cli/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/extended_builder.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/extended_builder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/logging.yml` & `ApiLogicServer-8.3.0/api_logic_server_cli/logging.yml`

 * *Files 9% similar despite different names*

```diff
@@ -21,22 +21,22 @@
         formatter: simple
 
 root:
   level: INFO
   handlers: [console]
 
 loggers:
-# can I
+
     create_from_model.api_logic_server_utils:   
 #        level: DEBUG
         handlers: [console]
         propagate: no
 
     sqlacodegen_wrapper.sqlacodegen.sqlacodegen.codegen:   
-#         level: DEBUG
+#        level: DEBUG
         handlers: [console]
         propagate: no
 
 # find  a.  Create Models
     api_logic_server_cli.sqlacodegen_wrapper.sqlacodegen_wrapper:   
 #        level: DEBUG
         handlers: [console]
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/models.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/modelsZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 2000 0000 0800  ....Bud1.. .....
 00000010: 0000 2000 0000 100c 0000 0000 0000 0000  .. .............
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0038  ...............8
+00000040: 0000 0000 0000 0002 0000 0000 0000 003a  ...............:
 00000050: 0000 0001 0000 1000 0063 006f 006e 0074  .........c.o.n.t
 00000060: 0061 0069 0000 0000 0000 0000 0000 0000  .a.i............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,15 +250,15 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0038 0000 000d  ...........8....
+00001000: 0000 0000 0000 0000 0000 003a 0000 000d  ...........:....
 00001010: 002e 0064 0065 0076 0063 006f 006e 0074  ...d.e.v.c.o.n.t
 00001020: 0061 0069 006e 0065 0072 6c67 3153 636f  .a.i.n.e.rlg1Sco
 00001030: 6d70 0000 0000 0000 08c1 0000 000d 002e  mp..............
 00001040: 0064 0065 0076 0063 006f 006e 0074 0061  .d.e.v.c.o.n.t.a
 00001050: 0069 006e 0065 0072 6d6f 4444 626c 6f62  .i.n.e.rmoDDblob
 00001060: 0000 0008 1186 9b26 a4b5 c441 0000 000d  .......&...A....
 00001070: 002e 0064 0065 0076 0063 006f 006e 0074  ...d.e.v.c.o.n.t
@@ -335,111 +335,111 @@
 000014e0: 7000 0000 0000 000c d300 0000 0600 6400  p.............d.
 000014f0: 6500 7600 6f00 7000 736d 6f44 4462 6c6f  e.v.o.p.smoDDblo
 00001500: 6200 0000 08c1 63ef 4f50 a9c4 4100 0000  b.....c.OP..A...
 00001510: 0600 6400 6500 7600 6f00 7000 736d 6f64  ..d.e.v.o.p.smod
 00001520: 4462 6c6f 6200 0000 08c1 63ef 4f50 a9c4  Dblob.....c.OP..
 00001530: 4100 0000 0600 6400 6500 7600 6f00 7000  A.....d.e.v.o.p.
 00001540: 7370 6831 5363 6f6d 7000 0000 0000 0030  sph1Scomp......0
-00001550: 0000 0000 0500 6c00 6f00 6700 6900 636c  ......l.o.g.i.cl
-00001560: 6731 5363 6f6d 7000 0000 0000 0003 a200  g1Scomp.........
-00001570: 0000 0500 6c00 6f00 6700 6900 636d 6f44  ....l.o.g.i.cmoD
-00001580: 4462 6c6f 6200 0000 0894 af86 5359 6dc4  Dblob.......SYm.
-00001590: 4100 0000 0500 6c00 6f00 6700 6900 636d  A.....l.o.g.i.cm
-000015a0: 6f64 4462 6c6f 6200 0000 0894 af86 5359  odDblob.......SY
-000015b0: 6dc4 4100 0000 0500 6c00 6f00 6700 6900  m.A.....l.o.g.i.
-000015c0: 6370 6831 5363 6f6d 7000 0000 0000 0010  cph1Scomp.......
-000015d0: 0000 0000 0800 7300 6500 6300 7500 7200  ......s.e.c.u.r.
-000015e0: 6900 7400 7962 7773 7062 6c6f 6200 0000  i.t.ybwspblob...
-000015f0: b962 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
-00001600: 0707 0907 0b07 5d53 686f 7753 7461 7475  ......]ShowStatu
-00001610: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
-00001620: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00001630: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-00001640: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00001650: 5b53 686f 7753 6964 6562 6172 0909 0809  [ShowSidebar....
-00001660: 5f10 197b 7b31 3738 2c20 3133 397d 2c20  _..{{178, 139}, 
-00001670: 7b31 3033 302c 2035 3636 7d7d 0908 1523  {1030, 566}}...#
-00001680: 2f3b 525f 6b6c 6d6e 6f8b 0000 0000 0000  /;R_klmno.......
-00001690: 0101 0000 0000 0000 000d 0000 0000 0000  ................
-000016a0: 0000 0000 0000 0000 008c 0000 0008 0073  ...............s
-000016b0: 0065 0063 0075 0072 0069 0074 0079 6c67  .e.c.u.r.i.t.ylg
-000016c0: 3153 636f 6d70 0000 0000 0000 eea1 0000  1Scomp..........
-000016d0: 0008 0073 0065 0063 0075 0072 0069 0074  ...s.e.c.u.r.i.t
-000016e0: 0079 6d6f 4444 626c 6f62 0000 0008 5563  .ymoDDblob....Uc
-000016f0: 2d1b 33bb c441 0000 0008 0073 0065 0063  -.3..A.....s.e.c
-00001700: 0075 0072 0069 0074 0079 6d6f 6444 626c  .u.r.i.t.ymodDbl
-00001710: 6f62 0000 0008 5563 2d1b 33bb c441 0000  ob....Uc-.3..A..
-00001720: 0008 0073 0065 0063 0075 0072 0069 0074  ...s.e.c.u.r.i.t
-00001730: 0079 7068 3153 636f 6d70 0000 0000 0001  .yph1Scomp......
-00001740: f000 0000 0008 0073 0065 0063 0075 0072  .......s.e.c.u.r
-00001750: 0069 0074 0079 7653 726e 6c6f 6e67 0000  .i.t.yvSrnlong..
-00001760: 0001 0000 0009 0074 0065 006d 0070 006c  .......t.e.m.p.l
-00001770: 0061 0074 0065 0073 6c67 3153 636f 6d70  .a.t.e.slg1Scomp
-00001780: 0000 0000 0000 0eb5 0000 0009 0074 0065  .............t.e
-00001790: 006d 0070 006c 0061 0074 0065 0073 6d6f  .m.p.l.a.t.e.smo
-000017a0: 4444 626c 6f62 0000 0008 dc36 863d 6a55  DDblob.....6.=jU
-000017b0: c441 0000 0009 0074 0065 006d 0070 006c  .A.....t.e.m.p.l
-000017c0: 0061 0074 0065 0073 6d6f 6444 626c 6f62  .a.t.e.smodDblob
-000017d0: 0000 0008 dc36 863d 6a55 c441 0000 0009  .....6.=jU.A....
-000017e0: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
-000017f0: 0073 7068 3153 636f 6d70 0000 0000 0000  .sph1Scomp......
-00001800: 1000 0000 0004 0074 0065 0073 0074 6c67  .......t.e.s.tlg
-00001810: 3153 636f 6d70 0000 0000 0001 4506 0000  1Scomp......E...
-00001820: 0004 0074 0065 0073 0074 6d6f 4444 626c  ...t.e.s.tmoDDbl
-00001830: 6f62 0000 0008 ea55 863d 6a55 c441 0000  ob.....U.=jU.A..
-00001840: 0004 0074 0065 0073 0074 6d6f 6444 626c  ...t.e.s.tmodDbl
-00001850: 6f62 0000 0008 ea55 863d 6a55 c441 0000  ob.....U.=jU.A..
-00001860: 0004 0074 0065 0073 0074 7068 3153 636f  ...t.e.s.tph1Sco
-00001870: 6d70 0000 0000 0001 a000 0000 0002 0075  mp.............u
-00001880: 0069 6277 7370 626c 6f62 0000 00b7 6270  .ibwspblob....bp
-00001890: 6c69 7374 3030 d601 0203 0405 0607 0709  list00..........
-000018a0: 070b 075d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-000018b0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-000018c0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-000018d0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-000018e0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-000018f0: 6f77 5369 6465 6261 7209 0908 095f 1017  owSidebar...._..
-00001900: 7b7b 3534 2c20 3330 387d 2c20 7b39 3230  {{54, 308}, {920
-00001910: 2c20 3439 327d 7d09 0815 232f 3b52 5f6b  , 492}}...#/;R_k
-00001920: 6c6d 6e6f 8900 0000 0000 0001 0100 0000  lmno............
-00001930: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00001940: 0000 0000 8a00 0000 0200 7500 696c 6731  ..........u.ilg1
-00001950: 5363 6f6d 7000 0000 0000 01d5 1400 0000  Scomp...........
-00001960: 0200 7500 696d 6f44 4462 6c6f 6200 0000  ..u.imoDDblob...
-00001970: 0847 9a71 8987 8fc4 4100 0000 0200 7500  .G.q....A.....u.
-00001980: 696d 6f64 4462 6c6f 6200 0000 0847 9a71  imodDblob....G.q
-00001990: 8987 8fc4 4100 0000 0200 7500 6970 6831  ....A.....u.iph1
-000019a0: 5363 6f6d 7000 0000 0000 0260 0000 0000  Scomp......`....
-000019b0: 0200 7500 6976 5372 6e6c 6f6e 6700 0000  ..u.ivSrnlong...
-000019c0: 0100 0000 0a00 7600 6500 6e00 7600 5f00  ......v.e.n.v._.
-000019d0: 7300 6500 7400 7500 706c 6731 5363 6f6d  s.e.t.u.plg1Scom
-000019e0: 7000 0000 0000 001a 8d00 0000 0a00 7600  p.............v.
-000019f0: 6500 6e00 7600 5f00 7300 6500 7400 7500  e.n.v._.s.e.t.u.
-00001a00: 706d 6f44 4462 6c6f 6200 0000 08c6 7186  pmoDDblob.....q.
-00001a10: 3d6a 55c4 4100 0000 0a00 7600 6500 6e00  =jU.A.....v.e.n.
-00001a20: 7600 5f00 7300 6500 7400 7500 706d 6f64  v._.s.e.t.u.pmod
-00001a30: 4462 6c6f 6200 0000 08c6 7186 3d6a 55c4  Dblob.....q.=jU.
-00001a40: 4100 0000 0a00 7600 6500 6e00 7600 5f00  A.....v.e.n.v._.
-00001a50: 7300 6500 7400 7500 7070 6831 5363 6f6d  s.e.t.u.pph1Scom
-00001a60: 7000 0000 0000 0060 0000 0000 0000 0000  p......`........
-00001a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001550: 0000 0000 0500 6c00 6f00 6700 6900 6362  ......l.o.g.i.cb
+00001560: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
+00001570: 7430 30d6 0102 0304 0506 0707 0907 0b07  t00.............
+00001580: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00001590: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+000015a0: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+000015b0: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+000015c0: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+000015d0: 6964 6562 6172 0909 0809 5f10 187b 7b34  idebar...._..{{4
+000015e0: 3531 2c20 3133 347d 2c20 7b39 3230 2c20  51, 134}, {920, 
+000015f0: 3439 327d 7d09 0815 232f 3b52 5f6b 6c6d  492}}...#/;R_klm
+00001600: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
+00001610: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+00001620: 0000 8b00 0000 0500 6c00 6f00 6700 6900  ........l.o.g.i.
+00001630: 636c 6731 5363 6f6d 7000 0000 0000 0003  clg1Scomp.......
+00001640: a200 0000 0500 6c00 6f00 6700 6900 636d  ......l.o.g.i.cm
+00001650: 6f44 4462 6c6f 6200 0000 0894 af86 5359  oDDblob.......SY
+00001660: 6dc4 4100 0000 0500 6c00 6f00 6700 6900  m.A.....l.o.g.i.
+00001670: 636d 6f64 4462 6c6f 6200 0000 0894 af86  cmodDblob.......
+00001680: 5359 6dc4 4100 0000 0500 6c00 6f00 6700  SYm.A.....l.o.g.
+00001690: 6900 6370 6831 5363 6f6d 7000 0000 0000  i.cph1Scomp.....
+000016a0: 0010 0000 0000 0500 6c00 6f00 6700 6900  ........l.o.g.i.
+000016b0: 6376 5372 6e6c 6f6e 6700 0000 0100 0000  cvSrnlong.......
+000016c0: 0800 7300 6500 6300 7500 7200 6900 7400  ..s.e.c.u.r.i.t.
+000016d0: 7962 7773 7062 6c6f 6200 0000 b962 706c  ybwspblob....bpl
+000016e0: 6973 7430 30d6 0102 0304 0506 0707 0907  ist00...........
+000016f0: 0b07 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00001700: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00001710: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00001720: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00001730: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00001740: 7753 6964 6562 6172 0909 0809 5f10 197b  wSidebar...._..{
+00001750: 7b31 3738 2c20 3133 397d 2c20 7b31 3033  {178, 139}, {103
+00001760: 302c 2035 3636 7d7d 0908 1523 2f3b 525f  0, 566}}...#/;R_
+00001770: 6b6c 6d6e 6f8b 0000 0000 0000 0101 0000  klmno...........
+00001780: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+00001790: 0000 0000 008c 0000 0008 0073 0065 0063  ...........s.e.c
+000017a0: 0075 0072 0069 0074 0079 6c67 3153 636f  .u.r.i.t.ylg1Sco
+000017b0: 6d70 0000 0000 0000 eea1 0000 0008 0073  mp.............s
+000017c0: 0065 0063 0075 0072 0069 0074 0079 6d6f  .e.c.u.r.i.t.ymo
+000017d0: 4444 626c 6f62 0000 0008 5563 2d1b 33bb  DDblob....Uc-.3.
+000017e0: c441 0000 0008 0073 0065 0063 0075 0072  .A.....s.e.c.u.r
+000017f0: 0069 0074 0079 6d6f 6444 626c 6f62 0000  .i.t.ymodDblob..
+00001800: 0008 5563 2d1b 33bb c441 0000 0008 0073  ..Uc-.3..A.....s
+00001810: 0065 0063 0075 0072 0069 0074 0079 7068  .e.c.u.r.i.t.yph
+00001820: 3153 636f 6d70 0000 0000 0001 f000 0000  1Scomp..........
+00001830: 0008 0073 0065 0063 0075 0072 0069 0074  ...s.e.c.u.r.i.t
+00001840: 0079 7653 726e 6c6f 6e67 0000 0001 0000  .yvSrnlong......
+00001850: 0009 0074 0065 006d 0070 006c 0061 0074  ...t.e.m.p.l.a.t
+00001860: 0065 0073 6c67 3153 636f 6d70 0000 0000  .e.slg1Scomp....
+00001870: 0000 0eb5 0000 0009 0074 0065 006d 0070  .........t.e.m.p
+00001880: 006c 0061 0074 0065 0073 6d6f 4444 626c  .l.a.t.e.smoDDbl
+00001890: 6f62 0000 0008 dc36 863d 6a55 c441 0000  ob.....6.=jU.A..
+000018a0: 0009 0074 0065 006d 0070 006c 0061 0074  ...t.e.m.p.l.a.t
+000018b0: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
+000018c0: dc36 863d 6a55 c441 0000 0009 0074 0065  .6.=jU.A.....t.e
+000018d0: 006d 0070 006c 0061 0074 0065 0073 7068  .m.p.l.a.t.e.sph
+000018e0: 3153 636f 6d70 0000 0000 0000 1000 0000  1Scomp..........
+000018f0: 0004 0074 0065 0073 0074 6c67 3153 636f  ...t.e.s.tlg1Sco
+00001900: 6d70 0000 0000 0001 4506 0000 0004 0074  mp......E......t
+00001910: 0065 0073 0074 6d6f 4444 626c 6f62 0000  .e.s.tmoDDblob..
+00001920: 0008 ea55 863d 6a55 c441 0000 0004 0074  ...U.=jU.A.....t
+00001930: 0065 0073 0074 6d6f 6444 626c 6f62 0000  .e.s.tmodDblob..
+00001940: 0008 ea55 863d 6a55 c441 0000 0004 0074  ...U.=jU.A.....t
+00001950: 0065 0073 0074 7068 3153 636f 6d70 0000  .e.s.tph1Scomp..
+00001960: 0000 0001 a000 0000 0002 0075 0069 6277  ...........u.ibw
+00001970: 7370 626c 6f62 0000 00b7 6270 6c69 7374  spblob....bplist
+00001980: 3030 d601 0203 0405 0607 0709 070b 075d  00.............]
+00001990: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+000019a0: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+000019b0: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+000019c0: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+000019d0: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+000019e0: 6465 6261 7209 0908 095f 1017 7b7b 3534  debar...._..{{54
+000019f0: 2c20 3330 387d 2c20 7b39 3230 2c20 3439  , 308}, {920, 49
+00001a00: 327d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  2}}...#/;R_klmno
+00001a10: 8900 0000 0000 0001 0100 0000 0000 0000  ................
+00001a20: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
+00001a30: 8a00 0000 0200 7500 696c 6731 5363 6f6d  ......u.ilg1Scom
+00001a40: 7000 0000 0000 01d5 1400 0000 0200 7500  p.............u.
+00001a50: 696d 6f44 4462 6c6f 6200 0000 0847 9a71  imoDDblob....G.q
+00001a60: 8987 8fc4 4100 0000 0200 7500 696d 6f64  ....A.....u.imod
+00001a70: 4462 6c6f 6200 0000 0847 9a71 8987 8fc4  Dblob....G.q....
+00001a80: 4100 0000 0200 7500 6970 6831 5363 6f6d  A.....u.iph1Scom
+00001a90: 7000 0000 0000 0260 0000 0000 0200 7500  p......`......u.
+00001aa0: 6976 5372 6e6c 6f6e 6700 0000 0100 0000  ivSrnlong.......
+00001ab0: 0a00 7600 6500 6e00 7600 5f00 7300 6500  ..v.e.n.v._.s.e.
+00001ac0: 7400 7500 706c 6731 5363 6f6d 7000 0000  t.u.plg1Scomp...
+00001ad0: 0000 001a 8d00 0000 0a00 7600 6500 6e00  ..........v.e.n.
+00001ae0: 7600 5f00 7300 6500 7400 7500 706d 6f44  v._.s.e.t.u.pmoD
+00001af0: 4462 6c6f 6200 0000 08c6 7186 3d6a 55c4  Dblob.....q.=jU.
+00001b00: 4100 0000 0a00 7600 6500 6e00 7600 5f00  A.....v.e.n.v._.
+00001b10: 7300 6500 7400 7500 706d 6f64 4462 6c6f  s.e.t.u.pmodDblo
+00001b20: 6200 0000 08c6 7186 3d6a 55c4 4100 0000  b.....q.=jU.A...
+00001b30: 0a00 7600 6500 6e00 7600 5f00 7300 6500  ..v.e.n.v._.s.e.
+00001b40: 7400 7500 7070 6831 5363 6f6d 7000 0000  t.u.pph1Scomp...
+00001b50: 0000 0060 0000 0000 0000 0000 0000 0000  ...`............
 00001b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -591,51 +591,51 @@
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
 00002500: 0000 0000 08c1 63ef 4f50 a9c4 4100 0000  ......c.OP..A...
 00002510: 0600 6400 6500 7600 6f00 7000 736d 6f64  ..d.e.v.o.p.smod
 00002520: 4462 6c6f 6200 0000 08c1 63ef 4f50 a9c4  Dblob.....c.OP..
 00002530: 4100 0000 0600 6400 6500 7600 6f00 7000  A.....d.e.v.o.p.
 00002540: 7370 6831 5363 6f6d 7000 0000 0000 0030  sph1Scomp......0
-00002550: 0000 0000 0500 6c00 6f00 6700 6900 636c  ......l.o.g.i.cl
-00002560: 6731 5363 6f6d 7000 0000 0000 0003 a200  g1Scomp.........
-00002570: 0000 0500 6c00 6f00 6700 6900 636d 6f44  ....l.o.g.i.cmoD
-00002580: 4462 6c6f 6200 0000 0894 af86 5359 6dc4  Dblob.......SYm.
-00002590: 4100 0000 0500 6c00 6f00 6700 6900 636d  A.....l.o.g.i.cm
-000025a0: 6f64 4462 6c6f 6200 0000 0894 af86 5359  odDblob.......SY
-000025b0: 6dc4 4100 0000 0500 6c00 6f00 6700 6900  m.A.....l.o.g.i.
-000025c0: 6370 6831 5363 6f6d 7000 0000 0000 0010  cph1Scomp.......
-000025d0: 0000 0000 0800 7300 6500 6300 7500 7200  ......s.e.c.u.r.
-000025e0: 6900 7400 7962 7773 7062 6c6f 6200 0000  i.t.ybwspblob...
-000025f0: b962 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
-00002600: 0707 0907 0b07 5d53 686f 7753 7461 7475  ......]ShowStatu
-00002610: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
-00002620: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00002630: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-00002640: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00002650: 5b53 686f 7753 6964 6562 6172 0909 0809  [ShowSidebar....
-00002660: 5f10 197b 7b31 3738 2c20 3133 397d 2c20  _..{{178, 139}, 
-00002670: 7b31 3033 302c 2035 3636 7d7d 0908 1523  {1030, 566}}...#
-00002680: 2f3b 525f 6b6c 6d6e 6f8b 0000 0000 0000  /;R_klmno.......
-00002690: 0101 0000 0000 0000 000d 0000 0000 0000  ................
-000026a0: 0000 0000 0000 0000 008c 0000 0008 0073  ...............s
-000026b0: 0065 0063 0075 0072 0069 0074 0079 6c67  .e.c.u.r.i.t.ylg
-000026c0: 3153 636f 6d70 0000 0000 0000 eea1 0000  1Scomp..........
-000026d0: 0008 0073 0065 0063 0075 0072 0069 0074  ...s.e.c.u.r.i.t
-000026e0: 0079 6d6f 4444 626c 6f62 0000 0008 5563  .ymoDDblob....Uc
-000026f0: 2d1b 33bb c441 0000 0008 0073 0065 0063  -.3..A.....s.e.c
-00002700: 0075 0072 0069 0074 0079 6d6f 6444 626c  .u.r.i.t.ymodDbl
-00002710: 6f62 0000 0008 5563 2d1b 33bb c441 0000  ob....Uc-.3..A..
-00002720: 0008 0073 0065 0063 0075 0072 0069 0074  ...s.e.c.u.r.i.t
-00002730: 0079 7068 3153 636f 6d70 0000 0000 0001  .yph1Scomp......
-00002740: f000 0000 0008 0073 0065 0063 0075 0072  .......s.e.c.u.r
-00002750: 0069 0074 0079 7653 726e 6c6f 6e67 0000  .i.t.yvSrnlong..
-00002760: 0001 0000 0009 0074 0065 006d 0070 006c  .......t.e.m.p.l
-00002770: 0061 0074 0065 0073 6c67 3153 636f 6d70  .a.t.e.slg1Scomp
-00002780: 0000 0000 0000 0eb5 0000 0009 0074 0065  .............t.e
-00002790: 006d 0070 006c 0061 0074 0065 0073 6d6f  .m.p.l.a.t.e.smo
-000027a0: 4444 626c 6f62 0000 0008 dc36 863d 6a55  DDblob.....6.=jU
-000027b0: c441 0000 0009 0074 0065 006d 0070 006c  .A.....t.e.m.p.l
-000027c0: 0061 0074 0065 0073 6d6f 6444 626c 6f62  .a.t.e.smodDblob
-000027d0: 0000 0008 dc36 863d 6a55 c441 0000 0009  .....6.=jU.A....
-000027e0: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
-000027f0: 0073 7068 3153 636f 6d70 0000 0000 0000  .sph1Scomp......
-00002800: 1000 0000                                ....
+00002550: 0000 0000 0500 6c00 6f00 6700 6900 6362  ......l.o.g.i.cb
+00002560: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
+00002570: 7430 30d6 0102 0304 0506 0707 0907 0b07  t00.............
+00002580: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00002590: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+000025a0: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+000025b0: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+000025c0: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+000025d0: 6964 6562 6172 0909 0809 5f10 187b 7b34  idebar...._..{{4
+000025e0: 3531 2c20 3133 347d 2c20 7b39 3230 2c20  51, 134}, {920, 
+000025f0: 3439 327d 7d09 0815 232f 3b52 5f6b 6c6d  492}}...#/;R_klm
+00002600: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
+00002610: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+00002620: 0000 8b00 0000 0500 6c00 6f00 6700 6900  ........l.o.g.i.
+00002630: 636c 6731 5363 6f6d 7000 0000 0000 0003  clg1Scomp.......
+00002640: a200 0000 0500 6c00 6f00 6700 6900 636d  ......l.o.g.i.cm
+00002650: 6f44 4462 6c6f 6200 0000 0894 af86 5359  oDDblob.......SY
+00002660: 6dc4 4100 0000 0500 6c00 6f00 6700 6900  m.A.....l.o.g.i.
+00002670: 636d 6f64 4462 6c6f 6200 0000 0894 af86  cmodDblob.......
+00002680: 5359 6dc4 4100 0000 0500 6c00 6f00 6700  SYm.A.....l.o.g.
+00002690: 6900 6370 6831 5363 6f6d 7000 0000 0000  i.cph1Scomp.....
+000026a0: 0010 0000 0000 0500 6c00 6f00 6700 6900  ........l.o.g.i.
+000026b0: 6376 5372 6e6c 6f6e 6700 0000 0100 0000  cvSrnlong.......
+000026c0: 0800 7300 6500 6300 7500 7200 6900 7400  ..s.e.c.u.r.i.t.
+000026d0: 7962 7773 7062 6c6f 6200 0000 b962 706c  ybwspblob....bpl
+000026e0: 6973 7430 30d6 0102 0304 0506 0707 0907  ist00...........
+000026f0: 0b07 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00002700: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00002710: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00002720: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00002730: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00002740: 7753 6964 6562 6172 0909 0809 5f10 197b  wSidebar...._..{
+00002750: 7b31 3738 2c20 3133 397d 2c20 7b31 3033  {178, 139}, {103
+00002760: 302c 2035 3636 7d7d 0908 1523 2f3b 525f  0, 566}}...#/;R_
+00002770: 6b6c 6d6e 6f8b 0000 0000 0000 0101 0000  klmno...........
+00002780: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+00002790: 0000 0000 008c 0000 0008 0073 0065 0063  ...........s.e.c
+000027a0: 0075 0072 0069 0074 0079 6c67 3153 636f  .u.r.i.t.ylg1Sco
+000027b0: 6d70 0000 0000 0000 eea1 0000 0008 0073  mp.............s
+000027c0: 0065 0063 0075 0072 0069 0074 0079 6d6f  .e.c.u.r.i.t.ymo
+000027d0: 4444 626c 6f62 0000 0008 5563 2d1b 33bb  DDblob....Uc-.3.
+000027e0: c441 0000 0008 0073 0065 0063 0075 0072  .A.....s.e.c.u.r
+000027f0: 0069 0074 0079 6d6f 6444 626c 6f62 0000  .i.t.ymodDblob..
+00002800: 0008 5563                                ..Uc
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/.vscode/launch.json` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api/customize_api.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/customize_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 # called by api_logic_server_run.py, to customize api (new end points, services).
 # separate from expose_api_models.py, to simplify merge if project recreated
 
 app_logger = logging.getLogger(__name__)
 
 def expose_services(app, api, project_dir, swagger_host: str, PORT: str):
-    """ Customize API - new end points for services """
+    """ Customize API - new end points for services 
+    
+        Brief background: see readme_customize_api.md
+    
+    """
     
     app_logger.debug("api/customize_api.py - expose custom services")
 
     @app.route('/hello_world')
     def hello_world():  # test it with: http://api_logic_server_host:api_logic_server_port/hello_world?user=ApiLogicServer
         """
         This is inserted to illustrate that APIs not limited to database objects, but are extensible.
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api/json_encoder.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/api_logic_server_run.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api_logic_server_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     See Main Code (at end).
         Use log messages to understand API and Logic activation.
 
 ==============================================================================
 """
 
-import os, logging, logging.config, sys, yaml
+import os, logging, logging.config, sys, yaml  # failure here means venv probably not set
 from flask_sqlalchemy import SQLAlchemy
 import json
 from pathlib import Path
 
 def is_docker() -> bool:
     """ running docker?  dir exists: /home/api_logic_server """
     path = '/home/api_logic_server'
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/config.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/env.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic/readme.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/alembic.ini` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/database/bind_databases.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/bind_databases.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/logging.yml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logging.yml`

 * *Files 0% similar despite different names*

```diff
@@ -23,30 +23,30 @@
 root:
   level: INFO
   handlers: [console]
 
 loggers:
 
     api.expose_api_models:   
-    #        level: DEBUG
+#        level: DEBUG
         handlers: [console]
         propagate: no
 
     logic_logger:
         level: DEBUG
         handlers: [console]
         propagate: no
 
     safrs:
         level: DEBUG
         handlers: [console]
         propagate: no
 
     api.customize_api:   
-    #        level: DEBUG
+#        level: DEBUG
         handlers: [console]
         propagate: no
 
     database.customize_models:   
 #        level: DEBUG
         handlers: [console]
         propagate: no
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/mypy.ini` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/mypy.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/readme.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,74 +10,49 @@
 
 To run your project, the system requires various runtime systems for data access, api, and logic.  These are [included with API Logic Server](https://apilogicserver.github.io/Docs/Architecture-What-Is/).  So, to run your project:
 
 1.  __Establish your Python Environment__ to activate these runtime systems
     * Choose the __either__ the _Local Install_ __or__ the _Docker_ approach below, then 
 2. __Run__
 
+For instructions, [see here](#setup-instructions).
 
 &nbsp;
 
-## Establish Your Python Environment - Local Install
-
-You `requirements.txt` has already been created, so...
-
-```bash title="Install API Logic Server in a Virtual Environment"
-python -m venv venv                        # may require python3 -m venv venv
-venv\Scripts\activate                      # mac/linux: source venv/bin/activate
-python -m pip install -r requirements.txt  # accept "new Virtual environment"
-```
-
-Notes:
-
-* See also the `venv_setup` directory in this API Logic Project.
-
-* If using SqlServer, install `pyodbc`.  Not required for docker-based projects.  For local installs, see the [Quick Start](https://apilogicserver.github.io/Docs/Install-pyodbc/).
+# Project Structure
+This project was created with the directory structure shown below.
 
-&nbsp;
+The ___Key Customization Files___ in the table are created as stubs, intended for you to add customizations that extend
+the created API, Logic and Web App.  Since they are separate files, the project can be
+[rebuilt](https://apilogicserver.github.io/Docs/Project-Rebuild/) (e.g., synchronized with a revised schema), preserving your customizations.
 
-## Establish Your Python Environment - Docker
+Please see the ```nw``` sample for examples of typical customizations.  You can open it in GitHub (use Shift + "." to view in project mode) - [click here](https://github.com/ApiLogicServer/demo).
 
-Your runtime systems are part of Dev Container, which you probably activated when you [opened the project](https://apilogicserver.github.io/Docs/IDE-Execute/).  If you did not accept the "Open in Container" option when you started VSCode, use __View > Command Palette > Remote-Containers: Reopen in Container__.
+| Directory | Usage                         | Key Customization File             | Typical Customization                                                                 |
+|:-------------- |:------------------------------|:-----------------------------------|:--------------------------------------------------------------------------------------|
+| ```api``` | JSON:API                      | ```api/customize_api.py```         | Add new end points / services                                                         |
+| ```database``` | SQLAlchemy Data Model Classes | ```database/customize_models.py``` | Add derived attributes, and relationships missing in the schema                       |
+| ```logic``` | Transactional Logic           | ```logic/declare_logic.py```       | Declare multi-table derivations, constraints, and events such as send mail / messages |
+| ```ui``` | Admin App                     | ```ui/admin/admin.yaml```          | Control field display - order, captions etc.                                          |
+| ```security``` | Authentication, Authorization   | ```security/declare_security.py```          | Control login, role-based row access         |
+| ```tests``` | Behave Test Suite              | ```tests/api_logic_server_behave/features```          | Declare and implement [Behave Tests](https://apilogicserver.github.io/Docs/Behave/)                                          |
 
 &nbsp;
 
-## Run
-
-To run your project:
-
-* **Start the API**, either by __IDE launch configurations__ (see below), or by command line: `python api_logic_server_run.py`.
-
-* **Open the Admin App -** either
-
-    * Open your Browser at [http://localhost:5656](http://localhost:5656), or 
-    
-    * Open in VSCode's Simple Browser (as shown below):
-
-        1. Click __View > Command__ to open the Command Palette
-            * Enter command: `Simple Browser: Show`
-            * Specify the URL: `http://localhost:5656`
-        2. Explore the swagger - open another simple Browser with URL `http://localhost:5656/api` 
-            * Note: you can drag windows to arrange your viewing area
-
-<figure><img src="https://github.com/ApiLogicServer/Docs/blob/main/docs/images/ui-admin/run-admin-app.png?raw=true"></figure>
-
-&nbsp;&nbsp;
-
 # Project Information
 
 | About                    | Info                               |
 |:-------------------------|:-----------------------------------|
 | Created                  | creation-date                      |
 | API Logic Server Version | api_logic_server_version           |
 | Created in directory     | api_logic_server_project_directory |
 | API Name                 | api_logic_server_api_name          |
 
-&nbsp;&nbsp;
 
+&nbsp;
 
 # Key Technologies
 
 API Logic Server is based on the projects shown below.
 Consult their documentation for important information.
 
 ### SARFS JSON:API Server
@@ -123,38 +98,60 @@
 It is used by JSON:Api, Logic Bank, and the Admin App.
 
 SQLAlchemy processing is based on Python `model` classes,
 created automatically by API Logic Server from your database,
 and saved in the `database` directory.
 
 
-
 ### Admin App
 
 This generated project also contains a React Admin app:
 * Multi-page - including page transitions to "drill down"
 * Multi-table - master / details (with tab sheets)
 * Intelligent layout - favorite fields first, predictive joins, etc
 * Logic Aware - updates are monitored by business logic
 
-&nbsp;&nbsp;
 
-# Project Structure
-This project was created with the following directory structure:
+&nbsp;
+
+# Setup Instructions
 
-| Directory | Usage                         | Key Customization File             | Typical Customization                                                                 |
-|:-------------- |:------------------------------|:-----------------------------------|:--------------------------------------------------------------------------------------|
-| ```api``` | JSON:API                      | ```api/customize_api.py```         | Add new end points / services                                                         |
-| ```database``` | SQLAlchemy Data Model Classes | ```database/customize_models.py``` | Add derived attributes, and relationships missing in the schema                       |
-| ```logic``` | Transactional Logic           | ```logic/declare_logic.py```       | Declare multi-table derivations, constraints, and events such as send mail / messages |
-| ```ui``` | Admin App                     | ```ui/admin/admin.yaml```          | Control field display - order, captions etc.                                          |
-| ```security``` | Authentication, Authorization   | ```security/declare_security.py```          | Control login, role-based row access         |
-| ```tests``` | Behave Test Suite              | ```tests/api_logic_server_behave/features```          | Declare and implement [Behave Tests](https://apilogicserver.github.io/Docs/Behave/)                                          |
 &nbsp;
 
-### Key Customization File - Typical Customization
+## Establish Your Python Environment - Local Install
 
-In the table above, the _Key Customization Files_ are created as stubs, intended for you to add customizations that extend
-the created API, Logic and Web App.  Since they are separate files, the project can be
-[rebuilt](https://apilogicserver.github.io/Docs/Project-Rebuild/) (e.g., synchronized with a revised schema), preserving your customizations.
+You `requirements.txt` has already been created, so...
+
+```bash title="Install API Logic Server in a Virtual Environment"
+python -m venv venv                        # may require python3 -m venv venv
+venv\Scripts\activate                      # mac/linux: source venv/bin/activate
+python -m pip install -r requirements.txt  # accept "new Virtual environment"
+```
+
+Notes:
+
+* See also the `venv_setup` directory in this API Logic Project.
+
+* If using SqlServer, install `pyodbc`.  Not required for docker-based projects.  For local installs, see the [Quick Start](https://apilogicserver.github.io/Docs/Install-pyodbc/).
+
+&nbsp;
+
+## Establish Your Python Environment - Docker
+
+Your runtime systems are part of Dev Container, which you probably activated when you [opened the project](https://apilogicserver.github.io/Docs/IDE-Execute/).  If you did not accept the "Open in Container" option when you started VSCode, use __View > Command Palette > Remote-Containers: Reopen in Container__.
+
+&nbsp;
+
+## Run
+
+To run your project
+
+![Start Project](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/nutshell/project-executable.png?raw=true)
+
+As shown above:
+
+1. Use the pre-supplied Run Configuration
+2. Click the url in the console to start the Admin App
+    * Use it to explore your data (shown below)
+    * And your API (via Swagger)
 
-Please see the ```nw``` sample for examples of typical customizations.
+![Admin App](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/ui-admin/run-admin-app.png?raw=true)
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/run.ps1` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/run.sh` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/declare_security.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/authentication.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authentication.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/authorization.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authorization.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/templates/index.html` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/test/basic/server_test.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/admin/home.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/util.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/py.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,17 @@
     """
         Simple constraint for error testing 
     """
     Rule.constraint(validate=models.Customer,
         as_condition=lambda row: row.CompanyName != 'x',
         error_msg="CustomerName cannot be 'x'")
 
+    Rule.constraint(validate=models.Employee,
+        as_condition=lambda row: row.LastName != 'x',
+        error_msg="LastName cannot be 'x'")
 
     """
         More complex rules follow - see: 
             https://github.com/valhuber/LogicBank/wiki/Examples
             https://github.com/valhuber/LogicBank/wiki/Rule-Extensibility
     """
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,7 +97,29 @@
     context.response_text = r.text
 
 
 @then("Reject - Raise too small")
 def step_impl(context):
     response_text = context.response_text
     assert 'meaningful raise' in response_text, f'Error - "meaningful raise" not in response:\n{response_text}'
+
+
+@when('Retrieve Employee Row')
+def step_impl(context):
+    """
+    Observe the use of `old_row
+    `
+    > **Key Takeaway:** State Transition Logic enabled per `old_row`
+
+    """
+    scenario_name = 'Manage ProperSalary'
+    test_utils.prt(f'\n\n\n{scenario_name}... Get Employee - verify contains virtual ProperSalary\n\n', scenario_name)
+    header = test_utils.login()
+    get_emp_uri = f'http://localhost:5656/api/Employee/5/'
+    r = requests.get(url=get_emp_uri, headers= header)
+    context.response_text = r.text
+
+
+@then("Verify Contains ProperSalary")
+def step_impl(context):
+    response_text = context.response_text
+    assert 'ProperSalary' in response_text, f'Error - "ProperSalary" not in response:\n{response_text}'
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -176,23 +176,28 @@
               <li> Observe the same effect on Update / Insert screens as you alter the value of <span style="font-family:'Courier New'">EmployeeType</span></li>
             </ul>
             <h1>Images</h1>
             Observe that "show" pages support images.
             <h1>Virtual Relationships</h1>
             Observe that "show" pages have tabs for Manages and Manager.<br>
             These foreign keys are *not* defined in the database, but in <span style="font-family:'Courier New'">database/customize_models.py</span>.<br>
+            <h1>Derived Attributes</h1>
+            <span style="font-family:'Courier New'">ProperSalary</span> is not defined in the database.<br>
+            See <span style="font-family:'Courier New'">database/customize_models.py</span>.<br>
     attributes:
       - label: ' Last Name*'
         name: LastName
         search: true
         sort: true
       - name: OnLoanDepartmentId
       - name: WorksForDepartmentId
       - name: Salary
         type: DECIMAL
+      - name: ProperSalary
+        type: DECIMAL
       - name: EmployeeType
       - name: Dues
         type: DECIMAL
         show_when: record["EmployeeType"] == "Hourly"
       - name: FirstName
       - name: Id
       - name: Title
```

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/.vscode/launch.json` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/readme.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/project_tutorial/sample_db.sqlite` & `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/sample_db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/templates/admin.yaml` & `ApiLogicServer-8.3.0/api_logic_server_cli/templates/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/templates/app_fiddle.md` & `ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/templates/app_fiddle.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/templates/index.html` & `ApiLogicServer-8.3.0/api_logic_server_cli/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/templates/login_endpoint.txt` & `ApiLogicServer-8.3.0/api_logic_server_cli/templates/login_endpoint.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/api_logic_server_cli/ui_basic_web_app_run.py` & `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.2.0/setup.py` & `ApiLogicServer-8.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,24 +69,24 @@
         "SQLAlchemy-Utils==0.38.2",
         "Werkzeug==2.2.3",
         "logicbankutils==0.6.0",
         "inflect==5.0.2",
         "itsdangerous==2.1.2",
         "Jinja2==3.1.2",
         "MarkupSafe==2.1.1",
-        "safrs>=3.0",
+        "safrs>=3.0.2",
         "Flask-Admin==1.5.7",
         "Flask-Cors==3.0.0",
         "Flask==2.2.2",
         "Flask-JWT-Extended==4.4.4",
         "Flask-Login==0.6.2",
         "Flask-OpenID==1.3.0",
         "python-dotenv==0.15.0",
         "email-validator==1.1.1",
-        "LogicBank>=1.08.03",
+        "LogicBank>=1.08.04",
         "PyMySQL==1.0.2",
 #         "pyodbc==4.0.32",
         "cryptography==36.0.1",
         "requests==2.27.1",
         "gunicorn==20.1.0",
         "psycopg2-binary==2.9.5",
         "dotmap==1.3.25",
```

